# Tata-1mg-Homeopathic-medicine-Analysis
## Introduction
In the modern era, there's a growing interest in homeopathic medicine due to its holistic approach to healing. This project aims to analyze data related to homeopathic medicine products, including benefits, pricing, brands, ratings, and ingredients.

## Problem Aimed to Solve
This project helps entrepreneurs estimate costs for a homeopathic store and select relevant products. It uses data analysis to empower informed decisions, aiming to create an interactive dashboard for cost evaluation and product selection based on benefits.

##  <img src="https://user-images.githubusercontent.com/106439762/181935629-b3c47bd3-77fb-4431-a11c-ff8ba0942b63.gif" width="48" height="48"> **User's Manual**

| Files/Folder| Description |
| ------------- | ------------- |
| **Excel file** | This file provides you the insights and the analysis and other files(merged_data.xlsx, medicine_details_final.xlsx, merged_data.xlsx) have the scrapped                   data from the 1 Mg website. |
| **Python File** | This contains the .ipynb file related to the web scrapping part.  |

## Data Description

- **Table - 1**: *medicine_name*

Column Name           | Description
----------------------|-----------------------------------------------------------
name                  | Name of the medicine
size_of_the_bottle    | Size of the medicine bottle or pack
MRP_of_the_bottle     | Industry of the company from which the job is
price_of_the_bottle   | Selling price of the bottle
1mg_url               | 1mg url where the medicine sold
##  Methodology

- **Scraped the data with the help of Python BeautifulSoup library.**

### For Table - 1

<img width="900" alt="image" src="https://github.com/Ankitaaa03/Tata-1mg-Homeopathic-medicine-Analysis/assets/133629631/9e5c6dfe-1f9e-4365-aca0-61fa97839172">

### For Table - 2

<img width="900" alt="image" src="https://github.com/Ankitaaa03/Tata-1mg-Homeopathic-medicine-Analysis/assets/133629631/24f5036a-f40c-49e1-935d-bb8699221f7d">

### Analysis was done with the help of Pandas and Excel.

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

## Challenges and learnings

- **Website Ban**: Faced repeated bans on the 1Mg official website during data scraping attempts.
- **Google Colab Solution**: Resolved the issue by migrating scraping operations to Google Colab.
- **Extended Scraping Time**: Extracting details of each medicine took more time than anticipated.
- **Duplicate Data Issue**: Encountered delays due to duplicate data in the scraping process.
- **Learning Efficiency**: Gained insights into optimizing scraping methods for speed and accuracy.

## Conclusions

Despite challenges in data scraping and extended collection time, this project recommends prioritizing "Digestion" benefit area medicines and considering products from SBL Pvt Ltd for a homeopathic store. The experience underscores the significance of adaptability, efficiency, and meticulous analysis in informed decision-making for the retail of homeopathic medicine.




