# Tata-1mg-Homeopathic-medicine-Analysis 💊
## Introduction
In the modern era, there's a growing interest in homeopathic medicine due to its holistic approach to healing. This project aims to analyze data related to homeopathic medicine products, including benefits, pricing, brands, ratings, and ingredients.

## Problem Aimed to Solve
This project helps entrepreneurs estimate costs for a homeopathic store and select relevant products. It uses data analysis to empower informed decisions, aiming to create an interactive dashboard for cost evaluation and product selection based on benefits.

##  <img src="https://user-images.githubusercontent.com/106439762/181935629-b3c47bd3-77fb-4431-a11c-ff8ba0942b63.gif" width="48" height="48"> **User's Manual**

| Files/Folder| Description |
| ------------- | ------------- |
| **Excel file** | This file provides you the insights and the analysis and other files(merged_data.xlsx, medicine_details_final.xlsx, merged_data.xlsx) have the scrapped                   data from the 1 Mg website. |
| **Python File** | This contains the .ipynb file related to the web scrapping part.  |

## Data Description 🚧

- **Table - 1**: *medicine_name*

Column Name           | Description
----------------------|-----------------------------------------------------------
name                  | Name of the medicine
size_of_the_bottle    | Size of the medicine bottle or pack
MRP_of_the_bottle     | Industry of the company from which the job is
price_of_the_bottle   | Selling price of the bottle
1mg_url               | 1mg url where the medicine sold
<img width="276" alt="img" src="https://github.com/Ankitaaa03/Tata-1mg-Homeopathic-medicine-Analysis/assets/133629631/1023164d-8b7a-4c93-be74-fdcc0d27fbad">



- **Table - 2** : *medicine_details*

Column Name         | Description
--------------------|-------------------------------------------------
name                | Name of the medicine
brand_name          | Brand name of the medicine
key_benefits        | Key Benefits area (Hair, eye, joint, skin)
key_ingredients     | Ingredient of medicine
rating              | User rating of the medicine
number_of_rating    | Number of people rated that product
<img width="517" alt="img1" src="https://github.com/Ankitaaa03/Tata-1mg-Homeopathic-medicine-Analysis/assets/133629631/28b5b756-ebdf-4d6f-a060-bfbe23e21048">



##  Methodology

**Scraped the data with the help of Python BeautifulSoup library.**

### For Table - 1

1. Imported libraries including requests for making HTTP requests, for parsing HTML content.
2. Created empty lists as Name, Sizes, MRPs , Prices, URLs to hold product-related information.

![img](https://github.com/Ankitaaa03/Tata-1mg-Homeopathic-medicine-Analysis/assets/133629631/f995a316-122d-4c8d-8228-864dc663ce81)

3. To scrape data from multiple pages, a variable called page is initialized with the value 1.
4. This variable helps in moving from one page to the next during the scraping process.

![img1](https://github.com/Ankitaaa03/Tata-1mg-Homeopathic-medicine-Analysis/assets/133629631/0484adab-23a6-4959-89c3-873d3cb51654)

5. Used While to scrape data  until it finds a "Page not found" message, indicating the end of available pages.
6. After scraping data from the current page, the script increments the page variable to move on to the next page.


### For Table - 2

1. Imported libraries including requests for making HTTP requests and BeautifulSoup for parsing HTML content.
2. Created empty lists as Name, brand_names, key_ingredients, ratings, number_of_ratings, key_benefits, count,to store details about each medicine.

![img](https://github.com/Ankitaaa03/Tata-1mg-Homeopathic-medicine-Analysis/assets/133629631/765f45d4-3a00-4d68-87c8-838a2c37bb4c)


3. Used For loop to iterate through a list of URLs from a DataFrame (df['1mg_url']).
4. Extracting data using Beautifulsoup If the name is found, it is appended to the name list. If not found, the list is populated with None.
   
![img1](https://github.com/Ankitaaa03/Tata-1mg-Homeopathic-medicine-Analysis/assets/133629631/4eb45d5e-94b3-4089-8bc8-96373a2d9be5)


5. Similar to the medicine name, the other details of the medicine is extracted and added to the relevant list. If it's not found, "None" is added.
6. The count variable is incremented with each URL processed, Once all URLs have been processed, the total count is printed to signify the end of the scraping process.

##  <img src="https://github.com/Ankitaaa03/Tata-1mg-Homeopathic-medicine-Analysis/assets/133629631/31f54d34-e844-423f-86f0-502e2fedb8e4"  width="48" height="48">  Analysis was done with the help of Pandas and Excel.


- **Insights were generated from the above analysis.**

  1). **The number of medicines in the benefits area Digestion is highest.**
  
  ![img2](https://github.com/Ankitaaa03/Tata-1mg-Homeopathic-medicine-Analysis/assets/133629631/e42737e0-6359-43b7-b181-80d75675678c)

  2). **Bhargava Phytolab has the highest number of customer ratings, i.e.1008.**
  
  ![img3](https://github.com/Ankitaaa03/Tata-1mg-Homeopathic-medicine-Analysis/assets/133629631/63d93dd6-4a99-4f78-be4c-6595fa107a30)

  3). **The brand SBL Pvt Ltd has most greater than 4-point review medicines.**
  
  ![image](https://github.com/Ankitaaa03/Tata-1mg-Homeopathic-medicine-Analysis/assets/133629631/17dff270-ec40-45ed-b510-7c718d6c5712)

### Excel is used for dashboard and data visualization.
  ## Dashboard
  
![image (2)](https://github.com/Ankitaaa03/Tata-1mg-Homeopathic-medicine-Analysis/assets/133629631/f05ca944-bd1e-4644-9134-8d43e3ee9ab9)

 ## Insights from the Dashboard

- The most used ingredient is Arsenicum album
- The number of medicines in the benefits area Digestion is highest.
- SBL Pvt Ltd has the highest average number of customer ratings.
- The brand SBL Pvt Ltd has most greater than 4-point review medicines.
- SBL Pvt Ltd and Bjain Pharmaceutical Pvt Ltd are the two brands that are used most among the benefit areas.
- The Brand SBL Pvt Ltd has the highest number of medicines of where a number of ratings is present.

## 🏥 Challenges and learnings

- **Website Ban**: Faced repeated bans on the 1Mg official website during data scraping attempts.
- **Google Colab Solution**: Resolved the issue by migrating scraping operations to Google Colab.
- **Extended Scraping Time**: Extracting details of each medicine took more time than anticipated.
- **Duplicate Data Issue**: Encountered delays due to duplicate data in the scraping process.
- **Learning Efficiency**: Gained insights into optimizing scraping methods for speed and accuracy.

## 🏥 Conclusions

Despite challenges in data scraping and extended collection time, this project recommends prioritizing "Digestion" benefit area medicines and considering products from SBL Pvt Ltd for a homeopathic store. The experience underscores the significance of adaptability, efficiency, and meticulous analysis in informed decision-making for the retail of homeopathic medicine.




