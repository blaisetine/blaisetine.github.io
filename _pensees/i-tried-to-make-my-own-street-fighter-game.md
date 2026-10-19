---
title: "I Tried to Make My Own Street Fighter Game"
subtitle: "A childhood story about learning to make my own games"
date: 2026-10-19
description: "A true story of growing up in Cameroon, falling in love with Street Fighter II, and trying to build a fighting game in Pascal—with no internet, scanner, or programming classes."
image: /images/pensees/street-fighter/arcade-cameroon.jpg
---

## Part 1: The Game That Changed Everything

*Street Fighter II* is my favorite video game of all time.

I fell in love with it growing up in Cameroon in the 1990s. I loved the music, the colorful fighters, the excitement of playing against another person, and the way every character had a different style. A beginner could learn to throw a punch in minutes, but becoming really good took patience, practice, and plenty of defeats.

![A teenager with an untucked light-blue school shirt and backpack watches two boys playing Street Fighter II in a busy neighborhood arcade in Cameroon.](/images/pensees/street-fighter/arcade-cameroon.jpg)
*The arcade: two players, a crowd of spectators, and a game I could never stop thinking about.*

There was something special about the competition. I remember Street Fighter tournaments in neighborhoods, high schools, and even between players from different cities. People gathered around the arcade cabinets, cheering, arguing about who was the best, and waiting for a chance to challenge the winner. One player could look unbeatable—until someone who had practiced a little harder came along.

It reminded me of soccer. Back home, I knew children who would spend every spare moment kicking a ball, practicing the same move again and again, dreaming of becoming great players. I understood that feeling. My game was just a different kind of competition. I wanted to get better at Street Fighter, to learn every move, and to understand why one player could outsmart another.

But I was fascinated by something else, too.

**How on earth had someone made this game?**

I watched the fighters as closely as I watched the matches. How could a computer draw such detailed characters? How did they move so smoothly? How could pressing a button make someone jump, kick, or throw a punch at exactly the right moment? And how did the computer manage all of that while playing music?

To most players, it was a game. To me, it was also an enormous mystery waiting to be solved.

### From tic-tac-toe to Street Fighter

By then, I already knew a little about programming. I had used **QBASIC** on an IBM PC and even written my own tic-tac-toe game. It wasn't much to look at, but the feeling was wonderful: I could type instructions, run a program, and watch a computer follow my ideas.

Tic-tac-toe, though, was mostly a grid of nine squares. Street Fighter had moving characters, animated backgrounds, sound, music, and two people pressing buttons at once. The difference seemed enormous.

And yet, the more impossible it looked, the more I wanted to try.

One day, I made a rather ambitious decision: **I would make my own Street Fighter game.**

### A language with my name

To do that, I decided to learn **Turbo Pascal**, a popular version of the Pascal programming language for the IBM PC. I had an unusual reason for being drawn to it: my name is Blaise-Pascal, and Pascal is also the name of the programming language. It was named after Blaise Pascal, the French mathematician. That connection delighted me. It made me even more determined to learn.

Of course, sharing a name with a programming language did not make it any easier to understand!

I was a French-speaking high-school student, and my English wasn't very good. I had never studied algorithms, data structures, or computer graphics. In Cameroon in those days, I had no internet access. If I didn't understand something, there was no video tutorial to watch and no search engine to ask.

Fortunately, Turbo Pascal came with some examples and tutorials. I read what I could, copied small programs, changed a few lines, and ran them again to see what happened. Sometimes the result surprised me. Often the program simply refused to work.

But each experiment taught me something. Little by little, I began to believe I might actually build my game.

I didn't yet know that **the hardest part would not be writing the game. It would be creating all the things the game needed.**

**Find out why in Part 2.**

## Part 2: First, I Had to Build the Tools

### A fighter is hundreds of little pictures

The first thing my game needed was a fighter. That sounded easy enough. After all, I could draw.

But take a close look at a character in Street Fighter. The character doesn't just stand still. He walks, crouches, jumps, punches, kicks, gets hit, falls down, and stands up again. Each movement is made from a series of slightly different pictures shown rapidly, one after another.

That is **animation**. A single picture is a *frame*; the little images used for game characters are often called *sprites*.

Think of drawing a person throwing a punch. First, the arm is pulled back. In the next picture it moves forward a little. In the next, a little farther. When the pictures are displayed quickly, the arm seems to move. The computer isn't drawing a moving arm—it is showing still pictures so fast that our eyes see motion.

Now imagine doing that for every punch, kick, step, and jump in a fighting game.

![An original childhood sheet of many hand-drawn fighter poses arranged in a grid, showing different movements and actions.](/images/pensees/street-fighter/fighter-pose-sheet.jpg){: style="max-width: 420px"}
*One of my old sheets of movement studies. Every pose meant another picture to create.*

I started sketching character poses on paper, trying to work out how the different movements could fit together. I filled pages with figures in different positions. What looked effortless on the arcade screen quickly became a mountain of work on my desk.

### My paper became a pixel grid

There was another problem. I didn't have a scanner, so I couldn't take a drawing on paper and put it straight into the computer.

I used squared and lined paper to plan my pictures. A computer image is made of tiny colored squares called **pixels**. By carefully coloring the squares on paper, I could work out where each color needed to go on the screen.

<div class="pensee-pair">
  <img src="/images/pensees/street-fighter/blanka-pixel-study.jpg" alt="A surviving color drawing of Blanka on lined paper, with visible individual colored squares.">
  <img src="/images/pensees/street-fighter/fei-long-pixel-study.jpg" alt="A surviving hand-colored study of Fei Long in a fighting stance, with a visible pixel grid.">
</div>
<p class="pensee-pair__caption"><em>My hand-colored studies of Blanka (left) and Fei Long (right), built up square by square.</em></p>

Finishing a drawing on paper was only half the job. I then sat at the computer, held the mouse, and drew it **all over again**, coloring the corresponding pixels one at a time. I couldn't just click a button to import my drawings. There was no scanner to do the work for me.

Some of the pictures I've kept are studies of characters and scenes from other games I loved, not necessarily artwork that made it into my own game. I was studying how game artists made recognizable characters out of little colored squares. I was also learning how much time every extra animation frame would cost me.

![An original childhood page mixing fighting-game character sketches, small sprites, and studies of scenes from different games.](/images/pensees/street-fighter/character-and-scene-studies-landscape.jpg)
*Character ideas, fighting poses, and scenes from games I admired.*

![An original page of scene and background studies, character drawings, and architectural details.](/images/pensees/street-fighter/background-studies.jpg)
*Backgrounds and character studies: a fighting game needed more than fighters.*

The work was exhausting. A character that took only a moment to appear on the arcade screen could take me hours to reproduce. And every time I wanted a smoother punch or kick, I needed more pictures.

I began to realize that making a video game required much more than knowing how to program.

### So I wrote my own drawing application

I needed a better way to work with pictures. Since I didn't have the drawing software I wanted, I decided to make my own.

I called it **Polaroid**.

![Screenshot of Polaroid, my MS-DOS drawing application, showing drawing tools and a picture on its canvas.](/images/pensees/street-fighter/polaroid.png)
*Polaroid, the drawing application I wrote in Pascal. [Explore the preserved program](https://blaisetine.github.io/polaroid/).*

It had a mouse-controlled drawing area, colors, and tools for drawing and erasing. More importantly, I worked out how to **save a picture to a file and load it back later**. That meant the pictures I created didn't have to disappear when the program stopped running.

This was exciting for another reason. I was beginning to understand that a picture inside a computer is also **data**. Each pixel has a position and a color. If I could store that information in a file, another program could read it and draw the same picture on the screen.

I had never taken a computer graphics course, but I was discovering some of its basic ideas by experimenting. I learned about representing pictures as data and drawing them into a **frame buffer**—the memory area that holds the image the computer displays.

I spent many nights on Polaroid. My fighting game was still far from finished, but I had written a real drawing application along the way.

### A fighting game needs music, too

Of course, I couldn't imagine Street Fighter without its music. The character themes were part of what made the game unforgettable. I especially loved **Ryu's theme**, and I wanted to hear it in my own game.

Once again, I didn't have the program I needed. So once again, I tried to build one.

I called this one **Cybersound**.

![Screenshot of Cybersound, my MS-DOS music application, with an on-screen piano and controls.](/images/pensees/street-fighter/cybersound.png)
*Cybersound, my homemade music program. [Explore the preserved program](https://blaisetine.github.io/cybersound/).*

Cybersound had an on-screen piano and controls for playing and recording notes. I worked out how to save music into a file so a program could read it back later. I painstakingly recreated the theme I loved and encoded it for my game.

That was another little discovery: music, like pictures, could become data. Instead of recording a sound with a microphone, I could tell the computer **which notes to play and how long to play them**.

Without planning to, I had started building an entire collection of tools. I wanted to make a fighting game, but first I had made a drawing program and a music program, and had begun figuring out how to turn their output into files my game could use.

The irony made me smile: **I was learning to write software so that I could write more software.**

At last, I could begin assembling my fighting game.

And that was when I ran into the problem I could not solve.

**Find out what happened in Part 3.**

## Part 3: The Game I Never Finished

### Making the fighter obey the player

I could draw pictures. I could load them, put them on the screen, and play music. But a fighting game has to do something much harder: **it has to respond to you.**

Press the left key, and your fighter should step backward. Press another key, and he should throw a punch. If you jump, the character should rise, fall, and land. If the other player attacks, your character should react. And all of that has to happen fast enough to feel natural.

That was where I struggled most.

I couldn't figure out how to organize the movements so the right animation played at the right time in response to the keys. Even when I got pictures moving, the animation was too slow. And every attempt to make it smoother seemed to demand more of those painfully hand-drawn frames.

When I played Street Fighter, I pressed a few buttons and the character seemed to come alive. When I tried to make my own version, I discovered how many little problems were hidden behind every button.

![Screenshot from Karate, the unfinished fighting game, with two fighters, a stage, and score and energy displays.](/images/pensees/street-fighter/karate.png)
*Karate, the unfinished game I made in Pascal. [See the surviving version](https://blaisetine.github.io/karate/).*

Meanwhile, I was still in high school. I had to prepare for my **Baccalauréat** examinations, and I couldn't spend every hour programming. My project was much bigger than I had imagined, and I didn't yet have the knowledge to complete it.

Eventually, I stopped working on the game.

I had music, graphics, and some animation, but not the responsive fighting game I had dreamed of creating.

### A little piece of my childhood survived

By the time I went to college, I had lost the original **source code**—the Pascal instructions I had written. Luckily, I had kept a copy of the **compiled program**, the file the computer could run.

That is the version that survives today. It runs under an MS-DOS emulator in a web browser, although it is incomplete: you can hear its music and see some graphics and limited animation, not a finished game you can properly play.

I'm glad I saved it. Together with my old drawings, it reminds me of the hours I spent at that computer, trying to make an idea in my head appear on a screen.

### What I learned while trying

When I went to college, I learned much more about programming. I studied languages such as C++ and Python, along with algorithms, data structures, and computer graphics.

Some of the problems that had seemed impossible in high school finally began to make sense. There were ways to organize a character's actions, handle input, control animation, and make graphics run efficiently. Many of the ideas I had struggled to discover alone even had names.

But I don't think of my unfinished game as wasted effort. I had taught myself Pascal. I had written Polaroid and Cybersound. I had learned to save images and music as files, display graphics in a frame buffer, and experiment with animation and keyboard input—all because I wanted to make a game I loved.

Nobody had assigned me this project. I wasn't doing it for a grade.

**I kept trying because I loved Street Fighter.**

### Where that passion led

Many years later, I worked at **Microsoft on the graphics technology behind Direct3D**, the software many PC and Xbox games use to draw their pictures. I sometimes thought about how strange that journey was. The teenager in Cameroon who struggled to draw a moving fighter had grown up to work professionally on technology that helps games display images.

I hadn't planned that career when I opened Turbo Pascal. I was just curious about a game I loved, and each question led me to something new to learn.

That is why I think back to the soccer-loving children I knew in Cameroon. Some spent countless afternoons practicing a sport because they loved it. My afternoons were often spent trying to understand computers. Whether your passion is soccer, music, drawing, mathematics, physics, or video games, there is something wonderful about wanting to get better at it—not because someone told you to, but because you can't wait to try again.

Of course, passion doesn't make every obstacle disappear, and it doesn't guarantee that you will achieve the exact dream you started with. My fighting game is proof of that.

But it can give you the determination to keep asking questions and learning new things, even when the path is difficult.

I tried to make my own Street Fighter game. **I never finished it.**

But I learned to make software, discovered computer graphics, and found something I would love doing for years to come.

And that turned out to be a reward I could never have imagined when I first stood watching those fighters on an arcade screen.

### Explore my childhood projects

The original programs I preserved are still available to explore:

- [Karate](https://blaisetine.github.io/karate/) — my unfinished fighting game. The original source code was lost; the saved compiled program survives.
- [Polaroid](https://blaisetine.github.io/polaroid/) — the drawing application I wrote in Pascal.
- [Cybersound](https://blaisetine.github.io/cybersound/) — my music application, also written in Pascal.

### Words to know

- **Pixel:** One tiny colored square in a computer image.
- **Sprite:** A little picture used to represent a character or object in a game.
- **Animation frame:** One of the still pictures that create the illusion of movement.
- **Frame buffer:** The part of memory that holds the picture a computer displays.
- **Source code:** The instructions a programmer writes for a computer.
- **Compiled program:** A version of those instructions translated into a form the computer can run.
- **Algorithm:** A set of steps for solving a problem.

### Try this

Make a tiny animation without a computer. Draw a stick figure at the corner of a page, then draw the same figure on the next page with one arm raised a little higher. Make three or four pictures, each with the arm in a slightly different position. Flip the pages quickly with your thumb. Does the arm move?

Now imagine drawing not four pictures, but dozens of them—and teaching a computer which one to show when someone presses a key. That's the challenge that kept me busy for so many afternoons.
