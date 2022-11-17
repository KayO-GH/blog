---
title: "Querying Arbitrary Name Arrangements in SQL"
date: 2022-11-17
---

Have you ever found yourself in that position where you wrote a SQL query to find somebody by searching through a `full_name` column in your database table, 
and although the name existed in the database you could not find it because you switched the first name and last name, and SQl was too dumb to figure it out?

And then you went online and tried to search for a solution, but all you found was code where first name searches and last name searches were neatly separated?  
As if data will always come to you in that format...

So you declared that it was no longer a bug, but a feature, where all queries had to be made in the format: `firstname lastname` 
and hope to God that most queries wouldn't fail and your users would the presence of mind to avoid typing the surname before the first name in your search bar?

No? Just me? Wow.

Anyway, after trying to work around this for a while, and taking inspiration from this [StackOverflow post](https://stackoverflow.com/questions/29795716/sql-query-to-search-by-namecontaining-combination-of-two-or-more-word) 
hidden in a corner fo the internet, I'm here to give you a delightful little hack so you never have to cry about searching for a full name ever again!😃
