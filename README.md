# JBOPS - Just a Bunch Of Plex Scripts

[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=4J6RPWZ9J9YML) 

Scripts pulled from my gist profile. https://gist.github.com/blacktwin

### PlexPy Script Arguments:
`-sn {show_name} -ena {episode_name} -ssn {season_num00} -enu {episode_num00} -srv {server_name} -med {media_type} -pos {poster_url} -tt {title} -sum {summary} -lbn {library_name} -grk {grandparent_rating_key} -ip {ip_address} -us {user} -uid {user_id} -pf {platform} -pl {player} -da {datestamp} -ti {timestamp} -purl {plex_url}`

#### Enabling Scripts:

In the Notification Agents in the Settings menu. Click the Scripts gear. Your scripts location will be there. Can't remember if it's set automatically or not. If not, then set it where you'll keep your scripts. Scroll down to option you want to use and select the script from the drop down menu. Save. Click the Bell next to Scripts and enable Recently Added. Then click Notifications. Scroll down to Scripts. Enter in the Script Arguments found in the .py script. Save.


## Scripts List

| Category | File | Description |
| :--- | :--- | :--- |
|[Maps](../tree/master/Maps "Look at this map")|||
||[ips_to_maps](../master/maps/ips_to_maps.py) | Use PlexPy draw a map connecting Server to Clients based on IP addresses.)|
|[Fun](../tree/master/fun "Fun Fun Fun Fun")|||
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/397f07724abebd1223ba6ea644ea1669)|[aired_today_playlist](../master/fun/aired_today_playlist.py) | Create a Plex Playlist with what was aired on this today's month-day, sort by oldest first. If Playlist from yesterday exists delete and create today's. If today's Playlist exists exit.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/4ccb79c7d01a95176b8e88bf4890cd2b)|[plexapi_haiku](../master/fun/plexapi_haiku.py)| Create a hiaku from titles found in Plex.|
|[Kill stream](../tree/master/killstream "Kill Kill Kill")|||
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/e1d199d98b258d6f2658dd9991c88ca0)|[create_wait_kill_all](../master/killstream/create_wait_kill_all.py)|Receive session_key from PlexPy when paused. Use session_id to create sub-script to wait for X time then check if still paused. If paused kill.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/2148bb0b2f8d67b8a08c50ace62ad39f)|[create_wait_kill_trans](../master/killstream/create_wait_kill_trans.py)|Receive session_key from PlexPy when paused. Use session_id to create sub-script to wait for X time then check if transcoding still paused. If so, kill.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/88fce565c8ecf56839641f22f4c5c422)|[kill_all_more_than](../master/killstream/kill_all_more_than.py)|If user has 2 or more concurrent streams kill all streams|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/d47d3ada86d02a494f9dc33e50dd15b5)|[kill_else_if_buffering](../master/killstream/kill_else_if_buffering.py)|Kill concurrent transcode streams of other users if Admin user is experiencing buffering warnings from PlexPy.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/6d08b94ca3e80d3ed0bb3c7172fae21d)|[kill_more_than](../master/killstream/kill_more_than.py)|If user has 2 or more concurrent streams and the IP of the 2nd stream differs from 1st kill 2nd. If 2nd stream IP is the same as 1st stream don't kill.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/eee23eeb95f1285fbb495c5a8592b242)|[kill_outsider_stream](../master/killstream/kill_outsider_stream.py)|Kill stream if user is outside of local network.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/8b174165cfc5e5e80c6698a1494fc9ee)|[kill_plex_stream](../master/killstream/kill_plex_stream.py)|Kill any Plex stream for whatever reason you want.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/77f6f1be32621ed71655ca27406ef772)|[kill_session_bitrate](../master/killstream/kill_session_bitrate.py)|Kill stream if bitrate is greater than 4 Mbps|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/0e6207346acfaaca602eb7dce80226a0)|[kill_trans_exp_audio](../master/killstream/kill_trans_exp_audio.py)|Kill Plex video transcoding streams only. All audio streams are left alone. Kill message based on platform.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/14d400a0f442da465389164fa046647a)|[new_kill_trans_pause](../master/killstream/new_kill_trans_pause.py)|Kill Plex paused video transcoding streams using PlexPy.|
|[Notify](../tree/master/notify "Notify")|||
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/e6d589a9af9bdf168717951083861e93)|[find_unwatched_notify](../master/notify/find_unwatched_notify.py)|Find what was added TFRAME ago and not watched and notify admin using PlexPy.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/1094dcf38249f36c8d374e0cba7a86cd)|[notify_added_custom](../master/notify/notify_added_custom.py)|Send an email with what was added to Plex in the past week using PlexPy. Email includes title (TV: Show Name: Episode Name; Movie: Movie Title), time added, image, and summary.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/099c07d8099c18a378bba6415d9253ba)|[notify_fav_tv_all_movie](../master/notify/notify_fav_tv_all_movie.py)|Notify users of recently added episode to show that they have watched at least LIMIT times via email. Also notify users of new movies.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/a2d4b2f2c3b616f1d6da0752fecb2ae7)|[notify_newip](../master/notify/notify_newip.py)|If a new IP is found send notification via the Email Notification Agent. Email contains User's Avatar image, link to location, IP address, and User's Email address.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/a327055da54d7feb3eef10e64a8b661a)|[notify_on_added](../master/notify/notify_on_added.py)|Send an Email notification when a specific show is added to Plex. Add shows to list that you want notifications for.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/18960ff01c03b67a05594daa6f53660c)|[notify_user_favorites](../master/notify/notify_user_favorites.py)|Notify users of recently added episode to show that they have watched at least LIMIT times via email.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/066c66328a795ebd6079a575e14f0b8b)|[notify_user_newip](../master/notify/notify_user_newip.py)|Notify user that their account has been accessed by a new IP. IP is cleared to make sure notification is sent again.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/261c416dbed08291e6d12f6987d9bafa)|[twitter_notify](../master/notify/twitter_notify.py)|Post to Twitter when TV/Movie is added to Plex. Include custom message and embed poster image. Option to tweet to TWITTER_USER if title is inside TITLE_FIND.|
|[Utility](../tree/master/utility "Utilities")|||
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/f4149c296f2d1ffd1cbd863c37bb3a3c)|[bypass_auth_name](../master/utility/bypass_auth_name.py)|Use PlexPy to pull last IP address from user and add to List of IP addresses and networks that are allowed without auth in Plex.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/0332f2dc9534bdf412ff3f664e9513c0)|[delete_watched_TV](../master/utility/delete_watched_TV.py)|From a list of TV shows, check if users in a list has watched shows episodes. If all users in list have watched an episode of listed show, then delete episode.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/76b0abf88181618af4598092dd6b0dbb)|[find_plex_meta](../master/utility/find_plex_meta.py)|Find location of Plex metadata.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/603d5da5b70b366e98d0d82d1aa1a470)|[find_unwatched](../master/utility/find_unwatched.py)|Find what was added TFRAME ago and not watched using PlexPy.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/f435aa0ccd498b0840d2407d599bf31d)|[grab_gdrive_media](../master/utility/grab_gdrive_media.py)|Grab media (videos, pictures) from Google Drive. All videos and pictures were automatically synced from Google Photos to Google Drive. Puts media into MEDIA_TYPE/YEAR/MONTH-DAY/FILE.ext directory structure.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/85a63ffd70c6ccb7c1faa70a8f33fc2e)|[plex_api_poster_pull](../master/utility/plex_api_poster_pull.py)|Pull Movie and TV Show poster images from Plex.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/17b58156f69cc52026b71fe4d5afea05)|[plex_imgur_dl](../master/utility/plex_imgur_dl.py)|Pull poster images from Imgur and places them inside Shows root folder.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/f10e0a1e85af00e878963b4570a99054)|[plex_theme_songs](../master/utility/plex_theme_songs.py)|Download theme songs from Plex TV Shows.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/45c420cbba4e18aadc8cc5090a67b9d1)|[plexapi_delete_playlists](../master/utility/plexapi_delete_playlists.py)|Delete all playlists from Plex using PlexAPI.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/df58032de3e6f4d29f7ea562aeaebbab)|[plexapi_search_file](../master/utility/plexapi_search_file.py)|Find full path for Plex items.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/3752a76fa0b3fc6d19e842af7b812184)|[refresh_next_episode](../master/utility/refresh_next_episode.py)|Refresh the next episode of show once current episode is watched.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/370ca42ee20a33fb00c8253fa9bd0de7)|[remove_watched_movies](../master/utility/remove_watched_movies.py)|Find Movies that have been watched by a list of users. If all users have watched movie then delete.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/2f619e62d99edcec27f680998379664c)|[stream_limiter_ban_email](../master/utility/stream_limiter_ban_email.py)|This is indented to restrict a user to the LIMIT amount of concurrent streams. User will be warned, punished, and banned completely if violations continue.|
|[Reporting](../tree/master/utility "If you could go ahead and... That’d be great..")|||
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/21823b3394f5b077d42495b21570b593)|[added_to_plex](../master/reporting/added_to_plex.py)|Find when media was added between STARTFRAME and ENDFRAME to Plex through PlexPy.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/f070dff29ddbeb87973be9c0a94a1df7)|[check_play](../master/reporting/check_play.py)|Check if user has play a file more than 3 times but has not finished watching. Hoping to catch play failures.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/1a8933252ad1a9bc2c97395a020c144a)|[check_plex_log](../master/reporting/check_plex_log.py)|Checking plex logs for debug code WARN and 'Failed to obtain a streaming resource for transcode of key /library/metadata/"titleID"'.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/561c3a404754eb7b9e543867619d3251)|[drive_check](../master/reporting/drive_check.py)|Check if drive exists. If not then notify via PlexPy notifier agent.|
|[![](https://img.shields.io/badge/gist-original-green.svg)](https://gist.github.com/blacktwin/bd905d39ab71c5d7c628e27fddd1086e)|[userplays_weekly_reporting](../master/reporting/userplays_weekly_reporting.py)|Use PlexPy to count how many plays per user occurred this week and send email via PlexPy.|
