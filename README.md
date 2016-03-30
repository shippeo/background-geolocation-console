# Background Geolocation Console

> A simple Node server & web app with SQLite database for field-testing & analysis of the [Background Geolocation plugin](https://github.com/transistorsoft/cordova-background-geolocation-lt).

![](https://dl.dropboxusercontent.com/u/2319755/cordova-background-geolocaiton/background-geolocation-console-map.png)

![](https://dl.dropboxusercontent.com/u/2319755/cordova-background-geolocaiton/background-geolocation-console-grid.png)

## Running

You must have [npm](https://www.npmjs.org/) installed on your computer.
From the root project directory run these commands from the command line:

    npm install

This will install all dependencies.

To build the project and run app in your browser, run this command:

    npm start

This will perform : 
* Build and start a watcher process that will update bundle.js with any changes you wish to make. (This watcher is based on [Browserify](http://browserify.org/) and [Watchify](https://github.com/substack/watchify), and it transforms React's JSX syntax into standard JavaScript with [Reactify](https://github.com/andreypopp/reactify) 
* Boot the web server

Now visit [http://localhost:8080](http://localhost:8080)

## Configure The Sample App

The Background Geolocation [Sample App](https://github.com/transistorsoft/cordova-background-geolocation-SampleApp) is perfect for use with this web-application.  To configure the app, simply edit `Settings->url` and set it to `http://<your.ip.ad.dress>:8080/locations`.

![](https://dl.dropboxusercontent.com/u/2319755/cordova-background-geolocaiton/settings-url.png)

You should also configure `Settings->autoSync` to `false` while out field-testing as well, so that the app doesn't try syncing each recorded location to the server running on your `localhost`.  Once you return after a test and you're back on your office Wifi, click the **[Sync]** button on the `Settings` screen to upload the cached locations to the **Background Geolocation Console** server.

## Credit

Chris Scott of [Transistor Software](http://transistorsoft.com)

## License

BSD-licensed.
