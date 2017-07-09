---
layout: post
title: "The 5 P's of Workloads"
date: 2014-01-17
redirect_from:
 - /blog/the-5-ps-of-workloads/
---

Wordplay comes out in the oddest places.

I was thinking about amusing apparel worn by several VCE folks and VCE alumni at conferences like OpenStack Summit, RICON, and Gluecon. Specifically, the "Vblock Systems: Loving Pets and Cattle Equally since 2009" came to mind.

![Good times](https://pbs.twimg.com/media/Bd4K0PYIcAAJR3o.jpg)

<blockquote class="twitter-tweet" lang="en"><p>. <a href="https://twitter.com/jdooley_clt">@jdooley_clt</a> <a href="https://twitter.com/stevie_chambers">@stevie_chambers</a> <a href="https://twitter.com/aka_dugan">@aka_dugan</a> so awesome &#10;/cc <a href="https://twitter.com/VMTrooper">@VMTrooper</a> <a href="https://twitter.com/jmckenty">@jmckenty</a> <a href="http://t.co/QJJxc2SFkh">pic.twitter.com/QJJxc2SFkh</a></p>&mdash; Jay Cuthrell (@Qthrul) <a href="https://twitter.com/Qthrul/statuses/422788431198961664">January 13, 2014</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

Of course, this "pets and cattle" micro meme was in reference to fairly recent clouderati neologism that seeks to distance the world of older IT workloads such as Microsoft Exchange from the new school of fancy new IT workloads like Node.js or flat out platform as a service or what a Google / Facebook / so-called web scale infrastructure would have on the menu.

While funny teeshirt slogans are a hit, I always felt there was a bit more nuance and not a hard bifurcation point in classifications of workloads. Indeed, one of the prevalent themes in most of the customer meetings is what is the best way to rationalize ever growing populations of workloads -- and there is rarely a mere two camps or categorizations.

Rather, there seems to be a very host oriented discussion in places where the exposure to Enterprise IT has been lesser than a greenfield view of the IT world. For example, even a simple home grown application might need various web servers, application services, and underlying datastores in addition to the plumbing and surrounding accouterments to make that workload a viable and sustainable part of an IT catalog of offerings or as part of an IT portfolio.

I call the vast oversimplification of this diversity the "Cloud Computing Canard" because of the duality of being duck like and a foul (fowl?) rumor. This is one with adequate jest and a respectful tip of the hat to [Simon Wardley](https://twitter.com/swardley).

The 5 P's of Workloads
======================

<blockquote class="twitter-tweet" lang="en"><p>Cloud Computing Canard: &#10;Parrots - MC Legacy IT&#10;Parakeets - Generational IT&#10;Poultry - Canard of Cattle&#10;Popeyes - SP IaaS&#10;Pigeons - Nuisances</p>&mdash; Jay Cuthrell (@Qthrul) <a href="https://twitter.com/Qthrul/statuses/392348600916668417">October 21, 2013</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

To better illustrate my point in meetings and when presenting to wider audiences, I am leery of rolling out the 'pets vs. cattle' neologism and have opted instead for a decidedly tiered approach to classify a simple collection of rationalized applications within a given IT portfolio. The simple way to say it is the 5 P's of Workloads: Parrots, Parakeets, Poultry, Popeyes, and Pigeons.

Parrots
=======

<a data-flickr-embed="true" data-header="true" data-footer="true"  href="https://www.flickr.com/photos/osseous/972258414/" title="100_1373"><img src="https://farm2.staticflickr.com/1332/972258414_dd9cfb8375_n.jpg" width="320" height="240" alt="100_1373"></a><script async src="//embedr.flickr.com/assets/client-code.js" charset="utf-8"></script>

Parrots are the legacy IT workloads that a C-level IT person would likely find on their first day at the office... and it would likely still be there on their last day in the office with an amazing amount of investment in capital and time to make that workload, forgive the pun, talk nicely. So, like actual parrots that very often outlive their owners in the real world, a parrot can live far longer than your career lifetime. Examples could include legacy business logic systems written or packaged to run on a specific dependency riddled OS and library collection that mandates a maniacal dedicated legacy silo of something akin to the bare metal only requirements seen in certain vertical industry specific ISV landscapes. Some would even say that a mainframe application is the canonical example of a parrot style workload.

<iframe width="300" height="168" src="https://www.youtube.com/embed/4vuW6tQ0218" frameborder="0" allowfullscreen></iframe>

Because, as we will all agree... a legacy mainframe application is sometimes quite far from being a post parrot.

Parakeets
=========

<a data-flickr-embed="true" data-header="true" data-footer="true"  href="https://www.flickr.com/photos/striatic/35454685/" title="FLAX on #flickr"><img src="https://farm1.staticflickr.com/29/35454685_775b6e6e29_n.jpg" width="240" height="320" alt="FLAX on #flickr"></a><script async src="//embedr.flickr.com/assets/client-code.js" charset="utf-8"></script>

Parakeets are the legacy IT workloads that a C-level IT person will likely cycle through with each new addition to their tactical or strategic teams that decides a new way of doing what the older IT workload did should do but a brand new everything is involved to make that happen. So, like the parakeet that parents give their children that has a life well lived but ultimately it passes away and a new parakeet is brought in to replace it over some period of time with new toys, cages, feeding gadgets, and more. Examples could include going from Microsoft Exchange 2007 to Exchange 2010 and brand new infrastructure to support that workload in ways that the older environment might not have had.

Poultry
=======

<a data-flickr-embed="true" data-header="true" data-footer="true"  href="https://www.flickr.com/photos/wattagnet/6726228131/" title="Chicken coop"><img src="https://farm8.staticflickr.com/7006/6726228131_07d32c08c5.jpg" width="300" height="225" alt="Chicken coop"></a><script async src="//embedr.flickr.com/assets/client-code.js" charset="utf-8"></script>

Poultry is the ownership oriented view of a C-level IT person that wants a near vertical level of integration in how IT workloads are deployed in a uniform and consistent manner. Like poultry farming there are lots of identical birds everywhere and a high degree of common supporting systems in place to care and feed those birds with regular cycling of the birds as demands rise and fall. Examples could include a specific Linux or Windows deployment where workloads can be virtualized or packaged for rapid deployment here or there of whatever makes the most economically sound path. These need not be public chicken coops per se... indeed, many viable chicken coops are private in nature. Still, most would agree that the largest of the large chicken farms are massively efficient and favor a flavor that tastes like chicken. It is truly the season of seasoning, no?

Popeyes
=======

<a data-flickr-embed="true" data-header="true" data-footer="true"  href="https://www.flickr.com/photos/clotee_allochuku/11523174093/" title="Popeyes Chicken &amp; Biscuits"><img src="https://farm3.staticflickr.com/2821/11523174093_7483ab393d_n.jpg" width="320" height="221" alt="Popeyes Chicken &amp; Biscuits"></a><script async src="//embedr.flickr.com/assets/client-code.js" charset="utf-8"></script>

Popeyes is the fully executed vision of any C-level IT person that realizes IT workloads that combines generalized and specific IT infrastructure all of which is managed, automated, and orchestrated with self-service capabilities aligned to specific lines of business. Granted, unless you travel a lot in the United States or spend time in the Southeastern United Stated, the Popeyes reference might be lost on you. Suffice to say, Popeyes is an example of Poultry as a Service if you will. It's in the business of supplying a fast and tasty experience involving plucked prepared poultry pleasantly peppered and packaged for popping in your mouth. Mmmm mmmm good. More importantly, you drive up to a window and get it. That's right. Poultry as a Service (PaaS). The tastier PaaS if you will. So, in this instance, Popeyes is the drive thru experience as applied to IT workloads. Hungry for some IT? Place your order and drive away. Hungry for more? Repeat this process.

Pigeons
=======

<a data-flickr-embed="true" data-header="true" data-footer="true"  href="https://www.flickr.com/photos/notionscapital/1469623511/" title="Bengals Pigeon Poop Poster"><img src="https://farm2.staticflickr.com/1419/1469623511_c3b2ba80cd_m.jpg" width="161" height="240" alt="Bengals Pigeon Poop Poster"></a><script async src="//embedr.flickr.com/assets/client-code.js" charset="utf-8"></script>

Pigeons are the failed executions of a C-level IT person that hoped to take workloads and create a new way to deliver but ended up with an overly complex and cumbersome sprawling implementation that becomes a far greater nuisance that only delights those that feed the systems involved and encourage their growth to a point where nobody remembers why the workload mattered in the first place or who owns it. So, like the pigeons that can often be a pest or nuisance within dense population centers it is the pigeon that leaves 'feathers and poop' where it lives. Worse still, they tend to multiply.

Plethoras of Peeping, Pecking, Poults
=====================================

Yeah, I said 5 P's and this is clearly number 6 to any possible number if you continue to fuse a letter _p_ approach to this poetic exercise. The point (sorry) being is that there is wondrous variation to take into account. For example, a marketing or vocal line of business led infrastructure selection could be a peacock. So, sometimes saying that it is pets vs. cattle isn't enough.

The good news... all of these fowl that are not so foul have [a place to roost](http://www.vce.com/products/vblock/overview) and can be [loved equally](http://www.vce.com/solution).
