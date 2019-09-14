---
layout: post
title: "Browser Caching"
---

### Leveraging browser caching

I heard about the term browser caching for the first time in one of the interviews.
Got curious about the concept and researched about it.

Let's start with the problem that affects page speed.
Some websites has lot of files and adds up to several megabytes or the files may be huge in size.

- Larger files takes long time to load and can be inefficient if you're in slow connection
- Each file makes a separate request to the server. The more requests the server gets,
  the more work it gets to do and it further reduces the page speed.

How can browser caching solve this issue?
By storing some of these files locally in the user's browser. User's first visit will take the same time to load, however when that user revisits, refreshes the page, or even moves to a different page of your site, they already have some of the files they need locally.

So, the amount of data the user's browser has to download is less, and fewer requests need to be made to your server. This results in decreased page load times. The huge advantage of using browser caching is it reduces the load on the browser that reduces the load time for users.

Caching guidelines for expiration:

- Truly static content (such as logos) - access plus 1 year
- Everything else - access plus 1 week

There is a caveat if expiration is too long for certain non static elements.
Users might not be getting the fresh version of the website after updates.
