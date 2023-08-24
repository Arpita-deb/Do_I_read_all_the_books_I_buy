# Do I read all the books I buy? 
## An analysis of my collection of books using Python and Tableau 

## Introduction:
This dataset was created as a personal budget in an excel file to keep track of all the books that I've bought from 2014 to 2023. 

## Objective of the project:

The key questions that I wanted to find answers were :

* *How much did I spend on books in recent years?*

* *How many books I've bought each year?*

* *Which books were most expensive and which were the cheapest?*

* *Which genre, language, writer and Publications were most favoured?*

* *What is the average rate of books from each genre?*

* *Have I read all the books that I buy?*

* *If not, how many books are there still unread or partially read?*

## Tools Used: 

For this project a combination of 3 tools were used.

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
| Transaction_method | Online or Cash or None (if the books are free) |
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

![1](https://github.com/Arpita-deb/Do_I_read_all_the_books_I_buy/assets/139372731/60d26821-389e-4e5e-af90-49d37b7a3905)

About half of the collection contains Non - Fictions i.e books based on facts, actual events, or real people. In contrast, fiction is a genre of literature that describes imaginary settings, events, and characters. 

![2](https://github.com/Arpita-deb/Do_I_read_all_the_books_I_buy/assets/139372731/0ca6d12d-ce3d-45f3-bad4-c9bb4dfde5e0)

Paperbacks are my preferred type of books. Next comes ebooks which are very handy and mostly free of cost, makes up 30% of the collection.

![3](https://github.com/Arpita-deb/Do_I_read_all_the_books_I_buy/assets/139372731/f44a99e5-3ca8-4a1e-82f8-4dd642950d7b)

More than half of the collection of books are already read. But there remains about 36% of books that I haven't read yet or partially read.

![4](https://github.com/Arpita-deb/Do_I_read_all_the_books_I_buy/assets/139372731/f89f99e4-6901-41a9-ae28-5391558ccccb)

The reason behind ebooks being unread may be due to the fact that they remain in out of my sight in some corner of a computer file and partially due to their digital format which can be hard on my eyes. 

![5](https://github.com/Arpita-deb/Do_I_read_all_the_books_I_buy/assets/139372731/68df5401-3784-42d1-a73f-e87ca34d8218)

Over the course of 9 years, about ₹35,000 have been spent on books? Is it too much or too few? Well, let's drop the topic.

![6](https://github.com/Arpita-deb/Do_I_read_all_the_books_I_buy/assets/139372731/d4462c51-6b76-4e86-bd10-6f39f5b97c3c)

Majority of the books are paperbacks and costs in the range of ₹100-₹300.

![7](https://github.com/Arpita-deb/Do_I_read_all_the_books_I_buy/assets/139372731/9a389b13-21bc-4757-823e-97b1c6f22e59)

Approximately ₹20,000 were spent in 2020 and 2021 alone, a period marked by Covid 19. During that trying time when all other external activities were prohibited, reading has been a great way to spend my time productively.

![9](https://github.com/Arpita-deb/Do_I_read_all_the_books_I_buy/assets/139372731/cab8856d-1e87-416e-b27c-db80bbb2b5a2)

![8](https://github.com/Arpita-deb/Do_I_read_all_the_books_I_buy/assets/139372731/fdab856f-ff9e-4050-a942-b48781f00ae3)

![11](https://github.com/Arpita-deb/Do_I_read_all_the_books_I_buy/assets/139372731/24eb8c13-38f2-4984-a6d3-7699cd36139c)

![10](https://github.com/Arpita-deb/Do_I_read_all_the_books_I_buy/assets/139372731/73e0dde5-dcea-423a-b66d-bdefa45d1984)

![12](https://github.com/Arpita-deb/Sweet-Symphony-Dessert-Shop-SQL-Analysis/assets/139372731/56a40927-9719-4460-b113-d6675c5b0453)


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

## Dashboard:

For this project I've created an exploratory dashboard providing an overview of the dataset

In order to build the tableau visualizations and the dashboards, I've taken the following steps:

* Used tiled containers (vertical and horizontal) that contain the individual data visualizations

* Used title for the dashboards

* Used consistent color scheme that enhances the data

* Cleared the chart junks such as titles of individual data viz, axis and axis labels, color legends etc that doesn't contribute to the data design

* Visually grouped the data by using layout containers and colored background

* Added an info button at the top right corner that provides information about the project and dataset used

* Created device specific layouts

![Screenshot (526)](https://github.com/Arpita-deb/Do_I_read_all_the_books_I_buy/assets/139372731/00d464dd-bdbe-440d-8168-bdcd0ce5002f)

You can Check out my [Tableau Dashboard](https://public.tableau.com/views/DoIreadallthebooksthatIbuy/Dashboard4?:language=en-US&:display_count=n&:origin=viz_share_link) here.
