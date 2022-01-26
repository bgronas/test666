---
author: Bengt Grønås
title: 'Home Assistant and Google [26.01.2022]'
date: '2022-01-26T11:03:17.941Z'
description: Home Assitant and Google. I've done this wrong. This is how it should be done
featured: false
draft: true
toc: false
usePageBundles: true
featureImage: ha-logo-history.png
thumbnail: ha-logo-history.png
shareImage: logo.png
codeMaxLines: 30
codeLineNumbers: false
figurePositionShow: false
categories:
  - Technology
tags:
  - Home Assistant
  - Google
comment: false
slug: 'home-assistant-google-[26-01-2022]'
keywords:
  - Google
  - Home Assistant
lastmod: '2022-01-26T14:39:28.205Z'
---
# How I mistakenly did the Google integration
I noticed that Alexa was super responsive to my "turn off kitchen table" messages, but my Google were so slow. One day my little **Google home mini** just referenced me to some Nabu Casa stuff, and I suddenly realized "Hey, We're going through the web for this!!" = crap!
- Previously I had just incorporated Google under: http://homeassistant.local:8123/config/cloud/account and It works, but it's not what I want!! This is not local! This is using a subscription! This is extremely much faster and responsive for **Amazon Echo Dot Smart speakers using Alexa** 
![google + nabu casa is OK, too...](google.jpg) 
# How I should have done it
It is not very trivial and intuitive to get this to work without the Home Assistat Nabu Casa suuport. 
1. Create a new project via the Actions on Google website, go to console.actions.google.com
3. 







