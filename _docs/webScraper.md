---
title: "Web Scraper"
permalink: /docs/web-scraper/
excerpt: "A powerful design that allows anyone to scrape the web for thousands of emails concurrently and in a scalable fashion. The possibilities are limitless!"
modified: 2016-09-08
redirect_from:
  - /theme-setup/
---

{% include base_path %}

## Abstract

In our information age, Marketing is extremely key to bussiness success. However, the importance arises in finding the correct people. I have designed a product that will allow anyone to find 12,000 unique email addresses a day for any bussiness goal. 

This product allows anyone to generate 12,000 emails a day concurrently. This article describes the technical aspects of the algorithm and how it generates these emails.

<figure>
  <img src="{{ base_path }}/images/emailmarketing.png" alt="emailmarketing">
</figure>

## Preliminary Definitions <- Skip if you are familiar about web scrapers

**Web scraping** - (web harvesting or web data extraction) is a computer software technique of extracting information from websites. This is accomplished by either directly implementing the Hypertext Transfer Protocol (on which the Web is based), or embedding a web browser.

**Multithreading** - is the ability of a central processing unit (CPU) or a single core in a multi-core processor to execute multiple processes or threads concurrently

<figure>
  <img src="{{ base_path }}/images/multithread.jpg" alt="multithread">
</figure>

## The Web Platform

The World Wide Web in today's world is filled with people who have shared their email on various websites. These sites generally surface from forums to blogs that serve very niche groups. These emails are public information that can be key to helping any bussiness grow. The Problem at hand is that we need a way to capture all these emails and process them in an efficient way.  

## The Ultimate Solution

I have built a web scraper on top of the anemone and nokogiri framework. You can learn more about these two libraries [here](https://www.ruby-toolbox.com/categories/Web_Content_Scrapers).

This webscraper will scrape thousands of webpages a hour and search for emails. These emails will then be classified into unique lists. Given the input of a damain name (ex. twitter.com), the web scraper will do an exhaustive search to find emails on the website. 

This type of product can bring any business owner value that wants the emails of a certain niche domain. For example, if a Rock Musician wants to sell his music. He will need to find very specific customers that enjoy rock music. Using the webscraper, we can target specific rock websites and help gnerate this musician potential customers.

<figure>
  <img src="{{ base_path }}/images/greenSpider.png" alt="spider">
</figure>

---

