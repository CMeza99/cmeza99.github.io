---
layout: article
title: "RedHat OpenShift Cartridge Patch"
modified: 2015-06-03T22:45:30-07:00
categories:
excerpt: "Pull request to update DokuWiki Quickstart Cartridge"
tags: [webdev, dev]
image:
  feature:
  teaser:
  thumb:
#date:
---
The [OpenShift](https://www.openshift.com/) [QuickStart Cartridge](https://developers.openshift.com/en/get-involved-extend-openshift.html) for [DokuWiki](https://www.dokuwiki.org/) was out of date and using a version that containted known security vulnerabilities. Naturally I did not want to use this version for my wiki, [http://wiki.droots.org](http://www.droots.org). I forked the cartridge and made the appropriate updates. After deploying and verifying my changes worked, I submitted a [pull request](https://github.com/openshift/dokuwiki-quickstart/pull/10).

OpenShift is [RedHat](http://www.redhat.com/)'s stack for cloud hosting.
