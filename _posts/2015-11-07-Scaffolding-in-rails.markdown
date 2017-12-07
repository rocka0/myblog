---
layout: post
tags:
- ruby
- web
title:  "Scaffolding in ruby on rails"
date:   2017-09-30 08:15:27
categories: jekyll update
description: > # this means to ignore newlines until "baseurl:"
  This is my blog where I(rocka0) will talk about all cool stuff on programming
---

Scaffolding is an easy way to get work done fast in ruby on rails. Scaffolding allows you to generate the <code> controller, model and views</code> all in one go.

Scaffolding basically generates the 7 actions ( create, update, destroy, etc) for a given model. It is just designed to make developing faster.
For beginners, it is OK to use but as you become more advanced, it is advised to hardcode a model, view and controller 

To generate a scaffold, all you have to do is run :
{% highlight ruby %}
rails generate scaffold [model-name] attribute1:type attribute2:type ...
{% endhighlight %}

The model name is the name of the model which will be generated, example: <code>students</code>
The atrributes can be anything like firstname, lastname, email etc.
The type can be a string, text, bool, integer, etc.
Here is a quick demo of you to use a scaffold to generate all the <code>model, views and controllers</code> for a student

<iframe src="http://showterm.io/53492b2f9b066afc3d634#fast" width="640" height="320" frameborder="0">  </iframe>
