---
layout: post
title: Scripting
---

## Background Story

I'm currently looking for a flat in Hamburg and to describe it in one word would be: hopeless. The real estate market there is [insane.](http://immobilien-kompass.capital.de/hamburg/eimsbuettel-stadtbezirk/eimsbuettel-stadtteil) Affordable flats in a loved quarter (*f.e Altona, Ottensen, Eimsbüttel*) stay online for one to three hours and in that time the landlord/real estate agent will receives on average about **200** emails (*So the landlords have told me, to whom I've talked to about this problem.*) 

That means, I need to be constantly online and hit the refresh button on the big 3,4 real eastet portals in Germany. Between my job and school I don't have the time to do that, which means I miss out on a lot of good offers.
<br>
<br>
<br>

## Solution

I need a program, that checks the portals I want, searches for the keywords I find interesting and then reports back to me (*f.e via email*), if there are any new offers, that I might find interesting. I need it running, even when I'm not home and I need a way to check, if it's doing what it's supposed to do (*f.e log a simple message*). A quick Google search and I landed on [this page](http://www.wohnungsengel.de/), which offers something, what I'm looking for. I tried it for a week, but the free version does not work as fast and exactly like I want it to, so I decide to write some code myself!
<br>
<br>
<br>

## First Try

So I open my Visual Studio - as I always do when I want to write some code (*My goto IDE*). After a half a days work I finish a *web-crawler-like* console tool in C#, that searches the websites, I tell him to and saves the links, that he finds, in a HTML-file, that I can then check. I used [Abot](https://github.com/sjdirect/abot) to help me. Turned out ok. 

Now for the second part - I need it to run even without me sitting at the computer and double clicking the EXE. Better yet - not at all on my PC, because I don't want to have it on the whole day. **Eureka moment!** I have a [PI](http://arghh.github.io/Raspberry-Pi/), so I just copy the program there and find some script to run the program for me! "Easy," I thought. Wait a minute, my PI is running a Debian based lightweight OS called [DIETPI](http://dietpi.com/). Great! My Visual Studio compiled C# code is useless :(
<br>
<br>
<br>
<br>

#### Lesson learned

**Think my steps through until the very end BEFORE writing any code ..**
<br>
<br>
<br>

I need a break ..
<br>
<br>
<br>

## Second Try

Actually what I needed is a script and not a program AND I need it to run on any OS. Something valuable I learned at this point - Always use the tools, that best help you solve a given problem and don't be afraid to pick something, that you are not so familiar with. So I googled a bit and picked **Python**. Installed it on my PC (*to code and debug*) and on my PI. All the needed packages I ended up using, I got over PIP (*Package management system for Python*) and to run/test my script on Windows, I just use the command line. After one day, I had a script, that was less then 70 lines of code long and did everything my C# program did - and even more. I copied my script to the PI and all worked fine. 
![Python Functions](http://arghh.github.io/images/python/functions.JPG)

Now for the second part - *that I failed on my first try* - run it automatically. I found [cron](https://www.raspberrypi.org/documentation/linux/usage/cron.md) to best suit my needs.
<br>
<br>
<br>
*cron service status tab*

![Cron Service Status](http://arghh.github.io/images/python/cron.JPG)
<br>
<br>
<br>
*my python script in action*

![Script In Action](http://arghh.github.io/images/python/script.JPG)
<br>
<br>
<br>

## Conclusion

For 2 weeks now I've not missed out any offer and I've learned some python!
<br>
<br>
<br>
<br>

### PS

I promise, that the next blog entry will be before ... christmas! :)

