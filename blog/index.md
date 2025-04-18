---
layout: default
title: Blog
permalink: /blog/
---

# 🧠 Blog

Browse articles created with your background in mind:

- [Individuals](#individual)
- [Institutions](#institution)
- [Incubators](#incubator)

---

## 👤 For Individuals

{% assign individual_posts = site.posts | where_exp: "post", "post.audience contains 'individual'" %}
{% for post in individual_posts %}
- [{{ post.title }}]({{ post.url }})
{% endfor %}

---

## 🏛️ For Institutions

{% assign institution_posts = site.posts | where_exp: "post", "post.audience contains 'institution'" %}
{% for post in institution_posts %}
- [{{ post.title }}]({{ post.url }})
{% endfor %}

---

## 🚀 For Incubators

{% assign incubator_posts = site.posts | where_exp: "post", "post.audience contains 'incubator'" %}
{% for post in incubator_posts %}
- [{{ post.title }}]({{ post.url }})
{% endfor %}

## Featured Post

[→ What’s a Development Brick?](./development-bricks/)

Stay tuned — more articles are coming that explore how different sectors and user types can benefit from [sensingskill.com](https://www.sensingskill.com).