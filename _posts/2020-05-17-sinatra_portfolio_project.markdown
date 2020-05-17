---
layout: post
title:      "Sinatra Portfolio Project!"
date:       2020-05-17 21:37:41 +0000
permalink:  sinatra_portfolio_project
---


WHEW. Okay, this project was a doozy. I don't think I've worked on anything this hard in a really long time, but it was definitely a learning experience! 

# Project:
My idea initially was going to be a website where people can create Soccer Players and Teams  but then I realized it was a lot of moving pieces.I simplified it by making it similar to the EA Sports FIFA Ultimate Team Model. There is a set database of players that the administrators can manipulate BUT the users can read it and create their own teams with the available players.

# Process:
My process started with the players model, I wanted to get that out of the way first because I figured it was the most important part of the whole relationship: You can't have a team without players. Once I finished the players, I moved on to the users. Handling all of the creation and authentication before moving on to clubs. Clubs was easily the most difficult part because I had to think of ways to itterate over my created players in an efficient and logical way. Once I got through that part it was smooth sailing, barring adding bcrypt  to the program, and I enjoyed the rest of it!

When I was working on adding bcrypt to encrypt my user passwords my heart was in my throat for the whole time!
Initially I had :password in my users table so when I went to change that I, somehow, wound up deleting all of my migrations! Thankfully I was able to get through it by running my initial migrations with :password_digest in the Users table THEN my editing migrations for Players and Clubs  and reseeding my database!

Looking back this was a stressful assignment, but I actually had quite a lot of fun with it! Im looking forward to doing more like this again!
