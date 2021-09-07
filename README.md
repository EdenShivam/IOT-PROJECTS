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

















