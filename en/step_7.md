## Add a timer

You will need to create two variables for this game: one to count the button presses, and one to count time.

- Repeat the first step to create another variable named **timer**.

To set a time limit that counts upwards for the game, you need to add two further scripts:

- Add `when green flag clicked` block to the scripts and connect the sensing block `reset timer` to it.

- Underneath, connect a `forever` looping control block.

- Inside the loop add the variable block `set control to 0` and using the drop-down menu on the block, change **control** to **timer** so that the block reads `set timer to 0`.

- Replace the value `0` in the `set timer to 0` block with the operator block `round`.

- Then add the sensing block `timer` inside the space on the `round' block. The completed block should look like:

	![](images/timer-script.png "Timer Script")

- Add another `when green flag clicked` control block to the scripts area and connect a `wait until` block to it.

- Add the operators block `=` to the space in the `wait until` block. In the left hand space, add the variable block `timer`. On the right hand side, type a value to represent time. If you want your game to last for ten seconds, type `10`.

- Connect a `stop all` control block to the end of this script.

- Finally, save your game by clicking on the save icon at the top of the screen.

	![](images/timer-script2.png "Set Timer Script")
