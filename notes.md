reference from day 0:
Here's my unfiltered notes for the day: will probably keep this in a separate document?? idk

Links I've gathered so far:
- https://www.reddit.com/r/3Dprinting/comments/sjnw7z/conveyor_belt_3d_printers_are_they_a_viable/
- https://www.youtube.com/watch?v=cfD20oOWD28
	- I want to do something like this? and then a fusion of The 100:

I want this thing to be very easy to mod & hack. Should be able to live on my desk if I want

MUST be enclosed. I'll print the parts out of ABS cause I have an X1C? Thinking of a cheaper, easier to mod V0 (albeit prints slower but that's okay)

Why do I want it to be enclosed again??
- VOCs
- Noise

Okay so I'm thinking let's do an enclosed setup with a nevermore filter? and then like each time a print finishes a trapdoor at the back will open and the print can slide out there

Let's de-prioritize the modability

Okay high level overview

Klipper macro after the thing automatically moves a stepper by X amount

Features:
- General CoreXY setup
- Klipper + mainsail probs
- MUST have a webcam installed

----- BAD NOTES ABOVE ^^^ ----

Okay, refresh:

- Hackable, somewhat portable machine that allows me to experiment with a bunch of diff stuff
- Should have a webcam so that I can just stop it at any point


Features I want to mess around with:
- Toolchanger!!!
- TOOLCHANGER!!!
- TOOLCHANGER!!!!!

Okay. just filled out a canvas

tl;dr we're gonna make an awesome printer, don't overoptimize on making an all-purpose manufacturing machine or max optimizing for speed

This is just gonna be "how many features can we cram in for $300" lol

Like tinkerer's dream

Anyhow, this issue of VOCs seems rlly interesting - didn't realize toluene and other organic stuff i learned in chemistry class would actually appear.

also it's really weird coming back to all of this.

as for build volume - playing around in prusaslicer and like 99% of my prints fit within ~160mm. I think i'll run with something around there. 

We do need a minimum size to fit the toolheads though. wonder how that'll work.

Okay so a toolhead is roughly like 60mm in width??

so apparently bed sizes are only 150, 200, etc. guess our work is cut out for us.


Let's change to LM8LUU bearings. We have the space to afford them and they should help with any inaccuracies that we might have to deal with

Re: M3 vs M5 hardware on the belts - I think we can just roll with m5 and if we run into issues we can deal with it later. The first run won't be perfect.

Also, I've yet to actually run into a print that reaches past 150mm; worst case we get one and can print diagonally.

This design can scale up anyways hopefully (?) aka won't suck this time around + it's fun to use old hardware from blot so that we're not wasting parts.

just spent 2-3h i think? idk

yeah 2-3

yapped w/ max


LOCK IN LOCK IN LOCK IN LOCK IN

FUCK LOOOOOOOOOOOOOL

TO FIX:
- [ ] Add limits for the y rod holders
- [ ] Optimize the X/Y joints better - it shouldn't feel jank like we're trying to squeeze every last mm IMO
- [ ] In general, just clean up dimensions to work better.

jesus christ man i am so tired

anyways as for the toolchanger - let's start with the stealthburner as a sanity check item for now.

Ok so the prusa PCB bed is roughly 3mm thick; it's out of FR4 which seems to be slightly weaker mechanically and it holds up fine? I think the difference is that it has screws under evenly distributed throughout so idk how prints will hold up and whether or not it'll sag. Let's just get 4mm and run with it, seems to be fairly cheap and also stable *enough*
(worst case its not and we figure something else out)

hmmm z-axis height...

150mm should in theory net at least 100mm of build volume, if not more. 

I honest to god cannot remember the last time I needed to print something that tall. Let's just roll with it and then worst case get a 200mm one after

As for webcam, I'm not too sure?? I can't get a solid read on the ov3660's quality so I think 

AHH THAT's A L ATER PROBLEM