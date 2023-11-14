# [Pear Shaped Theory](https://editor.p5js.org/alexwarr00/sketches/jgmcQRxVW)

This is a one day coding illustration of an idea I heard about when playing team sports with my friends at a local club. (I was playing underwater hockey, but that is a story for another time). 


## Background 
We are not the most organised team and although we try to stick to specific positions in the pool we often find ourselves in the wrong place. I asked my friends what the overall goal should be at different stages of the game and was told about something called 'Pear Shaped Theory', the idea that while defending you solely focus on pushing the puck away from your goal (radially outwards), then advance the puck up the walls, before brining the puck in towards the centre to attack. This seemed like a reasonable tactic to follow, but I wanted to be able to justify why this should be correct. I had the idea to craft an example 'value' function (from pitch positions to $\mathbb{R}$) and then look at it's derivative to explore where the team should try to push the puck. I finally got round to doing so recently.

## Outcome
I have created the following p5.js sketch: https://editor.p5js.org/alexwarr00/sketches/jgmcQRxVW

On the right hand side of the screen you should see a rectangle with many short lines - those lines follow the derivative of the value function, so they suggest which direction the puck should follow to increase the value function as quickly as possible.

There is a slider to describe how aggressive the team is, which has a reasonably intuitive effect on the resulting derivative (a value of 1 means that we show blatent disregard for defence, perhaps we are at the end of a game that we have already lost by a landslide and our sole focus is to score a single goal. A value of 0 means that we have no interest in scoring, a 'park the bus' strategy). In practice this value will never lie quite at the extreme values, so take the resulting value functions with a pinch of salt.

Lines 25 and 26 describe slightly different value functions (line 25 considers the apparent size of the goal and line 26 does not)

## Interpretation
The basic conclusions 