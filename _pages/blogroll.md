---
layout: default
title: Blogroll
links:
  - title: Read Max
    url: https://maxread.substack.com/
---


{% assign links = page.links | sort: "title" | sample: page.links.size %}
{%- for item in links %}
- [{{ item.title }}]({{ item.url }})
{%- endfor %}
