---
layout: post
title: "How to Create Iso File In Linux"
date: "2016-03-23 15:30:20 +0430"
---

<br />Some time you need to create Iso file from CD or DVD in linux you have very easy solution

<br />open terminal


<br />readom dev=/dev/scd0 f=/path/to/image.iso
<br />Or
<br />dd if=/dev/cdrom of=whatever.iso
<br />Or
<br />cp /dev/cdrom file.iso

<br />it is end :D

<br />thanks ...
