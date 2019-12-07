---
layout: post
title:      "CLI Data Gem/My First Blog Post"
date:       2019-12-07 18:26:57 +0000
permalink:  cli_data_gem_my_first_blog_post
---


So this is my first blog post (Sorry guys, I didn't realize I needed to do this from the beginning😥.) I've finally completed the CLI Data Gem project and despite being THE hardest thing I've done so far I had a lot of fun with it. It made me use everything that I know and to be honest, despite my app being super simple I'm so proud! It's the first piece of software I've written, independently and without a crutch of having tests to make sure things work. 
Each method and line of code took focus and serious thought to put together. I'm very grateful for Avi's walkthrough because, after sitting there futzing with code that I couldn't figure out how to put together, I was able to finally create a concise foundation for everything.

# Content Process
When I took a look at the project, I immediately knew I wanted it to have something to do with soccer! I looked into the league tables for the top soccer leagues in Europe and thought about what I wanted to do with them. Realizing that the three had very different Title races going on I decided I was going to scrape each league for the top team at any given moment.
-In England: Liverpool has a clear lead and probably won't give that up any time soon so I liked the fact that my code will not face any problems due to that.
       - In Spain: There is a Two-way race for the title but I figured the league leaders wouldn't change for at least a few                  weeks. While I was writing the code FC Barcelona was on top. When I went to record my Demo Video, however,                 Real Madrid was the new top team and, to my delight, my code actually WORKED and changed the data to reflect             that in the app!
       
      - In Germany: There is a Five-way title race going on so I figured it was a good chance for me to test the resiliency of my code and get some good practice in. When I wrote the code Borussia Mönchengladbach was on top currently it's RB Leipzig, and I'm imagining it will change again soon. *edit: when I started writing this it was RB Leipzig and it is now back to Borussia Mönchengladbach! #RESILIENT CODE!*

# Code Process
The figuring the actual code itself was difficult. I thought I'd create three separate classes to house and scrape each league, then create a class for the CLI controller. In each league I had initially thought I was going to pull all the available relevant information for the top team: Name, Goal Difference(Goals scored minus Goals conceded), Points, and Next Match. In the end, I wasn't able to do this because:

   - Each webpage was formatted differently, in that, not all of them had "Next Match" available.

   - Each Webpage's HTML was different, the Bundesliga webpage had classes that were very simple and easy to                     follow whereas the Premier League and La Liga webpages had classes that were long and full of letters and                         numbers that were not at all easy to read or parse through.

All in all, I had a great time with this despite feeling stressed at times. I'm definitely looking forward to working with more ruby applications in the future!




 
