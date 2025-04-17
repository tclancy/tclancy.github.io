---
layout: post
title: "Great North Property Management: Great North Website and Secured Areas"
tags: [django,api,integration]
date: 2010-06-01
author: "Tom Clancy"
---

# Great North Property Management: Great North Website and Secured Areas

## 2010-06-01

_Provided a Django CMS for the main website, a secured area for residents to manage their accounts and an engine to run individual sites for each property._

<p>Starting out, Great North felt like a fairly typical project: content management system for the main site, some API integration to grab data from their vendor and a secured area for clients. Each of these things is a regular feature in projects I build; API integration and secured areas are almost meta solutions: whatever industry a client is in, they may have need for these things. And a content management system is&nbsp;<em>de rigueur</em> for most client web sites nowadays (cue Old Man Mode: "In my day, we had to author all our pages by hand. And the only includes were SSI and they were dump ad you couldn't do any logic in them.").</p>
<p>Happily, this project turned out to be fun. While it didn't hurt that the client contact was a friend of Lightfin's, what made it enjoyable for me was perspective. When I started as a web developer, we lived in a series of apartments with consistently horrible management companies. Just before we moved into our home in Dover, we lived in a townhouse in a small condo community that barely felt like a community at all. So this project felt like a chance to build something that would improve users' lives. We could use the web to make something that would be a huge improvement over the experience I suffered through with deaf management companies whose only interaction was sticking a hand out to take your rent.</p>
<p>The <a href="http://greatnorth.net/">site itself</a> runs off the Django CMS I've been using for projects this year. The other two applications serve Great North clients. The first is a site for all members across the communities Great North manages. This site allows them to check their current account balance, review previous charges and any recurring charges they have. They can also submit maintenance requests and check the status of their previous requests. Finally, they can maintain their contact information in the site. These activities talk directly to the <a href="http://www.jenark.com/">Jenark</a> software running on the server in Great North's office via custom API calls written by Jenark. In addition to the user-facing API calls, the application calls out every night to get an updated list of all associations Great North manages, then updates the list of units and residents in each building to make sure new residents have automatic access to the site as soon as they move in (and make sure they lose that access once they move out).</p>
<p>The third application powers a "mini site" for each association. The mini sites help to provide that sense of community I found lacking when we lived in our townhouse; in spite of it being only 30 or so units in a very small space, it was easy to never really know your neighbors unless they threw a wobbler at the annual meeting. The mini sites provide a list of upcoming events in the community and the ability to subscribe to updates, a directory that lists all board members and any other resident who choses to be listed and any documents residents may need. Better still from Great North's perspective, all aspects of the mini sites can be managed by any resident listed as an administrator.</p>
<p>In the end, this wound up being a prototype for what I would like projects to be: a good working relationship with a client that results in a site/ application that both makes their lives easier and makes their users happy.</p><img src="/assets/portfolio/gn-1.jpg" alt="Homepage Great North's web site serves over 19,000 resident customers" />
<img src="/assets/portfolio/gn-2.jpg" alt="Member Area Members can check their account balance & history, submit maintenance requests and update their contact information." />
<img src="/assets/portfolio/gn-3.jpg" alt="Mini-Sites Each association has its own website with a member directory, calendar of events and a document library that can be managed by board members." />

