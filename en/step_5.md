## Test the button

You are going to use your sweet as a button! When someone squeezes the sweet, the wires inside will touch together to close the circuit, and you will be able to detect this in your program.

+ Click on the face sprite in your Scratch project.

+ Add some new code to constantly (`forever`{:class="blockcontrol"} ) check GPIO pin 17. Most of the time this pin will be **high**, except for when you press your sweet button.

```blocks
when flag clicked
forever
    if <not <gpio (17) is high> :: extension> then
        say [Yum!] for (1) secs
    end
end
```

When you press the sweet button, the pin will report that it is **not** high, so the message "Yum!" only displays when the button is pressed.

+ Click the green flag and test your program by squeezing the sweet button. If you don't see the message "Yum!" when you press the button, try adjusting the positions of the wires in the sweet so that they are closer together.

--- collapse ---
---
title: I can't get my sweet button to work
---
If you're having trouble, you can take the paperclip wires out of your sweet and test your code by touching the wires together. If you see "Yum!" when you touch the wires together, your program is working and you need to adjust the position of the wires within the sweet.

Sometimes the wires can get a bit gummed up with goo from the sweet, meaning you don't get a good connection. Try wiping off the wires before testing. Once you're happy that your program works, try to insert the wires back into the sweet so that they are close together but not touching until you squeeze the sweet. It's a bit tricky to get this right but it is possible!
--- /collapse ---

+ Once you know your button is working, you can move on to the next step to make a reaction game
