# School Index
Develop School Index for Studypool

## Description 
This capstone project aims to develop a comprehensive database of colleges, universities, and online schools in the United States tailored to the needs of students conducting research on potential educational institutions. The data will be presented in the form of a website for the company StudyPool. The website will serve as a centralized resource providing key information for each school such as the school’s location, website, logo, and picture. By organizing and presenting this information in a user-friendly manner, the website will empower students to make informed decisions about their academic pursuits. We will utilize web scraping for the data collection process to make the database easily scalable. Through the implementation of search and filtering functionalities, users will be able to efficiently explore and compare different schools based on their specific criteria. Ultimately, this project seeks to enhance the accessibility and transparency of information about educational institutions facilitating the college search process for students across the U.S.

## Project Demo 
<https://youtu.be/PRgV5qmOW-o?si=UOPrtdF9YKvSRovf>

## Project Website 
<https://ggc-dsa.github.io/SchoolIndex/> 

## Final notebook

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
<https://colab.research.google.com/drive/1g_mjqjC1Nx2u5h3dB9Y6kTNLTih8utay#scrollTo=hyI713epbeNe>

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
## Working Features
- Implemented a web scraper to extract the schools’ logos and summaries 
- Developed a data visualization showing schools in the data set on a map of Georgia with a color gradient showing how many total students are enrolled in the data set. 
- Developed a MySQL database to connect with the website. 
- Added a primary key and two unique constraints to columns in the MySQL database. 
## Data Sets
<https://www.kaggle.com/datasets/joebeachcapital/us-colleges-and-universities>
## Data Analysis Methods

## Data Analysis Results

## TODO Tasks
