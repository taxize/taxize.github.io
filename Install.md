---
layout: page
title: Install
---

## R

Stable version from CRAN

{% highlight coffee %}
install.packages("taxize")
{% endhighlight %}

Development version 

{% highlight coffee %}
install.packages("devtools")
library("devtools")
install_github("ropesnci/taxize")
library("taxize")
{% endhighlight %}

Or clone the repo down and use `devtools` to install locally, or use `R CMD INSTALL` to install from the terminal.

## Python

Stable version from pypi

{% highlight python %}
pip install pytaxize
{% endhighlight %}

Development version

{% highlight python %}
sudo pip install git+git://github.com/sckott/pytaxize.git#egg=pytaxize
{% endhighlight %}

Or clone the repo down and do `make` within the repo folder.