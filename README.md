# Tech Challenge for Test Automation

Hello and welcome to the orderbird tech challenge for mobile test automation. 


## Regarding this challenge
We know that your time is valuable. So if this challenge takes more than 4 h of your time please stop and get in touch anyways. For your solution please create a public github repo and share the link with us. Please do not fork this repo as it would give other candidates the solution to your hard work :-)


Your tasks, if you accept them, are as follows:

## 0. setup Appium
yes, setting up Appium is alway fun. But hopefully you already have an operational development environment where you can run Appium and the Appium Inspector. You can also use [this check list](https://github.com/orderbird/coding-challenge-test-automation/blob/main/Appium-iOS-setup.md) to get things rolling.

## 1. prepare "the app" for the iOS simulator
Under https://github.com/appium/ios-test-app you will find a simple test application. TheApp has no other purpose but to provide a playground for some mobile app testing. You need to build it yourself from the sources, it is a React Native app. If you are running an m1 mac, you can simply download the **[TheApp](https://github.com/orderbird/coding-challenge-test-automation/blob/main/TheApp_m1_simulator.zip)** from the root of this repository. 

Alternativly you can also compile the App for an Android simulator if you do not have an Apple Mac at your disposal. If you run into problems that you cannot resovle please let us know.

## 2. Automate the app using Appium & Python

As mentioned, TheApp provides very little real functionality other than providing some basic controlls. 

Please write some testcases for three different views, chose what you want to test in these views yourself:

1. Echo Box 
2. Login Screen (valid credentials are user: 'alice', password 'mypassword')
3. List Demo 

Please write your tests using Python.

## 3. Add a README.MD to your repo
So after your hard work please tell us 

* how we would setup our local environment to fire up your test suite. 
* Please also add documentation on your testcases (Why did you chose these, would you add others if you had more time?)

# Submitting your solution
* Send a link to your repo to tech-challenge@orderbird.com
* Do not remove the git information, so we can easily review your changes
* Do not fork this repository
