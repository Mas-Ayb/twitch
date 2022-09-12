# twitch
Browse Twitch website to extract streamers data

This code is used to browse twitch website in order to provide data of streamers. As the website does not provide API to get all the users data once, we first get all the streams. Then, the streams are filtered based on a tag (e.g. Iran tag). After that, the streams' usernames are applied to access the streamers links. Finally, streamers data such as number of viewers, followers, start data and so on are extracted by scraping.
