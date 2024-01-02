---
title: "Ember Upgrade Logs"
date: 2024-01-02T19:16:17+05:30
draft: true
toc: false
images:
tags: 
  - ember-js
  - software-development
---

### 02-01-2024

In my work we use ember and the app that I am working on is quite mature and was last updated to the version 3.16. From there we started to upgrade our code base step by step, point release by point release. This upgrade process is not a full time task, where me and my colleagues take up one point release when we have some free time.

#### Our upgrade process

1. We write an analysis doc based on ember's changelog before starting the upgradation process.
2. In the analysis doc, we list any impact to our code base and share the same with our QA for testing.
3. Then we upgrade our ember version using the utility ember-upgrade-cli.
4. Our tests are then run on the upgraded code base and any issues that arise are debugged and fixed.

And the cycle continues.

#### A small note on the issues that arise

Some issues will be very straight forward, they will be mentioned in the changelog clearly like deprecations or syntax changes. These are easy to fix. Sometimes, there will be issues caused because of some mistep the ember team had taken during their development and these will be hard to fix. Somtimes, upgrading to the next version of ember helps.