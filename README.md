# MiBand8WatchFaceTutorial

Things to note:

This guide is only for creating watchfaces and AOD from scratch, since you cannot import .bin files (watchfaces files) into the software [GitHub]

The official software wiki can be found here

you can find more information on telegram [Official channel and discussion]

by "watchface" I mean what you see when you turn on the screen, while AOD is what you see when your screen is turned off (if you have it activated)

In this tutorial I'll make a basic watchface (no weather/date/gauges)

I'm sorry for any mistake or misunderstandings, English's not my first language

----------------------------------------------------------------------------------------------------------------------------

Things you'll need [watchface]:

images of the numbers you'll use (they all have to be the same resolution)

You'll also need 4 extra copy of a number to use as the negative sign *

a background (192x420 pixels (8) or 336x480 pixels (8 pro)), otherwise it'll remain black

How to make the watchface:

Start by opening EasyFace (as admin) and creating a new project [select mi band 8] (see image)

Place your assets inside the folder "images" (inside the project folder in the directory you selected), subfolders won't work (see image)

You'll find your numbers and background in the left panel (image browsing)

Drag and drop the background on the watch preview and put as coordinates (x, y) 0 in the right panel (attributes) (see video)

you may have to deselect the image you just placed to make the attributes appear properly

Select "digital numbers" in the toolbox panel (on the left) and make a square/rectangle the same resolution as your numbers (you can't manually input the size of the square, you'll have to make it by changing it slowly and monitoring the attributes)

Once you've made 1 square, select it and copy it

Align the four digits however you want

As data source (right panel) you'll have to select Hour High (first digit of the hours) / Hours low (second digit of the hours) and minute high/minute low (see image)

Select the image of the numbers (see image)

As the negative sign select the extra number you copied * (they have to be different for each digit)

----------------------------------------------------------------------------------------------------------------------------

Things you'll need [AOD]:

Images of the numbers you'll use (Unless they are very small, they can't be fully white, but they have to be outlined)

You have to copy the numbers the same way as before for the negative sign

How to make the AOD:

The process for creating is the same as for the actual watchface, but you need to create a new project (has to be called AOD) inside the watchface directory

E.g. The watchface folder (Stripes) is under C:\User\Desktop, so the AOD has to be under C:\User\Desktop\Stripes (see image)

Just place the AOD numbers in the watchface images folder (see image)

Copy every image (including background and watchface numbers) into the AOD images folder (C:\User\Desktop\Stripes\AOD) (see image)

-------------------------------------------------------------------------------------------------------------------------------

How to upload the watchface to your mi band 8:

Once you've finished the AOD, return to the watchface project

Click on the compile icon (see image)

In the watchface output folder you'll find a .face file

Through third-party apps (I use This or this) you'll be able to install it on your mi band 8

I am not responsible for any error/brick of your device
