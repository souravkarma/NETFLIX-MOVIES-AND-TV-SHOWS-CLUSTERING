# NETFLIX-MOVIES-AND-TV-SHOWS-CLUSTERING
# Netflix-Movies-and-Tv-Shows
NLP , Clustering

## 📖Introduction
Netflix, the world’s largest on-demand internet streaming media and online DVD movie rental service provider.it Founded August 29, 1997, in Los Gatos, California by Marc and Reed. It has 69 million members in over 60 countries enjoying more than 100 million hours of TV shows and movies per day Netflix is the world’s leading internet entertainment service with enjoying TV series, documentaries, and feature films across a wide variety of genres and languages. I was curious to analyze the content released in Netflix platform which led me to create these simple, interactive, and exciting visualizations and find similar groups of people.

## Project Summary :
#### Problem Statement : 
This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine.<br>
In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.<br>
Integrating this dataset with other external datasets such as IMDB ratings, rotten tomatoes can also provide many interesting findings.<br>




#### About the Data :
We have the data of which contains details of customers like id , age, gender and also contains the details of the customers vehicle 


**Dataset info**

* 1. Number of records: 7787

* 2.Number of features: 12

### **Features information:**

The dataset contains features like:

* **show_id :** Unique ID for every Movie / Tv Show<br>
* **type :** A Movie or TV Show<br>
* **title :** Title of the Movie / Tv Shows<br>
* **director :** Director of the Movie<br>
* **cast :** Actors involved in the movie / show<br>
* **country :** Country where the movie / show was produced<br>
* **date_added :** Date it was added on Netflix<br>
* **release_year :** Actual Release year of the movie / show<br>
* **rating :** TV Rating of the movie / show<br>
* **duration :** Total Duration - in minutes or number of seasons<br>
* **listed_in :** Generes<br>
* **description:** The Summary description<br>


**Project Work flow**
----------------------------

1.Understand the dataset and problem statement
2.Exploratory Data Analysis
3.Dealing with missing values and outliers
4.Data Cleaning
5.Exploring Exceptional Cases
6.Pre-processing-TFIDF/bag of words
7.Selecting the approach and alogorithm to be used
8.Brief strategy for cluster formed
9.Future Work
10.Conclusion

## **Future Work**
From this clustering analysis we can create Netflix movies and tv shows
recommendation systems & also we can use topic modelling.

## **Conclusion**
1. In dataset we got 2389 null values in director, 718 in cast, 507 in country, 10 in date_added, 7 in rating column. after analyzing type column we got netflix has more movies than tv shows.(69% movies and 31% tv shows)
It defines that movies on netflix have high demand among people so netflix should focus more good quality movies and increase their business opportunity.

2. In title column we got 'Love','Man','World','Story','Life' seems very common word.overwhelming number of content having 'Christmas'also.We are suspecting "Christmas" titles to be a very seasonal thing with most of the shows likely to be released during the month of December.

3. After analyzing director column we got Raul Campos, jan suter combinely best director who directs most movies(18) in netflix followed by marcus roby(16), jay karas(14), catthy garcia-molina(13).

4. Anupam Kher is the most popular actor in netflix followed by sharukhkhan, nashiruddin shah,om puri,akshay kumar etc.
Anupam kher's movie count is over 40 in netflix and for sharukhkhan it is 35. even no body is nearer to them in terms of movie count in netflix. It defines that netflix prefers both of them very much in their movies.

5. From country column we can find that The United States stands out on top since Netflix is an American company.
India comes in second followed by the UK and Canada.

6. After analyzing date-added column we find 2018 has highest movie counts in netflix followed by 2017,2016,2015 etc.
year by year movie counts are increasing it defines public likes netflix content year by year and new public joins netflix. so it defines sustainable growth of netflix.

7. We can see that total contents in netflix sharply increases after 2015 this may because internet revolution in all over the world specially in big populated country like India.
In 2020 movie counts are higher than tv shows.
tv shows contents are sharply decreased after 2018 this shows people interest towards movie more in netflix.

8. Afteranalyzing rating column we find Most of the programme in netflix are TV-MA(36.8%) and TV-14(24.8%) rated
Most of the content in netflix are mature content.
 younger audience (under the age of 17), it is the opposite, there are slightly more TV shows than there are movies.
It defines may be young people are more fond of tv shows

9. From duration column we got Most movies in netflix have 70-120 min duration and Most of the tv shows are 1 to 2 seasons long.

10. from listed_in column we have created genres.from genres we can see that International Movies,Dramas,Comedies,International Tv shows are most popular genres on netflix.
TV thrillers, tv shows, classic & cult shows these are very bad genres and allmost no popularity.
Even though the United States has the most content available, it looks like Netflix has decided to release a ton of international movies. 

11. From country vs genres trend we find International Movies,Comedies,Dramas etc are most popular genres in most of the countries including US,India,France etc.
Interestingly US people prefers drama, comedies genres more as netflix is an us company so they do not prefer international movies much in netflix.
Indian people prefers international movies in netflix like most of other countries.
so from this we can conclude that netflix should focus more on their international movie and tv shows as people likes and consumes their content most often from all over the world. It will surely impacts their businesses positively.

12. From country vs rating trend we find TV-MA( Mature content) is the most popular rating in netflix in most of the countries.
In India and China TV-14 is the most rated while TV-MA rated movies are 2nd best preffered.
US,france,Israel,UK all countries watch TV-MA rated movies mostly.
It concludes that Netflix should focuses more on mature content movies quality as most of the countries all over world likes it in netflix.it should increase their content watch hours and business opportunities.

13. From country vs type trend we find most countries preferred movies over tv shows in netflix .
It concludes that to expand their business netflix should produce more tv shows and must increase the quality of movies as it is their most popular type.

14. we can see december month relesed most content in netflix followed by october,november,january.

15. 
    * In text analysis (NLP) and data pre-processing I removed punctuations,stop words as they are unhelpful part  then we count vocabulary items using countvectorizer() which create dictionary of most frequent important words.
    * To normalize the text we use stemming here.Through text vectorization process we transform text into a meaningful representation of numbers which is used to fit a machine learning algorithm for prediction here we use Tf-IDF vectorization as it contains contains information on the more important words and the less important ones as well.
    * seref,orai,lukasz these words are top in vocab present in description and top vocabulary present in listed_in are tv,thriller,teen,talk etc.

16. By applying the silhouette score method for n
range clusters on dataset we got best score for 3 clusters it means content explained
well on their own clusters, by using elbow
method after k = 3 curve gets linear it means k =
3 will be the best cluster.

17. From DBSCAN clustering algorith we identified different shapes and sizes from a large amount of data, which is containing noise and outliers.Applied different clustering models like Kmeans, hierarchical, Agglomerative clustering,DBSCAN on data we got the best cluster arrangements.

18. After creating recommendation system based on description and genre we got best movies according to our recent interest. for example for "Indiana Jones and the Last Crusade" movie first two results are highly recommended and those are also Indiana Jones series movie.It will defnetly increases watch time, content retention and impacts netflix business with more profitability and business opportunities. 

 
 

Miscellaneous :
* Google colab tools
