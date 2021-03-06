# Stormpath SPA Development Server

[![NPM Version](https://img.shields.io/npm/v/stormpath-spa-dev-server.svg?style=flat)](https://npmjs.org/package/stormpath-spa-dev-server)
[![NPM Downloads](http://img.shields.io/npm/dm/stormpath-spa-dev-server.svg?style=flat)](https://npmjs.org/package/stormpath-spa-dev-server)

[Stormpath](https://stormpath.com/) development server that provides your SPA or mobile app with a Stormpath integrated back-end.

Front-end applications can not communicate with the Stormpath API directly, and thus need an integrated back-end. Before your back-end has been integrated, use this development server when integrating Stormpath with your front-end app, using for example the [AngularJS SDK](https://github.com/stormpath/stormpath-sdk-angularjs).

## Install

1. Make sure you have [Node.js](https://nodejs.org/) installed
2. Install the server

  ```bash
  $ npm install -g stormpath-spa-dev-server
  ```

3. [Download a key file](https://support.stormpath.com/hc/en-us/articles/203697276-Where-do-I-find-my-API-key-) from the Stormpath Console
4. Open it and grab the **API Key ID** and **API Key Secret**, then run these commands to configure the server with your credentials:

  ```bash
  $ export STORMPATH_CLIENT_APIKEY_ID=<YOUR-ID-HERE>
  $ export STORMPATH_CLIENT_APIKEY_SECRET=<YOUR-SECRET-HERE>
  ```

5. Login to the [Stormpath Console](https://api.stormpath.com/) and grab the *href* (called **REST URL** in the UI) of your *Application*
6. Run this command with your **App Href**:

  ```bash
  $ export STORMPATH_APPLICATION_HREF=<YOUR-APP-HREF>
  ```

## Usage

1. Start the server

  ```bash
  $ stormpath-spa-dev-server <path-to-your-spa-app>
  ```

  Example:

  ```bash
  $ stormpath-spa-dev-server /home/joe/dev/my-app/
  ```

2. It's now listening at <http://localhost:3000/> and ready to use with your front-end app

## Help

Contact us via email at support@stormpath.com or visit our [support center](https://support.stormpath.com). You can also see the Stormpath [documentation](https://docs.stormpath.com/) for more information.

## License

Apache 2.0, see [LICENSE](LICENSE).
