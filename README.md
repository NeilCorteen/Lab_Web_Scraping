## The aim of the project was to collate music data for use in a machine learning application to make user recommendations.

### Neil Corteen, May 2021

Music was collated music using various methods:
- Web scraping, single pages/
- Web scraping, multiple pages/
- Application Programming Interface (APIs)/
- Application Programming Interface (API) Wrappers/

The main websites used were:
- www.billboard.com
- www.spotify.com
- www.imdb.com


Initial steps explored how to extract data from websites using the html and css code.

A basic testing phase with annotations can be seen [here](./Webscraping_basic_testing_with_annotations.ipynb)

An example of extracting data from billboard using html/css data and then collating the information in a dataframe can be seen [here](./Webscraping_Billboard_Top100.ipynb)

An example of using an API functions from Spotify and then collating the information in a dataframe can can be seen here: 



### A full outline of the exercise:
Business goal:
•	Check the case_study_gnod.md file.
•	Make sure you've understood the big picture of your project:
o	the goal of the company (Gnod),
o	their current product (Gnoosic),
o	their strategy, and
o	how your project fits into this context.
Re-read the business case and the e-mail from the CTO, take a look at the flowchart and create an initial Trello board with the tasks you think you'll have to accomplish.
Instructions - Scraping popular songs
Your product will take a song as an input from the user and will output another song (the recommendation). In most cases, the recommended song will have to be similar to the inputted song, but the CTO thinks that if the song is on the top charts at the moment, the user will enjoy more a recommendation of a song that's also popular at the moment.
You have find data on the internet about currently popular songs. Billboard maintains a weekly Top 100 of "hot" songs here: https://www.billboard.com/charts/hot-100.
It's a good place to start! Scrape the current top 100 songs and their respective artists, and put the information into a pandas dataframe.

### Case Study: The site for recommendations - "Gnod"
###Scenario
  
You have been hired as a Data Analyst for "Gnod".
"Gnod" is a site that provides recommendations for music, art, literature and products based on collaborative filtering algorithms. Their flagship product is the music recommender, which you can try at www.gnoosic.com. The site asks users to input 3 bands they like, and computes similarity scores with the rest of the users. Then, they recommend to the user bands that users with similar tastes have picked.
"Gnod" is a small company, and its only revenue stream so far are adds in the site. In the future, they would like to explore partnership options with music apps (such as Deezer, Soundcloud or even Apple Music and Spotify). However, for that to be possible, they need to expand and improve their recommendations.
That's precisely where you come. They have hired you as a Data Analyst, and they expect you to bring a mix of technical expertise and business mindset to the table.
Jane, CTO of Gnod, has sent you an email assigning you with your first task.
Task(s)
  
This is an e-mail Jane - CTO of Gnod - sent over your inbox in the first weeks working there.
Dear xxxxxxxx, We are thrilled to welcome you as a Data Analyst for Gnoosic!
As you know, we are trying to come up with ways to enhance our music recommendations. One of the new features we'd like to research is to recommend songs (not only bands). We're also aware of the limitations of our collaborative filtering algorithms, and would like to give users two new possibilities when searching for recommendations:
  
•	Songs that are actually similar to the ones they picked from an acoustic point of view.
•	Songs that are popular around the world right now, independently from their tastes.
  
Coming up with the perfect song recommender will take us months - no need to stress out too much. In this first week, we want you to explore new data sources for songs. The Internet is full of information and our first step is to acquire it do an initial exploration. Feel free to use APIs or directly scrape the web to collect as much information as possible from popular songs. Eventually, we'll need to collect data from millions of songs, but we can start with a few hundreds or thousands from each source and see if the collected features are useful.
Once the data is collected, we want you to create clusters of songs that are similar to each other. The idea is that if a user inputs a song from one group, we'll prioritize giving them recommendations of songs from that same group.
On Friday, you will present your work to me and Marek, the CEO and founder. Full disclosure: I need you to be very convincing about this whole song-recommender, as this has been my personal push and the main reason we hired you for!
Be open minded about this process: we are agile, and that means that we define our products and features on-the-go, while exploring the tools and the data that's available to us. We'd love you to provide your own vision of the product and the next steps to be taken.
Lots of luck and strength for this first week with us!
-Jane
