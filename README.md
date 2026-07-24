# Hello! 

This is a web scraper for a university course equvalency website built in conjuction with Claude Code in Jupyter Notebooks. 


**NOTE**
The site this scraper targets is not designed to be scraped. Do not scrape this website. Due to the target site being ASP.NET, scraping is a unreasonably heavy load on its server. 
More discussion of both Claude Code and the ethics of webscraping can be found in the last section of this README. 


## Web Scraper  

### Objective

Develop a program that can export every course listed on a univerity's course equvalency and its equvalency into a CSV file in order to make the content searchable by course, 
a feature unavailable on the target website. 

#### Specifications

- Create a functional web scrapper to capture the full list of insitutions
- Iterate through the list of insitutions to scrape each page in order to capture course information
- Handle CAPTCHA
- Ensure polite wait times and loads on server
- Export into a CSV, if scraping is interuppted, begin where the CSV left off.
- If an error is raised, capture a screenshot of the page at the time of the error & save to file for debugging. 

## Discussion: Thoughts on the Process, Claude as a Tool, Morality of Scraping in General 

- (To be fleshed out)
- Claude made it very easy to have something working, scraping, and getting results without having to think about any repercussions.
- Claude made many assumptions about the site and generated huge chunks of code based on simple assumptions that weren't valid.
- Claude added "data validation' features that broke code and didn't hold to the data, readded them later even after being asked to remove them.
- Had I done research before hand instead of relying on Claude, I wouldn't have built the scrapper. Resources found after having a semi functional program made by humans warned around the ethics of scraping
- Further research before diving in would've given necessary context, espcially around scrapping an ASP.NET site, which is a stateful "app" and not similar to more standard html pages. The load on the server to generate each instance of data after a change in state is high, and origninally Claude did not have safe guards around redoing scraping that had already been done, which resulted in much higher loads on the server than necessary in order to get to the end result of a CSV of the course information. 
