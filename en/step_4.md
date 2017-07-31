## Create a sweet-munching sprite

The sweet shop reaction game needs a munching face to entertain the player. You will draw a face using the paint editor in Scratch, and animate it to open and close its mouth.

- Open Scratch by clicking on **Menu** > **Programming** > **Scratch**. It is very important that you use this version of Scratch on Raspberry Pi to be able to control the GPIO pins.

- Once Scratch is running choose `Start GPIO Server` from the **Edit** menu. 

- If asked, click **OK** to enable remote sensor connections.

- Delete the Scratch Cat sprite by **right-clicking** on it with your mouse and selecting **delete**.

- Click on the **paint new sprite** icon above the sprites palette, and draw a face with a closed mouth using the paint editor. When you are happy with your sprite click **OK**.

- Next, with your newly painted sprite selected, click on the **Costumes tab**. Rename the costume to **face1** by clicking on the sprite name followed by the edit button, and typing the new name.

- Click the **copy** button to make an exact copy of the face. You will now have two identical faces on the costumes tab called face1 and face2.

- The next step is to edit face2 to change the mouth from closed to open. With face2 selected, click on the **edit** button to open the paint editor.

- Erase the mouth using a paintbrush tool or an erase tool and then replace it with an open mouth. When you are happy with your sprite costume click **OK**.

- To animate your sprite to switch between costumes, you will need to click on the **Scripts tab** of your sprite. Drag the control block `when green flag clicked` from the blocks palette to the scripts area.

- Next, drag the look block `switch to costume face1` and connect it to the control block.

- Then add the control block `forever` underneath the look block.

   The `forever` block is a loop that will run the same sequence of blocks inside it over and over again.

- Add the control block `wait 1 secs` and the look block `next costume` inside the forever loop.

- Change the time from one second to half a second. How could you represent time as a value? If one is a whole, what would half of one be?

- Time to save your work so far and test that your script to animate a sprite works. Go to **File** and **Save As**. Name your file **SweetShopGame** and click **OK**.

- Finally, click on the **Green Flag** in the top right hand of the screen and you should see your sprite face open and close its mouth.

	![](images/face-script.png "Face Script")

