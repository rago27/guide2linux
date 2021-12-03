# A Noob’s Guide to Linux

To do sections: Software, Terminal, Packages, Gaming
The title makes it sound like there’s a ‘huge’ learning curve, because there is (kind of, depending on what you want). Any terminology you don’t understand, please google. :)

Link to a discord server I’ve made for Linux (valid till 9/12/21): https://discord.gg/RAv4nBgm


My Story 
(read this in parts, when you get bored of the normal guide ;) )

I started tinkering with Linux (or rather GNU/Linux) in the last 6 months of JEE prep as a way to pass time, learn something new and have fun during my breaks. Before that all I knew was that it was an OS for computer geeks. Today I’m glad I started this journey.

Another reason I was interested was because I’d used MacOs since I could remember, so the windows UI looked horrible to my eyes. My 2011 Macbook Pro was ageing (obviously) and I didn’t want to buy a new macbook. So naturally the OS choice I was left with was Linux. 

Everything I know is a result of haphazard searching on the web, watching many videos and reading articles. Everyone has to do this initially, but the effort is generally worth it (especially for programmers or people who want total control over their system). This doc aims at making the very beginning more streamlined.

I started with Pop Os, on an external hard drive. After figuring out that it is very polished and beginner-friendly. I was booting into it in my free time and experimenting (mainly ui customization). I learned how to use the terminal and it turned out to be more useful than I’d ever imagined. After tinkering with Pop Os till JEE Adv, I wiped MacOs and used it as a daily driver. In a few weeks, I decided to try Arch Linux (has a meme attached to it in the Linux community) on my new laptop (X1 Carbon 6th Gen). Arch (the vanilla version at least) is not beginner-friendly at all. Its installation is manual, nothing (not even gui) is pre-installed. Only wifi works out of the box. Despite all this, Arch is the best shot you have at making the perfect OS for yourself. It’s like a clean slab that you can build on. That’s what I’m currently doing, I’ve got most things working and I’m just tweaking little things here and there. My install is very minimal, it only has barebones stuff and some apps I need. It idles at 380-400Mb of RAM and has low power consumption. 



Introduction

Linux refers to a family of operating systems that use the linux kernel.
Each OS based on the linux kernel is called a distribution (in short, distro). Popular distros include: Ubuntu, Manjaro, Fedora, PopOs, Linux Mint Etc…

Video about above info: What is Linux?

To be honest, the distro doesn’t matter too much (once you get deeper into Linux), but a general distinction will be:
Ubuntu - very popular
Pop_Os! - polished Ubuntu distro, supports Nvidia out of the box
Linux Mint - ui similar to windows, decent Nvidia support 
Elementary OS - ui similar to macos
Fedora - comes with gnome, very solid and polished

I recommend PopOs or Linux MInt (for windows familiarity). Heard Fedora is great, but I have no experience with it.

Distro family tree (Each dot is a different OS): https://commons.wikimedia.org/wiki/File:Debian_family_tree_11-06.png

Seeing this you obviously realise that there are too many options. That’s what this guide helps with. And with DE’s(desktop environment) and WM’s(window manager, more advanced, not for beginners). 

Note: most things in linux (scripts, config files etc.) are written in a language called bash.














Why Linux?

Linux is freedom. It is completely open-source (meaning the source code of the OS is public) and as the name suggests it’s free(in most cases).
Linux is highly customizable i.e. the user owns his machine and can make it however they want. (Check out some extreme examples of customization on the subreddit r/unixporn: https://www.reddit.com/r/unixporn/
Eg1. https://www.reddit.com/r/unixporn/comments/r6jg1n/i3_my_second_rice_better_ig/
Eg2. https://www.reddit.com/r/unixporn/comments/r5ot7x/kde_pixarch/
)

Advantages of Linux:
Open Source (mentioned above)
Lightweight/Less bloat- Linux is very lightweight and generally less bloated (varies distro-wise) than mainstream OSes. To give an idea, I have a lightweight linux distro installed on a giant Toshiba laptop from 2007, with half a GB of RAM and it works pretty well. So it is generally faster than win/mac.
Fast file transfers- noted by my friend who switched from windows to Linux
Powerful Terminal- once you learn it properly, there’s no going back ;)
Great for coders- ease of life (many operations are easy on linux, probably why the CS101 professor was recommending it)
Customizability- This is the main point for many people, you can make your system as cool/light/weird as you want. You can customize the workflow to whatever suits you best.
Softwares(also in disadvantages)- Basically all open source softwares can directly be downloaded from the terminal with a one-line command
Tiling- this feature is not present in all distros, but take a look at it in the second screenshot above. Tiling allows ‘most’ people to work more efficiently and easily. 

Disadvantages(not everything can be good, else everyone would have been on Linux):
User Friendliness- Linux used to be daunting, only for computer geeks. Now, many distros are trying to solve this and they are succeeding, but still pretty far behind windows for now. But any slightly motivated and intelligent person can learn how to use linux for sure.
Battery Life- Linux was originally made for servers (nearly all servers today, probably even Microsoft’s, are on Linux). Eventually it started coming to desktops and laptops. There were barely any provisions to conserve battery life, which windows and macos have (because they were made keeping laptops in mind). The situation has improved quite a lot, but there’s some way to go. Generally, battery life can be improved by some manual tweaking and installation of certain packages (will be mentioned later).
Softwares- Many proprietary softwares like Adobe Suite, MS Office etc. don’t work on Linux (good open source alternatives are available, but they’re obviously not perfect clones). Quite a few games won’t work (will be mentioned later). This is a result of companies choosing to not develop softwares given how small the linux user base is (<2%). Will be talked about in depth later on.


Window Manager (WM)
A window manager is a program that draws and manages windows on your screen. Like size, placement etc. Every DE comes with its own WM and a lot of other stuff. For a minimal install a WM is preferred, but it’s tough to configure and generally used by advanced users. So, for now we’ll leave WM’s. Don’t go into details for now.
Thoughts on window Managers - first get comfortable with linux and some desktop environments and the terminal before moving on to a WM

Tiling WM’s eg. bspwm(what I use rn), AwesomeWM, Qtile(written in python), Xmonad(written in Haskell)
Stacking WM’s eg. Openbox

Desktop Environments (DE)

The OS is what runs in the background while the DE refers to all the user interfaces i.e. the things you interact with. It draws your windows, includes standard apps like calendar, text editor etc., handles notifications and a bunch of other stuff. In windows/macos the DE and OS are essentially bundled together, but on Linux you can mix or match.

DE video: https://www.youtube.com/watch?v=2sBsxrWD9to
Examples:

Gnome - a weird ui unlike anything else, comes with most beginner-friendly distros like ubuntu, popos etc. (this is what I started with, and it’s probably a nightmare for windows users)

Cinnamon - comes with Linux Mint, Most windows-like interface, overall very smooth experience. Recommended for new users who are used to the windows feel.

KDE(comes with kubuntu, kde neon, and kde flavours of other distros) - HIGHLY customisable, but VERY overwhelming for new users. The experience isn't as smooth as one would expect, in my (Ravi’s) personal experience there were many bugs and overall inconsistencies with animation

Budgie (comes with a distro called Solus)- imo the best looking interface out of the box, it is essentially a skin of gnome, basic functionality is present, not much further customisation.

Xfce (comes with xubuntu) - Out of the box this looks trash, complete waste, but it doesn't require much to make this into anything you want basically. the level of customisation is at the level of kde without being overwhelming. It is very good for potato systems, uses very few system resources, bugs occur once in a blue moon. Overall a good choice if you're looking to transition from any of the other environments, it can be used as a first DE, but it would most likely require custom install and config, which can get a bit technical, but very lightweight






Now that you know a bit more about Linux, go online and do some research yourself :) . The only way to learn more is by yourself. Next, I’ll discuss the installation.







Disclaimer

I recommend you to install Linux on an external hard drive (like I did initially), until you get comfortable with it, iron out all the issues, learn the terminal, customize it till it looks cool to you and are ready to ditch your current OS. Only then install it on your internal hard drive on your main device..

Before proceeding with the install, go online and search up your specific device and its linux compatibility. There may be some caveats, but most devices work perfectly. Generally Nvidia GPU’s are a pain (mostly fixed now) as summarised here: 
https://www.youtube.com/watch?v=i2lhwb_OckQ
And I don’t have information on ARM macbooks, but I doubt anyone with one is looking at Linux rn ;).

Btw, I don't recommend dual booting (i.e. 2 OSes on the same physical hard drive), cause I've heard windows updates screwing over the Linux partitions
I recommend using Linux on a separate (external) hard drive till you're ready to ditch windows completely







Installation 
(same for external and internal drives)

Bootable USB
Hopefully you’ve found a distro you’ve liked. So go to their website and download the latest .iso file. To try or install a distro, you have to make a bootable usb and boot into it. A bootable usb basically has the iso flashed on it. Eject the usb after balena etcher is done flashing it.

All this is described in the video below (for PopOs, but it’s basically the same for all distros): https://www.youtube.com/watch?v=wupmowZNVgM&ab_channel=Herbertech

Boot into Linux Live Environment
Now that your USB is flashed. You have to boot into it. This process will NOT affect your computer/data unless you manually go through the installation process after boot. 
Go online and find out how to enter the boot menu and bios on your specific device (generally involves spamming some key upon boot).
In the bios you have to turn off secure boot (for any distros except ubuntu and fedora). 
Link 1: https://www.youtube.com/watch?v=brXcxmdWU9Q
Link 2: if secure boot is blanked: https://www.youtube.com/watch?v=nCxoOyUQqUE


Once you’ve booted into the usb, you’ll be prompted to install the OS. Skip that for now (close the window). First check if everything is working (wifi, bluetooth, speakers, keyboard, mouse and trackpad (direction of scroll can be fixed easily, just check if the inputs work), proper scaling on screen etc..

Now, poweroff and reboot into the usb via boot menu. Connect an external drive before booting. This time follow the installation window. While selecting the installation destination ENSURE you choose the correct drive as this process will FORMAT the selected drive leading to LOSS of all data on it.

Video describing installation (for Pop Os, but the process is nearly the same for all beginner-friendly distros): https://www.youtube.com/watch?v=e_oZkBuhExM

Now you’re done (only with the beginning)! Welcome to GNU/Linux. Learn, tinker, research and explore. 
Boot into the linux drive normally (if internal) or via boot menu (if external) whenever you want to use it as the OS

Some linux subreddits: r/linuxmasterrace, r/unixporn and most distros have their own subreddits as well

Some youtube channels: LearnLinuxTV, Chris Titus Tech, DistroTube, and may more…...
(Work in Progress, Will be completed soon, updated/improved gradually)

