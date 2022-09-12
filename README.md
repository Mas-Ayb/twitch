# Twitch
Browse Twitch website to extract streamers data

## Description
This code is used to browse twitch website in order to provide data of streamers. As the website does not provide API to get all the users data once, we first get all the streams. Then, the streams are filtered based on a tag (e.g. Iran tag). After that, the streams' usernames are applied to access the streamers links. Finally, streamers data such as number of viewers, followers, start data and so on are extracted by scraping.

## Requirement
In this example, the following libraries are used:
- pandas
- requests
- datetime
- bs4
- selenium
- lxml
- sys

If selenium library and chrome driver are not installed by default, they can be installed by following codes:

! pip install selenium

! apt install chromium-chromedriver

For accessing Twitch APIs, **Client Id** and **Client Secret** are required. To get these values, it is necessary to register in twitch website. More details can be found in this link:

https://dev.twitch.tv/docs/authentication

## File structure
Code in Jupyter Notebook can be found in __Twitch.ipynb__

## Goals
The following goals are reached in this example:
1) Working with APIs
2) Web scraping
3) Applying Selenium library instead of popular BeautifulSoup in order to scrape dynamic js pages
4) Working with pandas dataframes

## Results
The followng streamers' data is stored in dataframe:
- user_id
- user_name
- type
- broadcaster_type
- description
- profile_image_url	offline_image_url
- view_count
- created_at
- days_from_create
- followers
- follower_acquisition_rate
- total_videos_watching_minutes

## Future works
In future, more data of streamers for analysing can be added. In the analysis, visualization can be applied to make it more understandable.
