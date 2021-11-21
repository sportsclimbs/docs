---
title: "Intro"
date: 2021-11-21T07:28:55Z
draft: false
---

The content management system (CMS for short) allows editing of the site through a friendly interface from anywhere with a web connection.

All you need is a username and accompanying password. This works in a similar way to Wordpress's CMS.

## How to use it

The current CMS is [Netlify CMS][1]. To access it you simply add a forward slash and the word `admin` to the end of the Sport Climbs url: [sportclimbs.uk/admin](https://sportclimbs.uk/admin)


## Use with Cloudinary

Cloudinary is a website where we can keep images and then use them in our website. It's possible to set this up with the CMS. I've included some code to do so but it may not be working yet.

Anyway to do so requires that we are first [logged into our Cloudinary account[5]] on [Cloudinary][3] in a different browser tab. 

See [images][4] in the to do section for more on Cloudinary.


## Which CMS?

For static sites like sportclimbs.uk there is [a wide range][2] of different CMS's available. Most of these work as  cloud based *software as a service* (SaaS).

[Netlify CMS][1] is free, open source software so has no limitations for free use. However it does require authentication for login and access to the website's files. For this we are using Netlify's built in *Identity* system which does come with limits (maybe a maximum of 10 users) for the free tier.


[1]: https://www.netlifycms.org/
[2]: https://blank-try.netlify.app/posts/headless-cms-review/
[3]: https://cloudinary.com/
[4]: /to-do/technical/#images
[5]: https://www.netlifycms.org/docs/cloudinary/#connecting-cloudinary-to-netlify-cms