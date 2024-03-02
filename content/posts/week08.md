---
title: "Week 08"
date: 2024-03-02T13:31:23+01:00
draft: false
---

# Progress Admist The Chaos

Long story short, I've had one of the most insane weeks in recent memory. Work alone was bad enough but a number of other unforseen circumstances all perfectly aligned to ensure I had no time to work on my game.

Despite it all, I've managed to enough progress to complete a major piece of the game.

# Game Updates
This week saw me completing the hit reaction piece for the zombie characters.

Now when hit by a shot they'll react to it and with enough shots they'll die...and at least for now, with a pretty entertaining finish.

{{<youtube 7ZFiebGGFBY>}}

The hardest part of all of this was handling the specific interactions based on where I hit on the enemy character.

At first I was handling this by adding a temporary rotational offset to the bone hit.

However, on issue with this solution is that it becomes quite complicated with all the different bones. For instance hitting the head and having it "tilt" back 45 degrees looks good, however I would want a different degree for the chest and limbs. As with most things I'm sure there's a smart way to handle this...but at my current level and need, I abandoned this idea in favor of the more common "enable physics" path.

In short my solution is to enable physics specifically for that bone and child bones when hit. Additionally an impulse is applied in the direction of the bullet's path. Finally a blend takes place back to the animatuion over a second of so.

This created a pretty good effect of the zombie's limbs reacting to the hit but not totally thrown out of their animation. Also I swapped out the gun sparks for blood which lends to the "realism".