# wswebcreation-react-native-app

[![Join the chat at https://gitter.im/wswebcreation](https://badges.gitter.im/wswebcreation.svg)](https://gitter.im/wswebcreation/Lobby)

An app which is build with React Native and will be used for test (automation) purposes.


![wswebcreation.ios](./assets/wswebcreation-ios.gif) ![wswebcreation.android](./assets/wswebcreation-android.gif)

## About
As mentioned above I want to use this app to explore the possibilities for testing a (React) Native app (iOS / Android).
In order to understand what I need to test I told myself that I needed to be able to build a React Native app, so here it is :-) 
This app has three tabs that all do something different. More info will follow in the coming months. You can also follow my progress on my [site / blog](http://www.wswebcreation.nl/)

### Home
This is the intro of the app

### Webview
In the Webview you can enter an URL and load it in the Webview

### Chats
In the chats I created multiple API calls to retrieve JSON data from [GitHubGist](https://gist.github.com/wswebcreation). 
When you select a chat you will get a chatbox. Here you can add chats and you will get a response (some movie onliners) from my gist.

## Install
This will only work on a MAC so get started execute the following steps:

1. Clone the project: `git clone https://github.com/wswebcreation/wswebcreation-react-native-app.git`
2. Go to the folder: `cd wswebcreation-react-native-app`
3. Install all (dev)dependencies: `npm install`
4. Start the project for iOS `npm run ios`, for Android run `npm run android`
5. Happy playing!

## Testing

### Appium
>**Make sure you've installed Appium on your local machine. There are a lot of good articles on the web the help you with that. You can start with the [Appium Docs](http://appium.io/docs/en/about-appium/getting-started/)**

>**Don't forget to set all the environment variables for Android, see [here](https://stackoverflow.com/questions/19986214/setting-android-home-enviromental-variable-on-mac-os-x) or Google it ;-)**

#### Android and ChromeDriver
When accessing a webview on Android it could be that you get this error

    An unknown server-side error occurred while processing the command.
    Original error: unknown error: Chrome version must be >= 55.0.2883.0

You can fix this by checking the [docs](https://appium.io/docs/en/writing-running-appium/web/chromedriver/) on Appium by downgrading ChromeDriver during install. The right version can be found [here](https://chromedriver.storage.googleapis.com/2.35/notes.txt). 
 
> **Change the number of ChromeDriver tot the latest version to see an overview of all versions**

### Detox
See **TODO**

## TODO
- [x] Create an iOS app
- [x] Add an APP icon
- [x] Create an Android app
- [x] Refactor code
- [x] Refactor `ChatBox.js` code
- [x] Add test properties (`testID` for iOS and `accessibilityLabel` for Android) 
- [x] Add Appium setup
- [x] Add Appium tests for navigation
- [ ] Add Appium tests for home screen
- [ ] Add Appium tests for webview screen
- [ ] Add Appium tests for chat screen 
- [ ] Add Detox setup
- [ ] Add Detox tests for navigation
- [ ] Add Detox tests for home screen
- [ ] Add Detox tests for webview screen
- [ ] Add Detox tests for chat screen
- [ ] Implement different environments / build types
- [ ] Disable animations for automation
- [ ] Add mocking for the API's
- [ ] Add UT's with Jest and Enzyme

## Issues
- [ ] Check issue in Tabnavigator with `tabBarTestIDProps`, it's not working for Android, got a workaround for it
- [ ] Check how to "slow down" swiping on Android, looks like it is taking 2 screens at the same time
- [ ] Fix issue Android stackmenu and chatbox scroll to much up

## Contributing
If you'd like to contribute feel free to create a PR. If you have some code feedback you may also add a PR or contact me through [Gitter](https://gitter.im/wswebcreation)

## Credits
- I'd like to thank [yllongboy](https://medium.com/@yllongboy) for his clear article about creating a "WhatsApp Layout through React Native".
- I'd also like to thank [randomuser.me](https://randomuser.me/) for generating random users with avatars.
