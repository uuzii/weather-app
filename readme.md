# Nearsoft Test

This is a sample of Nearsoft Test

### Setup

##### Prerequisites

First, install [Polymer CLI](https://github.com/Polymer/polymer-cli) using
[npm](https://www.npmjs.com) (we assume you have pre-installed [node.js](https://nodejs.org)) avobe v8.

    npm install -g polymer-cli

Second, install [Bower](https://bower.io/) using [npm](https://www.npmjs.com)

    npm install -g bower

### Configure and start the proxy

We need a proxy to avoid cors issue, install the packgages with these commands:

    cd weather-app/proxy
    npm install cors-anywhere

Run this command to serve the app at `http://localhost:8080/` the command also provides a method for
intercept the frontend requests and add headers to avoid the cors block

    node cors.js

### Start the app locally

Donwload the frontend components with these commands:

    cd weather-app/front
    bower install

The next command serves the app at `http://127.0.0.1:8081/home` and provides basic URL
routing for the app:

    polymer serve

### See unit tests

Serve the app with this command:

    polymer serve

Open the unit tests diagnostic at `http://127.0.0.1:8081/test/`

