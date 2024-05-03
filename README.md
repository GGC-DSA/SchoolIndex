# School Index
Develop School Index for Studypool

## Description 
This capstone project aims to develop a comprehensive database of colleges, universities, and online schools in the United States tailored to the needs of students conducting research on potential educational institutions. The data will be presented in the form of a website for the company StudyPool. The website will serve as a centralized resource providing key information for each school such as the school’s location, website, logo, and picture. By organizing and presenting this information in a user-friendly manner, the website will empower students to make informed decisions about their academic pursuits. We will utilize web scraping for the data collection process to make the database easily scalable. Through the implementation of search and filtering functionalities, users will be able to efficiently explore and compare different schools based on their specific criteria. Ultimately, this project seeks to enhance the accessibility and transparency of information about educational institutions facilitating the college search process for students across the U.S.

## Project Demo 
<https://youtu.be/PRgV5qmOW-o?si=UOPrtdF9YKvSRovf>

## Project Website 
<https://ggc-dsa.github.io/SchoolIndex/> 

## Poster 
<https://app.marq.com/invitations/accept/inv_07d72d23-d092-4894-9b69-1ba5bcebe784>

## Final Report


## Spring 2024 Team
Niecia - Team Manager and Data Modeler 

![Photo](https://github.com/GGC-DSA/SchoolIndex/assets/125173695/2304a624-f74a-48bc-a0e5-099377ec9689)


Cobi - Client Liason and Data Analyzer 

![IMG_20240210_162436(1)](https://github.com/GGC-DSA/SchoolIndex/assets/125174228/9afd55c0-16f1-4de0-a388-8bad8ec0455d)


Nathaniel - Visualizer and Project Documentation

![IMG_0053](https://github.com/GGC-DSA/SchoolIndex/assets/144246936/7747f168-9c7f-452c-a961-3c237f644eef)

### Client
Our client is StudyPool. Studypool is an online marketplace where students can post academic questions or assignments and receive help from tutors or educators. It provides a platform for students to get personalized assistance and support for their academic needs. This project was taking care with Studypool's COO Helen Merhout and full stack engineer Benardo Avancena.

## Notebook
File: 
Link: <https://colab.research.google.com/drive/1g_mjqjC1Nx2u5h3dB9Y6kTNLTih8utay#scrollTo=hyI713epbeNe>

## Outreach Activities
- Presented at the STaRS event on April 8th, 2024.
- Presented at the CREATE Symposium on April 25th, 2024.

## Awards
- Received honorable mention (4th place) at the STaRS event.
- Our team is the rightmost team in the following image.

![image](https://github.com/GGC-DSA/SchoolIndex/assets/125174228/3e74122a-7fee-4c76-a876-45934509e0fc)

## Technologies
### Data Modeler Technology 
- Google Colab 
- SerpApi 
- Python Notebook
- Excel 
- Wikipedia API 

### Data Analyzer Technology 
- Excel
- Python Notebook
- Matplotlib Python library
- Tableau 
- MySQL 

### Data Visualizer Technology 
- Figma UI/UX website design platform: https://www.figma.com 
- HTML 
- CSS 

## Project Setup and Usage
### Extraction of schools’ summaries  
The code uses the Wikipedia library to access Wikipedia's vast repository of articles and retrieve summaries for a list of schools. The Wikipedia library acts as an interface to interact with Wikipedia's content programmatically, providing functions to access article text, summaries, images, and more. To use this code, you need to ensure that you have the necessary libraries installed, including csv and Wikipedia. Prepare a CSV file containing a list of school names, ensuring that it is formatted correctly and named "GA_College_Name.csv". Then, simply run the script. It will read the CSV file, iterate through each school name, retrieve its summary from Wikipedia using the `get_school_summary` function, and store the summaries in a new CSV file named "school_summaries.csv". Once the script finishes execution, you can find the collected summaries saved in the output CSV file. With this script, you can efficiently gather comprehensive summaries of schools from Wikipedia. 

### Extraction of schools’ logos 
The code utilizes the SerpApi library to perform an image search for "colleges in Georgia logos" on Google Images. It retrieves image results using pagination to ensure comprehensive coverage of the search.  To use the script, ensure that you have the necessary libraries installed, including csv,  serpapi, and dotenv. Set up a .env file containing your SerpApi key. Then, run the script, and it will automatically perform the image search, retrieve results, and save them into the specified CSV file.  

### Data Analysis and Visualizations
All of the data analysis operations were done in the Colab notebook. The [cleanDataset](https://github.com/GGC-DSA/SchoolIndex/blob/main/code/Data%20Files/cleanDataset.csv) file is the filtered data set that only includes the 100 colleges in Georgia that we used throughout the late stages of the project. The [us-colleges-and-universities](https://github.com/GGC-DSA/SchoolIndex/blob/main/code/Data%20Files/us-colleges-and-universities.csv) file is the entire data set with all of the colleges and all of the columns removed from the clean data set.
The [visualizations](https://github.com/GGC-DSA/SchoolIndex/tree/main/docs-Spr2024/Tableau%20Visualizations) were made in Tableau. The beta visualization was made using the cleanDataset while the main visualization was made using the [trimmedDataset](https://github.com/GGC-DSA/SchoolIndex/blob/main/code/Data%20Files/trimmedDataset.csv). In the Tableau files themselves, the beta visualization's data source is titled "cleanDataset.csv" while the main visualization's data source is titled "fullDataset.csv". These files may need to be renamed in order for the Tableau visualizations to work.

### SQL Database
The SQL Database was created in MySQL Workbench. There is a fulldataset.idb file in the Data Files folder. If this file cannot be used to create the MySQL database, then the Table Data Import Wizard can be used to recreate it. The data types of each column are displayed in the following image. The ID column was set as the primary key, and the IPEDSID column was given the unique constarint.

![image](https://github.com/GGC-DSA/SchoolIndex/assets/125174228/257df32e-9f65-4fe5-a1f7-92547c57cbe3)

## Working Features
- Implemented a web scraper to extract the schools’ logos and summaries 
- Developed a data visualization showing schools in the data set on a map of Georgia with a color gradient showing how many total students are enrolled in the data set. 
- Developed a MySQL database to connect with the website. 
- Added a primary key and two unique constraints to columns in the MySQL database.
  
## Data Set
<https://www.kaggle.com/datasets/joebeachcapital/us-colleges-and-universities>

## Data Analysis Methods
This project did not have a focus on data analysis. This is a data modeling project, and the client has expressed very little interest in the data analysis aspects. As a result, minimal data analysis was performed, but that does not mean there was no data analysis performed.

The data analysis techniques are discussed in the [notebook](https://colab.research.google.com/drive/1g_mjqjC1Nx2u5h3dB9Y6kTNLTih8utay#scrollTo=hyI713epbeNe). Initially, matplotlib was used to plot longitude vs. latitude to create the initial visualization. A failed attempt at utilizing a linear regression ML algorithm can be observed. Total enrollment vs. latitude was plotted resulting in a graph with little correlation. Afterwards, the longitude vs. latitude graph was recreated in Tableau. The resulting visualizations show each college on a map of Georgia with a color scheme that denotes how many students are enrolled in each school - the darker the blue, the more students enrolled. It is worth noting that the final version of the visualization excluded the universities with a null value for total enrollment as well as universities with a value over 10,000 for total enrollment. The visualization may be redone to include some schools over 10,000.

## Data Analysis Results
Three results can be observed from the data analysis:
- There is not always an application for linear regression between two given columns. The reason why linear regression was not pursued for enrollment vs. latitude was because latitude data needs its corresponding longitude data to extract meaningful information. There are schools that can have the same latitude as well.
- There is a cluster of colleges near the Atlanta area which can be expected due to it being a population center.
- The most popular colleges on the visualization are spread out throughout the state with a slight lean towards northern Georgia which may be in part due to Atlanta.

## TODO Tasks
- Set up local server to host website to allow for testing of client’s API. 
- Finish cleaning the logos data file and clean the descriptions file. 
- Merge cleaned logo/description files into the SQL database. 
- Send the client the output of a mysqldump Powershell command. 
- Finish connecting the MySQL database to the website. 
- Extract logos and summaries from the remaining schools in Georgia and across the US in the dataset. 
- Find a solution to address schools without logos and summaries. 
- Address disambiguation errors caused by ambiguous school names. 
- Mobile-friendly website interface. 
- Re-styling of website to match Studypool's website theming. 
- Expansion of data set beyond Georgia colleges. 
