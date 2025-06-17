https://solder.hackclub.com/tutorial

### Setting up the Images (2 hrs)

First, I found an image of a duck that I wanted to use from my camera roll. After a while (searching for what platform to use), I used [remove.bg](http://remove.bg) to take out the background, and put it into a [Canva whiteboard](https://www.canva.com/design/DAGqcYytvX4/wS42PJTTld9inSXreSQHhA/edit?ui=eyJIIjp7IkEiOnRydWV9fQ) to edit. From there, I used the **Tracer** tool to get only the outline of the duck. Then, I went to [**Adobe**](https://new.express.adobe.com/id/urn:aaid:sc:VA6C2:f0548beb-a51e-421c-8bfe-8de2d6e1cd4b?category=brands&resumeid=1750155545739), where I used the **Erase** tool to clear some parts of the duck so that it looks like the duck from behind. I took a screenshot of that, took out the background, and put that into Canva as well with the Tracer tool. 

Then, when I realized just enlarging it wasn’t a good shape for the PCB, I went to [**LightX Editor**](https://www.lightxeditor.com/edit-tools/edit?from=sticker-maker-online&tab=cutout&subTool=stickify&img=blob:https:%2F%2Fwww.lightxeditor.com%2F1432e288-33e1-4690-8d9d-21b384862536&w=490&h=510&action=default_project&social_platform_id=0&targetPage=&edType=3) to make the duck look like a sticker. I took a screenshot of this, removed background, and took out the insides (aka the duck part) via Adobe again. Removed the background of this, used Canva Tracer again to get a more defined line for the border. But the problem was, it was two lines. So I took another screenshot, removed bg, went back to Adobe, erased the inside line, screenshot, bg remove, back to canva. There, I added a **Shadow** and made the thickness 5. But - oh no! - one part of the line was too thin, so it broke there. SO, screenshot, bg remove, went to **Paint App,** and drew in the gap. Then screenshot, bg remove, back to canva to add the thickness. 

So, now I have - the Edge.cuts of the PCB (aka all the sticker stuff), the front image, and the back image.

### Circuit Time! (0.5 hrs)

Once I had all that, I set to making the actual PCB. Obviously, to do this, my first step was making the schematic and adding the footprints.

![image (4)](https://github.com/user-attachments/assets/016af21d-c45a-4227-ae74-6ef5290023f7)

### Layout Time!! (1 hr)

Now, it’s time to start laying everything out. I went to the PCB editor and imported my schematic into it, then imported my Edge.cuts outline (after converting it to an SVG using [**this**](https://www.freeconvert.com/jpg-to-svg/download)). There was an overlap error, so I spent quite a bit fixing that, deleting all polygons that weren’t the main shape. 

(eventually skipped edge cuts… come back to that later)

### edge cuts… and traces!! (2.5 hrs)

Omg, this part was the most time-consuming. Basically, I’d imported the image of the outline of the duck that I made at the start  (after converting it to an SVG using [**this**](https://www.freeconvert.com/jpg-to-svg/download)), right? But it would make it so that the PCB was ONLY that much space:

![image (5)](https://github.com/user-attachments/assets/32fd997d-54c2-46cb-8c1d-67179360a07e)

So, I set to work deleting ALL the inside lines of that shape… but when I did, it said the components (like the LED, resistors, etc) were interfering with the border. When I deleted it, I accidentally hit something and it made the outline of the shape that I wanted into a copper line. So then I searched how to convert that to the Edge.cuts layer, but couldn’t find anything.

After this, I was drawing a blank. I thought maybe I imported the image wrong so tried again, converting it to a .dxf a couple times as well. Eventually though, I had an idea: what if I just made the duck image COMPLETELY filled in, and after importing that unselected “Fill shape”? 
Once I did that, the cutout worked! 

After that, I found how to put the traces on the *back* of the PCB and finished up that. 

And… here is the final product!! 

![image (1)](https://github.com/user-attachments/assets/49034232-796a-441b-beac-dffb8775c450)
![image (2)](https://github.com/user-attachments/assets/f8db3a84-e1cd-4f32-9f5a-0b4c78e83224)
![image (3)](https://github.com/user-attachments/assets/9eefd42c-cd86-46c7-bcb8-a016a1ac3305)


### oh wait one last thing…

Almost forgot! This is a gift, so I’ll put a keychain hole on it.
