---
layout: post
title: "Remove the duplicate shortcuts"
date: 2013-07-28 23:58
comments: false
categories: [Mac OS]
---




###删除OSＸ打开方式中的重复项

---

 [原文链接](http://bbs.weiphone.com/read-htm-tid-6248807.html/) 
####10.5及以后的系统：


    /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/LaunchServices.framework/Versions/A/Support/lsregister -kill \
    -r -domain local -domain system -domain user

####10.4及以前的系统：


    /System/Library/Frameworks/ApplicationServices.framework/Frameworks/LaunchServices.framework/Support/lsregister -kill \
    -r -domain local -domain system -domain user

之后重启系统即可。
