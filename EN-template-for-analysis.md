**November 9th 2025**<br>
**MPAD 2003-A**<br>
**Gilven Senires, Annabel Young and Kiana Emile**<br>
**Presented to Jean-Sébastien Marier**<br>

# Exploratory Data Analysis (EDA) & Pitch

Use one hashtag symbol (`#`) to create a level 1 heading like this one.

## Foreword

For this assignment, you must extract data from a dataset provided by the instructor. You must then clean and analyze the data, create exploratory charts/visualizations, and find a potential story idea. Your assignment must clearly detail your process. You are expected to write about 1500-2000 words, and to include several screen captures showing the different steps you went through. Your assignment must be written with the Markdown format and submitted on GitHub Classroom.

I have been assigning different versions of this project to my digital journalism and data storytelling students for a few years now. Its structure was inspired by the main sections/chapters of [*The Data Journalism Handbook*](https://datajournalism.com/read/handbook/one/). This version was further inspired by the [Key Capabilities in Data Science](https://extendedlearning.ubc.ca/programs/key-capabilities-data-science) program offered by the University of British Columbia (UBC).

**Here are some useful resources for this assignment:**

* [GitHub's *Basic writing and formatting syntax* page](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
* [The template repository for this assignment in case you delete something by mistake](https://github.com/jsmarier/jou4100_jou4500_mpad2003_project2_template)

Did you notice how to create a hyperlink? In Markdown, we put the clickable text between square brackets and the actual URL between parentheses.

And to create an unordered list, we simply put a star (`*`) before each item.

## 1. Introduction

For this assignment, we will be analyzing a City of Ottawa dataset to explore the question: How many people of the Indigenous groups graduate with a university degree or diploma (post-secondary education) in the city of Ottawa? The dataset, titled “2021 Long Form Census - Ward Data” was collected through the 2021 Census and published on the [Open Ottawa](https://open.ottawa.ca/datasets/ottawa::2021-long-form-census-ward-data/explore) platform. In our context, it provides demographic data about Ottawa’s population, including Indigenous identity, status, ancestry, and various education levels. The information was gathered by Statistics Canada and is organized into categories that show both total population counts and breakdowns of educational attainment. The dataset can be accessed on Open Ottawa and the CSV version is available on this [GitHub portal](https://github.com/jsmarier-courses/exploratory-data-analysis-and-pitch-mpad2003-f25-group-4). This project is divided into five main sections. It starts with the “Getting Data” section, which explains how the dataset was sourced and imported. The next major section, Understanding Data, includes three subsections, “VIMO Analysis, Cleaning, and Exploratory Data Analysis (EDA).” In these subsections, we review the dataset’s validity by identifying any missing, invalid, or outlier values and assessing its overall accuracy. To make the data easier to interpret, we will clean the spreadsheet and create both a table and a chart to provide a clearer visual overview. Following that, the “Potential Story” section uses the cleaned data to propose a possible story that connects the data to actuality. Finally, the “Conclusion” summarizes the overall experience, reflecting on strengths, challenges, and what could have been improved during the process. The project ends with a “References” section formatted according to APA guidelines.

## 2. Getting Data

To import the data into Google Sheets, we used the link provided in the Dataset category titled “2021 Long Form Census – Ward Data.” The link redirected us to the City of Ottawa’s dataset page, where the origin and reliability of the data are briefly explained. The census data came from both short and long questionnaires; the short one was sent to every household for a general overview, and the long one was sent to 25% of households for more detailed information. Yet, for this project, we worked specifically with the Long Form Census, which the City of Ottawa made available as a downloadable table. Instead of downloading the CSV file, we imported the dataset directly into Google Sheets. To do this, we right-clicked the dataset link, selected “Copy link address,” and in a new spreadsheet, we used the formula: `IMPORTDATA`. This automatically imported the complete dataset from the Long Form Census. Finally, to make the data editable, we converted the imported information into plain values. Since we couldn’t remember the keyboard shortcut, in the Google Sheets we clicked on Edit then Paste special, then Values only. This allowed us to create a fully customizable spreadsheet based on the data provided by the City of Ottawa.

With 26 columns and 2,603 rows, our first impression of the dataset was that it looked overwhelming. At first glance, we felt confused and unsure where to even start. The data appeared unclean and disorganized, making it difficult to sort through the endless rows and columns. Many of the row descriptions were duplicates, which made it harder to tell sections apart and understand what each value referred to. The most confusing part was Column A, labeled “Characteristics.” Its sections were formatted inconsistently, each containing different variable types that seemed scattered with no clear structure. Overall, the dataset wasn’t visually appealing and was quite unclear to navigate at first. 

![](dataset-screen-capture.png)
*Figure 1: The "Dataset" prompt on Google Sheets just after importation.*

**Public Link to Google Sheets Spreadsheet:**
* [2021 Long Form Census - Ward Data](https://docs.google.com/spreadsheets/d/16wwc8f8S7XUzIEwFFINbTcRVEzD9WPAFdmFGat0rJ5g/edit?usp=sharing)

To simplify things, we decided to keep only Columns A and B, focusing on two main sections: Indigenous identity types and education levels. In terms of variables, Column A, titled “Characteristics,” includes nominal variables because it lists categories instead of numbers. Such as Indigenous identity, Métis, etc, or the Highest certificate, diploma, or degree. According to Statistics: Power from Data! in the “Types of Variables” section under nominal variables, these labels are used “to name and organize the data, but there’s no particular order between them.” Whereas Column B, which lists “City of Ottawa,” contains discrete numerical variables. From the same site under discrete variables, however, these are countable numbers that represent population totals within each category, for instance, 26,395 Indigenous identity, which are fixed counts of people. Moreover, within the education section, the dataset also involves ordinal variables, like “No certificate, diploma, or degree,” “High school diploma,” “Bachelor’s degree,” etc.  These are ordered categories because each represents a different level of educational accomplishment, ranking from lower to higher qualifications. What we found that was missing is that while Ottawa shows a highly educated population overall, with more than ​550,005 people having postsecondary education the data doesn’t reveal how education levels differ across groups. For example, whether Indigenous populations have the same access to higher education. Including this context could have been a potential story about educational access and equity in Ottawa.

**Here are examples of functions and lines of code put in grey boxes:**

1. If you name a function, put it between "angled" quotation marks like this: `IMPORTHTML`.
1. If you want to include the entire line of code, do the same thing, albeit with your entire code: `=IMPORTHTML("https://en.wikipedia.org/wiki/China"; "table", 5)`.
1. Alternatively, you can put your code in an independent box using the template below:

``` r
=IMPORTHTML("https://en.wikipedia.org/wiki/China"; "table", 5)
```
This also shows how to create an ordered list. Simply put `1.` before each item.

## 3. Understanding Data

### 3.1. VIMO Analysis

Use three hashtag symbols (`###`) to create a level 3 heading like this one. Please follow this template when it comes to level 1 and level 2 headings. However, you can use level 3 headings as you see fit.

Insert text here.

Support your claims by citing relevant sources. Please follow [APA guidelines for in-text citations](https://apastyle.apa.org/style-grammar-guidelines/citations).

**For example:**

As Cairo (2016) argues, a data visualization should be truthful...

### 3.2. Cleaning Data

Insert text here.

### 3.3. Exploratory Data Analysis (EDA)

Insert text here.

**This section should include a screen capture of your pivot table, like so:**

![](pivot-table-screen-capture.png)<br>
*Figure 2: This pivot table shows...*

**This section should also include a screen capture of your exploratory chart, like so:**

![](chart-screen-capture.png)<br>
*Figure 3: This exploratory chart shows...*

## 4. Potential Story

Insert text here.

## 5. Conclusion

Insert text here.

## 6. References

Include a list of your references here. Please follow [APA guidelines for references](https://apastyle.apa.org/style-grammar-guidelines/references). Hanging paragraphs aren't required though.

**Here's an example:**

Bounegru, L., & Gray, J. (Eds.). (2021). *The Data Journalism Handbook 2: Towards A Critical Data Practice*. Amsterdam University Press. [https://ocul-crl.primo.exlibrisgroup.com/permalink/01OCUL_CRL/hgdufh/alma991022890087305153](https://ocul-crl.primo.exlibrisgroup.com/permalink/01OCUL_CRL/hgdufh/alma991022890087305153)
