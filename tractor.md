# Connecting your tractor

Every tractor is different I'm afraid and we've just not had access to test them all. As we get more tho, we'll update this list, so check back now and again, or check the [Facebook](https://fb.me/freertk) page!

But in short, you're looking for settings somewhere in the menus that mention:

- NTRIP or RTK (**not** RTX, that's different)
- IP address or hostname
- port (this will be 2101)
- username (for rtk2go, your email address - for centipede, use "centipede")
- password (for both - "centipede")
- mount point (the mount point name you registered)

When you connect your tractor to rtk2go.com, they only ask that you provide a valid email address in case you're having issues and they want to contact you. I've never received an email from them for what it's worth. Password can be anything you like.

**Centipede have a good documentation guide [here](centipede.md) on how to set various types up!**

Uhfortunately, I don't have a lot of screenshots for this, but here's a couple:

On Fendt, you'll be into the guts of the GPS auto-steer menus. I had to blank out the info in this as it was the previous commercial supplier's details.

![Fendt](fendt.png)

On FJ Dynamics, it's in the settings, (again, had to blank out the information). Here, you put in "rtk2go.com" and port 2101, then press "Get Source", it will list all the mount points at rtk2go, pick yours and you're away. Fill in your email address for account, and again, password can be anything you like!

![FJ Dynamics](fjd.png)