---
comments: true
date: 2010-05-17 11:35:34
layout: post
slug: blackberry-spf-records
cover: http://farm3.static.flickr.com/2271/2115303225_1688c64d8b_m.jpg
title: Blackberry SPF Records
wordpress_id: 34219
categories:
- Consulting Days
- random
tags:
- blackberry
- dns
- email
- spf
---
[If you use Blackberry Internet Service and have seen delivery issues related to SPF records when using your own domain name or company domain name you should consider the following suggestions:
  
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<!-- topline -->
<ins class="adsbygoogle"
     style="display:inline-block;width:728px;height:90px"
     data-ad-client="ca-pub-4341041390314512"
     data-ad-slot="5282472782"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

[Firewall and connection requirements for the BlackBerry Internet Service](http://www.blackberry.com/btsc/search.do?cmd=displayKC&docType=kc&externalId=KB11036&sliceId=SAL_Public&dialogID=119218117&stateId=1%200%20119212726)
  

[Corey Gilmore's Blog](http://coreygilmore.com/blog/2007/08/21/spf-for-the-blackberry-bis-and-google-for-your-domain/)
  

[Easy SPF Wizard](http://spfwizard.com/)
  

  

Example:
`
$ host -t txt somedomainyouareusing.com
somedomainyouareusing.com text "v=spf1 a:smtp01.bis.na.blackberry.com a:smtp02.bis.na.blackberry.com a:smtp03.bis.na.blackberry.com a:smtp04.bis.na.blackberry.com a:smtp05.bis.na.blackberry.com ~all"
`

