+++
author = "Frederic Branczyk"
title = "Current Projects"
date = "2013-11-18"
+++

Essentially what has been keeping me from completing projects before, was 
frustration, then forget about it and just don't look at it again. To not break
this habit I want to use a GitHub streak to see that I actually work on 
something daily. My hypothesis: even if I only spend a couple minutes a day on
any of my projects, the progress will be greater than if I just try to finish
the software not keeping track of how much time I spend.

I will present the projects of my current streak and then talk about experiences
I have made so far.

![Octocat](/images/Octocat.jpg)

#### Le start: URAAAS

Even though it was not the start of the GitHub streak the first project I 
worked on me and a friend of mine writing an obviously very balant copy
of foaas (Fuck Off As A Service) called uraaas (You are awesome as a Service).
It is written in scala using scalatra (for those unfamiliar with it, it is
like sinatra for scala). It was a couple hours of fun, but since we're not too
proud of the resulted code, we have not yet published it.

Take a look at it and tell us what you think: 
[URAAAS](http://uraaas.herokuapp.com) (it might take a while since the dyno
shuts down, when no one visits it for 30 minutes)

#### Second project: vim-pastebin [Running App](http://vim-pastebin.herokuapp.com/)

I have started to learn Rails and written my first app the
vim-pastebin. Although it is not a very complicated application I was very
surprised how fast I learned to use Rails. That's when I decided to keep that
pace up. Since it's my first rails project there are probably a lot of mistakes
and wrong assumptions. This project is basically done regarding features.
My friend tried to create a vim plugin for it, however, up until now he has not
succeeded in doing so mostly because vim-script is some weird shit. It would be
cool if I could get some feedback on the rails app to be able to learn from my
mistakes.

#### Project #3: Suploy

As part of software engineering course at university we had to form teams and
create a software we desired. Since my team and I are big fans of Open-Source
we soon decided it should be open source. We wanted to create something
that could help us and other developers in their process of creating more
awesome software. The idea started to gain shape and we ended up planing an
open source PaaS and called it suploy.

At first we doubted being able to create such a system but we started
experimenting with a combination of git, gitolite, docker, buildstep and nginx.
We soon had somewhat working prototypes and went on to building the webapp in
which users are supposed to manage their webapps, ssh-keys, etc.

#### Last but not least: OSHome

This project was my Dads idea because he wanted to collect and analyse data
around our house. Our first attempt used an arduino (yes an arduino, because I 
had never worked with hardware before and it seemed simple enough to get
started with) to collect the data and put it in a mysql database through a php
script. Then I also wrote a pretty complex java application through which my
dad could analyse it. I also experimented with a webinterface which used the
google chart api written in php (which back then was the only language I knew
to write "webservices"). Based on that I also started building an android app
which I soon stopped because android lacked good chart libraries.

The arduino died after about half a year of collecting data. That was the time
I started to think about redoing the project completely, since it was also when
I was amazed by the rails magic and have developed a hate against php.

Now I am rebuilding the system with rails using d3js to generate the graphs.

#### Preliminary result

I have never felt so productive before! My biggest fear before starting this
was that I possibly won't enjoy programming as much, since I push myself to
work regularly. Ironically I actually enjoy it even more. I can't really
explain why but it probably has to do with knowing that you are being
productive.

Another thing I thought would be difficult was finding something to do,
however, I soon realized there is always something todo. Even if it's just
styling something so the user interface looks nicer. On some days it was 
literally adding one line to make it look nicer, but hey I won't have to do it
another time! I tend to ignore styling websites because I don't find I 
particularly interesting. I rather enjoy solving problems using algorithms, 
math, and statistics. Styling a website doesn't give me that.

Sometimes I even challenge myself a bit more by adding the most I can do on a
day just so I have to come up with something new the next day. That way I make
myself think about how I can improve my projects.
