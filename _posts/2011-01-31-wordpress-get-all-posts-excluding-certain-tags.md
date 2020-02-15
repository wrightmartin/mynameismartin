---
id: 310
title: 'WordPress: Get all posts excluding certain tags'
date: 2011-01-31T22:19:07+00:00
author: Martin Wright
excerpt: |
  This is something I do in almost every WordPress theme I create, yet whenever I come to do it I can never remember how. I'm hoping that writing it down will help me remember.
  To get all posts, except those with certain tags, you have to use the function 'tag__not_in()'.
layout: post
guid: http://mynameismartin.com/?p=310
permalink: blog/wordpress-get-all-posts-excluding-certain-tags/
categories:
  - Development
  - Wordpress
tags:
  - exclude
  - tags
  - tag__not_in
  - Wordpress
  - WP_Query
---
This is something I do in almost every theme I create, yet whenever I come to do it I can never remember how. I&#8217;m hoping that writing it down will help me remember.  
To get all posts, except those with certain tags, you have to use the function &#8216;<a title="tag__not_in on the WordPress Codex" href="http://wordpress.org/tags/tag_not_in" target="_blank">tag__not_in()</a>&#8216;. It takes an array of tag IDs as an argument, and hey presto! Example code below:  
`//get all news except those tagged with 'feature' (ID=14) or 'also' (ID=16)<br />
$args=array(<br />
'showposts'=> 6,<br />
'tag__not_in'=> array(14, 16),<br />
);<br />
$recent = new WP_Query($args); while($recent->have_posts()) : $recent->the_post();?>`