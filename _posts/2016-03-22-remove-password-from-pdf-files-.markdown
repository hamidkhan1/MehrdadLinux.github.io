---
layout: post
title: "remove password from pdf files "
date: "2016-03-22"
comments: true
---
![pdfpass](http://cdn.osxdaily.com/wp-content/uploads/2013/05/password-protect-pdf.jpg)
<br />hello my frind today i have another problem with password security
<br />i found pdf in net that protected by password i dont like it because
<br />after a days i forget where i downloaded and i loss a password
<br />we have very good solution in linux
<br />you must only install pdftk from repositori
<br />apt-get install pdftk
<br />after that use pdftk like this
<br />pdftk yourpdf password protect.pdf input_pw yourpassword output ./1.pdf
<br />solved
