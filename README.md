## scrapper-walmart

## Reason for Project -

In using grocery pickup, I will often find that the review of an items. I constructed this script. The goal is to output a csv file available for easy data analysis to make that determination.
Personal Usage
I have setup this script to run as a cron job (every 15 minutes during Grocery Pickup hours) on a Linux droplet from Digital Ocean. I have determined that the 2GB Memory/2 vCPU droplet architecture is sufficient for this job. It typically takes less than one minute to perform this task and update the files, which are automatically updated via cloud storage accessible on my local machines.

## Dependencies -

Uses following Python modules:
web drivers
csv
time
Selenium
os
time
pandas
beautifulsoup


## Categories -

Clorax disinfected wipes
crsip lemon
Fresh scent

## Fields -

- Review date
- Reviewer name
- Review title
- Review body or description
- Rating given by the user

## (a) How you have implemented the scraper, what challenges you faced and how did you solve them?
- Web scrapping menas it scrapes the data from the web using the website link and that was meant for the user compared to the data that is intended for another application or database.
THe challenge that faces on scrapping are -
*Many different formats of product page listings/templates that are constantly being tweaked/updated along with UX A/B testing of new layouts, ad placements, etc. that Amazon is always testing,
*Different product variations (one product page but multiple colors, sizes, flavors available), different layouts for product variations, and consistent changes in the approach to displaying variations,
*Collecting data at scale while avoiding web captchas and IP blacklisting,
*nconsistent versions and features of Walmart across the growing list of countries in which Amazon has a presence

## (b) What else you could do to improve your scraper?
If you can reduce the number of requests sent, your scraper will be much faster. For example, if you are scraping prices and titles from an e-commerce site, then you don't need to visit each item's page. You can get all the data you need from the results page.

## (C) How would you design it to make it work on other retailers as well?
We can design a retail design to make it work on other retailes is -
Use the right floor plan.
Be aware of where you “lead” shoppers.
Ensure that your product quantities are appropriate. 
Have enough space between products and fixtures. 
Freshen up your displays regularly. 
Find ways to appeal to multiple senses.

## Usage Instructions -
User should change/enter their preferred:

Zipcode in the zipcodeToCheck variable
File name in the exportFileName variable
XPATH for correct selection in the penultimate wait.until for store selection block
URLs for personalized items in the personalFavorites array
After making these changes, ensure the CSV file is not open in another application, then build/execute the script.
