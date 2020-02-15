---
id: 697
title: A new website
date: 2013-01-21T22:39:54+00:00
author: Martin Wright
excerpt: "Seven months after starting I've launch a new portfolio site, here's a writeup of what I did and why I did it."
layout: post
guid: http://mynameismartin.com/?p=697
permalink: blog/a-new-website/
background_image:
  - "715"
  - "715"
categories:
  - Life
  - News
tags:
  - Design
  - gridset
  - new
  - typecast
  - Wordpress
---
In July of 2012 I started a new job at Torchbox, so one sunny evening in July I fired up my text editor to make some minor changes to my site to reflect my recent career change. Predictably, here we are seven months later at the end of what escalated into a ground-up redesign and rebuild of my site.

There was a lot I wanted to achieve in this redesign, a lot of theory I wanted to put into practice and a lot of my personality I wanted to come through, something that was always missing from my previous generally minimal sites.

In August I started [dribbbling a few details](http://dribbble.com/wrightmartin/projects/14532-mynameismartin-com) and set myself the deadline of the 1st of October to go complete the rebuild and go live. And tah-dah, a few weeks into 2013 it&#8217;s live (Hey, I moved house and have a one year old, I&#8217;d like to see you meet that ridiculous deadline).

So here&#8217;s a breakdown of what I did and why I did it.

## Projects, projects, projects

Over the years I have amassed a varied portfolio of work and I wanted a way to show it off in a way that looks great but remains flexible,  to cater to my lazier side &#8211; if it&#8217;s not easy to add projects to my portfolio I&#8217;m not going to do it. So I&#8217;ve built a halfway house solution using WordPress custom post types. If I want make a full art-directed case study of a project I can, but I am also able to add a new project with just paragraph of text and a screenshot through the WordPress interface.

## Responsive, and properly this time.

The last version of this site had a responsive retrofit shortly after reading [that book](http://www.abookapart.com/products/responsive-web-design), so this version of the site was to be a ground-up mobile first design (oh yeah, I read [that _other_ book](http://www.abookapart.com/products/mobile-first) too) built on a fluid grid (designed with Gridset, more on that later). I was glad to be able to put all that theory in to practice and learnt a lot in the process, it&#8217;s still not 100% and I haven&#8217;t even looked at it on an Android device (although I did get a brief test with a Windows phone &#8211; thanks Mum).

## Gridset

I designed the grid for this site using the beta of <a href="http://gridsetapp.com" target="_blank">Gridset</a> and I was impressed with the speed at which I was protoyping in the browser and changing the grid with minimal impact on my code. It wasn&#8217;t until implementing the HTML in WordPress template that I ran into problems and was reminded the hard way (once again) that I don&#8217;t get on well with frameworks (even good ones) due to my OCD over code control. When Gridset came out of beta Sass mixins came with it, but even with those I had problems (although it did force me to get to grips with CSS preprocessors, fun!). So in the end I implemented the grid myself, using Gridset&#8217;s cheat sheet and [JavaScript overlay](?gridset=show) as a guide (nearly worth the money alone).

## Typecast

Choosing type is one of my favourite things to do, and in the past I&#8217;ve used a test Typekit library filled with as many fonts as I could and played with different combinations using Chrome&#8217;s web inspector, but this isn&#8217;t the best way of working so I took the opportunity to use the wonderful [Typecast](http://typecast.com/) app.  I was able to spend a good amount of time experimenting with typefaces in Typecast (something that would&#8217;ve been cumbersome using my previous method) and am happy with the choices I eventually made.  
<img class="pull-left" alt="typecast" src="http://mynameismartin.com/blog/wp-content/uploads/2013/01/typecast.png" /> 

I knew wanted to move on from Skolar, which was the sole typeface I used on the last version and it had begun to grate on me. Truthfully I hadn&#8217;t done it justice, and every time I saw it used more effectively by someone else it made me wince. After much experimentation and research I settled on FF&#8217;s lovely [Meta Serif](https://typekit.com/fonts/ff-meta-serif-web-pro), accompanied by the sans-serif of the same family, which I swapped out at the last minute and replaced with [Proxima Nova](https://typekit.com/fonts/proxima-nova) after I realised how often I used it in caps, and I just love they way Proxima looks capped up.

## Photography

I take a lot of photos, and last years&#8217; New Years&#8217; resolution was to do more with my photography, so using WordPress custom fields I can set a header photo for any page or blog post, let&#8217;s see how long it takes before every blog post has a photo of my daughter. Parents and their baby photos eh?

## Retina

<img class="pull-right" alt="responsive" src="http://mynameismartin.com/blog/wp-content/uploads/2013/01/responsive.png" width="600" height="450" />  
A big part of the responsive design puzzle is how we keep things nice and sharp for the ubiquitous high-density mobile phone displays and our rich friends with retina MacBook Pros. To tackle this I&#8217;m serving icons in a web font via <a href="http://symbolset.com" target="_blank">Symbolset</a>&#8216;s excellent social icon set and relying on the method described in [this post](http://blog.netvlies.nl/design-interactie/retina-revolutie-follow-up/) for photography. I&#8217;m not 100% sure either of these methods are the best way but they&#8217;re working for now, no doubt when I start to look more closely at performance optimisation I will re-examine these choices.

## Sass

I&#8217;ve long resisted the desire to delve into the world of CSS preprocessors; I&#8217;m proud of my ability to write vanilla CSS and was wary of becoming reliant on third-party functionality but after my experiments with Gridset it became a necessity. Initially  I wasn&#8217;t bowled over but as I began to play with more complex functions and calculations I am happy to let Sass do the heavy lifting, and after experimenting further with LESS (the preferred preproc at work) I am well and truly sold, and have now become one of _those_ people, looking down at my friends who haven&#8217;t taken the jump with pity.

## Still to come

I&#8217;ve got lots more projects to add to the portfolio and I&#8217;ll perhaps create a couple of case-studies when I revisit some of the more interesting ones. I need to spend a good amount of time on optimisation, something I skipped over in development, mainly due to time constraints (the 800kb payload of the homepage is frankly embarrassing). There are still a few bugs here and there, I&#8217;ll get to them eventually but if you spot one feel free to yell about it to me on [Twitter](http://twitter.com/wrightmartin).

Generally I&#8217;m happy with how the site turned out, given that the majority of it was designed on a 13&#8243; mid-2010 MacBook Pro screen in a bedsit over the equivalent of a 56k modem, and I&#8217;m looking forward to the motivation to blog and create that a new site brings.