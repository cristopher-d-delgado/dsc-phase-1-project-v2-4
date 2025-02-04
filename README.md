# Movie Analysis for Movie Production
**Author**: Cristopher Delgado 

## Overview 
This project analyzes movie characteristics such as genres, return on investment (ROI), and ratings. The data analysis performed in this repository is based on datasets from [Box Office Mojo](https://www.boxofficemojo.com/), [IMDB](https://www.imdb.com/), [Rotten Tomatoes](https://www.rottentomatoes.com/), [TheMovieDB](https://www.themoviedb.org/), and [The Numbers](https://www.the-numbers.com/).  
## Business Problem
Microsoft sees all the big companies creating original video content and they want to get in on the fun. They have decided to create a new movie studio, but they don’t know anything about creating movies. You are charged with exploring what types of films are currently doing the best at the box office. You must then translate those findings into actionable insights that the head of Microsoft's new movie studio can use to help decide what type of films to create.
> ### Business Understanding  
> Microsoft wants to enter the movie production business however as a rookie in this business they need insight on audience opinions about characteristics about movies. Audience opinions impact ROI. In addition to learning about what an audience enjoys, Microsoft must also consider when to release their movies to get the most ROI. 
## Data
The data analysis performed in this repository is based on datasets from [Box Office Mojo](https://www.boxofficemojo.com/), [IMDB](https://www.imdb.com/), [Rotten Tomatoes](https://www.rottentomatoes.com/), [TheMovieDB](https://www.themoviedb.org/), and [The Numbers](https://www.the-numbers.com/). The Box Office Mojo dataset contains information about movie domestic gross and worldwide gross. The IMDB database contains information about movie production team, cast, basic information, and ratings. The Rotten Tomatoes dataset contains information about critic reviews along with there rating and if the movie was fresh or rotten. The TheMovieDB dataset contains information about a movies genre, vote average, vote count, and popularity score. The Numbers dataset contains information about a movies production budget, domestic gross, worldwide gross, and release date. 
## Methods
This project analyzes the trends over time in regards to movie performance. The analysis can provide insight to movie production.
## Results 
The popularity score is a unique characteristic property in the TMDB dataset. 

The popularity score is the lifelong culmination of: 
- Number of votes for the day 
- Number of views for the day
- Number of users who marked it as a 'favorite' for the day 
- Release date
- Number of total votes 
- Accounts for the previous days score
> Information about the [popularity score](https://developer.themoviedb.org/docs/popularity-and-trending). 

It was essential to consider this score from the TMDB dataset to truly factor in many factors calculated by TMDB. This score is a good representation of popularity over the movies lifetime since the release date. Taking this score into consideration we can determine which genres are the most popular. 

![Popularity Score Based on Genre](images/image.png)

Sales are important in movie production as this will determine the ROI. Considering a movies characteristics such as intended audience and its release date can impact its Box Office Sale. As we can see PG-13 movies and PG make the most Box Office Sales which can make the most ROI. Releasing a movie at a certain tim of the year can impact the Box Office Sales as we can see below. 

![Sale Based on Appropriate Movie Audience](images/image-1.png)

![Sale Based on Month](images/Sales_Based_on_Month.png)

![ROI Domestic by Month](images/ROI_Domestic.png)

![ROI Worldwide by Month](images/ROI_Worldwide.png)

## Conclusion
This analysis has lead to three recommendations for Microsoft's new movie production studio:

- **Make movies with the following genres: Western, Romance, History, Animation, Family, Mystery, Thriller, Science Fiction, War, Crime, Fantasy, Action, Adventure.** These genres had a popularity score of 40 percent or higher which according to TMDB is considered good through excellent. 
- **Make movies with the intended Audience of PG-13 and PG.** These intended audience ratings proved to have the higher box office sales in comparison to rated R and G movies. 
- **Release movies in the summer time as well as the end of the year.** The time of the year matters when releasing movies. We can see this occur in the months of May, June, July, November, December and February. 

### Next Steps
Further analysis can provide additional insights for Microsoft and there new movie production studio. Other exploratory routes to take can be the following directions: 
- Explore the ROI based on director for the movie. Directors are important to any movie production as they will be the ones to organize and envision movie scenes and guide its production. The main goal is to pick the best director. 
- Create a model where you can predict the best years to release movies. Eventually any movie studio will have to create an organized timeline for movie releases especially if sequels are made. Predicting a year to release movies can be crucial to obtain the most ROI.
- Merge Box Office Mojo data with The Number since they contain similar information and look at the domestic gross made on average throughout the year. 

### Repository Structure 

```
├── images
├── zippedData
├── .gitignore
├── Movie Analysis for Future Movie Productions.pdf
├── PROJECTDESC.md
├── README.md
├── exploratory.ipynb
└── movie_analysis.ipynb
```
