# Spotify_Playist_Generator
Automated Spotify with python.
A simple script that takes your liked videos on Youtube, and generates a Spotify playlist based on the song in your liked videos.
Table of Contents
•	Video
•	Technologies
•	Setup
•	ToDo
•	Troubleshooting
Video
Check out the youtube video for a step by step walk through Youtube Video
Technologies
•	Youtube Data API v3
•	Spotify Web API
•	Requests Library v 2.22.0
•	Youtube_dl v 2020.01.24
LocalSetup
1.	Install All Dependencies
pip3 install -r requirements.txt
2.	Collect You Spotify User ID and Oauth Token From Spotfiy and add it to secrets.py file
o	To Collect your User ID, Log into Spotify then go here: Account Overview and its your Username  
o	To Collect your Oauth Token, Visit this url here: Get Oauth and click the Get Token button  
3.	Enable Oauth For Youtube and download the client_secrets.json
o	Ok this part is tricky but its worth it! Just follow the guide here Set Up Youtube Oauth ! If you are having issues check this out Oauth Setup 2 and this one too Oauth Setup 3
4.	Run the File
python3 create_playlist.py
o	you'll immediately see Please visit this URL to authorize this application: <some long url>
o	click on it and log into your Google Account to collect the authorization code
ToDo
•	Tests
•	Add Error Handling
Troubleshooting
•	Spotify Oauth token expires very quickly, If you come across a KeyError this could be caused by an expired token. So just refer back to step 3 in local setup, and generate a new token!

