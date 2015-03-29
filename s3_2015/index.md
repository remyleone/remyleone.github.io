---
layout: page
title: S3 2015 proposal
---

# Life of a web request. How the Internet works?

![Project image](internet_is_fascinating.jpg)

The Internet is becoming one of the most important tool that people use to
read, do and share research, messages and ideas. Many people use it as a tool
but not so many really understand how networks and the Internet works, evolve
and keep spreading its influence. The Internet is by itself a very vivid
subject of research related to the domain of distributed systems with very
active and open research mixing industry and academics. Making computers talk
to each others seems like obvious today but network protocols are the results
of a long process mixing engeering and scientific research.

The goal of this project would be to study, understand and recreate all the
protocols that make the Internet what it is.  We would study the Internet's
structure and protocols through experiments and dissecting network activity.
We'll use and write programs to explore what happens at a networking level as
you surf the Web, use a search engine, send emails, use torrents and more. All
these protocols would be tested and played with. At the end, students would be
able to craft a little Internet working within their own network.

## Required material

- Curious students.
- Relatively recent computer (Intel i3,5 or 7 and at least 2GB of RAM)
- Mostly PC running a recent UNIX system (GNU/Linux or MacOSX). For people
  running windows I can find workarounds using virtualbox.
- If computers are provided can you ensure that I will be able to install software on it and more generally have administrative privileges? That would help in the very low level part of the networking stack.
- If you have some raspberry pi/Arduino available that would be great. Otherwise I will see if I can bring some with me.

## Agenda

| Day 1  |             Presentation            |
| Day 2  |        Life of a Web Request        |
| Day 3  |           Life of an Email          |
| Day 4  |          Life of a torrent          |
| Day 5  |          Life of a web chat         |
| Day 6  |     Life of an Autonomous System    |
| Day 7  | Life of a request inside a computer |
| Day 8  |        Life of a Wifi Network       |
| Day 9  |          Internet of Things         |
| Day 10 |                Sum up               |


## Aims

### What is the problem you are going to solve? / What will be the challenge in this project?

How computers connect to each others on the other side of the world. How
computers talk to each others.

### What is the final result you will get? / What will you try to accomplish in the end?

We obtain the same thing at the beginning that at the end. Rather than
building something we are going to dissect a living system. At the end I want
to hear a story. What happen when I press enter while visiting a website. What
happen when I launch a process.

## Project Course

### Theoretical concepts

How protocols are constructed. General pictures of how computers works and what are the different levels.

As a teaching assistant I got all the material from my introduction course to
networks. My objectives is to have a more hand-on experience. Go from working
stuff and then try to dissect the different encapsulation and understand how
they work with each others.

### Experiments performed

Dissecting protocols, seeing what are the packets sends on the internet. See
how they evolve how they move. For that we will use wireshark that is a packet
dissector and different virtual machines interconnected in a virtual network
to see how communications happen between machines. The agenda of our different
focus is presented in Agenda.

## Science with benefits

### Benefits for the students

- A basic understanding of the processes happening inside the internet and also inside their computer.

- Some notion about python and python libraries that might help them later on if they continue working in science/tech fields

### Why should it be featured?

Understanding the Internet and the problematic behind how it works can be
useful for every scientist that want to preserve an open Internet and being
able to solve problems that might occurs while using it to share/talk with
other people with it.

There is an other benefit. The Internet is probably one of the most decoupled
achievement of humanity. It doesn't have a single creator, controler or
regulator. It's an ecosystem mixing scientists, industrials and people.
Understanding the human processes behind this can be relevant to scientist as
well.

## Security risks

All experiments will be run on virtual machine or uncriticals machines.
Students should be safe.

## Backup plans

### Hardware issues

As long as I got working and recent machine where I can do whatever I want or
install virtual box, I think I will be fine. One safer bet would be to tell
the students to bring their own devices. Therefore, no matter what is provided
we might have a fallback. I can find dirtier hacks if that fail as well but I
would strongly appreciate to have some safety that I will have proper
materials.

### Interest/Understanding issues

In the case where students are not interested and/or don't understand what is
going on I can change subjects relatively quickly to an other aspects of
computing. All of them are pretty much independant. I would strongly
appreciate to have students interested in computer science/networking. Worst
case scenario we could probably team up with the guys in Automating Biology -
An End to End Approach and focus on how to make the research sharable easily
with IPython for instance.

### Outperforming issues

An alliance between the guys in Automating Biology - An End to End Approach
could also be done in case where students are working fast and we have enough
times to propose collaboration with other teams.


## The part where I talk about myself with the third pronon

*don't forget to show my head to the people. it's well worth seeing*

![Here is my face](http://fbcdn-profile-a.akamaihd.net/hprofile-ak-snc4/275438_593375686_6720633_n.jpg) 

Remy LEONE a PhD student working at Telecom Paris Tech in the field of
Wireless Sensors Networks. His research interests are passive monitoring of
networks, active estimation of energy reserve and lifetime expectancy of a
network. He studies technologies working at the edge of a constrained network
to help it live longer.

Student of S3++ in 2007 and member of [Paris Montagne](//paris-montagne.org)
since 2006. This association spreads science and taste of scientific research
in youngs and not so young minds.

<!--
You can know more by looking at http://sieben.fr/about. Happy stalking :)
-->
