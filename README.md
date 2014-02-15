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

![alt text](image.png "Components")

## Step 0: Set up your Raspberry Pi

[See the Raspberry Pi Quick Start Guide here](http://www.raspberrypi.org/quick-start-guide) 


## Step 1: Create a Sweet Munching Sprite



**Activity Checklist**

1. On the desktop of your Raspberry Pi you should see a **ScratchGPIO** icon. To open it, double click the icon. It is very important that you use this version of Scratch and not the default application. 

![alt text](scratch-interface.png "ScratchGPIO interface")

2. Delete the Scratch Cat Sprite by **right clicking** on it with your mouse and selecting **delete**.

3. Click on the paint new sprite icon above the sprites palette and draw face with a mouth that is closed using the paint editor. When you are happy with your sprite click OK.

4. Next with your newly painted sprite selected, click on the **Costumes tab**. Rename the costume to **face1** by clciking on the sprite name about the edit button and typing the new name. 

5. Click the **copy** button to make an exact copy of the face. You will now have two identical faces on the costumes tab called face1 and face2.

6. The next step is to edit face2 to change the mouth from closed to open. With face 2 selected click on the **edit** button to open the paint editor. 

7. Erase the mouth using a paintbrush tool or an erase tool and then replace it with an open mouth. When you are happy with your sprite costume click **Ok**.

8. To animate your sprite to switch between costumes you will need to click on the **Scripts tab** of your sprite. Drag the control block **when green flag clicked** from the blocks palette to the scripts area.

9. Next drag the look block **switch to costume face1** and connect it to the control block. 

10. Then add the control block **forever** underneath the look block. 

    The `forever` block is a loop that will run the same sequence of blocks inside it over and over again.

11. Add the control block **wait 1 secs** and the look block **next costume** inside the forever loop.

12. Time to save your work so far and test that your script to animate a sprite works. Go to **File** and **Save As**. Name your file **SweetShopGame** and click **Ok**.

13. Finally click on the **Green Flag** in the top right hand of the screen and you sould see your sprite face open and close it's mouth. 

## Step 2: Design a Sweet Shop Background
To make the game a little more interesting let's set the scene by changing the background from white to a picture of a sweet shop.

**Activity Checklist**

1. 


## Step 3: Program the Sweet Shop Reaction Game Machanics

Many people enjoy testing their reaction time against a clock. Let's create a reaction sytle game using ScratchGPIO that later on we can connect a squiggy sweet button to.

## Step 4: Wire up your sweet button

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


    
