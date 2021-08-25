# SyncVR-TechDemo
TechDemo for SyncVR by Koen Groot.

# Instructions
In this tech demo there is only one action to perform.
 - Click the button "Next number" to generate and display the next number in the 
 fibonacci sequence.
 
 Every click has a small three second cooldown timer that can be seen in the 
 bottom right after clicking the button. Once the timer dissapears you can click
 the button again to generate the next number.

# Design choices
I decided it would be a fun idea to have the current number of the fibonacci sequence
in front of the ten next numbers in the sequence. To do so, I've placed two canvas', 
one in front of the other. The numbers on the back canvas will be floating around 
seperately from each other so they will need their own objects. This also means I'll
need some kind of manager to maintain all the floating numbers.

When requesting the next number in the sequence a button can be pressed at the bottom of 
the canvas that's in front. This will update both the front canvas to the new number and
the back canvas to update the number that was just placed on the front canvas.

Because you could click the next button a bit too often in my opinion I made a visible
little timer in the bottom right corner that displays how long you have to wait to call
the next number in the sequence.

Next I figured it'd be nice to get some more feedback when requesting the next number in 
the sequence. So I've added some audio on the button when it's clicked and some simple 
particle effects I made quickly.

The particle effects spawn on the position of the mouse where you user clicks and lastly
I made the button a little more transparant because it just looked a bit better.
