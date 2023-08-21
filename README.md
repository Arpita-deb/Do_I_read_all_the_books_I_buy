# Do I read all the books I buy? 

## Introduction:
This dataset was created as a personal budget in an excel file to keep track of all the books that I've bought from 2014 to 2023. The initial data cleaning has been done in Excel,the EDA is performed with Python and Dashboards are created in Tableau. The key questions that I wanted to find answers were :

* Do I read all the books that I buy?

* If not, how many books are there still unread or partially read?

* How much did I spend on books in recent years?

* How many books I've bought each year?

* Which books were most expensive and which were the cheapest?

* Which genre, language, writer and Publications were most favoured?

* What is the average rate of books from each genre?

## Tools Used:
* Excel for initial Data CLeaning
* Jupyter Notebook(Python) for Exploratory Data Analysis
* Tableau for creating data visualizations and a dashboard

## Data Dictionary: 

| Column Name | Column Description |
| :--- | :--- |
| ID | Unique ID for each book |
| Name | Name of the book |
| Writer | Name of the writer |
| Original_Language | Language in which the book is originally written |
| Genre | Genre of the book |
| Binding | Whether book is Paperback, hardcover or ebook|
| Publication | Name of the Publication agency |
| Price | Price of the book in INR(₹) |
|Transaction_method | Online or Cash or None (if the books are free) |
| Year | Year of buying |
| Read/Unread | Yes- If I've read, No- If I've not read; Partially read- If I've started reading but didn't finish |
| Rating | How I rated the books - Excellent, Moderate, Bad, None(for unread books) |
| Gender of the writer | Male, Female, No information, Male and Female (for multiple authors) |


## Data Cleaning:
Before exporting the file into Jupyter Notebook, I've used Excel to clean up the data. The following steps are taken to clean and organise the data:

* Creating a backup copy of the original data in a separate workbook.

* Ensuring that the data is in a tabular format of rows and columns with: similar data in each column, all columns and rows visible, and no blank rows within the range.

* Doing tasks that don't require column manipulation first, such as fixing mispelling and typos with the help of Spellcheck or using the Find and Replace dialog box.

* Filling up the cells with the help of dropdown to reduce the typographic errors.

* Removing duplicates using Remove Duplicate.

* Changing the case of the text using PROPER Function.

* Using TRIM function to remove the leading or trailing spaces from the texts.

* Checking the formats of the data points.
  
*  Using Conditional formatting to find null data points.

* Using Pivot tables to check inconsistencies and preliminary calculations.

## Data Visualization: 

## Conclusion:
From the Exploratory Data Analysis of this small dataset, I've been able to answer some important questions and also came up with some interesting insights.

* The answer to the first question, Do I read all the books that I buy? is unfortunately No. No matter how much I really enjoy reading books, there are almost 1/3 of books that I haven't read yet. Most of them are ebook formats.

* 44 out of 184 books are unread and 21 partially read.

* The total price of the books is ₹ 34694.

* About ₹20,000 has been spent in 2020 and 2021 alone, which corresponds to the covid pandemic, when all other outdoor activities were prohibited. One couldn't spend these trying times in a more productive way.

* Interestingly it is in 2022 that I bought highest number of books, presumambly in much lower price (₹5815).

* The average price of books in this collection is ₹294.

* The most expensive book in my collection is the Complete Chronicle of Narnia(₹1337).

* The cheapest book is The Cycle of Time(₹20).

* Non_Fiction and Fiction are the two most popular genres.

* Most of my books are Paperbacks, and Penguin is my preferred publishing company.

* Fyodor Dostoevsky has the highest number of books in this collection.

* Surprisingly, 157 out of 178 writers are male, only 20 are females.

* Most of the books are originally written in English.

## Tableau Dashboard: 

1. In order to build the tableau visualizations and the dashboards, I've taken the following steps:

2. Used tiled containers (vertical and horizontal) that contain the individual data visualizations

3. Used titles for each of the dashboards

4. Used filter and annotations to highlight important data points

5. Used consistent color scheme that enhances the data

6. Cleared the chart junks such as titles of individual data viz, axis and axis labels, color legends etc that doesn't contribute to the data design

7. Visually grouped the data by using layout containers and colored background

8. Added filter actions to provide user interactivities

9. Added a Go to page to navigate between dashboards

10. Created device specific layouts.
