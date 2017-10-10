## Count the squishes

The object of the game is to see how many times you can squeeze the sweet button in ten seconds.

+ Create a variable called `counter`{:class="blockdata"}. We will use this to count how many times the button is pressed

[[[generic-scratch-add-variable]]]

+ Add some code so that when the flag is clicked the program will reset the counter to 0 to make sure that the player begins on 0 button presses.

```blocks
when flag clicked
set [counter v] to [0]
```
+ Attach some more code underneath to add 1 to counter whenever GPIO 17 is not high. Use the code you wrote to test your button to help you.

--- hints ---
--- hint ---
Constantly (`forever`{:class="blockcontrol"} ) check `if`{:class="blockcontrol"} GPIO 17 is `not`{:class="blockoperators"} high.

If it is not high, `change counter by 1`{:class="blockdata"}.
--- /hint ---
--- hint ---
Here are the blocks you will need:

![Hint for blocks to add one to counter](images/hint-add-one.png)
--- /hint ---
--- hint ---
Here is the code you will need:

```blocks
when flag clicked
set [counter v] to [0]
forever
    if <not <gpio (17) is high>> then
        change [counter v] by (1)
    end
end
```
--- /hint ---

--- /hints ---

+ Test your code by clicking the green flag and then squishing the sweet button. You will probably see that the counter goes up by more than 1 each time you squish the sweet, and you can cheat and get lots of points by just holding the sweet squished.

Let's stop the cheaters in their tracks! We will force the player to release the sweet by waiting until GPIO 17 is high again before allowing any more points to be scored.

+ Add this code after the block which adds one to counter:

```blocks
wait until <gpio (17) is high>
```

+ Test your game again and try to cheat by keeping the sweet permanently squished. You should find that this no longer gives you any points!
