---
id: 924
title: Getting headings right
date: 2013-11-24T19:00:45+00:00
author: Martin Wright
excerpt: When marking up web pages I often struggle balancing the styling of headings against making my document outline correct, earlier this week I think I solved my problem
layout: post
guid: http://mynameismartin.com/?p=924
permalink: blog/getting-headings-right/
background_image:
  - ""
categories:
  - Development
tags:
  - best
  - document outline
  - headings
  - html5
  - markup
  - trick
---
When marking up web pages I often struggle balancing the styling of headings against making my document outline correct, earlier this week I think I solved my problem by doing this:  
`<br />
h1,<br />
.primary-heading {<br />
font-size: 2.25em;<br />
}</p>
<p>h2,<br />
.secondary-heading {<br />
font-size: 1.6875em;<br />
}</p>
<p>h3,<br />
.tertiary-heading {<br />
font-size: 1.3125em;<br />
}</p>
<p>h4,<br />
.quarternary-heading {<br />
font-size: 0.875em;<br />
}<br />
`  
Now I can rely on the regular html selectors but when I want to I can override them using a class. So when I need an `h2` to look like an `h4`, for example in a sidebar or footer, the addition of a simple class does the job. I&#8217;ve also tried to keep the classnames separate from the document outline, so it should self-document okay too.