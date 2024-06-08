Repository containing Jupyter notebook on the prediction of La Liga matches based on past data/events.
Use the request function to load website.
Import and use BeautifulSoup python library to scrape website data.
Get links for all teams by using the anchor tag.
Read the downloaded HTML file into a dataframe(Matches).
Use BeautifulSoup to scrape shooting data stats from website.
Read downloaded shooting HTML file into a dataframe(Shooting).
Merge both dataframes together into a new dataframe.
Do the merge on the date column(Team_data).
Scrape data for multiple teams and seasons with a 'for' loop(All Teams, Two seasons[2022-2024].
Use "a.prev" on BS to scrape for previous seasons.
Use the for loop to individually scrape match logs for all teams, get links for teams using the anchor tag, get shooting stats using "all_comps/shooting/" and read the dataframes individually.
Merge corresponding Sores & Fixtures dataframes with Shooting stats dataframe.
Specify that you need data with only La Liga competitions in them.
Append team_data to the all_matches list.
Use 'time.sleep' so not to get IP flagged for continuous scraping.
Concatenate all dataframes to a single dataframe(All_matches).
Write data to a csv file.
Convert Date for object to date_time attribute Convert Venue, opponent to categorical codes.
Create new column "Day_code" by converting Date to 'dayofweek'.
Create target column from result and use categorical codes for encoding.
Using Random Forest Classifier, build a model for predicting test data based on train data.
Use accuracy score to see percentage of correct predictions.
Use precision score to know percentage of wins when wins were predicted.
Create one dataframe for every squad in data(grouped_matches).
Apply rolling averages funtion to each team in our dataframe.
Use the make_predictions funtion to retrain models.
Merge in specific columns into our data based on corresponding index numbers.
