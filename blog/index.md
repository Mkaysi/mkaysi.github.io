---
layout: page
title: Blog
permalink: /blog/
excerpt: "Blog index, posts in English and posts in Finnish — Blogin etusivu, postaukset englanniksi ja postaukset suomeksi."
---

* [Posts in Finnish / Suomenieliset kirjoitukset](#suomeksi)

## In English

*Please keep in mind that old blog posts might not reflect the current
 reality or my opinions etc.*

<ul>
  {% for post in site.categories.english %}
    <li>
        <strong><a href="{{ post.url }}">{{ post.title }}</a></strong><br />
        <em>{{ post.excerpt | strip_html }}</em>
    </li>
  {% endfor %}
</ul>

## Suomeksi

*Pidäthän mielessä etteivät vanhat blogaukseni välttämättä heijasta
 todellisuutta tai nykyisiä mielipiteitäni jne.*

<ul>
  {% for post in site.categories.finnish %}
    <li>
        <strong><a href="{{ post.url }}">{{ post.title }}</a></strong><br />
        <em>{{ post.excerpt | strip_html }}</em>
    </li>
  {% endfor %}
</ul>
