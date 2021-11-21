---
title: "Technical"
date: 2021-11-17T09:53:46Z
draft: false
---

Technical aspects of the website that could be added to the site

1. A CMS (Content Management System)
2. A search function using Algolia, Lunr or ...?
3. [Configure](https://mcshelby.github.io/hugo-theme-relearn/basics/configuration/) this docs site better
4. Adding class names for the content section at the page level. Use this instead of `columns: true` in the front matter. Maybe `contentclass: columns topo` for instance.
5. Shortcode for columns ??? See how this is done for [Hugo Book theme](https://hugo-book-demo.netlify.app/docs/shortcodes/columns/)
6. Maps: 
   1. button that expands the maps to full screen
   2. button that resets the map
7. A logo for the website.
8. icons for the footer (RSS, Contact, Facebook, Instagram etc.)
9.  Some subtle animations for page loads
10. top menu colour coded to identify which region is the current region.
11. Dropdown menu items from the top menu for faster navigation.
12. Change updated to use git info, so that any edits will count rather than just new pages.
13. Add a page count: The site currently has x pages including of which are y topos.
14. Comments section each topo page. This could be a good way to get extra info for the topo pages.


## Images

Most of the site is images and it makes sense to optimize delivery of these for both the end user of the web site and also to reduce bandwidth for the future. Currently there are 3 technologies that could help though much depends on what will work when adding images from the CMS.

These are:

1. Git LFS. This is an extra piece of software used in the Git workflow.
2. Netlify Large Files helps keep image out of the repo, instead using pointer code in the web site to where the images are (on Netlify) The bandwidth limit for the free tier is 100gb per month which is the same as the free web hosting we are using. There is also a limit on the number of *image transformations* per month too.
3. Cloudinary is an alternative to Netlify Large File but the bandwidth is limited to 40gb per month for the free tier.

Currently most images are served directly from the web site. This is fine however if the images are changed each version will be saved in the Git and tend to bloat the repository. We also now have a Cloudinary account and some images are saved there instead. Although the bandwidth limitation is 40gb per month this is in addition to the Netlify limit of 100gb per month.

## Progressive Web Apps (PWA's)

One of the biggest changes since the first Sport climbs website is the profileration of smart phones. Although the website design is responsive (ie. it scales to different screen sizes) a limiting factor in using the website as a guidebook at the crag is the lack of a mobile signal.

Mobile devices tend to use mobile apps typically downloaded from an app store specific to the operatiing system (eg. iOS or Android). Progressive Web Apps are designed using basic web technologies like HTML, CSS and Javascript and are device independent. This means they can work anywhere: Windows, Linux, iOS, Android etc..

Websites can be turned into PWA's. This means the website is downloaded onto a device like a phone and then used just like an app is. Because the information is downloaded to the phone a mobile signal is no longer needed to access the website. This would be a good way for users to be able to use the website and a guidebook where there is no mobile signal.

Because the website is relatively large it would make more sense to just allow sections of the site to be saved to a phone as a PWA. This could be at the crag level, say Horseshoe Quarry or Harpur Hill or for a whole area like Stoney Valley or Buxton.