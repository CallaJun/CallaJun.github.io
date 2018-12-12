---
title: "Pollen Nation"
layout: post
date: 2018-11-20 12:00
tag: games
image: /../assets/images/pollennation1.png
headerImage: true
projects: true
hidden: true # don't count this post in blog pagination
description: "Pollen Nation is an asymmetrical, virtual reality and controller-driven game."
category: project
author: callacarter
externalLink: false
---

Pollen Nation is an asymmetrical, multiplayer, virtual reality (VR) and controller-driven game built for the HTC Vive and PC. I worked as a game designer and programmer on a team of five to design and develop it in three weeks.

* Personal Contributions
	* Worked on an interdisciplinary team to design and develop an asymmetrical, multiplayer game for VR and PC
	* Developed the game in C# in the Unity Game Engine with another programmer
	* Wrote scripts to handle character controls and behavior
	* Wrote game controller which orchestrated the sequence of events throughout the experience

It's the Kentucky Derby of the bug world. A praying mantis, embodied by a player in a VR headset, takes on three bees, controlled by three Xbox controller players. The bees' goal is to work together to pollinate all of the flowers in the arena before the timer reaches zero, and the mantis's goal is to stop them. At the mantis's disposal are magical Venus flytrap seeds that can be thrown to slow the bees down.

<dl>
	<iframe width="560" height="315" src="https://www.youtube.com/embed/Aw_DF2T4vqU" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</dl>

___

### Design
The team went through multiple iterations informed by prototypes and playtests before we reached our final product. From the beginning, we set out to design an asymmetrical game with one player in a VR headset and *n* players using Xbox controllers. 

#### Stage 1: Ideation & Prototyping
<dl>
	<img width="50%" align="right" src="/../assets/images/pollennation2.jpeg">
</dl>
From boxing worlds and angry mobs to a praying mantis a riding circus phoenix to escape an evil ringmaster, we explored many different worlds before arriving at a mantis versus bees pollination experience. 

Most of our original ideas involved a stationary VR player riding and controlling a flying animal with a fire-emitting tail while fending off a mob of angry bees' stings by punching and shielding. We removed the player's control of the flying animal early on in fear that the multitasking would be too overwhelming. We soon determined that the bird - or whichever object on which our VR player would stand - must be stationary for two reasons:

1. We did not intend for speed to be one of the bees' challenges, so a flying bird would not enhance the the bees' experiences. Since the bees ejected stingers from behind, it was awkward for them to fly in front of a moving object (the bees could not sting from behind or they would be killed by the bird/phoenix's fire-emitting tail). 
2. With diverted attention and no control over the flying object, the VR player might become overwhelmed and motion sick. 

To answer the question "Why bees?" we gave the bees a pollination mechanism. Our initial prototype stood a mantis magician at a circus at the center of an arena, on top of a large flower. 

<dl>
	<img align="right" src="/../assets/images/pollennation3.png">
</dl>

The mantis's goal was to pull various objects - venus flytraps, random household items, rabbits - out of a magician's hat and throw them at the bees to decrement their health, and the bees' stung the mantis by ejecting stingers and launching them to decrement the mantis's health. The game ended in three cases:

1. All of the bees were dead (mantis victory).
2. The bees fully pollinated the flower (bees victory).
3. The mantis lost all health (bees victory).

#### Stage 2: Reeling It In
<dl>
	<img width="50%" align="right" src="/../assets/images/pollennation4.png">
</dl>
A round of playtesting confirmed our suspicions - the game was simply too *much*. The mantis was overwhelmed by the bees flying toward it, the bees were easily subdued by the mantis's many objects, and there was no clear strategy on either side. However, feedback showed that players were intrigued by the asymmetrical nature of the game and enjoyed the mechanisms (throwing, pollinating, flying). 

We knew we needed to eliminate one of the bees' objectives (two goals - pollinating the flower and killing the mantis - was too much). The question was which one. We chose the mechanism that we believed would be more immediately clear to new users: the stinging. It was a fight to the death between a mantis and several bees. Now, bees could regain health by pollinating the flower on which the mantis stood (and risking being attacked by the mantis). 

Playtests had revealed that when the pollination goal was made clear, many bees did not try to sting the mantis (aiming was difficult). We liked the pollination mechanism (it justified the bees' existence, opened the door for satisfying haptic feedback on the Xbox controllers, and seemed more interesting), so we kept it and nixed the stinging mechanism.

<dl>
	<img width="50%" align="left" style="margin-right: 1%;" src="/../assets/images/pollennation7.png">
</dl>

To simplify the throwing mechanism and its place in the game, we eliminated all throwable objects but the Venus flytrap seed. We also changed the mantis from a magician - a remnant of the old circus theme - to a non-magical mantis with a magical seed bag. 

Subsequent playtests revealed that the game was still an overwhelming experience for both sides, so we made our most dramatic change and further limited the bees' objectives. Rather than the mantis trying to kill the bees and vice versa, we changed the bees' goal to pollinating the flower and avoiding being hit by the mantis's Venus flytrap seeds (which reduced their health). Bees, in this iteration, could not regain health. The pollinating mechanism they once used to regain health now contributed to the flower's total pollination, which was displayed on a bar at the bottom of the screen. 

After this change, playtesters playing as bees did not feel overwhelmed, but the mantis felt accosted whenever bees flew in the vicinity of the flower. When bees flew directly into the mantis, the authenticity of the VR experience was compromised because the mantis could not feel the bees. 

<dl>
	<img width="100%" align="right" src="/../assets/images/pollennation5.png">
</dl>

We fixed this with a change of scenery. The mantis now stood on a teacup pedastal at the center of the arena and prevented bees from pollinating three flowers around the arena.

#### Stage 3: Tweaking
At last, we had our game. Now, we had to adjust variables to balance the mantis and bees' strength. Through multiple rounds of playtesting, we adjusted the following:

* The length of the game. We started at two minutes and after reducing it to 90 seconds, we decided that each game would include three one-minute rounds so that a new players on each side would develop strategies.  
* The length of time bees were trapped by Venus flytraps. When the game was two minutes long, the bees were trapped for 20 seconds. We wanted the bees to be trapped for long enough that they had an incentive to save each other. 
<dl>
	<img width="60%" style="margin-left: 1%;" align="right" src="/../assets/images/pollennation6.png">
</dl>
* The ratio of bees to flowers. We played around with more and less bees and flowers, but settled on three and three. Playtests had shown that with this arrangement, of the three rounds each side won 2 to 1 roughly 50% of the time. The three flower technique created a climax in the game's interest curve. During the pollination of the first two flowers, generally, the bees split up and the mantis's attention was divided. By the time only the third flower was left, generally in the last seconds of the game, the mantis was only focusing on one flower, which the bees needed to pollinate. 

Finally, we playtested tutorial images that were concise and gave players of many gaming experience levels enough information to succeed in the game. 

<dl>
	<img width="70%" src="/../assets/images/pollennation8.gif">
	<img width="100%" src="/../assets/images/pollennation9.gif">
	<img width="100%" src="/../assets/images/pollennation10.gif">
</dl>

___

### Engineering

___

### Team
* [Chia-chi Chang](https://chiachiaurorakingdom.weebly.com/portfolio.html) 
* [Swapnil Mengade](https://swapnilmengade.wordpress.com)
* [Varun Mehra](https://www.varunmehra.me)
* Alexander Woskob
