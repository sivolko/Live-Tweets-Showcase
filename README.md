# Live Tweets Showcase
Live Tweets Showcase is OpenSource project developed for showcasing live tweets which contains particular hashtags within. we proudly use this project in GDG Rajkot DevFest'19 😎

---
**This project is divided into two small projcts**
 1. NodeJS (Server - Backend)
 2. ReactJS App (Client - Frontend)


 # ReactJS App
at root you will find `twitterstatsapp` directory. and this is frontend this react app will listen all tweets from server using `WebSocket` and display on screen. and also calculate top tweeted user. you will also find `bg.jpg` in this project just please with your own banner

**How to Setup and Run**
1. Install all need dependency goto `twitterstatsapp` directory and run this commmand
    ```
    npm install
    ```
2. open `twitterstatsapp/src/App.js` and find variable `SERVER_URL` and replace with your Server URL

3. now it's time for Build 😎. goto `twitterstatsapp` directory and run this command
    ```
    npm run build
    ```
    this will create a build folder in `twitterstatsapp` directory



# NodeJS
**index.js** which located at `root` which listen for real-time tweets using Twitter Stream API. in this project it listen tweets which contains specific **hashtags**. on `index.js` you will find a variable `hashtag` just replace with your own hashtags and you are all done 👌. this project stores all tweets so we can count tweets later with something went wrong at runtime

**How to Setup and Run**
1. Install all need dependency by using this command 
    ```
    npm install
    ```
2. Create a Twitter App. generate `consumer_key`, `consumer_secret`, `access_token_key` and `access_token_secret` and replace all keys in `twitterConfig.json` file located at root

3. Run by using this command
    ```
    node index.js
    ```

**Volla! You are ready to go 🚀**

**Commands**
* `/reloadAll` to reload all connected user browsers
* `/allowRetweet/yes` to allow retweets count and showcase
* `/allowRetweet/no` to disallow retweets count and showcase
* `/retweetStatus` to check if Retweet is allowed or not
* `/blockList` to see all blocked users
* `/blockUser/:USERNAME/:PASSWORD` to block any user
* `/unblockUser/:USERNAME/:PASSWORD` to unblock any user
* `/retweetStatus` to check if Retweet is allowed or not
* `/reset/:PASSWORD` to reset all stored data

more commands are coming soon 😎.

**Note** You'll find this `PASSWORD` variable in `appConfig.json`
