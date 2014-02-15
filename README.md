# Sweet Shop Reaction Game

**Introduction**

Some Penny Sweets or Candy can make great input devices for a game using a Raspberry Pi. You will learn how to turn a squiggy sweet into an input button for your Raspberry Pi. You will then create a quick reaction game in Scratch that counts how many times in 10 seconds a player can squeeze your sweet input device!

**Requirements**

This guide assumes that you have the following:
- A Raspberry Pi
- Connected to a monitor or TV
- A keyboard and mouse
- A speaker or headphones
- An SD card with the latest version of Raspbian installed via NOOBS
- ScratchGPIO downloaded and installed. [Use this guide to learn how to do this](http://cymplecy.github.io/scratch_gpio/)
- Two female to female jumper wires
- Two metal paper clips
- Some squiggy sweets/candy like marshmallows or jelly babies
- A cardboard box to put your Raspberry Pi and cables into
- Some colouring pens/pencils to decorate your box.

## Step 1: Wire up your sweet button

You will need to connect a sweet or piece of candy to your Raspberry Pi to act as an input device and test it.

**Activity Checklist**

1. Take the metal paper clips and unfold them to make straight wires.

2. Insert the paper clip wire into the end of a female to female jumper cable.

3. Do the same to the other jumper cable so that the two cables are identical.

4. Insert the paper clips into a soft sweet so that they are close to each other but not touching. 

    Raspberry Pi GPIO header pins. The diagram above the pins shows the pin numbers. You will be using pin 3 and pin 25.

5. Take the other end of one of the jumper cables (not connected to a paper clip) and push onto pin 3 of the General Purpose Input-Output (GPIO) header which is connected to one of the GPIO channels.

6. Take the end of the other jumper cable and push onto pin 25 of the GPIO header which is connected to ground.

    **Warning!** You can damage your Raspberry Pi if you do not use the GPIO pins correctly!

7. Set up the rest of your Raspberry Pi with an SD card with the latest Raspbian image installed via NOOBS, a keyboard, mouse, a HDMI cable to a monitor or TV, a connection to the internet, and a speaker so that you can hear your Jelly Baby screaming. [See the Raspberry Pi Quick Start Guide here](http://www.raspberrypi.org/quick-start-guide)    

8. Finally plug in a Micro USB power supply to start your Pi and log in. The default login for Raspberry Pi is: login `pi` and password `raspberry` 
    
