---
title: "The Other Way"
layout: post
date: 2018-10-20 12:00
tag: 
- game
- vr
image: /../assets/images/otherway_thumbnail.png
headerImage: true
projects: true
hidden: false # don't count this post in blog pagination
description: "The Other Way is a virtual reality bicycling experience built for the HTC Vive."
category: project
author: callacarter
externalLink: false
---

The Other Way is a virtual reality (VR) bicycling experience built for the HTC Vive. I worked as a game designer and programmer on a team of five to design and develop The Other Way in two weeks.

* Personal Contributions
	* Worked in an interdisciplinary team to design a VR bicycling experience
	* Developed the game using C# in the Unity Game Engine with another programmer
	* Wrote scripts to connect physical bicycle handle and pedal movement to virtual bicycle asset in a 3D space
	* Created dust and wind particle system to create a realistic natural environment
	* Wrote game controller which orchestrated the sequence of events throughout the experience
	* Composed and chose music and sound effects using Logic Pro

The world presents simple story about childhood independence. The player is a child who is on a bike ride with their mother. When a tree falls blocking their path, the child must set off their own and take an alternate path. While simple, telling the story required considerable thought and iterating to arrive at a VR bike experience that was fun, realistic, and not motion-sickness-inducing. 

<dl>
	<iframe width="560" height="315" src="https://www.youtube.com/embed/nmwFswWJpf8" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</dl>

___

### Story
The original story was quite different from our final product. Initially, we aimed to tell a story about being lost. A child - the player - became separated from their mother, and had to find her in the terrifying environment of an unfamiliar forest. While the experience was engaging, we found that the fear the child felt conflicted with the player's real-life sense of adventure and wonder inside the virtual reality bike experience. 

In order to close the gap, we altered the story to evoke a more similar sense of discovery. The child in the final game is encouraged to take another path through the forest by their mother. They are unsure about the journey, but also excited, curious, and increasingly confident, just like a player experiencing the VR biking world for the first time. 

___

### Bicycle Mechanics
To detect bicycle mechanics, the bike uses two HTC Vive trackers; one on the handlebars to track rotation, and one around the player's ankle to track pedaling. Through playtesting, we determined the precise ideal maximum speed, rates of acceleration and deceleration, and rotation speed to make the bicycle feel as real as possible while the player moves through the world. 

When the player is moving on the bike, we add tunnel vision to create a constant point of focus and prevent motion sickness. Initially, we (and our playtesters) experienced abrupt, intense, and lingering nausea while riding the bike. We were inspired by [Google Daydream](https://developers.google.com/vr/elements/tunneling) to add tunnel vision to the VR space. Our subsequent playtesters' experiences were consistent with Google's studies in that they did not notice the tunnel vision while riding through our world. 

___

### Team

* [Conor Triplett](https://www.conortriplett.com)
* [Shengzhi Wu](http://www.wushengzhi.xyz/about)
* [Siyu Chen](http://siyuchenarts.com)
* Max Hsieh


