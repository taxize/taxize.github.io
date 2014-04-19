---
layout: default
title: Home
---

# taxize <i class="fa fa-sun-o"></i> taxonomic toolbelt for R & Python

Taxonomy deals with the names of living things - well, in this context, we're dealing with living things. So let's call it biological taxonomy. 

Almost all biologists are likely to deal with names, whether they study a single species or 10 species, or 10,000 species. Organism names are created by people - thus they are messy of course. Two different names can be given to the same species, and two completely different taxonomic groups could have the identical name at different taxonomic ranks. All these problems and more make it so that you of course want to do your taxonomic sleuthing with a powerful, repeatable, for-loopable, tool. 

We created a tool to ease the headache of taxonomy. What makes it possible is the many online taxonomy databases that we can give you an interface to. Take a look at the sources of taxonomic databases we wrap in taxize at the [Sources](/Sources) page.

What can you actually do? Let's take a look.

### R

{% highlight coffee %}
library("taxize")
col_children(name = "Apis")
{% endhighlight %}

And you get 

{% highlight coffee %}
    id                name     rank
6971712  Apis andreniformis  Species
6971713         Apis cerana  Species
6971714        Apis dorsata  Species
6971715         Apis florea  Species
6971716  Apis koschevnikovi  Species
6845885      Apis mellifera  Species
6971717    Apis nigrocincta  Species
{% endhighlight %}

Awesome eh.


### Python

{% highlight python %}
import pytaxize
pytaxize.col_children(name = ["Apis"])
{% endhighlight %}

{% highlight python %}
[    id                name     rank
6971712  Apis andreniformis  Species
6971713         Apis cerana  Species
6971714        Apis dorsata  Species
6971715         Apis florea  Species
6971716  Apis koschevnikovi  Species
6845885      Apis mellifera  Species
6971717    Apis nigrocincta  Species]
{% endhighlight %}

-----

Want to see something else added? Open an <a href="https://github.com/ropensci/taxize/issues/new">R</a> or <a href="https://github.com/sckott/pytaxize/issues/new">Python</a> issue.