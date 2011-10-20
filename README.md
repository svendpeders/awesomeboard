Harvest Tweets and display them with the Awesome Board
=============

Simple application we use to harvest tweets about our company real time and then have them displayed in an application.
The name Awesome Board is in fact somewhat of a joke and we don't actually think it is that awesome :)

The Harvester utilize the [Twitter Streaming API](https://dev.twitter.com/docs/streaming-api) and stores the data in MongoDB.
The Awesome Board is an [ExpressJS](http://expressjs.com/) web application which reads from the database and displays the data.

We use this at [FINN.no](http://finn.no) to display customer feedback on various screens in our office


Pre-requisits
------------

* Sign up for a [Twitter account](http://twitter.com)

Installation
------------

We currently only support storing the tweets in MongoDB. Therefor you must install it in order to get started.

* Install [MongoDB](http://www.mongodb.org/) on your machine or on some server

Below is a list of the required NodeJS modules.
Either install these with NPM or place the content of the modules into the lib directory

* [ExpressJS](http://expressjs.com/)
* [Mongodb for NodeJS](https://github.com/christkv/node-mongodb-native)
* [Twitter-node](https://github.com/technoweenie/twitter-node)
* [Connect](http://senchalabs.github.com/connect/)
* [Mustache for NodeJS](https://github.com/raycmorgan/Mu)



Useage
------------

Starting the harvester

    node harvester.js
	
Starting the Awesome Board

    node app.js

Now you can check `http://localhost:29099/` or you can view the list mode on http://localhost:29099/list	

About the Awesome Board
------------

The board application uses [jQuery](http://jquery.com), [Mustache for JS](https://github.com/janl/mustache.js) and the [eventHub](https://github.com/leftieFriele/eventhub) JS libraries in order to make it's magic.
The list view is pretty crap, but we might get round to fixing it.

Developed by [FINN.no](http://finn.no), check our blog for more cool stuff http://tech.finn.no