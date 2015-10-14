---
layout: post
title: Learning by doing
---

I finally finished the beta version of my first tiny 2D game and I learned a lot by doing it.

In the end I named it **Rotes Flugzeug** (*Red Plane in English*) - original I know - after a childhood favorite called [Red Plane](http://www.addictinggames.com/shooting-games/redplane.jsp). It is a simple arcade game using a [parallax scrolling effect](https://en.wikipedia.org/wiki/Parallax_scrolling), where a player flies in a circle and needs to destroy falling bombs, before they hit the ground. The idea is based on a classic Atari game from 1988 called [Starray](http://www.atarimania.com/game-atari-st-starray_11375.html). I use similar turning and moving patterns as does the original game. Rotes Flugzeug is written in C++ and uses [SFML libraries](http://www.sfml-dev.org/index.php) to animate and move sprites. As IDE I used [Visual Studio 2013](https://www.visualstudio.com/en-us/news/vs2013-community-vs.aspx). The game art is a mixture of my own paint skills plus what I found at [OpenGameArt](http://opengameart.org/). 

For the artwork I had a fixed 800 x 600 screensize in mind while cutting and combining the artwork. (*f.e three times the same motive 800px wide to create the illusion of never ending gamefield*). For programing the movement I also assumed that the screen will always be 800x600 pixels big. So the game is not very responsive nor flexible and converting it into an app or a browser game in the future will be very difficult. But I'm fine with it. That was also not my goal. My goal was to learn the basics of game development. It was just a project to learn the basics of game design. Also it runs only on Windows OS and requires OpenGL for better movement. However in the near future I'd like to program for all platforms, just to see the difference, when designing for a specific screensize and platform in mind vs all screens and all environments combined.

I learned a lot developing **Rotes Flugzeug**. The source-code grow over 500+ lines long in the end and I was a bit mad at myself for not **structuring** my code properly from the getgo. Now I need to do a lot of extra work - *which could have all been avoided* - when I would have followed one design logic throughout my program. When you start programing, you should always have an idea, how you design your project. Even if your project is small and you won't lose the overview, having a good structure helps you a lot later on when designing bigger project or adding new features to your smaller projects.

**Commenting** is another thing I did not do properly from the start. I did add comments, but not constantly enough and not every day. 

Third thing I learned: **naming** things is really-really **hard**. When we write a new function, we name it and then focus **only** on what comes between the curly braces. After finishing a method, I often saw that the name I gave it at start (*might have been hours/days before I actually wrote the body of the function*), did not actually describe what the function did at all, so I had to rename a lot of methods and variables, too better represent, what they ended up doing. 

The project was a lot of fun and I will definitely keep working on it. First thing on my list to do is to rewrite the sourcecode: remove the useless parts, replace a lot of if-else statements with loops or switch cases, give variables and methods better names. All of that is extra work and I should have planned my work better so I would not have to do it afterwards, but this was my first bigger project *(500 lines of code)* so it was something totally new for me. I now have a lot of new things I need to start learning. 

In conclusion I can say, that the project was a success, because I now know the basics of game loops, rendering, frames and importance of **time** in *time * speed = distance* in **game design**. Those where the things I wanted to learn when I started my project and that I managed to accomplished.





*A little TODO-list to make the game more fun and playable.*

        Proper Menu (start/end screen)
        Highscores
        Radar
       

[**Download Rotes Flugzeug** (*.zip file for windows only.*) - *compressed size 599KB.*] (http://arghh.github.io/data/RotesFlugzeug.zip)
