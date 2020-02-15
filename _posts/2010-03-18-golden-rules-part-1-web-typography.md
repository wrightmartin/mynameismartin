---
id: 219
title: 'Golden Rules: Web Typography'
date: 2010-03-18T20:36:26+00:00
author: Martin Wright
excerpt: 'This is a collection of rules, best practices and other tidbits I have been collecting over the last 3 years, I thought that as I find them so useful I would share them with the world. The first part focuses on my favourite part of web design: typography.'
layout: post
guid: http://mynameismartin.com/?p=219
permalink: blog/golden-rules-part-1-web-typography/
categories:
  - Design
  - Freebies
tags:
  - golden rules
  - leading
  - measure
  - typography
  - vertical rhythm
---
This is a collection of rules, best practices and other tidbits I have been collecting over the last 3 years, I thought that as I find them so useful I would share them with the world. The first part focuses on my favourite part of web design: typography. This collection is all derivative and I have done my best to list my sources below. 

## Sources & Essential Reading:

  *  <http://www.smashingmagazine.com/2009/08/20/typographic-design-survey-best-practices-from-the-best-blogs/>
  *  <http://www.markboulton.co.uk/journal/comments/five-simple-steps-to-better-typography>
  *  <http://www.adobe.com/education/pdf/type_primer.pdf>
  *  <http://www.webtypography.net/toc/>
  *  <http://www.aisleone.net/2009/design/8-ways-to-improve-your-typography/>
  *  <http://www.alistapart.com/articles/on-web-typography/>
  *  <http://www.alistapart.com/articles/settingtypeontheweb/>
  *  <http://www.smashingmagazine.com/2008/08/11/top-ten-web-typography-sins/>
  *  <http://24ways.org/2006/compose-to-a-vertical-rhythm> 

## Line-length (Measure)

A general good rule of thumb is 2–3 alphabets in length, or 52–78 characters (including spaces). A simple way to calculate the measure is to use Robert Bringhurst’s method which multiples the type size by 30. So if the type size is 10px, multiplying it by 30 gives you a measure of 300px or around 65 characters per line.

**Why?** Long lines of text require longer periods of attention before the eye moves lines, short lines of text require moving lines too often, which can break rhythm, an optimum measure means creating a comfortable balance.

## Line-height (Leading)

Optimum line-height is 1.5 x text size (1.5em), this should be lowered for large headings (1.2-1.4em).

**Why?** Too much leading causes the eye to jump from line to line and can be disruptive to reading, too little leading creates a dense &#8216;typographic color&#8217; which looks less appealing, and can create the illusion of &#8216;more&#8217; text.

Measure and leading are related, when increasing your measure, ensure you adjust your leading, longer measure requires greater leading and vice-versa. These rules can change depending on choice of font, for example, a font with a larger x-height (literally the height of the x character) such as Verdana, may require more leading. 

## Letter-spacing

In most cases letter spacing should remain default, as fonts are designed to work best at this setting, in special cases, such as all uppercase or small caps increase letter-spacing by a small amount (~1px).

**Why?** Uppercase characters are tighter and will require extra spacing to improve readability.

## Vertical Rhythm

Ensure that the spacing between elements is equal to, or multiples of, your line-height (Measure) e.g.

`body {<br />
font-family: Helvetica, sans-serif;<br />
font-size: 12px;<br />
line-height: 15px;<br />
}<br />
p {<br />
margin-bottom: 15px;<br />
}`

**Why?** The baseline grid is the skeleton of your typographic layout and provides consistency. Conforming to your baseline ensure flow and improves readability. A continuous rhythm in the vertical space keeps all the text on a consistent grid so that proportion and balance are retained throughout the page, no matter the type size, leading or measure.

## Hanging Punctuation

Quotation marks and bullets should always be set &#8216;outside&#8217; in the gutter outside of your body text, so that the text remains consistently aligned.

**Why?** Maintaining left alignment means that the text is scannable and rhythm is uninterrupted. The eye looks for straight lines everywhere, when type is indented in this way, it maintains the flow of text.

Got any of your own to add? Let me know in the comments.