---
layout: post
title:  "Ruby on rails"
tags:
- ruby
- web
date:   2015-09-29 05:15:27
categories: jekyll update
description: > # this means to ignore newlines until "baseurl:"
  This is my blog where I(rocka0) will talk about all cool stuff on programming
---

What is Ruby on rails? It is a web framework for ruby. That means you can made web apps using ruby on rails like the example given here : ["the example"](http://foodpandapp.herokuapp.com)

It is so cool and all it takes to make an amazing app is this :


{% highlight ruby %}

rails new appname

# => This generates a new rails app

{% endhighlight %}

After you generate the app, cd into the appname directory.

then type :


{% highlight ruby %}
rails generate controller Pages
# ==>> This makes a controller Pages for us
{% endhighlight %}

then in the app/controller/pages.rb file, edit:

{% highlight ruby %}
class PagesController < ApplicationController
end
{% endhighlight %}

to :

{% highlight ruby %}
class PagesController < ApplicationController
  def index
  end
end
# => Make index action in our controller
{% endhighlight %}

after that, go to the app/views/pages/index.html.erb and type :

{% highlight ruby %}
This is my first ruby page!
# => Content on our page. Can be changed to your liking!
{% endhighlight %}

Lastly, go to the config.routes.rb and make it like this :
{% highlight ruby %}
Rails.application.routes.draw do
  root 'pages#index'
  # => sets our default page as our index.html.erb page
end
{% endhighlight %}

This will set your default page as our app/views/index.html.erb

Thats all it take to make a rails app!!


Here is a video tutorial for the same :


<iframe src="https://player.vimeo.com/video/141025380" width="500" height="313" frameborder="0">  </iframe>
Have fun making apps! <em>:D</em>
