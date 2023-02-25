---
title: Mann-Kendall
description: |
  A look into Mann-Kendall test for monotonic trend.
author: Josh Erickson
show_post_thumbnail: true
show_author_byline: false
show_post_date: true
# for series listing page layout
layout: list-sidebar# list, list-sidebar, list-grid

# for list-sidebar layout
sidebar:
  title: What is monotonicity?
  author: Josh Erickson
  description: In the context of monotonicity, a function can be either **monotonically** increasing (A), decreasing (B), or neither (C). Basically, there are ways to look at a function and determine if it is increasing, decreasing or neither. One way to do that is that for all $x$ and $y$ such that $x \leq y$ preserves an order within a function or not($f(x)\leq f(y)$ or $f(x) \geq f(y)$ or neither). This is **not strictly speaking** in which case $\lt$ or $\gt$ are then used. Mann-Kendall tests to what level this is meaningful or not (monotonic trend) by using a test statistic. 

# set up common front matter for all individual pages in series
cascade:
  author: Josh Erickson
  show_author_byline: true
  show_post_date: true
  sidebar:
    show_sidebar_adunit: false
    text_link_label: ""
    text_link_url: ""
    
  tags:
  - R
  categories:
  - R
  - Statistics
---

** No content below YAML for the series _index. This file is a leaf bundle, and provides settings for the listing page layout and sidebar content.**