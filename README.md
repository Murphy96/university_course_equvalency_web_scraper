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
