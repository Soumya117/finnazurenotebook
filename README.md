# finnazurenotebook


This project contains some python scripts and small functions to parse a website called finn.no (https://www.finn.no/).
The main requirement of the project is to note any changes to the price (currently only price is being calculated. It 
can be easily extended to represent different kind of data other than price. 

The python script has two main jobs:
1. Scan the website (filter already applied to Oslo region) for new ads (new buildings excluded for now).
   Add it into links.json if not already there with a timestamp.
2. Take link from links.json and parse it to obtain the price listed. Insert the link as key along with the price in 
   another json called pris.json. 1 link can have multiple prices in the json if finn updates the price. This json
   also contains the timestamp with the new price. 
 
 
 
So it is easy to check when the price was updated for one ad. The project can be extended to parse different data and keep a record 
of the changes.
