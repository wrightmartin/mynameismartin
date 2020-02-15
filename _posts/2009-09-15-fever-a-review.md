---
id: 93
title: Fever, a Review
date: 2009-09-15T23:29:49+00:00
author: Martin Wright
excerpt: |
  RSS has always been a technology that never really fit right with me, until recently I was happy using tabbed bookmarks to fire up my 65+ sites of <a href="http://delicious.com/skip694/daily_reading" title="Martin's daily reading links via Delicious">daily reading</a>, letting them load for 5 minutes or so and then clicking through.
layout: post
guid: http://mynameismartin.com/?p=93
permalink: blog/fever-a-review/
categories:
  - Reviews
tags:
  - fever
  - mint
  - review
  - rss
  - shaun inman
---
RSS has always been a technology that never really fit right with me, until recently I was happy using tabbed bookmarks to fire up my 65+ sites of [daily reading](http://delicious.com/skip694/daily_reading "Martin's daily reading links via Delicious"), letting them load for 5 minutes or so and then clicking through. It took a while and made Firefox groan under the strain but it served a purpose, and besides, I had never found an RSS reader I could get along with.

I stumbled across [Fever](http://www.feedafever.com "Fever website") while aimlessly web browsing one day, I am familiar with [Shaun Inman](http://shauninman.com/pact/ "Shaun Inman's website") and the acclaimed analytics package [Mint](http://www.haveamint.com "Mint website") and I had not long acquired a new web host so I decided to throw $30 (£18) at it and give it a go.

### What is Fever?

Fever is a self hosted RSS reader with a twist. Once you have loaded it with RSS feeds it performs some clever aggregation and gives you your feeds sorted by temperature.

### How it works

Fever gives you multiple choices when adding an RSS feed. The feeds you read every day get marked as &#8216;kindling&#8217;, other feeds of the kind that you may not want to read as consistently get marked as &#8216;sparks&#8217;. For example I have a feed from Smashing Magazine which I read daily so I&#8217;ve marked that as kindling, whereas the feed from Digg&#8217;s technology section that is not always going to contain stuff I want to read gets added as a spark. When an item appears in one or more kindling feeds and also one or more spark feeds the temperature of the item is raised.

What you end up with is a chart of the hottest items by week (this is the default but you can change the timeframe). This is great for those busy periods when you can&#8217;t read your feeds all day long, you can get a good overview of the most talked about things. Fever still functions like a traditional RSS reader if you are into that kind of thing, and it allows grouping of feeds and saving so you can categorise feeds however you like and save RSS items you want to remain in your feed.

### The roof is on fire

When I first installed Fever I had somewhere between 65 and 70 feeds to add, over the next few days I got the bug and went feed hunting, I used my Twitter following list, anything I could get my hands on. The great thing about Fever is if you aren&#8217;t sure about a feed you just mark it as a spark and you don&#8217;t have to read it, it just makes the whole program work better. Imagine that, an RSS feed reader that work better the more feeds you throw at it.

### The downside?

Because Fever is a self-hosted service you need a web server (not IIS), with PHP and MySQL. If you are familiar with the above technologies then installation shouldn&#8217;t cause you too much trouble, if you aren&#8217;t though you may struggle as you have to do some fairly low level stuff to prepare your server for deployment, such as creating a database and setting up a user and the installation notes don&#8217;t exactly walk you through the process.

Fever will use your server&#8217;s bandwidth and CPU time so if you are on a cheaper, limited hosting plan you will want to keep an eye on it. You can configure Fever to update via cron jobs to limit this. It&#8217;s not a bandwidth hog or anything but if you regularly run at the red line you&#8217;ll notice.

### What are you waiting for?

If you only want an RSS reader to manage 10 or so feeds then maybe Fever isn&#8217;t for you. If, like me, you have a lot of feeds to manage and traditional RSS feed readers don&#8217;t quite cut the mustard then I wholly recommend you check Fever out, it has completely changed the way I read on the web and has actually allowed me to do much more reading than back when I was wrestling with 65 tabs. Since installing Fever I have doubled my subscribed feeds and I&#8217;m far less afraid of adding more to the reading list. While I&#8217;m not saying it will work for everyone, it has worked for me after many years of trying to crowbar passive RSS into my daily routine.