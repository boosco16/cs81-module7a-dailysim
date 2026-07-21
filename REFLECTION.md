# Reflection – Daily Schedule Simulator

## What was your approach to designing the schedule?

I chose activities that I would follow on a any normal day, rather than random events. 
I wanted the delays between each activity to feel like they were in an order, starting with morning activities and ending with nighttime activities.

## What was one challenge or unexpected behavior you encountered?

I originally thought the events would somehow wait for each other with the earlier ones 
appearing and the next activity apearing accordingly. But, thats not what happens. All
the setTimeout calls start counting down the moment the page loadsm at the same time, 
completely independent of each other. So if I'd used the same delay number twice by accident, both events would've appeared at the exact same moment, which caught me off guard when I was testing it. 

## What does this assignment teach you about async code?

A normal top to bottom script runs everything immediately, in order, with no gaps. With setTimeout, the code still gets read top to bottom, but the actual work inside each setTimeout gets set aside and only runs later, once its time is up. 

## What creative element did you add?

I added a random mood emoji using Math.randmon(). If one of the events picks a random
emoji from a list of 5 instad of always showing the same one. So refreshing the page gives a slightly differnt result each time, even though the schedule stays the same.


## How does this project simulate or differ from real-world schedules?

It gets ordering right, but the actual timing is completely compressed into 15 seconds.
It also doens't acccount for stuff running long or short the way a real day does, every event appears at exactly its scheduled time. Real days aren't that precise, with events such as wake time and breakfast happening earlier or later depending on the day.
  
