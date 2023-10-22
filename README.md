Things to note:
* This is not the official guide
* This guide is only for creating watchfaces and AOD from scratch, since you cannot import .bin files (watchfaces files) into the software \[[GitHub](https://github.com/m0tral/EasyFace)\]
* The official software wiki can be found [here](https://github.com/m0tral/EasyFace/wiki)
* you can find more information on telegram \[[Official channel](https://t.me/s/mi_watch_news) and [discussion](https://t.me/mi_watch_int)\]
* by "watchface" I mean what you see when you turn on the screen, while AOD is what you see when your screen is turned off (if you have it activated)
* In this tutorial I'll make a basic watchface (no weather/date/gauges)
* I'm sorry for any mistake or misunderstandings, English's not my first language

\----------------------------------------------------------------------------------------------------------------------------

Things you'll need \[watchface\]:

* images of the numbers you'll use (they all have to be the same resolution)
   * You'll also need 4 extra copy of a number to use as the negative sign \*
* a background (192x490 pixels (8) or 336x480 pixels (8 pro)), otherwise it'll remain black

How to make the watchface:

1. Start by opening EasyFace (as admin) and creating a new project \[select mi band 8 / 8 pro\] [(see image)](https://imgur.com/a/tkxPrQj)
2. Place your pictures inside the folder "images" (inside the project folder in the directory you selected) [(see image)](https://imgur.com/a/yJPRWac)
3. You'll find your numbers and background in the left panel [(image browsing)](https://imgur.com/a/HyuLsml)
4. Drag and drop the background on the watch preview and put as coordinates (x, y) 0 in the right panel (attributes) [(see video)](https://imgur.com/a/enkSJKV)
   1. you may have to deselect the image you just placed to make the attributes appear properly
5. Select "digital numbers" in the toolbox panel (on the left) and make a square/rectangle the same resolution as your numbers (you can't manually input the size of the square, you'll have to make it by changing it slowly and monitoring the attributes)
6. Once you've made 1 square, select it and copy it
7. Align the four digits however you want
8. As data source (right panel) you'll have to select Hour High (first digit of the hours) / Hours low (second digit of the hours) and minute high/minute low [(see image)](https://imgur.com/a/IgUAdKc)
9. Select the image of the numbers [(see image)](https://imgur.com/a/LM2f9Rh)
   1. As the negative sign select the extra number you copied \* **(they have to be different for each digit)**

\----------------------------------------------------------------------------------------------------------------------------

Things you'll need \[AOD\]:

* Images of the numbers you'll use (Unless they are very small, they can't be fully white, but they have to be outlined)
   * You have to copy the numbers the same way as before for the negative sign

How to make the AOD:

* The process for creating is the same as for the actual watchface, but you need to create a new project (has to be called AOD) inside the watchface directory
   * E.g. The watchface folder (Stripes) is under C:\\User\\Desktop, so the AOD has to be under C:\\User\\Desktop\\Stripes [(see image)](https://imgur.com/a/SO1p0lE)

1. Just place the AOD numbers in the watchface images folder  [(see image)](https://imgur.com/a/OeiAYbp)
2. Copy every image (including background and watchface numbers) into the AOD images folder (C:\\User\\Desktop\\Stripes\\AOD) [(see image)](https://imgur.com/a/YTD9dOq)

\-------------------------------------------------------------------------------------------------------------------------------

How to upload the watchface to your mi band 8:

1. Once you've finished the AOD, return to the watchface project
2. Click on the compile icon [(see image)](https://imgur.com/a/fNKvchd)
3. In the watchface output folder you'll find a .face file
4. Through third-party apps (I use [This](https://play.google.com/store/apps/details?id=com.mc.xiaomi1) or [this](https://play.google.com/store/apps/details?id=asn.ark.miband8&hl=en&gl=US)) you'll be able to install it on your mi band 8
   1. I am not responsible for any error/brick of your device
