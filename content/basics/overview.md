---
title: "Overview"
date: 2021-11-18T07:25:27Z
draft: false
---

How the website works?

The sportclimbs.uk website is based upon three main technologies: Hugo static site generator, Git version control and Netlify serverless web hosting.

## Hugo

Hugo is a type of program called a static site generator. These programs take template files and content files and blend them together to create a whole web site.

Hugo is currently one of, if not the, fastest static site generator. To build the sportclimbs.uk website, which is about 400 pages, currently takes about a minute.


## Git and GitHub

Git is a very popular *version control program*. When developing a piece of software, or it could be a website, it will save the whole project when you tell it to. This mean you are able go back in time to see older versions of the project.

Git is used with *GitHub* which is a website for storing and sharing Git based software or website projects. The files making up the sportclimbs.uk website (in their unbuilt form) are stored on GitHub. When we make changes to the website files it's fast and easy to update these on GitHub.

## Netlify

Netlify is one of several online services especially designed for hosting *static websites*. A term used is *serverless web hosting*. Although websites have to have a server to share them with the world wide web the term refers to the invisibilty of the server to us.

Netlify is connected to the unbuilt website files on GitHub. If these are changed Netlify gets a signal and rebuilds the website using it's own version of Hugo.

Netlify also has other built in services like the contact form for the site. Another service is authentication which will be used for logging into the CMS safely.

We are currently using the free tier on Netlify which allows 100gb of bandwidth per month. Looking at the records of the old website in the busiest summer months we only used about 6gbs of bandwidth. So we have plenty of extra at the moment.

The Netlify free tier also allows for 300 minutes of build time per month. As the time to rebuild the site currently takes about 1 minute this means we can update the site about 300 times per month or 10 times per day.

There are several similar services to Netlify. Cloudflare is a good one and has unlimited bandwidth. But the build time limit is less and it harder to set up the CMS. Vercel is another similar service but has less bandwidth (the last time I looked) but is possibly better for programming features for more complicated apps.


## Other technologies

### Netlify CMS

This is free open source software built by Netlify. Although it works with other services (apart from Netlify's webhosting) it's easier to set up with Netlify.

It works by editing the website files on GitHub. These changes then trigger a rebuild of the site on Netlify web hosting.