---
id: 1022
title: Two-dimensional arrays and Liquid
date: 2014-03-18T20:55:51+00:00
author: Martin Wright
excerpt: "For the (R)evolution conference site this year I'm using Mixture's models to manage our speaker data"
layout: post
guid: http://mynameismartin.com/?p=1022
permalink: blog/two-dimensional-arrays-with-liquid/
background_image:
  - ""
categories:
  - Development
tags:
  - access
  - array
  - dimension
  - index
  - inner
  - jekyll
  - liquid
  - loop
  - mixture
  - multidimensional
  - shopify
  - template
  - value
  - vector
---
For the [(R)evolution](http://2014.shropgeek-revolution.co.uk) conference site this year I&#8217;m using [Mixture](http://mixture.io)&#8216;s models to manage our speaker data. As information about speakers is used across the site in multiple places and can change fairly often it makes sense to have it in one place. To do this I have json file containing data about each speaker as follows:

<pre>"organisations": [
  [
    {
      "name": "Headscape",
      "url": "http://www.headscape.co.uk"
    },
    {
      "name": "Boagworld",
      "url": "http://www.boagworld.co.uk"
    }
  ]
]</pre>

Each speaker will be a member of one or more organisations, each with a name and url. This is stored in a two-dimensional array called &#8216;organisations&#8217;, each entry in an organisation is a name:value pair. To access this data I need to loop through the list of organisations and then loop again through each organisation. I can then output the name and url as a link inside a list item.

<pre>{% for org in speaker.organisations %}
  {% for value in org %}
    &lt;li&gt;&lt;a href="{{ org[forloop.index0].url }}"&gt;{{ org[forloop.index0].name }}&lt;/a&gt;&lt;/li&gt;&lt;
  {% endfor %}
{% endfor %}</pre>

Working out how to loop within a loop using Liquid was a bit of a struggle as you can&#8217;t really write traditional loop, as you can&#8217;t do mathematical operations on a variable. I couldn&#8217;t find many articles or tutorials online that helped me out, so I guessed it and it seems to work.

And the output:

<pre>&lt;li&gt;&lt;a href="http://www.headscape.co.uk"&gt;Headscape&lt;/a&gt;&lt;/li&gt;
&lt;li&gt;&lt;a href="http://www.boagworld.co.uk"&gt;Boagworld&lt;/a&gt;&lt;/li&gt;</pre>

I&#8217;m not a developer. &#8216;Proper&#8217; development doesn&#8217;t come naturally to me so any coding I do tends to be as a result of Googling for pre-existing solutions and then adapting them for my own needs. I couldn&#8217;t find any working examples of dealing with multidimensional arrays using Liquid, so I put this together via various tutorials, documentation and plenty of stabs-in-the-dark. If it helps you (or you know a better way) it would be really cool if you could [let me know](http://twitter.com/wrightmartin).