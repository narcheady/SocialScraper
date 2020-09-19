# SocialScraper
This project can be used to crawl, scrape data from different social media websites. (As of now this only supports Twitter, other modules will be added soon.) </br>

## Scraping Tweets from Twitter
<b>This project does not use Twitter API</b>. For performing searches from Twitter API, you can use <a href="http://docs.tweepy.org/en/latest/api.html">Tweepy</a>.</br>
This script can be used to scrape Tweets using <code>requests</code> to retrieve the content and <code>Beautifulsoup4</code> to parse the retrieved content and then <code>Pandas</code> to save all data in csv format.</br>

## Why this alternative?
Well if you're here you already know why :P
One of the major disadvantages of Twitter Search API is that you can only access Tweets written in the past 7 days. This is a major bottleneck for anyone looking for older data.
Using this code you can scrape beyond 7 days.

## Installation
<pre>
$ git clone https://github.com/narcheady/SocialScraper.git
$ cd SocialScraper/
$ pip install -r requirements.txt
</pre>

## Usage

You can search for tweets using certain words or hashtags within specific dates. 

<pre>
searchWord = "#Twitter"
searchFrom = "2020-01-01"
searchUntil = "2020-09-19"
</pre>

Using these inputs as parameters, script will scrape tweets and create a dataframe which then will be converted to csv.
