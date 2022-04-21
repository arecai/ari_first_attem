# Title

**Authors**: Ariadna Recasens

## Overview

Microsoft has decided to start a new film studio, but lack expertise in the field. In this project, we will explore different datasets obtained from 3 online databases of information related to film and provide insights to help Microsfot create top ranking movies. 

## Business Problem

Microsoft wants to explore the trending of creating original video content and has decided to create a new movie studio. Still, there is a complete lack of expertise in the field. This case study will provide actionable insights to help the head of Microsoft's new movie studio decide what type of films to create.
***
Some of the questions that we will consider are:
* What films are currently doing the best at the box office?
* What do they have in common (e.g. genre?)
* Who is behind their production? 
* In which studios where they created? 
* What was their budget?
***

## Data

This case study will explore data provided by some of the most reliable and well-know online database of information related to film:
* [IMDB](https://www.imdb.com/)
* [The Numbers](https://www.the-numbers.com/)
* [Box Office Mojo](https://www.boxofficemojo.com/)


***
In particular, we will use the following datasets:
* imdb.title.basics.csv.gz: 146144 entries with the following information: tconst, primary_title, original_title, start_year, runtime_minutes, genres.
* imdb.title.ratings: 73856 entries with the following information: tconst, averagerating, numvotes.
* imdb.name.basics.csv.gz: 606648 entries with the following information: nconst, primary_name, birth_year,  death_year, primary_profession, known_for_titles
* imdb.title.crew.csv.gz: 146144 entries with the following information: tconst, directors, writers.
* tn.movie_budgets.csv.gz: 5782 entries with the following information: id, release_date, movie, production_budget, domestic_gross, worldwide_gross.
* bom.movie_gross.csv.gz: 3387 entries with the following information: title, studio, domestic_gross, foreign_gross, year

Based on the questions provided in the business problem, the variable that we will focus are:
* Average ratings
* Total gross
* Studios that produced the top movies 
* Directors involved in top movies
* Budget

***

## Methods

To know what are the films that are doing the best, we will create top 20 list with the best movies. After exploring our available datasents and understanding which information we have available, we will create lists based on:

* **Ratings**: using IMDB datasets
* **Total gross**: using TN and BOM datasets


We want to focus on recent movies, so we will only select the past 5 years movies. The data collected in our datasets cover films from up to 2019, so we will set our range between 2015-2019. 

Furthermore, we will set up a minium of votes (at least 25,000 following the IMDB guidelines) to make our list more reliable.

Since we want to create lists based on rating and total gross, we will omit the raws that have no values in those fields. 

We will use these list to gain insights and help Microsoft to create a succesfull new film studio. 


## Results



### TOP20 IMDB highest rated movies 
![TOP20 IMDB highest rated movies](./images/top20_IMDB_movies.png)

## Conclusions

Provide your conclusions about the work you've done, including any limitations or next steps.

***
Questions to consider:
* What would you recommend the business do as a result of this work?
* What are some reasons why your analysis might not fully solve the business problem?
* What else could you do in the future to improve this project?
***

## For More Information

Please review our full analysis in [our Jupyter Notebook](./dsc-phase1-project-template.ipynb) or our [presentation](./DS_Project_Presentation.pdf).

For any additional questions, please contact **name & email, name & email**

## Repository Structure

Describe the structure of your repository and its contents, for example:

```
├── README.md                           <- The top-level README for reviewers of this project
├── dsc-phase1-project-template.ipynb   <- Narrative documentation of analysis in Jupyter notebook
├── DS_Project_Presentation.pdf         <- PDF version of project presentation
├── data                                <- Both sourced externally and generated from code
└── images                              <- Both sourced externally and generated from code
```
