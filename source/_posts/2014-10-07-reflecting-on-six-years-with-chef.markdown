---
layout: post
title: "Reflecting on Six Years with Chef"
date: 2014-10-07 11:36:43 -0600
comments: true
categories: chef, personal
---

It actually started a bit over seven years ago. I saw the writing on the wall at IBM; my job was soon to be outsourced. I found an open position with the SANS institute, accepted an offer there, and was due to start work in a couple of weeks. Around the same time, my friends Adam Jacob and Nathan Haneysmith had started HJK Solutions. Nathan was on my team at IBM, and he was leaving too. They invited me to join them then, but it wasn't the right time for me. Adam told me that at SANS I should at least use the tools and general infrastructure management model they used. It turned out this was sage advice, as it prepared me to join them a year later.

Around April, 2008, Adam told me he was working on "Chef," a Ruby based configuration management and system integration framework. I was excited about its potential, and a few months later on July 2, 2008, I started with HJK Solutions as a Linux system administration consultant. I got familiar with HJK's puppet-based stack, and ancillary Ruby tools like iClassify while working on their customer infrastructures over the coming months. After Opscode was founded, and we released Chef, my primary focus was porting HJK's puppet modules to chef cookbooks. I was also one of the primary members of the team active in our brand new community. I helped users in IRC and on the mailing list, I wrote blog posts and documentation, and I was the primary/lead developer of opscode/cookbooks.

Why opscode/cookbooks?

Adam had started the repository to give new users a place to begin using Chef with full examples. I continued their development, and solved hard problems of integration using them. There were three important reasons for the repository to exist:

1. We have a body of knowledge as a tribe, and that can be codified.
1. Infrastructure as code is real, and it can be reusable.
1. The best way to learn Chef is to use Chef, and I had a goal to know Chef well enough to teach it to new users and companies.

The development of general purpose cookbooks ends up being harder than any of us really imagined, I think. Every platform is different, so not only did I have to learn Chef, I had to learn how different platforms behave for common (and uncommon) pieces of software in web operations stacks. The platform differences stem from fundamental differences in policy, besides simple filesystem path differences. Fortunately Chef is a flexible framework - it was built to meet these challenges, in fact - so I was able to account for the differences. I think I did a pretty good job overall, but obviously some people disagree. Over the years of managing these cookbooks, I learned a lot about how the community was developing workflows for using Chef, and how they differed from our opinions. I learned also learned how to manage and contribute to open source projects at a rather large scale, and how to have compassion and empathy for new or frustrated users.

In my time at CHEF, nee Opscode, I've had more job changes than anyone else. I started working on cookbooks, added package and release management, switched to technical evangelism and training, came back to cookbooks, and have been solely in production operations for the last year and a half. In that time, I've been frustrated by somewhat sudden job role and manager changes, but I have come to learn this was all preparing me for the future of my career.

I've had the privilege to do work that I love, which is automating hard problems, especially using Chef. I've also had the privilege of being part of the web operations, infrastructure as code, devops, and Chef communities over the past six years. I've been to all four Chef summits, and all three ChefConfs. A thing I've noticed over the years is that many conversations keep coming up at the summits and ChefConf. Fresh on my mind because the last summit was so recent is the topic of cookbook reusability. See, during the time that I managed opscode/cookbooks, I eventually saw the point people in the community were making about these being real software repositories that need to be managed like other complex software projects. We split up the repository into individual repositories per cookbook. We started adding test coverage, and conforming to consistency via syntax and style lint checking. That didn't make cookboks more reusable, but it lowered the barrier of contribution, which in turn made them more reusable as more use cases could be covered.

While using Chef is one of my favorite technical things to do, I have come to the conclusion that based on my experience the best thing I can do is be a facilitator of stronger technical discipline with regard to using Chef. Primarily, this means improving how CHEF uses Chef to build Chef for our community and customers. What this means is overcoming the notion of "the cobbler's children have no shoes," that we have internally. That is to say, there's some gaps in our technical teams in their understanding of Chef itself (despite knowing server protocols and APIs), and we have gaps in the way we use Chef to enable full infrastructure automation. I believe we can overcome these issues, and we should have the best kicks in the land, using the cobbler metaphor.

That is why I'm moving into a new role at CHEF. I'll be joining the team that Jez Humble and Jeff Hackert are on, the "Office of Continuous Improvement and Velocity." In this new role, I will focus on improving our overall technical excellence so we can deliver better products to our community and customers, and so we can have awesome use cases and examples for managing Chef Server at scale.

My first short term goal in this new role is a cookbook to manage Chef Server 12 clusters, including all the add-ons. From the earliest days of opscode/cookbooks, I maintained cookbooks to setup the open source Chef Server. Long time users may remember the "chef solo bootstrap" stack. Since then, we've continued to iterate on that idea, and the "ctl" management commands largely use chef-solo under the hood. The new cookbook will combine and wrap up manual processes and the "ctl" commands to enable us, our community, and our customers to build scalable Chef Server clusters using the omnibus packages. The cookbook uses chef-metal to do much of the heavy lifting.

It should be easy for organizations to be successful with Chef. That includes CHEF! My goal in my new position is to fuel the love of Chef internally and externally, whip up awesome, and stir up more delight. I also look forward to seeing what our community and customers do with Chef in their organizations.

Thank you, and here's to another 6+ years!
