# basic-firebase-app-without-css

Basic Web Application with Vanilla JS and Firebase backend, no CSS library

Authentication
==============

This app implements several methods of the Firebase web SDK for signing in using the authentication quickstarts in [Firebase Github repo](https://github.com/firebase/quickstart-js):

  - The [Firebase email and password authentication quickstart](email-password.html) demonstrates using a Firebase stored email & password to authenticate - you can both create and sign in a user.

  - The [Firebase email link authentication quickstart](email-link.html) demonstrates using an email address to sign-in without a password, via a link sent through email - you can both create and sign in a user.

  - The Firebase Google Sign in quickstarts demonstrate using a Google account to authenticate to Firebase using three different techniques: with a [popup](google-popup.html), a [redirect](google-redirect.html) and an [auth token](google-credentials.html).

  - The Firebase Facebook Login quickstarts demonstrate using a Facebook account to authenticate to Firebase using three different techniques: with a [popup](facebook-popup.html), a [redirect](facebook-redirect.html) and an [auth token](facebook-credentials.html).

  - The Firebase Twitter Login quickstarts demonstrate using a Twitter account to authenticate to Firebase using two different techniques: with a [popup](twitter-popup.html) and a [redirect](twitter-redirect.html).

  - The Firebase Microsoft Login quickstarts demonstrate using a Microsoft account to authenticate to Firebase using two different techniques: with a [popup](microsoft-popup.html) and a [redirect](microsoft-redirect.html).

[Read more about Firebase Auth](https://firebase.google.com/docs/auth/)

Getting Started
---------------

 1. Create a Firebase project on the [Firebase Console](https://console.firebase.google.com).

 1. Add a support email to your project in the [settings page](https://console.firebase.google.com/u/0/project/_/settings/general/). Some auth methods won't work without this.

 1. Enable the authentication method you want to use by going to the **Authentication** section in the **SIGN-IN METHOD** tab. For **Facebook** and **Twitter** you will need to create an application as a developer on their respective developer platform, whitelist `https://<project_id>.firebaseapp.com/__/auth/handler` for auth redirects and enable and setup the app's credentials in the **Firebase Console > Authentication > SIGN-IN METHOD**.

 1. You must have the [Firebase CLI](https://firebase.google.com/docs/cli/) installed. If you don't have it install it with `npm install -g firebase-tools` and then configure it with `firebase login`.
 
 1. On the command line, `cd` in the app directory.
 
 1. Run `firebase use --add` and select your Firebase project.

To run the sample app locally during development:
 1. Run `firebase serve`.
    This will start a server locally that serves `auth/index.html` on `http://localhost:<port>`. Check the output of the command for the exact port.
 1. Navigate in your browser to the URL output by the `firebase serve` command.

To deploy the sample app to production:
 1. Run `firebase deploy`.
    This will deploy the sample app to `https://<project_id>.firebaseapp.com`.

License
-------

© Google, 2016. Licensed under an [Apache-2](../LICENSE) license.
