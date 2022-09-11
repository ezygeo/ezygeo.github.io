---
layout: default
title: products
permalink: /products
weight: 1
---

{% assign sorted = site.projects | where_exp: "item", "item.type == 'products'" | sort: "date" | reverse %}

{% include projects/index.html %}