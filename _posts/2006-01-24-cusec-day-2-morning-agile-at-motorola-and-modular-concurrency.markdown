---
author: jfcouture
comments: true
date: 2006-01-24 02:26:49+00:00
layout: post
link: http://jfcouture.com/2006/01/23/cusec-day-2-morning-agile-at-motorola-and-modular-concurrency/
slug: cusec-day-2-morning-agile-at-motorola-and-modular-concurrency
title: 'CUSEC day 2 morning:  Agile at Motorola and Modular Concurrency'
wordpress_id: 31
categories:
- Agile
- CUSEC
---

On thursday, I also attended a presentation on "Software Testing as a Social Science" by Cem Kaner, from the Florida Institute of Technology. It wasn't bad, but he spent so much time with traditional definitions of testing that he barely had time to scratch the surface of the social aspects of testing, and missed an opportunity to come up with something really interesting.

Friday morning I went to a talk on an agile experience at Motorola, a CMM level 5 organization. Unfortunately, I did not have time to ask what obstacles this posed to the implementation of an agile process. Things however seemed to go pretty good. The second release delivered the same number of new features in half the time with half the people as the the first release that was only using an incremental style of development, but otherwise the same practices as traditional waterfall inside Motorola. The speaker gave cautions on a lack of documentation to help new members get up to speed (I would have thought that pair programming would help here). He also mentioned that automating tests can be very time consuming, which is something that I've experienced myself.

The next keynote was by Peter Grogono, from Concordia University, about modular concurrency. His plan was to show that OOP has problems and that something better is needed. He of course showed trivial examples in Java to prove that you can do stupid stuff. Duh. So OOP is bad because Java made some stupid choices, especially when it comes to concurrency. Things got more interesting here as he mentioned research that was done in the seventies that offered much better and safer concurrency than Java does today. He quickly showed an example of what he is developing, something that uses "cells" to separate modules. However, his example was the traditional hello world that took 20 lines of bizarre redundant setup. But there was an interesting concept here where the deployment of the code, meaning where it will run, what process, can be changed separately from the the actual program because of the way the language is designed. If I understood correctly, that means you could write the program without worrying too much about concurrency (but still making things modular) and it would be easy afterwards to scale or parrallelize the execution of the program across machines. This talk would have been very cool if Dr. Grogono had skipped the useless and pointless OOP (Java) bashing.
