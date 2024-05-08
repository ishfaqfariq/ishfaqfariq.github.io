---
layout: post
title:  "Unlocking Premium CV Features: My Journey to Downloading CVs for Free"
tags:
 - Bug Bounty
 - Bypass Premium Feature
 - AppSec
 - Web Application Testing
 - API Penetration Testing
 - Ishfaq Fariq
author: "Ishfaq Fariq"
Comments: true
description: |

    "Circumventing Premium CV Features: A Tale of Ethical Hacking and Responsible Disclosure" tells the story of a savvy individual who found a way to access premium CV features without payment. This person, driven by curiosity and a desire to understand systems, encountered a CV-making platform that required a pro account for certain features. Using Burp Suite, a tool in their arsenal, they delved into the website's workings and uncovered a method to manipulate the system. By altering the CV's ID in the download request, they gained access to the premium features for free"
---

### Unlocking Premium CV Features: My Journey to Downloading CVs for Free

So, there I was, just your average person looking to create a snazzy CV. But here's the twist - I'm also a Pentester, which means I can't help but wonder how stuff works and if there's a way to bend the rules a bit.

I stumbled upon this CV-making platform one day and decided to give it a shot. After putting in some solid 30–40 minutes crafting a killer CV, I hit the download button, thinking I'd be good to go. But, nope, they hit me with that classic "you need a pro account" message. What caught my eye was the tantalizing "REMOVE PRO FEATURES" option.

<p align="center">
<img src="/assets/images/posts/Premium-bypass/1 OKbhx-sFdBstGFpUf4gPGA.webp" >
</p>

Now, here's where the fun begins. When you try to snag a CV with those fancy pro features, they throw this message at you when you click download. That's when I thought, "How are they telling who's a pro user and who's not?" And, oh yeah, you'll have their app branding on your free version CV, just FYI.

<p align="center">
<img src="/assets/images/posts/Premium-bypass/1 NRUqU5amHz-SgbWO58sI9w.webp" >
</p>

So, naturally, I did what any curious techie would do - I fired up Burp Suite, the trusty tool in my arsenal, and started intercepting some website traffic. Lo and behold, I discovered that when you hit that download button, the website sends a request to some other place, and it slips in the CV's ID in the message. That's when I had my 'Yeah, boyyy!' moment!

<p align="center">
<img src="/assets/images/posts/Premium-bypass/1 Lmh6DxbxDcfBnMDRwXJnlw.webp" >
</p>

I simply swapped out that ID with the one from my painstakingly crafted CV, which, remember, had left me disappointed a while back. Guess what? The website coughed up an S3 link tied to my CV ID. I popped that link into my browser, and voila! I had the CV in my hands, and I didn't need to pay a dime for it.

<p align="center">
<img src="/assets/images/posts/Premium-bypass/1 qW6KZKuNks4mCE6B0u-zYw.gif" >
</p>

Before I wrap up, I want to make something crystal clear: I'm all about ethical hacking and responsible disclosure. As soon as I discovered this workaround to access premium CV features for free, I didn't just keep it to myself. Instead, I took the responsible route.

<p align="center">
<img src="/assets/images/posts/Premium-bypass/1 enr_HSb--jMFusYOGKrOfg.gif" >
</p>

I promptly reported this issue to the company, ensuring that they were aware of the vulnerability in their system. Ethical hacking is about making the digital world safer for everyone, and that includes helping companies fix security gaps like this one.