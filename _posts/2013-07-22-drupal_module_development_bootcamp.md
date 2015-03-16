---
layout: article
title: "Drupal Module Development Bootcamp"
modified:
categories:
excerpt:
tags: [webdev, php, drupal]
image:
  feature: 2013-07-22-feature-Drupal-7-Module-Development.png
  teaser: 2013-07-22-teaser-Drupal-7-MockupCover.png
  thumb:
#date:
---

### About the bootcamp
> This free program is designed to improve the Drupal skills of beginner- to` intermediate-level Drupal and PHP developers. Together as a group, we're diving into Drupal's APIs and helper functions, developing custom modules (many of us for the first time), using version control and other Drupal developer best practices, and advancing our Drupal skills to the next level.

### My experiance
I took this class with the intent of refreshing and updating my php skills. About 25 people were selected to participate in the bootcamp. Less then 10 of us were able to complete the class, develope a fuctional module  and submit it to the Drupal project. I meet  a great bunch of people and had a lot of fun.

I developed the [Password Backup & Recovery](https://www.drupal.org/sandbox/digitalroots/2153457). It started out as a joke to make use of the module [Bad judgement](https://www.drupal.org/project/bad_judgement). But it was inspired by every manager who has asked to have their subordinate passwords.

I leveraged the [AES encryption](https://www.drupal.org/project/aes) module to maintain some security when exporting the passwords. In the process I discovered a major bug in the module, which I submitted a bug report for and later submitted a patched.

{% comment %}
link to post about patch
https://www.drupal.org/node/2188325
https://www.drupal.org/node/2228367
{% endcomment %}
