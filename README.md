### WeRateDogs
#### Data wrangling of WeRateDogs tweets including gathering and analysis.
#### Data Gathering
#### Read data from twitter-archive-enhanced.csv 
#### write tweet_json.txt from the api
#### Source 1
#### Save the retweet and favorite counts for each tweet ID in a new pandas DataFrame 
#### Source 2
#### Download image-predictions.tsv from the url 
#### create the image_prediction dataframe from image-predictions.tsv
#### Source 3
#### create twitter-archive-enhanced dataframe from twitter-archive-enhanced.csv
#### Assessment
#### Visual assessment¶
#### Data Wrangling
#### Analyse data type,size,null,duplicates,unique etc for all 3 sources
#### Issues noted during visual and programmatic assessment is done by opening the twitter_archive_enhanced.csv in google sheets
#### Quality Issue in twitter_archive_enhanced.csv
#### Issue 1. Retweet id is present for many rows
#### Issue 2. Ratings are accessed by programmatic addition of column ratings and fixing the rows with 0 denominator values
#### Issue 3. 181 are retweet
#### Issue 4. in_reply_to_status_id is float and has nulls
#### Issue 5. in_reply_to_user_id is float and has nulls
#### Issue 6. retweeted_status_id,retweeted_status_user_id are not needed for analysis.
#### Issue 7. Names with value 'None' or 'a'
#### Issue 8. tweet_id is defined as object and int64
#### Issue 9. timestamp is object
#### Issue 10 expanded_url is null
#### Quality Issue in jason
#### Issue 11. tweet_id, retweet_count & favorite_count are object.
#### Tidyness issues
#### Issue 12. Columns doggo ,floofer, pupper, puppo need to be under one column heading DoggoLingo
#### Issue 13. Column retweet_count , favorite_count of jtweet_jason_df need to be with columns of twitter_archive_enhanced.csv as it makes more relevance along with other variables
#### Issue 14. Image and highest prediction need to be with columns of twitter_archive_enhanced.csv as it makes more relevance along with other variables
#### Clean
#### Exploratory Data Analysis
