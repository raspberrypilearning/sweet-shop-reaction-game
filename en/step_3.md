## Create a sweet-munching sprite

The sweet shop reaction game needs a munching face to entertain the player. You will draw a face using the paint editor in Scratch, and animate it to open and close its mouth.

- Open Scratch on your Raspberry Pi

[[[rpi-scratch-opening]]]

- Enable the Scratch GPIO extension. This will allow you to use Scratch to talk to the GPIO pins on your Raspberry Pi.

[[[rpi-scratch-add-pi-gpio]]]

- Delete the Scratch Cat sprite and click on the **paintbrush** icon to draw a new sprite. Draw a face with a closed mouth using the paint editor.

![Closed mouth face](images/closed-face.png)

- Name this costume **face1**.

- Duplicate the costume so you have two identical face costumes.

[[[generic-scratch-duplicate-costumes]]]

- In the copy of the costume you just made, erase the mouth and then replace it with an open mouth.

![Open mouth face](images/open-face.png)

- Click on the **Scripts tab**. Drag the control block `when green flag clicked` from the blocks palette to the scripts area.

- Next, drag the look block `switch to costume face1` and connect it to the control block.

- Then add the control block `forever` underneath the look block.

   The `forever` block is a loop that will run the same sequence of blocks inside it over and over again.

- Add the control block `wait 1 secs` and the look block `next costume` inside the forever loop.

- Change the time from one second to half a second. How could you represent time as a value? If one is a whole, what would half of one be?

- Time to save your work so far and test that your script to animate a sprite works. Go to **File** and **Save As**. Name your file **SweetShopGame** and click **OK**.

- Finally, click on the **Green Flag** in the top right hand of the screen and you should see your sprite face open and close its mouth.

	![](images/face-script.png "Face Script")
