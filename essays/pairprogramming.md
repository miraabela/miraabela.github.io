---
layout: essay
type: essay
title: Pair Programming
date: 2019-06-07
published: true
labels:
summary: Pair Programming
---


Pair programming has the potential to be a lot of fun at the same time though I think it has special use cases. Since I worked on a different library than all of my team members, we couldn’t code things together, and we mostly used all of our pair programming sessions as Code Review sessions. 

## Sessions

With Kelli, we both used Floobits. Her scraper of choice was osmosis, so we spent the time comparing the differences between osmosis and cheerio. We both scraped the website simplyhired so it was interesting to see how little code she had compared to mine. The thing I like about Floobits is that it follows the hosts cursor, shows which lines are highlighted, and also follows which file the host is on. This feature is really nice for giving presentations or showing demos.  In our case since we were presenting our code to each other it was very convenient since I knew right away which line she was talking about. Although, I see how this could cause problems if two people were coding on different parts of the program, because it follows the hosts screen, it would only be convenient if two people were coding on the same file. Also, I realized I downloaded the plugin for Floobits in IntelliJ but the whole time, I just used the viewer in the browser, which I found to be very easy and similar to the IDE. 

With Jenny, we had a code review session where she sent me her CodeTogether viewer, and I sent her my Floobits viewer. The CodeTogether UI reminds me more of Visual Studio Code. CodeTogether also has the feature of following the host’s cursor and everything, except this is optional in CodeTogether, so it would be fine if two people were in different files. Jenny used Xray as her scraper, and she also scraped simplyhired.com. She also had much less code than me, and where I had to hard-code pagination, Xray had a simple method that automatically handles it. Xray also has a simple .write method instead of using the fs module’s writeFile method. 


With Aubrie, similarly she sent me her CodeTogether viewer, and I sent her my Floobits viewer. She also used Xray, but she also used Tattoine as her scrapers. I recommended she check out Xray’s paginate method since I noticed she didn’t take advantage of it, and I just finished a session with Jenny. Xray looks a lot like a JSON when it extracts information. I also shared a resource for testing Xpath queries in real time: http://xpather.com/. She said she came across the problem of being detected as a bot so she didn’t get much results from the website. I sent her a link https://www.scrapehero.com/how-to-prevent-getting-blacklisted-while-scraping/ to help her

## Overall & Extra Notes

I kept the browser tabs open after all our sessions were done, and I noticed in Floobits you can still explore all the files after the session is over. However, in CodeTogether, you cannot open or explore any files after the session is over. You can only view the code that was last open before the session was over. Personally, I think pair programming is good for specific use cases, such as when two people both are working on the same file or part of a project, and committing and pulling would take too much time. However, I personally prefer working alone if we are working on separate parts of a project or on different files. I think getting help is good, but I like to figure things out on my own before taking up someone else's time.  