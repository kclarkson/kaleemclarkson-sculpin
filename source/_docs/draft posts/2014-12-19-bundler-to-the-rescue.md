---
draft: true
title: Bundler to the Rescue! Saved from the Conflicting Rubies Purgatory 
tags:
    - ruby
    - bundler
categories:
    - front end
---
It was a late night in November after one of my sons freezing football games where all limbs had lost just a little bit of feeling. After a hot coffee and some heat I was eager to work on a project. Open my terminal and run compass watch and whack errors everywhere !@#@(%#@# is what I screamed outloud to myself. 

I stared at the screen with that familiar feeling that I was now lost in the conflicting rubies purgatory.  But wait Bundler to the Rescue!!

What Causes the Error
Sometimes for me understanding why things are going wrong provides a sense of clarity to the situation. So what is really going on? These errors are happening because they are conflicting because one of your projects may require 1.1 of a gem you have 1.2 installed.  So the lazy suggestions would be to delte the wrong gem.  But wait!!!!! When you go back to your previous project you more errors will arise. When working with different frameworks that have ruby gem dependencies

Solution:
So how could we install different versions of the needed gems and tell the specific project which ones to use? Or how could we prevent the errors 

Well what if


Implement in Your Workflow: Don't Get Lazy:

You see I had just returned from BadCamp in San Francisco so I had all sorts of things on my local computer. Drupal 8 which needed a Drush update, Sculpin my static generator for my github page and other compass theming projects.   

Bundler to the Rescue!!  The worst part is that I had installed bundler over a year ago. But after a few times of not implementing into my workflow I forgot about it and was to use a similar stack for a while.  Then one day boom! Conflicting rubies errors everywhere. 

So I took a deep breath and really tooke the time to understand the concept of bundler.  Well it keeps the required gems in its own little bundle. hahaha see what did did there?  

So as along as you create a specific gem file in your project, run bundle install, then to watch or compiling your css you would run 
~~~
"bundle exec watch" or "bundle exec compile".
~~~ 

I asked someone well don't you hate writing "bundle exec" before all of your commands?  And he said, you only have to "watch" in the begining so its totally worth the 11 extra key strokes.


You can also use [fenced code blocks][like] with a syntax declaration at the top.
The markers are `~` instead of <code>`</code>.

[like]: http://michelf.ca/projects/php-markdown/extra/#fenced-code-blocks

~~~php
if ($fencedCodeBlock->syntax !== 'PHP') {
    throw new UnexpectedValueException("wat");
}
~~~
Like this addition to the skeleton? You can thank for [@Pawka](https://github.com/Pawka)
for suggesting it. :)  
