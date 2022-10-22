# kayak_webscraping

<img width="1356" alt="Schermata 2022-10-22 alle 12 41 59" src="https://user-images.githubusercontent.com/114148028/197334871-eaaf4eac-274d-4eb5-8386-158982a38727.png">

The aim of the code is to provide a reproducible way to gather flight offers data on Kayak. The bot can be easily scheduled to repat the process at the same interval (e.g. every hour for one week).

The bot will go on kayak.com/best-flights and scrape all flight offers data every 3 hours. At each iteration an e-mail will be sent containing the price variation with respect to the average price of all previous iterations. In addition the advice of Kayak will be included that could be 'monitor the price' or 'buy now' depending on kayak's analyists prices forecast. 

the scraped data includes:
- company
- price
- outband time schedule
- return time schedule
- stops or direct
- outband flight duration
- return flight duration
- outband airports 
- return airports
- date and time of scraping

The code is fully reproducible by anyone but you must have installed the required packages in python. 

Using the search_flight function the user can specify:
- departure city abbr. (e.g. NYC for New York or MIL for Milan)
- arrive city abbr. 
- outband date (the format is: 'YYYY-MM-DD')
- return date

With the sendmail function the user can specify:
- the sender's e-mail
- the sender's password
- the receiver's e-mail


