A simplified Strava training log
==============================================

![](http://i66.tinypic.com/mohn5.png =250x)

This nameless project attempts to provide an easy and streamlined solution to viewing a training log of your Strava activities. It is intended to be primarily used as a 'new tab' page in your web browser, but can also be accessed as a regular site.

This project is built with node.js on the server side and jQuery/vanillaJS/Bootstrap on the client side.

Available on my website here: http://quiet-reef-29901.herokuapp.com/

If you don't have a Strava account, you can access a demo version of the site: <LINK>

Running the project
--------------------

1. Install node.js and npm
2. ```$ git clone https://github.com/ednunezg/StravaLog```
3. Install dependencies ```$ npm install```
4. Edit the data/strava_config file with your Strava API token, ID and secret
5. Start app ```$ nodemon start```
6. Go to http://localhost:3000

Project issues / Future features
--------------------------------

1. Client requests activities on a week to week basis from the server. This can be optimized by having the server giving a JSON response with activities from multiple weeks at a time for a significantly faster page load.
2. Accessing the home page should redirect you to the /traininglog page if the server still has your access token cached.