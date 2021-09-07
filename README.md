# IOT-PROJECT
Telegram Bot to Control a Light Bulb using Python

Introduction-Hey,everyone this is Shivam,this was my first project done in my college life.
I did an online internship provided by INMOVIDU TECH in which I learnt about how to use Telegram Bot , Adafruit_IO with help of API(Application Programming Interface).


Crux Before you Move on-In this project, we’ll create a Telegram Bot using python-telegram-bot and deploy it to Heroku.It is also programmed to control a feed on Adafruit. The program sends values of 1 and 0 to the feed and turns the status indicator on or off.

What is API?
An application programming interface (API) is a computing interface which defines interactions between multiple software intermediaries. It defines the kinds of calls or requests that can be made, how to make them, the data formats that should be used, the conventions to follow, etc.
Our aim is to control light using Telegram Bot with Adafruit_IO.

Before starting
You will have to sign up for the following services:
a Telegram account, on which we will build our bot
an Adafruit account,
a Heroku account, which is a free cloud platform

Things to be done in Adafruit_IO:
At first, create your account in Adafruit_IO and then create feed by coding in Google Colab and then create Status indicator for manually checking . Next I have created Telegram Bot.
1--->Getting the API keys from Adafruit
Your keys from Adafruit is required to access its API and send values to the required feed. This can, in turn, be programmed to be connected to an Arduino, which can receive the values you send.
![image](https://user-images.githubusercontent.com/69396799/132363879-b39a86dd-f4a6-4f62-8c3b-a2f21fed6ffa.png)
link-https://io.adafruit.com/

Along with this, create a feed and a dashboard on Adafruit and set it to ‘public’.Like this:


![image](https://user-images.githubusercontent.com/69396799/132364490-bc525480-ed92-4c64-aa61-263c7b1867f4.png)
![image](https://user-images.githubusercontent.com/69396799/132364554-fe1b8c55-162e-4e97-a26d-586c3cb9db84.png)
![image](https://user-images.githubusercontent.com/69396799/132364655-1743e5f2-fa8b-459f-abfe-e90adc4debe5.png)

Feeds
![image](https://user-images.githubusercontent.com/69396799/132364827-fba32a06-ef90-439b-9dec-290180eac4fc.png)

This Feed named bots shows contants right now when,its is implemented:At begining
![image](https://user-images.githubusercontent.com/69396799/132365092-ed816660-2fde-45b8-b708-bf4fa1487507.png)
Result will be shows to anyone as a binary value naming 0/1 or On/Off
![image](https://user-images.githubusercontent.com/69396799/132365326-c3258d3f-fc0f-446b-aab5-66e93c811ed5.png)

.
Creating the Bot on Telegram
Create a bot on the Telegram app on your phone. Bots on Telegram can be created using BotFather. The process is shown below. Commands are prefixed with a / . After creating your bot, save the token given carefully. This is required to access the Telegram Bot HTTP API.
![image](https://user-images.githubusercontent.com/69396799/132366779-5299b05b-31bd-4ad6-b6a5-d9efe60e014c.png)

This bot takes 3 commands: /start ,/lighton and /lightoff
Command /start will return a message instructing the user to give the appropriate inputs
/lighton will display the message “Light turned on”. It will also return an image of a lit bulb and will send a value to Adafruit indicating that its ON.
/lightoff will display the message “Light turned off”. It will also return an image of an unlit bulb and will send a value to Adafruit indicating that its OFF.
If any unknown command is given, the bot will reply with the message indicating that it hasn’t understood your command.
![image](https://user-images.githubusercontent.com/69396799/132367572-57a284f0-a955-4f63-87a1-9fbfd1b8cee0.png)
![image](https://user-images.githubusercontent.com/69396799/132367533-212d3835-1588-4bf2-92dd-0387df240fc7.png)

Deploying the app on Heroku
Create a new account or use an existing one to build an app in Heroku. Name your app suitably and click next. Here, we will connect our GitHub account to Heroku as the ‘Deployment Method’ instead of using Heroku CLI. Search your repository and connect it. Also, enable ‘Automatic Deploys’.
Go to the ‘Settings’ page and set your ‘Config Vars’ to values containing your Adafruit username, password, and Telegram API token. Create a ‘Procfile’ on your connected GitHub repo and refresh the ‘Overview’ tab page on Heroku. On doing this, you will see that it has recognized your ‘Procfile’ under ‘Dyno formation’. Click on ‘Configure Dynos’ and set it to ON.
With these steps, your app should start building and get deployed successfully.

To code or run the python script use googlecolab best to implement this project,Thank you.


To see the live working example of this bot is being showed in a live video:
Click this link or copy if not working:
https://drive.google.com/file/d/1BM_weewDTs4mICuaWTPTAzNP17oJDstk/view?usp=sharing














