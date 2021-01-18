# DiscordTwitterBot
To set up this Discord bot you need:
• NodeJS v12 (optimised, v14 works)
• NPM v6 (or higher)

Node Dependencies
Firstly, open the terminal / Windows PowerShell in the folder the code is (where index.js and
config.json are)

Please then enter the following commands:
npm i discord.js
npm i node-tweet-stream
npm i fs

Please do each line at one time, this shouldn’t take more than a minute


Configuration
(config.json)
The file says:
“discordBotToken”:””,
“twitterConsumerKey”:””,
(continuous)


So when talking about for example the discordBotToken, please change it so it looks like:
“discordBotToken”:”<value>”,
“twitterConsumerKey”:””,
  
You will need to have access to Twitter Developer, and create an application in
https://developer.twitter.com/en/portal/dashboard for 4 of the values.

• To find the discordBotToken, go to https://discord.com/developers/applications ,
create an application by pressing “New Application” or go for a pre-existing application,
then in the section “Bot”, create one. Beneath the username it should say “Token”. Hit
“Copy” and enter it in
• To find the twitterConsumerKey, in the Twitter Developer Portal, in the new project
created, select “Keys and tokens” and go to “Consumer Keys”. Besides “API Keys &
Secrets” please view it. Regenerate if needed. The API Key is the value
• To find the twitterConsumerSecret, stay on the tab stated in twitterConsumerKey
and copy the “API key secret”.
• To find the twitterAccessTokenKey, go back to the “Keys and tokens” page and
scroll down to “Authentication Tokens”, please regenerate the “Access Token & Secret”
and copy the “Access token” into this.
• To find the twitterAccessTokenSecret, stay on the tab stated in
twitterAccessTokenKey and copy the “Access token secret” into config.json.
• The following is an array, so you can follow multiple people, so the value may look like
[“twitter-a”] or [“twitter-a”,”twitter-b”] or even [“<twittera”,”twitter-b”,”twitter-c”]. These values however must be the user’s ID, which 
you can find at https://tweeterid.com/ – so for example, @macroaistech is
1279202409403777024
• The channelsToPost is also an array like following. To find these values, make sure you
have developer mode on discord, then simply right click a channel and press “Copy ID” and
paste it in. Please make sure it is in an array format.
• The title is the title of what you want to come up, so for example “New Tweet”
• The colour is the colour that the line is, so for example #1A91DA is the Twitter Blue 
