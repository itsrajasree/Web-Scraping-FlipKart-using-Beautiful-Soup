# Web-Scraping-FlipKart-using-Beautiful-Soup
The details of Samsung mobile phones from flipkart are scraped using Beautiful Soup and saved in a CSV file.

In this project, the details of Samsung mobile phones from Flipkart are scraped and are saved in .csv format. The details such as name, price, rating, and specifications of the phone are scraped. The result of this project help to analyze various factors like price, rating, etc, and how the specifications affect these factors. Web Scraping method automatically retrieves data from websites and makes the process of data collection much easier. Python contains a lot of methods for web scraping like BeautifulSoup, Scrapy, Selenium, etc. In this project, BeautifulSoup is used for scraping data from Flipkart.

As the initial stage, the necessary libraries, i.e; pandas, requests, and BeautiulSoup are imported to the notebook. Then, the URL of the website is passed on to a variable using get() method in requests. Then checked for the status of the URL. Since the value is 200, no error.

i. Parsing Html :
Using the Html parser in BeautifulSoup, the content in the URL is parsed into a variable. Using prettify() method, the content is aligned properly to improve the readability.

ii. Getting Values from Html :
From the Html file,  the required variables of all the mobile phones shown in the category are obtained using find_all() method. Further, the tags are removed and the values are stored in lists using the for() loop. Then, the unnecessary data are removed. Also, some details were separated into different lists using if-else() method.

iii. Saving the data into DataFrame :
A data frame is created using pandas and the values in the lists are stored in the data frame as the columns.

iv. Converting to CSV :
With to_csv() method in pandas, the data frame is stored as a .csv file in the specified location. Index values are given as True.
