---
title: How to Exclude Block Content from Your Template in Twigsn 
tags: 
    - Sculpin
    - Markdown
categories:
    - Front End
---
When looking through the Twig Documentation an Sensio Labs you can often get lost in the great feature sets that come baked into twig. One of the awesome features in Twig is the ability to use the extends feature for templating. Verys similar to how you can use @extend in SASS to reuse code the extend feature is great. 

This is common when you want to re-use code from for the <head> tag.  Butwhat if you want to use some of the header code but want to cusomize some of it.

Simple solution is give them blocks the print with a space empty. 