# Jelly Fin

<!-- Badges -->
[![Discord](https://badgen.net/badge/chat/on%20Discord/cyan)](https://discord.gg/xveZ3FT)
[![PRs Welcome](https://badgen.net/badge/PRs/welcome/green)](http://makeapullrequest.com) 
[![contributions welcome](https://badgen.net/badge/contributions/welcome/green)](https://github.com/jonathan-irvin/jelly-fin/issues)
[![Inline docs](http://inch-ci.org/github/jonathan-irvin/jelly-fin.svg?branch=master)](http://inch-ci.org/github/jonathan-irvin/jelly-fin)
[![Build Status](https://badgen.net/travis/jonathan-irvin/jelly-fin)](https://travis-ci.org/jonathan-irvin/jelly-fin)
[![codecov](https://badgen.net/codecov/c/github/jonathan-irvin/jelly-fin)](https://codecov.io/gh/jonathan-irvin/jelly-fin)
[![Maintainability](https://api.codeclimate.com/v1/badges/79a0ff74669610205478/maintainability)](https://codeclimate.com/github/jonathan-irvin/jelly-fin/maintainability)
<!-- End Badges -->
---

Finances are hard.  It's one of the first _adulting_ things everyone has to wrestle with.  So, let's make it easy and automate it.  Over the course of several years, my wife and I have tracked our finances using a forecasting method and had done it all within a spreadsheet.  The time came where I wanted to take this concept and make it mobile using serverless architecture and clean design.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

* Node v8.x.x or use [NVM](https://github.com/creationix/nvm#installation)
* [A Firebase project](https://firebase.google.com/console)

**For iOS**
Remember that you need to have Mac OS in order to develop for iOS
*  [Cocoapods](https://guides.cocoapods.org/using/getting-started.html) (Only for Mac OS)
*  [Xcode](https://developer.apple.com/xcode/) (Only for Mac OS)
* Firebase project's [GoogleService-Info.plist](https://firebase.google.com/docs/ios/setup#add_firebase_to_your_app) file

**For Android**
* Connected device or emulator
* Firebase project's [google-services.json](https://firebase.google.com/docs/android/setup#add_firebase_to_your_app) file

### Setting up Firebase
** For Android**
* Put your `google-service.json` file inside the android/app/ folder

** For iOS **
* Open `ios/JellyFin.xcworkspace` in Xcode and right click on the folder `JellyFin` and "Add files to JellyFin"
* Check "Copy items of needed" option
* Select your `GoogleService-Info.plist`


### Installing and Running

1. Clone the repo.
2. Run `npm install` to cover any dependencies.
3. If are on a Mac OS: Enter `npm run ios:install`
4. Enter `npm start` to start the server
6. Open a new tab/terminal and run the project for the desired platform: `npm run ios` or `npm run android`

## Running the tests

After installing all prerequisites and dependencies, just run `npm test`

## Dependencies

Dependency PRs are automagically opened using [Dependabot](https://dependabot.com/https://dependabot.com/).  We want to make sure the app stays green by ensuring the build doesn't break when dependencies are bumped and each dependency is well tested to ensure stability.

## Deployment

Handled by TravisCI.  Checkout [.travis.yml](.travis.yml) for configuration details.  Current build status: [![Build Status](https://badgen.net/travis/jonathan-irvin/jelly-fin)](https://travis-ci.org/jonathan-irvin/jelly-fin)

## Built With

* React Native
* Firebase

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/jonathan-irvin/jelly-fin/tags). 

## Authors

* **Jonathan Irvin** - *Initial work* - [Jelly Fin](https://github.com/jonathan-irvin/jelly-fin)

See also the list of all [![contributors](https://badgen.net/github/contributors/jonathan-irvin/jelly-fin)](https://github.com/jonathan-irvin/jelly-fin/contributors) who participated in this project.

## License [![license](https://badgen.net/github/license/jonathan-irvin/jelly-fin)](LICENSE)

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details

## Acknowledgments

* Thanks to my wife for the idea, motivation, and support
* Thanks to [Ben Halpern](https://dev.to/ben) for encouraging me to open source this

## Why are we doing this?

The idea is to take what we know: the transactions that are predictable like mortgage and insurance and just keep track of them against the account balance.  Then take transactions that aren't predictable and try to predict them using seasonality analytics.  Does your electric bill go up in the summer?  Let's predict what it would be and try and account for it.
