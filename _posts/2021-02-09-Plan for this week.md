---
layout: post
title: "Using dates"
date: 2021-02-09 00:00:00
category: Category
author: User
tags: [plan]
summary: Summary of the article
---

{% newthought 'Week' %} {{ page.date | date: "%W" }} _{{ page.date | date: "%A"   }}, {% assign d = page.date | date: "%-d" %}{{ page.date | date: "%B" }} {% case d %}{% when "1" or "21" or "31" %}{{ d }}st{% when "2" or "22" %}{{ d }}nd{% when "3" or "23" %}{{ d }}rd{% else %}{{ d }}th{% endcase %}, {{ page.date | date: "%Y" }}&nbsp;_{:  .marginnote}

# Using the date