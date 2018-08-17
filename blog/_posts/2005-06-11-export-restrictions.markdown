---
comments: true
date: 2005-06-11 12:58:35
layout: post
slug: export-restrictions
title: Export restrictions
cover: http://farm4.static.flickr.com/3165/3075583696_a6b8926b60_m.jpg
wordpress_id: 2686
categories:
- NeoNova and Digitel
- random
tags:
- bugs
- export
- social
- software
---

I’ve got a Mac. I have a metric ton of contacts (+10k). One might expect this makes for an elegant and natural fit since there is Address Book for the Mac.

Having lots of contacts should mean you are able to communicate with those contacts. Or, maybe that you want to feel like you are making up for lost time when you were the last kid picked for kickball. In either case, you want it to be a simple matter for keeping these contacts updated. Plaxo is useful for automation of the update process. LinkedIn is useful for the mining of these contacts and the relationships that flow from them. .Mac just works with my Mac. I’ve also got a .Mac email account that can use the iSync managed Address Book I store there. I’ve also got a Gmail account. So, why can’t they all just get along?

Jason Calacanis noted noted [the absence of Gmail functionality to export contacts](http://calacanis.com/2005/06/11/exporting-gmail-contacts-or-are-you-trying-to-lock-me/). He goes on to mention his goal is to sync up with LinkedIn. I periodically ping their feature request form to request the same export functionality. Sadly, I can only export from Plaxo to LinkedIn — but not the other way.

So far, I’ve ended up writing a perl script to just strip away LinkedIn contact listings to the format I need. You’ll also recall that export from Orkut was extremely simple — and it is another Google property. Then, I can dump these into Address Book once they are in Plaxo since Plaxo has a vCard export feature that works. At this point, Plaxo is the only thing that seems to want to play well with others.

Well, If you are on my LinkedIn or have access to my Plaxo then you know I try to maintain both. Yes, I’ve got a bluetooth phone that can sync with the Mac via Address Book and iSync. Yes, I’ve got a .Mac account so that I can maintain contacts there. The ultimate would be universal sync of a vCard service or something that gave a central repository like .Mac that you could dip across via API from other services such as LinkedIn and Plaxo that both have different goals but require a database of your contacts. Also, there are some folks that I don’t put in LinkedIn or Plaxo because of the sometimes nebulous stance on privacy that these services might [project](http://www.google.com/search?q=plaxo+%22privacy+concerns%22), infer, [exhibit](http://www.google.com/search?q=linkedin+%22privacy+concerns%22), or [evolve](http://www.google.com/search?q=gmail+%22privacy+concerns%22).

So, if there was a dip ready service out there it would have to have a few features that no service (I’ve seen) has _yet_. There would have to be opt in and opt out that could be controlled by the contact. Oh, now that’s a prickly concept. Think of all those “We Care About Your Privacy [tm]” pamphlets that you get in the snail mail regarding how financial service groups sell protect your privacy and personal information. Does that mean for this fictional service — when I add you to my contact list — would you get a copy of my intentions and the privacy policy of the service sent to you with the ability to allow for your inclusion in this service? Or, would it just add you and now I’ve become another attack against your privacy?

If you have used Plaxo for any period of time you know that many email administrators simply block anything and everything that Plaxo tries to send on your behalf. Plaxo lets you handle bounces and some of them have very informative messages from the email administrator (well, their servers) that politely say “pound sand” and “your kind is not welcome here”.

So, Plaxo might want to play well with others, but it does not mean everyone will let their children out to play with them. That makes Plaxo the kid with the really cool bike that other kids want to play with but the parents don’t trust completely.

