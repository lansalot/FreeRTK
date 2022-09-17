# How to assemble the kit

## The hardware, and the software

Don't be daunted - it might seem tricky, but this isn't that bad. And if you get stuck, ping us a message on [Facebook](https://fb.me/freertk).

First, we'll get the rtkbase software installed on the memory card.

The rtkbase home page is [here](https://github.com/Stefal/rtkbase#ready-to-flash-release), and you want to scroll down to "Ready to flash release". Then click the link for the "ready to flash iso file [here](https://github.com/jancelin/pi-gen/releases/latest" and that'll take you to the next page.

At time of writing, that was version [2.3.4](https://github.com/CentipedeRTK/pi-gen_RTKbase/releases/tag/BaseGNSS-RPi-2.3.4), so scroll down until you reach the assets section. You're looking for the biggest file there, highlighted in the below example:

![Assets](assets.png)

You can unzip the file or not, Etcher will understand it either way.

---

### OK, so we've got the software prepared, now we need to write it to the memory card

Using your card writer/adapter, plug them into your PC
![Memory card writer](memcardreader.jpg)

Then, go download [Etcher](hhttps://www.balena.io/etcher/) and run it. You likely want the Installer one.

![Etcher](etcher.png)

Now, here's the tricky bit - this piece of software absolutely SHOULD recognise your memory card and NOT your actual hard drives, so you need to pay attention!

If you have a 16gb memory card, then you'll be looking for that sort of size in Etcher. If you've a 32gb card, then you're looking for something in that amount.

I can't stress this enough - **proceed at your own risk here and ensure you are looking at the right device**! Also, if you usually have a USB drive plugged in, of any kind, **UNPLUG IT WHILE YOU DO THIS**!

On my PC, I first did this **without** the memory card installed, and this is what Etcher showed me. It wouldn't let me select a target, and that's correct.

![No memory card](etchernomemcard.png)

Then, I put my 32gb card in the reader, plugged the reader in and started Etcher again, and this time it found it:

![With card](etcherwithmem.png)

Notice the size is 31.7gb (for my 32gb card, that's right, the numbers won't be exact).

When i selected "Change", I got this additional confirmation:

![Confirmation](etcheradvanced.png)

So, now we know we have the right card - and again, if you are in ANY DOUBT DO NOT PROCEED - we can write the image, so you'll be selecting "Flash from file" and pick your downloaded rtkbase file.

![Zip file](bigfile.png)

So now we have the right device selected, and the image file picked:

![Ready to write](readytowrite.png)

Click Flash and accept any prompt that asks if you're sure... the file will then be decompressed, and written to the memory card!

![Writing](writing.png)

It'll verify it, and then, you're done!

![Finished Writing](finishedwriting.png)

Rather annoyingly, Etcher ejects the drive when finished - so unplug it and plug it straight back in to your computer.

In my case, that pops up as an M: drive, and if I scroll down, right at the bottom I can see an interesting file called wpa_supplicant.conf. If you're going to use wifi, you should edit this now:

![Boot drive](bootdrive.png)

Open it in notepad, and you can see it looks like the following:

![Before changing wifi](wpa1.png)

Change it and put your wifi access point name and password in exactly as it should be, with the right upper/lowercase where applicable!!

![After changing](wpa2.png
)

Save the file, eject the card reader, and you're done!

