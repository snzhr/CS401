# CS401
project for insformation security. This tutorial is only in educational purpose.

# SocialFish

For SocialFish you need python 3.x . I have run SocialFish in Linux, so I will describe how to run in Linux.
Once you cloned or downloaded my github repository (CS401), you have to open SocialFish phishing directory. ($ cd SocialFish phishing)
Then you need run SocialFish.py (as it was written in Python 3, $ python3 SocialFish.py)
Then it will open in terminal. After that you will see 2 options, 1. Social Media, 2.Others. 
You have to choose Social Media (s). It will return you list of Social Media. When you will choose one of them, you have to type redirect url, when submit button clicked will redirect our victim to the original website. Then "ngrok" will create a link for our phishing web page. It's done. When victim will enter login credentials, you will see in terminal.

# Weeman 

For weeman you need python 2.x , and Ngrok(you have to download it from official website (https://ngrok.com/download)) 
Then open the "weeman phishing" directory in terminal. Run it ( $ ./weeman.py ). It returns weeman bash. First you need to type 
weeman >  set url http://facebook.com(e.g.)
weeman >  set port 8080(e.g.)       
weeman >  set action_url https://facebook.com(e.g.),   (will redirect to orinal website login page_
weeman >  run

Then you will see the link to your local machine (http://localhost:8080), this link is our phishing page. So, how to send this link to the victim or someone? For this situation you will need Ngrok. It opens a tunnel to our localhost, or creates a link to localhost.

Once you have downloaded ngrok, unzip it, then type ./ngrok, it will show more info about itself. One more thing, you have to sign up to ngrok for proper work. Then you have to copy your authtoken (you will find it ngrok account page), and type next in terminal ($ ./ngrok authtoken your token).
Then you can use it. As we set our port as 8080 from weeman, we have to type ($ ./ngrok http 8080), if you change port from weeman, type that port to ngrok. You will see links to your localhost8080, which is phishing page. 