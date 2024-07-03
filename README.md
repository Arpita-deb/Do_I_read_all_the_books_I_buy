# Do I read all the books I buy? 
### An analysis of my collection of books 
![Do I read all the books I buy](https://github.com/Arpita-deb/Do_I_read_all_the_books_I_buy/assets/139372731/06dbfa73-832d-4cde-b584-9e7b2d7c5bd9)

## Introduction:
Books have been my constant companion since my childhood. But I've taken it seriously when life came to a standstill with the pandemic. And ever since my fascination with the world of literature has not reduced a bit. 

Following the 6 phases of data analysis - namely ask, prepare, process, analyze, share and act, I've gained some interesting insights of my books collection. For instance, I read Non Fictions most of the time and the ratio of female vs male writers is surprisingly 1:8. Here, I've documented the entire process of collecting, cleaning and analyzing the data.

## Tools Used: 

For this project a combination of 3 tools were used.

* Excel for initial Data Cleaning
* PostgreSQL for Database Design
* Python Programming Language (Jupyter Notebook) for Exploratory Data Analysis
* Tableau for creating data visualizations and dashboard

# PHASE 1 - ASK
In order to analyze the data, I compiled a set of questions that would act as a guide to gain insights, and keep us in track.

## Objective of the project:

The key questions that I wanted to find answers were :

* *Have I read all the books that I buy?*

* *If not, how many books are there still unread or partially read?*

* *How much did I spend on books in recent years?*

* *How many books I've bought each year?*

* *Which books were most expensive and which were the cheapest?*

* *Which genre, language, writer and publications were most favored?*

* *What is the average rate of books from each genre?*

# PHASE 2 - PREPARE
For this project I've created a dataset named Books_Management as a personal budget to keep track of all the books that I've bought from 2014 to 2023. The dataset contains 13 columns and 184 rows. Each cell represents an attributes of a unique book. The data description is given below.

## Data Dictionary: 

| Column Name | Column Description | Data Type |
| :--- | :--- | :--- |
| ID | Unique ID for each book | int |
| Name | Name of the book | chr |
| Writer | Name of the writer | chr |
| Original_Language | Language in which the book is originally written | chr |
| Genre | Genre of the book | chr |
| Binding | Whether book is Paperback, hardcover or ebook| chr |
| Publication | Name of the Publication agency | chr |
| Price | Price of the book in INR(₹) | int |
| Transaction_method | Online or Cash or None (if the books are free) | chr |
| Year | Year of buying | int |
| Read/Unread | Yes- If I've read, No- If I've not read; Partially read- If I've started reading but didn't finish | chr |
| Rating | How I rated the books - Excellent, Moderate, Bad, None(for unread books) | chr |
| Gender of the writer | Male, Female, No information, Male and Female (for multiple authors) | chr |

## Reliability: 
The data set used for this project is created from 184 books that I've collected (hardcovers, paperbacks and eBooks from 2014 to 2023) in June 2023 and processed by me in Excel before loading it to the Jupyter Notebook.

## Limitation of the data set:
Since it is used as a personal tracker of budget, it is not open for public. And the data contains information till June 2023 and naturally will not include the books that'll buy later.


# PHASE 3 - PROCESS
The first step to data analyze is to clean the typographical errors and other table junks, provide a structure to the table, remove redundant information and duplicates. Before exporting the file into Jupyter Notebook, I've used different Excel tools and functions to clean the dataset.

## Data Cleaning:
The following steps are taken to clean and organize the data:

1. Creating a backup copy of the original data in a separate workbook.
2. Fixing misspelling and typos with the help of Spellcheck and Find and Replace dialog box.
3. Filling up the cells with the help of dropdown to reduce the typographic errors.
4. Removing duplicates using Remove Duplicate.
5. Changing the case of the text using PROPER Function.
6. Using TRIM function to remove the leading or trailing spaces from the texts.
7. Checking the formats of the data points.
8. Using Conditional formatting to find null data points.
9. Using Pivot tables to check inconsistencies and preliminary calculations.

## Database Normalization:
In addition to cleaning the dataset, I've also designed a database system with normalized tables (upto 3rd Normal Form) using PostgreSQL. This project is available [here](https://github.com/Arpita-deb/Books-Database-Normalization.git), or you can read about the steps taken to create this database system in this [medium article](https://medium.com/@arpita_deb/from-spreadsheets-to-database-c2e8dbeb6a76).

However, for the analysis phase I've used the cleaned dataset for simplicity's sake.

# PHASE 4 - ANALYZE

For analysis I've used Python and Jupyter Notebook which is provided as EDA_in_Python. The results of the analysis in presented as Tableau visualizations for quick and easy understanding.

## Data Visualization: 

### 1. Genre:
![genre](https://github.com/Arpita-deb/Books-Database-Normalization/assets/139372731/8a24f8e5-3cfc-40b3-b1a7-e868fa910374)

About half of the collection contains Non - Fictions i.e books based on facts, actual events, or real people. In contrast, fiction is a genre of literature that describes imaginary settings, events, and characters. 


### 2. Format:

![binding](https://github.com/Arpita-deb/Books-Database-Normalization/assets/139372731/09755729-e715-405e-8e2f-9314d419665d)

Paperbacks are my preferred type of books. Next comes ebooks which are very handy and mostly free of cost, making up 30% of the collection.

### 3. Books that are read, partially read or unread

![books partially read](https://github.com/Arpita-deb/Books-Database-Normalization/assets/139372731/d66f40cd-4f1d-46aa-81b3-e4c9d9770587)
More than half of the collection of books are already read. But there remains about 36% of books that I haven't read yet or partially read.

### 4. Identifying Unread books

![unread books](https://github.com/Arpita-deb/Books-Database-Normalization/assets/139372731/7b22a48f-5e13-4df6-a2b1-72525a48840c)

The reason behind ebooks being unread may be due to the fact that they remain out of my sight in some corner of a computer file and partially due to their digital format which can be hard oto read. 

### 5. Total expenses

![5](https://github.com/Arpita-deb/Do_I_read_all_the_books_I_buy/assets/139372731/68df5401-3784-42d1-a73f-e87ca34d8218)

Over the course of 9 years, approximately ₹35,000 have been spent on books. 

![6](https://github.com/Arpita-deb/Do_I_read_all_the_books_I_buy/assets/139372731/d4462c51-6b76-4e86-bd10-6f39f5b97c3c)

Majority of the books are paperbacks and costs in the range of ₹100-₹300.

![7](https://github.com/Arpita-deb/Do_I_read_all_the_books_I_buy/assets/139372731/9a389b13-21bc-4757-823e-97b1c6f22e59)

Approximately ₹20,000 were spent in 2020 and 2021 alone, a period marked by Covid 19. During that trying time when all other external activities were prohibited, reading has been a great way to spend my time productively.

### 6. Distribution of Languages

![lang](https://github.com/Arpita-deb/Books-Database-Normalization/assets/139372731/78cbb9bb-27d9-4d90-ac25-3b9b56697be8)

### 7. Most expensive books

![top 20 books by price](https://github.com/Arpita-deb/Books-Database-Normalization/assets/139372731/c5ded1fc-6d45-430d-b040-fde354383bfd)

### 8. Popular writers

![top 10 writers](https://github.com/Arpita-deb/Books-Database-Normalization/assets/139372731/e5534558-5a05-4f57-be6b-c11478890a37)

### 9. Gender distribution

![gender](https://github.com/Arpita-deb/Books-Database-Normalization/assets/139372731/836d1e0f-34b7-45a8-9a7a-fdceb1e42ee6)

### 10. Ratings

![rating](https://github.com/Arpita-deb/Books-Database-Normalization/assets/139372731/5e6f218e-c1e3-4aeb-b299-d8c363f0de7a)

## Dashboard:

For this project I've created an exploratory dashboard providing an overview of the dataset. In order to build the tableau visualizations and the dashboard, I've taken the following steps:

* Used tiled containers (vertical and horizontal) that contain the individual data visualizations.

* Used title for the dashboards.

* Used consistent color scheme that enhances the data.

* Cleared the chart junks such as titles of individual data viz, axis and axis labels, color legends etc that doesn't contribute to the data design.

* Visually grouped the data by using layout containers and colored background.

* Added an info button at the top right corner that provides information about the project and dataset used.

* Created device specific layouts.

![Screenshot (526)](https://github.com/Arpita-deb/Do_I_read_all_the_books_I_buy/assets/139372731/00d464dd-bdbe-440d-8168-bdcd0ce5002f)

You can check out my [Tableau Dashboard](https://public.tableau.com/views/DoIreadallthebooksthatIbuy/Dashboard4?:language=en-US&:display_count=n&:origin=viz_share_link) here.

# PHASE 5 - SHARE
It's time wrap up the entire project with a few takeaways.

## Conclusion:

From the Exploratory Data Analysis of this small dataset, I've been able to answer some important questions and also came up with some interesting insights.

* The answer to the first question, **Do I read all the books that I buy?** is unfortunately **No**. No matter how much I really enjoy reading books, 33% of the total books are unread. Most of them are ebook formats.

* **44** out of 184 (24%) books are **unread** and **21 partially read** (11%).

* I've spent total **₹34,694** on books over the course of 9 years.

* About **₹20,000** has been spent in **2020** and **2021** alone, which corresponds to the covid pandemic. 

* Interestingly it is in **2022** that I bought highest number of books, presumably in much lower price (₹5815).

* The average price of books in this collection is **₹294**.

* **Non-Fiction** and **Fiction** are the two most popular genres.

* Most of my books are **Paperbacks**, and **Penguin** is my preferred publishing company.

* The most expensive book in my collection is the **Complete Chronicle of Narnia(₹1337)**.

* The cheapest book is **The Cycle of Time(₹20)**.

* **Fyodor Dostoevsky** has the highest number of books in this collection.

* Surprisingly, **157** out of 178 writers are male, only **20** are females, almost 1/8th of the whole collection.

* Most of the books are originally written in **English**.

# PHASE 6 - ACT

This analysis has enabled me to understand my own taste in books, and which type of books I really enjoy reading. I can do the following to make my books collection richer and more diverse-

* Before buying more books, I must complete reading the unread/partially read books.
* Read more literature penned by Women.
* Read some more poetries and Proses, along with dramas.
* Read some books in French or German, or more translations of books in other languages.

## Limitation of the project:

1. The data contains information of books bought upto 2023. No data is available for 2023 onwards. So, it will not reflect the current state of my collection.
2. Majority of the data is categorical, I could have collected more numerical data to perform predictive analysis, by binning, encoding or creating dummy variables.
3. The analysis doesn't include correlations between various variables, so we could not know which variables affect most my preference of books.
4. Since the data is a private collection, it might not be publicly and widely useful.

## Appendix:
* [Database Normalization Project Documentation](https://github.com/Arpita-deb/Books-Database-Normalization.git)
* [From Spreadsheets to Database - A Comprehensive study of Database Normalization](https://medium.com/@arpita_deb/from-spreadsheets-to-database-c2e8dbeb6a76)

