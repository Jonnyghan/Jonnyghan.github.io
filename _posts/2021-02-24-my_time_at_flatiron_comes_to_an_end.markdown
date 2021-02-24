---
layout: post
title:      "My time at Flatiron comes to an end!"
date:       2021-02-24 17:55:31 +0000
permalink:  my_time_at_flatiron_comes_to_an_end
---





After just completing my final review, I've come to realize how important it is to look at a problem from different perspectives. I was trying to create a button to toggle sorting on and off for the soccer teams I was mapping through.

```
 useEffect( () => {
  const sortArray = type => {
  
	const sortProperty = types[type];
  
	const sorted = [...props.teams].sort( (a,b) => {
		a[sortProperty] -b[sortProperty])
		}
  
    setData(sorted);
  };
    sortArray(sortType)
}, [ sortType,props.teams]);

```
 
 This was the problem I was stuck on, I was sure that I had everything right during my live coding but for some reason it just wasn't sorting my array of objects. I thought it was a problem with the hooks I was using, useState and use Effect, so i changed this functional component into a class component. I basically had to rewrite my entire component from scratch and it still wouldn't work. I undid all the changes and tried different ways of sorting and filtering but that still wasn't working. Then I was able to find a blog using a "compare" function. It was a last ditch effort, but I gave it a shot.
 After it worked I realized that my ``` [...props.teams].sort``` wasn't being specific with what it was trying to do.  
 
 The fix was this:
 ```
  useEffect( () => {
  const sortArray = type => {
  
    function compare(a, b) {
      // Use toUpperCase() to ignore character casing
      const types = {
        name: 'name',
        id: 'id'
      };
      const sortProperty = types[type];
      const teamA = a[sortProperty]
      const teamB = b[sortProperty]
      
      let comparison = 0;
      if (teamA > teamB) {
        comparison = 1;
      } else if (teamA < teamB) {
        comparison = -1;
      }
      return comparison;
    }
    const sorted = [...props.teams].sort(compare)
   
    console.log(sorted);
    setData(sorted);
  };
    sortArray(sortType)
}, [ sortType,props.teams]);
```


Once I got more specific and exact with how I wanted the sorting to occur, I was able to make it work. That is going to be the greatest lesson I've gotten from Flatiron and it's a bit funny that it's coming at the end of my time here. Other than that, I'd like to thank my cohort leads Michael, DJ, Juan, Z and Madeline and the rest of the students that I've had the opportunity to get to know over the course of this program.
		

	

