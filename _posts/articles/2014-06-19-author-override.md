---
title: Override Author Byline Test Post
date: '2014-06-19 00:00:00'
layout: post
excerpt: An article to test overriding the default site author.
categories: articles
tags:
- sample-post
- readability
- test
author: billy_rick
comments: true
share: true
modified: '2016-06-01T18:18:57.000+00:00'
image:
  feature: "/forestryio/images/Screen Shot 2016-07-22 at 9.40.16 AM.png"
  credit: WeGraphics
  creditlink: http://wegraphics.net/downloads/free-ultimate-blurred-background-pack/
---

For those of you who may have content written by multiple authors on your site you can now assign different authors to each post if desired.

Previously the theme used a global author for the entire site and those attributes would be used in all bylines, social networking links, Twitter Card attribution, and Google Authorship. These `owner` variables were defined in `config.yml`

Start by modifying or creating a new `authors.yml` file in the `_data` folder and add your authors using the following format.

```yaml
# Authors

billy_rick:
  name: Billy Rick
  web: http://thewhip.com
  email: billy@rick.com
  bio: "What do you want, jewels? I am a very extravagant man."
  avatar: bio-photo-2.jpg
  twitter: extravagantman
  google:
    plus: BillyRick

cornelius_fiddlebone:
  name: Cornelius Fiddlebone
  email: cornelius@thewhip.com
  bio: "I ordered what?"
  avatar: bio-photo.jpg
  twitter: rhymeswithsackit
  google:
    plus: CorneliusFiddlebone
```![]({{ site.baseurl }}/forestryio/images/Screen Shot 2016-07-21 at 2.24.18 PM.png)

To assign Billy Rick as an author for our post. You'd add the following YAML front matter to a post:

```yaml
author: billy_rick
```
