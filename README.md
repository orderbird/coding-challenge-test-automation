# Tech Challenge for Test Automation

Hello and welcome to the orderbird tech challenge for test automation. 
Your tasks, if you accept them, are as follows:

## 0. setup Appium
yes, setting up Appium is alway fun. But hopefully you already have an operational development environment where you can run Appium and the Appium Inspector. 
## 1. prepare "the app" for the iOS simulator
Under https://github.com/appium/ios-test-app you will find a simple test application. TheApp has no other purpose but to provide a playground for some mobile app testing. You need to build it yourself from the sources, it is a React Native app. If you are running an m1 mac, you can simply download the **[TheApp](https://github.com/orderbird/coding-challenge-test-automation/blob/main/TheApp_m1_simulator.zip)** from the root of this repository. 

Alternativly you can also compile the App for an Android simulator if you do not have an Apple Mac at your disposal. If you run into problems that you cannot resovle please let us know.

## 2. Automate the app using Appium & Python

As mentioned, TheApp provides very little real functionality other than providing some basic controlls. 
![](https://github.com/orderbird/coding-challenge-test-automation/blob/main/TheApp-Startscreen.png)

Please write some testcases for three different controlls:

1. Echo Box ![](https://github.com/orderbird/coding-challenge-test-automation/blob/main/TheApp-EchoBox.png)
2. Login Screen (valid credentials are user: 'alice', password 'mypassword')
3. List Demo 

## 3. Provide your test suite as a link to your github repository
