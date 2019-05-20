# FeedReader Testing Project

This project is a web-based application that reads RSS feeds. The original developer of this application started writing their first test suite by using [Jasmine](http://jasmine.github.io/) Since they left the company, my mission is complete test suite.


## Guide

`git clone https://github.com/tsenbaba/feedReader` and open the files in your editor. 


## How I completed this project
I have to write some tests in different test suites to complete the project.

1. `url is defined` test checks `allFeeds` object to make sure URL is defined and not empty. 
2. `name is defined` test checks `allFeeds` object to make sure a name is defined and not empty. .
3. `menu is hidden` test ensures the menu element is hidden by defult. I need to analyze the HTML and CSS to understand how to work hiding/showing menu element. 
4. `changes visibility when menu is clicked` test ensures the menu changes visibility when the menu icon is clicked.
5. `loadFeed is called and completes its work` test checks there is at least a single `.feed` element when `loadFeed` function is called. Since `loadFeed()` is asynchronous so I need to use Jasmine's `beforeEach` and asynchronous `done()` function.
6. `contains different content` test ensures when a new feed is loaded by the `loadFeed()` function that the content actually changes.


## What I learned?

I learn how to use Jasmine to write a number of tests against a pre-existing application. 