---
layout: default
title: "文章分类"
permalink: /category/
description: "像素信标文章分类页面 - 按分类浏览所有文章，包括实用教程、网赚教程、技术教程、软件工具、购物攻略等。"
---

# 文章分类

按分类浏览像素信标的所有文章内容：

## 📚 实用教程
<p>各种实用的数字工具使用教程，包括网盘扩容、下载提速等实用技巧。</p>
<ul>
{% for post in site.categories['实用教程'] %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span> - {{ post.date | date: "%Y-%m-%d" }}</span>
  </li>
{% endfor %}
</ul>

## 💰 网赚教程
<p>网络赚钱方法和教程，包括网盘推广、分享赚钱等副业项目。</p>
<ul>
{% for post in site.categories['网赚教程'] %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span> - {{ post.date | date: "%Y-%m-%d" }}</span>
  </li>
{% endfor %}
</ul>

## 🔧 技术教程
<p>技术相关的教程和指南，包括编程、脚本、自动化等技术内容。</p>
<ul>
{% for post in site.categories['技术教程'] %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span> - {{ post.date | date: "%Y-%m-%d" }}</span>
  </li>
{% endfor %}
</ul>

## 🛠️ 软件工具
<p>实用的软件工具推荐和使用指南，提升工作效率。</p>
<ul>
{% for post in site.categories['软件工具'] %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span> - {{ post.date | date: "%Y-%m-%d" }}</span>
  </li>
{% endfor %}
</ul>

## 🛒 购物攻略
<p>购物优惠信息和攻略，包括电商活动、红包雨时间表等。</p>
<ul>
{% for post in site.categories['购物攻略'] %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span> - {{ post.date | date: "%Y-%m-%d" }}</span>
  </li>
{% endfor %}
</ul>

---

<div class="category-stats">
  <h3>分类统计</h3>
  <ul>
    {% for category in site.categories %}
      <li><strong>{{ category[0] }}</strong>: {{ category[1].size }} 篇文章</li>
    {% endfor %}
  </ul>
</div>