---
title: (240517) The hack that almost broke the internet
date: 20240517
tags: #PlanetMoney
citation: “Planet Money,” _NPR_, 2 Juni 2023. [https://www.npr.org/podcasts/510289/planet-money](https://www.npr.org/podcasts/510289/planet-money) (diakses 4 Juni 2023).
---


----
# Points

- 

----
# Article
https://www.npr.org/2024/05/17/1197959102/open-source-xz-hack
Last month, the world narrowly avoided a cyberattack of stunning ambition. The targets were some of the most important computers on the planet. Computers that power the internet. Computers used by banks and airlines and even the military. 

The hack that almost broke the internet
May 17, 20246:35 PM ET

By 

Jeff Guo

, 

Nick Fountain

, 

Jess Jiang

, 

Emma Peaslee
25-Minute Listen

    Download

    Transcript

Guinness World Records challenge Jenga enthusiasts to build 30 levels of the popular building game in the fastest time possible at The Walkways, Tower Bridge on March 22, 2005 in London.
Getty Images

Last month, the world narrowly avoided a cyberattack of stunning ambition. The targets were some of the most important computers on the planet. Computers that power the internet. Computers used by banks and airlines and even the military.

What these computers had in common was that they all relied on open source software.

A strange fact about modern life is that most of the computers responsible for it are running open source software. That is, software mostly written by unpaid, sometimes even anonymous volunteers. Some crucial open source programs are managed by just a single overworked programmer. And as the world learned last month, these programs can become attractive targets for hackers.

In this case, the hackers had infiltrated a popular open source program called XZ. Slowly, over the course of two years, they transformed XZ into a secret backdoor. And if they hadn't been caught, they could have taken control of large swaths of the internet.

On today's show, we get the story behind the XZ hack and what made it possible. How the hackers took advantage of the strange way we make modern software. And what that tells us about the economics of one of the most important industries in the world.

This episode was hosted by Jeff Guo and Nick Fountain. It was produced by Emma Peaslee and edited by Jess Jiang. It was engineered by Cena Loffredo and fact checked by Sierra Juarez. Alex Goldmark is Planet Money's executive producer.

Help support Planet Money and hear our bonus episodes by subscribing to Planet Money+ in Apple Podcasts or at plus.npr.org/planetmoney.

Always free at these links: Apple Podcasts, Spotify, Google Podcasts, the NPR app or anywhere you get podcasts.

Find more Planet Money: Facebook / Instagram / TikTok / Our weekly Newsletter.

Music: NPR Source Audio - "Strange Tango," "Warped Worlds," and "Detective Dan"

# Transcribe
https://www.npr.org/transcripts/1197959102
SYLVIE DOUGLIS, BYLINE: This is PLANET MONEY from NPR.

(SOUNDBITE OF COIN SPINNING)

JEFF GUO, HOST:

Now that Richard Jones knows how close the entire world came to disaster, he's been looking back for any hints, any clues that he might have missed. For him, the first clue was this message that showed up in his inbox on February 26.

RICHARD JONES: So I remember I got this email, and It was not anything unusual.

GUO: Richard is a senior engineer at Red Hat. He helps make an operating system that is used all over the world. We're talking Fortune 500 companies, major hospital systems, banks, even the U.S. military.

NICK FOUNTAIN, HOST:

And what's interesting about that operating system is that it is completely open source, meaning it's made out of all these different pieces of software that people are putting out for free.

GUO: So Richard is often emailing with strangers on the internet.

JONES: I don't know who half the people I talked to on the internet about software are. I don't know who they are in real life. I've never met any of them. Instead, we'd work on reputation.

FOUNTAIN: And that email he had gotten, it was from a guy who was new-ish on the scene, but who had built up a pretty solid reputation - a guy named Jia Tan. For about a year, Jia had been the volunteer in charge of this very popular software program called XZ, which helps compress data.

JONES: It's not the fastest, but it is the one that compresses the most. It's very useful for us.

GUO: Look, I don't think I'm exaggerating when I say that compression is key for everything - for storing files, for sending stuff over the internet - everything.

FOUNTAIN: In the email, Jia sounds pretty enthusiastic, but in a way that a lot of open-source volunteers sound enthusiastic. He says, hey, I just made this cool update to XZ. Hope you guys can put it into your operating system.

GUO: And this email, I will say, it looks very innocent. It's written in this chipper tone. It's got smiley emojis.

FOUNTAIN: It has exclamation points, which just signals, you know, no threat here. And so Richard goes ahead. He puts the new updated XZ code into a preliminary version of their operating system to test out. But pretty soon, he starts getting these bug reports.

JONES: They were quite strange but not totally unusual.

GUO: This new version of XZ, it seemed to be messing with other parts of the computer, like, critical parts of the memory.

JONES: But, you know, bugs happen in software, right? You know, software is full of bugs.

FOUNTAIN: So Richard emailed Jia and asked him to, you know, take a look at the problem.

JONES: He came back within two or three days and said, I'm really sorry. We've just released a new version which fixes this bug for you. So could you upgrade to that?

GUO: Which Richard does, and everything seems fine - until about a month ago.

FOUNTAIN: That is when someone discovers that this new version of XZ, it is not what it seems to be. And Jia Tan is not who he seems to be.

JONES: I was surprised. I was a bit shocked. I was angry. I just didn't expect that somebody would try that.

FOUNTAIN: What we now know is that Jia Tan was a hacker or probably a group of hackers. And they were trying to pull off one of the most audacious cybersecurity attacks in history.

GUO: Over the course of two years, these hackers had infiltrated one of the most popular programs out there - XZ. And if they hadn't been caught, they would have had a secret back door to some of the most important computers in the world. Hello, and welcome to PLANET MONEY. I'm Jeff Guo.

FOUNTAIN: And I'm Nick Fountain. If you peek under the hood of the internet, what you'll find is that most of the computers powering it or running free open-source software.

GUO: But here's a dirty secret. A lot of that software is written by small teams, sometimes teams of only one person, which makes them pretty vulnerable and easy to infiltrate. Today on the show, the story of the XZ hack, how it took advantage of the strange way we make modern software and what it tells us about the economics of one of the most important industries in the world.

(SOUNDBITE OF MUSIC)

GUO: The hack that we're talking about today, the XZ hack, could not have happened if it weren't for the weird way that most modern software is made. We have these trillion-dollar corporations working side by side with unpaid, sometimes even anonymous, volunteers to write the software that powers the internet.

FOUNTAIN: Right. And so before we can get into how the XZ hack went down, we're first going to have to understand how modern software got to be this way. For that, we went to one of the founders of the open-source software movement, Bruce Perens.

BRUCE PERENS: Back when I was starting this, you would have asked what drugs I was using and where you could get some.

GUO: Bruce says, for him, it all started with this epiphany he had about how to write software efficiently. At the time, it was the 1980s, and he was a young programmer at Pixar. He wrote software that helped make movies like "Toy Story 2."

FOUNTAIN: I'm a bigger fan of 4, but whatever. Bruce would keep running into this annoying problem. His programs, they would glitch out, and they would accidentally overwrite other parts of the computer.

GUO: Yeah, and, you know, these bugs, they would happen all the time back then. It was like the Wild West of software.

FOUNTAIN: So Bruce's solution was to write up a piece of software that would monitor other programs, and it would alert him whenever a program started to overwrite stuff that it shouldn't be writing over.

PERENS: It would stop your program in the instant that happened and let you see the exact instruction that you had wrong. And I called this Electric Fence because when you touched the fence, it would zap you.

GUO: Bruce's Electric Fence proved to be pretty handy, so he shared it with his colleagues at Pixar. But then he thought maybe other people would find it useful, too. And at the time, there were these online bulletin boards where programmers would hang out. And Bruce was a regular. He says this community had a culture of sharing. Programmers from different companies would show each other new ways of doing things, even provide code for others to copy.

PERENS: So all of the engineers - software engineers - at the time started sharing software together, and we started using it in our work. And no one in management or legal knew that it was happening.

FOUNTAIN: Bruce went ahead, and he posted the code for Electric Fence onto that bulletin board. And Electric Fence became incredibly popular. All of a sudden, people around the world started using it.

PERENS: Someone wrote to me and said, your Electric Fence program has just saved my job. If you...

GUO: Whoa.

PERENS: ...Ever go to Ireland, please stay in my home.

GUO: Oh, my gosh. Did you go?

PERENS: No, no, I never met this guy, but you know, I was getting fans.

GUO: That felt pretty good. But then something even more gratifying started to happen. Some of Bruce's fans, some of these programmers he'd never met, they made their own improvements to Electric Fence, and they shared these improvements with Bruce. They sent him their tweaks and upgrades to his code.

PERENS: And I thought, you know, whatever work I've put into this, I just got back. And it kept happening.

GUO: This experience helped Bruce realize two things. First, it illustrated an unexpected benefit of giving away your code because not only could your code help other people, these total strangers, but now those strangers could help make your code better. And second, Bruce realized that if they all worked together this way, they could write software so much faster and better.

FOUNTAIN: Yeah. Bruce says a lot of programmers in their day-to-day jobs would spend hours doing essentially the same thing as their counterparts at other tech companies, writing the same basic code to solve the same basic problems.

PERENS: So back then, it would be like building a house, and you'd have to dig up this clay and fire all the bricks. And open source was - the idea was we would all chip in on making all the different bricks, and we would give them to each other for free. And now you are not wasting your time on the bricks. You're building the architecture.

GUO: This is where Bruce saw the beginnings of a powerful idea 'cause there's already this culture of sharing software in order to be a good citizen or to promote a free society or whatever. But Bruce saw that this could also transform the whole economic model for making software. Bruce believed that if people could get together to produce software in an open and crowdsourced way, you could outcompete even the mightiest corporations.

FOUNTAIN: Now, Bruce wasn't the only one who realized this. By the 1990s, a lot of programmers were attracted to this open-source model, but, you know, they weren't taken too seriously. But the open-source movement would soon have an opportunity to prove itself.

GUO: Yeah. You see, by the late '90s, the internet was really starting to take off. Remember, this was the era when there were so many AOL online CDs floating around - people were using them as coasters.

FOUNTAIN: What a time to be alive. And the big question at that time was, what software would this new internet run on?

GUO: And a person who would play a pivotal role in the war over the internet was Sam Ramji.

SAM RAMJI: Software was becoming infrastructure. It was becoming the roads and bridges that we built the emerging internet out of.

GUO: In the mid-2000s, Sam worked for one of the biggest software companies in the world - Microsoft.

FOUNTAIN: Here's where we mention that both Microsoft and the Gates Foundation are funders of NPR.

GUO: And Microsoft wanted this emerging internet to be built on top of Microsoft stuff, Microsoft operating systems, software that Microsoft owned and controlled.

RAMJI: I was in the business development group working in Silicon Valley, trying to get startups to adopt more Microsoft software, which was a hard sell, actually.

FOUNTAIN: Yeah. Because the open-source alternatives, they were becoming popular. Sam started to notice that all the new hot startups, companies like Google and Salesforce, they weren't interested in what he and Microsoft had to offer.

GUO: No. Most of these startups, they were cobbling together something DIY. They were using a free, open-source operating system called Linux and free open-source software that ran on top of Linux. It was open-source on top of open-source on top of open-source.

RAMJI: You had a stack of software, right? The whole stack just made sense together.

FOUNTAIN: And yeah, a lot of the open-source software at the time was kind of janky. There were bugs. There were missing features. But Sam, he noticed that there was also this kind of snowballing effect. The more startups that were building their products on top of that open-source software stack, the better that software became.

RAMJI: This was this huge emerging economic movement of how software was going to get shipped, licensed, distributed, used, and Microsoft was nowhere to be found.

GUO: So Sam writes this kind of cheeky memo to his superiors, tells them, look, Microsoft is not going to win the battle over the internet. It never will. We've already lost. Open source is the future.

RAMJI: If we can't figure out how to work with and use open-source software, we're going to go out of business.

GUO: So your message was, there's no way we're going to beat them - we have to join them?

RAMJI: That's exactly right.

GUO: And so you send it off, and what are you feeling? How do you think they're going to receive it?

RAMJI: Trepidation.

GUO: This memo eventually makes it all the way to Bill Gates. And to Sam's surprise, the higher-ups at Microsoft are like, yeah, you do have a point here. And so they promote him. They put him in charge of open-source strategy at Microsoft. They ask him to help turn around the ship.

FOUNTAIN: And this was a huge deal. Microsoft had kind of pioneered the idea that people should pay for software, and now it was changing its business model - slowly - to embrace open source. Over the next decade, it stops seeing Linux as the enemy, and it starts making sure that Microsoft software works on Linux, even uses Linux on its own servers.

GUO: Also, Microsoft starts giving away some of its own software for free, making it open source. Sam says that's extremely common these days. All the major tech companies do it, like Meta, for example. They started sharing all the tools they use to make interactive websites.

FOUNTAIN: Yeah. And to be clear, these companies aren't giving away all their software. Like, Meta is not giving away the Facebook algorithm. But what they've realized is that it's more valuable for them to share some of their internal software and have the public suggest fixes or build off of it, than it is to keep all of it secret.

GUO: Open source is now the default way to make modern software. Bruce's dream of having this library of open-source building blocks, these free bricks for anyone to use, that dream came true. Those free bricks are now the foundation for most of the software we use today. But there's also a weakness to this open-source model, a weakness that became painfully obvious when the XZ hack went down. That is after the break.

(SOUNDBITE OF DANIEL ALEXIS PEMBERTON'S SONG, "WARPED WORLDS")

GUO: There's this kind of famous cartoon about how the internet works. You might have seen it. It's from the webcomic xkcd. It's this drawing of a giant Jenga tower, all these blocks stacked on top of each other, and the whole thing is balancing on this one tiny, skinny little block.

OMKHAR ARASARATNAM: I know exactly what you're talking about, and it all rests - the entire internet relies on this one guy in Nebraska (laughter).

GUO: Omkhar Arasaratnam is not that one guy in Nebraska, but he thinks a lot about the Jenga tower problem. He's the head of the Open Source Security Foundation.

FOUNTAIN: And he says, yeah, they worry about how fragile this whole internet Jenga tower is. See, open-source software is this huge, decentralized community of people building software on top of other software on top of other software. And that is an incredibly efficient way of making software, but it can also lead to these weak spots.

GUO: Which brings us back to the story of XZ. In this story, the proverbial guy in Nebraska is, well, not in Nebraska. We actually couldn't confirm where he's from. He wouldn't return our emails. But his website's hosted in Finland, so a lot of people think he's Finnish. Anyway, his name is Lasse Collin. He's the main creator of XZ. Omkhar remembers when Lasse first published XZ back in 2009.

ARASARATNAM: It was one of these breakthroughs in compression, right? It was one of these things where, oh, my God, this literally got 2- to 300% increase in compression performance overnight.

FOUNTAIN: And so everyone started using XZ, building programs on top of it. XZ became one of the most widely distributed programs in the entire world.

ARASARATNAM: There's a good chance it's on your phone. There's a good chance that it's on your TV. It's everywhere.

GUO: This is how the Jenga tower problem starts, how the whole world can come to depend on one random person.

FOUNTAIN: Omkhar says this is pretty common, that there are a lot of critical software projects that rely on just one person. And the big problem with this is that it is an ongoing job. Software isn't just a thing you write once and that's that. You've got to maintain it.

ARASARATNAM: Computers change, operating systems change. New processors are released. New kinds of computers come out. And thus we have to keep our software up to date, or it rots.

GUO: And someone needs to oversee all of these small little updates. It's not the most glamorous work. Most open-source volunteers want to be contributing to new projects, not looking after old ones. So for many years, the work of maintaining XZ falls to Lasse.

FOUNTAIN: Fast-forward to 2021. This is when the hacker, or hackers, calling themselves Jia Tan come onto the scene. And here's what we know about how their ingenious plot unfolded. This Jia Tan character basically appears out of nowhere and soon starts suggesting some improvements to XZ, which is great. This is how open-source is supposed to work - right? - what makes it so special - strangers on the internet helping each other out. Heartwarming.

GUO: But a few months later, Lasse starts getting these emails from users of XZ. They're complaining that Lasse's been falling behind on maintaining XZ. One of them is kind of nasty, saying how sad it is that Lasse clearly does not care about this project anymore.

ARASARATNAM: Hey, this has been delinquent for a long time. How come nobody's updated this? When are you going to get to it? That kind of thing.

GUO: That's pretty rude. I'm sorry, like...

ARASARATNAM: It is.

GUO: ...This guy's doing it for free.

ARASARATNAM: Well, you know, this is the - I guess this is one of the failure modes of how society has consumed open-source. The overhead of having to deal with this stuff can become overwhelming.

FOUNTAIN: Lasse tells these people, you know, I'm sorry the work is going slow. I'm dealing with some personal stuff right now.

GUO: But his critics are still not satisfied. Someone suggests, why doesn't he just step down and let someone else manage this thing?

FOUNTAIN: And pretty soon, that's what Lasse does. He decides to pass the baton on to that new volunteer, Jia Tan. Now, Jia is going to be the one holding up that Jenga tower instead of Lasse.

GUO: Omkhar says what we know now is that Jia Tan was probably an invented personality. But also, these people harassing Lasse, they, too, seem to be invented personalities, people who were created just to convince Lasse to pass that baton to Jia.

ARASARATNAM: It was literally a social engineering attack, somebody basically running a long con and tricking Lasse into doing things and giving permission that they shouldn't have.

FOUNTAIN: Jia takes over, and over the course of the next few years, Jia starts to make all these little changes to XZ - seemingly innocuous changes that start to turn XZ into a Trojan horse.

GUO: You see, a lot of programs depend on XZ, including a very important program called OpenSSH. It's basically the garage door opener for the internet. It lets you remote-control other computers. Pretty much every web server is running it.

ARASARATNAM: It is literally the thing that controls access to every server on the internet. It is really important.

GUO: This garage door opener program is a really well-guarded piece of software. Everybody has their eye on it.

FOUNTAIN: But what Jia Tan, or what the hacker group behind the identity known as Jia Tan, had figured out was that if they could secretly sabotage XZ, they could sabotage this garage door opener and give themselves access to basically every important computer on the internet.

ARASARATNAM: This was incredibly well-orchestrated. I think somebody should make a movie about this. I mean, I'd definitely watch it. I'd watch it in IMAX.

FOUNTAIN: Earlier this year, Jia starts pressuring the major open-source operating systems to use their new sabotaged version of XZ. That's when they sent emails to people like Richard from the top, and the compromised XZ starts slowly spreading across the internet.

GUO: Now, the way this hack was eventually discovered is kind of by accident. It was discovered by this programmer at Microsoft named Andres Freund, who worked on open-source software, actually. A couple of months ago, Andres noted that the garage door opener software was acting kind of slow.

ARASARATNAM: And he started picking it apart. And he pulled that thread, and he eventually unpacked all the stuff we know now.

FOUNTAIN: Andres sends out an email about this. He's like, hey, guys, I think one of the most important pieces of software in the world has been compromised. And also, I'm pretty sure this is exactly how they did it.

GUO: When Omkhar sees this email, he almost falls out of his chair.

ARASARATNAM: My first reaction was, oh, my God, how many people have downloaded this? (Laughter).

FOUNTAIN: Luckily, the sabotaged XZ was caught before it got widespread distribution. It mostly only got onto computers running experimental, or beta, software.

GUO: Can you run me through, like, what the nightmare scenario would have been if Andres hadn't caught this?

ARASARATNAM: Nightmare scenario is it gets broad distribution. Whoever Jia Tan is quietly logs into computers all over the internet stealing money, your personal information. I mean, anything - stealing your email. It could have been anything.

FOUNTAIN: Omkhar says it was a pretty shockingly close call. And it has started to make people reconsider the entire economic model of open-source.

GUO: The open-source movement succeeded beyond anybody's wildest dreams. It started with these programmers who were writing code in their free time 'cause they thought it was fun or they wanted to make something cool, or they wanted to make the world a better place. But over the last three decades, all those volunteers have built this efficient, decentralized, maybe even beautiful, system of writing software, software that became the foundation for the internet.

FOUNTAIN: Yeah. But out of this efficient and decentralized and beautiful system, you also get the Jenga tower problem where one person can write a program that's so good, it changes the world, and it leads to the whole world depending on that one person.

GUO: Omkhar says the solution is not that open-source software goes away. But we have to reconsider how we treat the open-source software community. He says open-source has become this incredibly valuable public good. It's become, like, the pipes and sewers of the internet. And like any public good, there aren't really strong incentives for people to help maintain them.

ARASARATNAM: Open-source folks are all incentivized to work on the new shiny thing - right? - to build skyscrapers. In the meantime, the less-interesting projects that we're all relying on, the proverbial sewer pipes, nobody's taking care of them. And when the sewage backs up, we're all in trouble.

GUO: How many vulnerable programs like XZ are there? Omkhar says there could be a lot. He and his colleagues are working on this giant census to try and identify all the single little Jenga blocks holding up the internet. He says they expect to have new results later this year.

(SOUNDBITE OF DANIEL ALEXIS PEMBERTON'S SONG, "DETECTIVE DAN")

FOUNTAIN: On our next episode - layoffs. They happen all the time. They're a business reality. But of course, they can be really destabilizing.

UNIDENTIFIED PERSON #1: Honestly, I felt like I was being swallowed by a sinking hole.

FOUNTAIN: Like, when this person lost his job, he and his husband had a lot of questions, especially for the HR rep who handled the layoff.

UNIDENTIFIED PERSON #1: Like, do you get training on how to be human in these conversations?

FOUNTAIN: Those questions and more on our next episode.

GUO: This episode was produced by Emma Peaslee and engineered by Cena Loffredo. It was edited by Jess Jiang and fact-checked by Sierra Juarez. Alex Goldmark is our executive producer. I'm Jeff Guo.

FOUNTAIN: And I'm Nick Fountain. This is NPR. Thank you for listening.

Copyright © 2024 NPR. All rights reserved. Visit our website terms of use and permissions pages at www.npr.org for further information.

NPR transcripts are created on a rush deadline by an NPR contractor. This text may not be in its final form and may be updated or revised in the future. Accuracy and availability may vary. The authoritative record of NPR’s programming is the audio record.

----

**(Adam Davidson):**

**(Laura Conaway):**


**faster whisper:**
What does it sound like to record an album inside a jail?
On the documentary podcast, Track Change,
you'll hear four men make music inside Richmond City Jail,
and hear how they're trying to break free from a cycle of addiction and incarceration.
Been so long since I've been free
Listen to Track Change from Narratively and VPM, part of the NPR network.
This is Planet Money from NPR.
Now that Richard Jones knows how close the entire world came to disaster,
he's been looking back for any hints, any clues that he might have missed.
For him, the first clue was this message that showed up in his inbox on February 26th.
So I remember I got this email, and it was not anything unusual.
Richard is a senior engineer at Red Hat.
He helps make an operating system that is used all over the world.
We're talking Fortune 500 companies, major hospital systems, banks, even the U.S. military.
And what's interesting about that operating system is that it is completely open source,
meaning it's made out of all these different pieces of software that people are putting out for free.
So Richard is often emailing with strangers on the Internet.
I don't know who half the people I talk to on the Internet about software are.
I don't know who they are in real life. I've never met any of them.
Instead, we work on reputation.
And that email he had gotten, it was from a guy who was new-ish on the scene,
but who had built up a pretty solid reputation, a guy named Jia Tan.
For about a year, Jia had been the volunteer in charge of this very popular software program called XZ, which helps compress data.
It's not the fastest, but it is the one that compresses the most. It's very useful for us.
Look, I don't think I'm exaggerating when I say that compression is key for everything,
for storing files, for sending stuff over the Internet, everything.
In the email, Jia sounds pretty enthusiastic, but in a way that a lot of open source volunteers sound enthusiastic.
He says, hey, I just made this cool update to XZ. Hope you guys can put it into your operating system.
And this email, I will say, it looks very innocent. It's written in this chipper tone. It's got smiley emojis.
It has exclamation points, which just signals, you know, no threat here.
And so Richard goes ahead. He puts the new updated XZ code into a preliminary version of their operating system to test out.
But pretty soon he starts getting these bug reports. They were quite strange, but not totally unusual.
This new version of XZ, it seemed to be messing with other parts of the computer, like critical parts of the memory.
But, you know, bugs happen in software, right? In software, it's full of bugs.
So Richard emailed Jia and asked him to, you know, take a look at the problem.
He came back within two or three days and said, I'm really sorry, we've just released a new version which fixes this bug for you.
So could you upgrade to that?
Which Richard does, and everything seems fine, until about a month ago.
That is when someone discovers that this new version of XZ, it is not what it seems to be.
And Jia Tan is not who he seems to be.
I was surprised, I was a bit shocked, I was angry. I just didn't expect that somebody would try that.
What we now know is that Jia Tan was a hacker, or probably a group of hackers.
And they were trying to pull off one of the most audacious cyber security attacks in history.
Over the course of two years, these hackers had infiltrated one of the most popular programs out there, XZ.
And if they hadn't been caught, they would have had a secret backdoor to some of the most important computers in the world.
Hello and welcome to Planet Money, I'm Jeff Guo.
And I'm Nick Fountain.
If you peek under the hood of the internet, what you'll find is that most of the computers powering it are running free open source software.
But here's a dirty secret.
A lot of that software is written by small teams, sometimes teams of only one person.
Which makes them pretty vulnerable and easy to infiltrate.
Today on the show, the story of the XZ hack.
How it took advantage of the strange way we make modern software.
What it tells us about the economics of one of the most important industries in the world.
You care about what's happening in the world.
Let State of the World from NPR keep you informed.
Each day we transport you to a different point on the globe and introduce you to the people living world events.
We don't just tell you world news, we take you there.
And you can make this journey while you're doing the dishes or driving your car.
State of the World podcast from NPR.
Vital international stories every day.
You care about what's happening in the world.
Let State of the World from NPR keep you informed.
Each day we transport you to a different point on the globe and introduce you to the people living world events.
We don't just tell you world news, we take you there.
And you can make this journey while you're doing the dishes or driving your car.
State of the World podcast from NPR.
Vital international stories every day.
The hack that we're talking about today, the XZ hack, could not have happened if it weren't for the weird way that most modern software is made.
We have these trillion dollar corporations working side by side with unpaid, sometimes even anonymous volunteers to write the software that powers the internet.
Right. And so before we can get into how the XZ hack went down, we're first going to have to understand how modern software got to be this way.
For that, we went to one of the founders of the open source software movement, Bruce Perrins.
Back when I was starting this, you would have asked what drugs I was using and where you could get some.
Bruce says for him, it all started with this epiphany he had about how to write software efficiently.
At the time, it was the 1980s and he was a young programmer at Pixar.
He wrote software that helped make movies like Toy Story 2.
I'm a bigger fan of four, but whatever.
Bruce would keep running into this annoying problem.
His programs, they would glitch out and they would accidentally overwrite other parts of the computer.
Yeah. And you know, these bugs, they would happen all the time back then.
It was like the Wild West of software.
So Bruce's solution was to write up a piece of software that would monitor other programs and it would alert him whenever a program started to overwrite stuff that it shouldn't be writing over.
It would stop your program in the instant that happened and let you see the exact instruction that you had wrong.
And I called this electric fence because when you touch the fence, it would zap you.
Bruce says electric fence proved to be pretty handy, so he shared it with his colleagues at Pixar.
But then he thought maybe other people would find it useful too.
And at the time, there were these online bulletin boards where programmers would hang out.
And Bruce was a regular. He says this community had a culture of sharing.
Programmers from different companies would show each other new ways of doing things, even provide code for others to copy.
So all of the engineers, software engineers at the time, started sharing software together and we started using it in our work.
And no one in management or legal knew that was happening.
Bruce went ahead and he posted the code for electric fence onto that bulletin board.
And electric fence became incredibly popular. All of a sudden, people around the world started using it.
Someone wrote to me and said, Your electric fence program has just saved my job. If you ever go to Ireland, please stay in my home.
My gosh, did you go?
No, no, I never met this guy, but you know, I was getting fans.
That felt pretty good. But then something even more gratifying started to happen.
Some of Bruce's fans, some of these programmers he'd never met, they made their own improvements to electric fence.
And they shared these improvements with Bruce. They sent him their tweaks and upgrades to his code.
And I thought, you know, whatever work I've put into this, I just got back.
And it kept happening.
This experience helped Bruce realize two things. First, it illustrated an unexpected benefit of giving away your code.
Because not only could your code help other people, these total strangers, but now those strangers could help make your code better.
And second, Bruce realized that if they all worked together this way, they could write software so much faster and better.
Yeah, Bruce says a lot of programmers in their day to day jobs would spend hours doing essentially the same thing as their counterparts at other tech companies, writing the same basic code to solve the same basic problems.
So back then, it would be like building a house and you'd have to dig up this clay and fire all the bricks.
And open source was the idea was we would all chip in on making all the different bricks and we would give them to each other for free.
And now you are not wasting your time on the bricks. You're building the architecture.
This is where Bruce saw the beginnings of a powerful idea.
Because there's already this culture of sharing software in order to be a good citizen or to promote a free society or whatever.
But Bruce saw that this could also transform the whole economic model for making software.
Bruce believed that if people could get together to produce software in an open and crowd sourced way, you could outcompete even the mightiest corporations.
Now, Bruce wasn't the only one who realized this.
By the 1990s, a lot of programmers were attracted to this open source model, but they weren't taken too seriously.
But the open source movement would soon have an opportunity to prove itself.
Yeah, you see, by the late 90s, the Internet was really starting to take off.
Remember, this was the era when there were so many AOL online CDs floating around. People were using them as coasters.
And the big question at that time was what software would this new Internet run on?
And a person who would play a pivotal role in the war over the Internet was Sam Ramsey.
Software was becoming infrastructure. It was becoming the roads and bridges that we built the emerging Internet out of.
In the mid 2000s, Sam worked for one of the biggest software companies in the world, Microsoft.
Here's where we mentioned that both Microsoft and the Gates Foundation are funders of NPR.
And Microsoft wanted this emerging Internet to be built on top of Microsoft stuff, Microsoft operating systems, software that Microsoft owned and controlled.
I was in the business development group working in Silicon Valley trying to get startups to adopt more Microsoft software, which was a hard sell, actually.
Yeah, because the open source alternatives, they were becoming popular.
Sam started to notice that all the new hot startups, companies like Google and Salesforce, they weren't interested in what he and Microsoft had to offer.
No, most of these startups, they were cobbling together something DIY.
They were using a free open source operating system called Linux and free open source software that ran on top of Linux.
It was open source on top of open source on top of open source.
You had a stack of software, right? The whole stack just made sense together.
And yeah, a lot of the open source software at the time was kind of janky.
There were bugs that were missing features.
But Sam, he noticed that there was also this kind of snowballing effect.
The more startups that were building their products on top of that open source software stack, the better that software became.
This was this huge emerging economic movement of how software was going to get shipped, licensed, distributed, used, and Microsoft was nowhere to be found.
So Sam writes this kind of cheeky memo to his superiors, tells him, look, Microsoft is not going to win the battle over the Internet.
It never will. We've already lost. Open source is the future.
If we can't figure out how to work with and use open source software, we're going to go out of business.
So your message was there's no way we're going to beat them. We have to join them.
That's exactly right.
And so you send it off. And what are you feeling? How do you think they're going to receive it?
Chepidation.
This memo eventually makes it all the way to Bill Gates.
And to Sam's surprise, the higher ups at Microsoft are like, yeah, you you do have a point here.
And so they promote him. They put him in charge of open source strategy at Microsoft.
They ask him to help turn around the ship.
And this was a huge deal.
Microsoft had kind of pioneered the idea that people should pay for software.
And now it was changing its business model slowly to embrace open source.
Over the next decade, it stopped seeing Linux as the enemy.
And it starts making sure that Microsoft software works on Linux, even uses Linux on its own servers.
Also, Microsoft starts giving away some of its own software for free, making it open source.
Sam says that's extremely common these days.
All the major tech companies do it, like Metta, for example.
They started sharing all the tools they use to make interactive websites.
Yeah. And to be clear, these companies aren't giving away all their software.
Like Metta is not giving away the Facebook algorithm.
But what they've realized is that it's more valuable for them to share some of their internal software
and have the public suggest fixes or build off of it than it is to keep all of it secret.
Open source is now the default way to make modern software.
Bruce's dream of having this library of open source building blocks, these free bricks for anyone to use.
That dream came true.
Those free bricks are now the foundation for most of the software we use today.
But there's also a weakness to this open source model,
a weakness that became painfully obvious when the XZ hack went down.
That is after the break.
Every weekday, NPR's best political reporters come to you on the NPR Politics Podcast
to explain the big news coming out of Washington, the campaign trail, and beyond.
We don't just want to tell you what happened, we tell you why it matters.
Join the NPR Politics Podcast every single afternoon to understand the world through political eyes.
Numbers that explain the economy. We love them at the indicator from Planet Money.
And on Fridays, we discuss indicators in the news, like job numbers, spending, the cost of food, sometimes all three.
So my indicator is about why you might need to bring home more bacon to afford your eggs.
I'll be here all week.
Wrap up your week and listen to the indicator podcast from NPR.
The Bullseye Podcast is, according to one journalist, the, quote,
kind of show people listen to in a more perfect world.
So make your world more perfect.
Every week, Bullseye puts the pop in culture, interviewing brilliant authors, musicians, actors, and novelists
to keep you on your pop culture target.
Listen to the Bullseye Podcast, only from NPR and Maximum Fun.
Truth, independence, fairness, transparency, respect, excellence.
This is NPR.
Darian Woods here.
As the U.S. federal debt grows, so too does the interest on it.
And this year, it hit a milestone.
Interest payments this year will actually be larger than national defense spending for the first time.
And that's not a small number.
That is one of the largest items in the entire federal budget.
That's from our latest bonus episode.
It's my conversation with a longtime debt hawk about the potential risks to the economy and when spending makes sense.
You can check that out now if you're a Planet Money Plus listener.
If that's you, thanks for your support.
If it's not, it could be.
You get bonus content, sponsor-free listening, and support the work of Planet Money.
Go to plus.npr.org.
There's this kind of famous cartoon about how the Internet works.
You might have seen it.
It's from the webcomic XKCD.
It's this drawing of a giant Jenga tower, all these blocks stacked on top of each other,
and the whole thing is balancing on this one tiny skinny little block.
I know exactly what you're talking about.
And it all rests, the entire Internet relies on this one guy in Nebraska.
Omkar Arasaratnam is not that one guy in Nebraska,
but he thinks a lot about the Jenga tower problem.
He's the head of the Open Source Security Foundation.
And he says, yeah, they worry about how fragile this whole Internet Jenga tower is.
See, Open Source software is this huge decentralized community
of people building software on top of other software on top of other software.
And that is an incredibly efficient way of making software,
but it can also lead to these weak spots.
Which brings us back to the story of XZ.
In this story, the proverbial guy in Nebraska is, well, not in Nebraska.
We actually couldn't confirm where he's from.
He wouldn't return our emails, but his website's hosted in Finland,
so a lot of people think he's Finnish.
Anyway, his name is Lasse Kotlin.
He's the main creator of XZ.
Omkar remembers when Lasse first published XZ back in 2009.
It was one of these breakthroughs in compression, right?
It was one of these things where, oh, my God,
this literally got two to 300% increase in compression performance overnight.
And so everyone started using XZ, building programs on top of it.
XZ became one of the most widely distributed programs in the entire world.
There's a good chance it's on your phone.
There's a good chance that it's on your TV.
It's everywhere.
This, this is how the Jenga tower problem starts,
how the whole world can come to depend on one random person.
Omkar says this is pretty common,
that there are a lot of critical software projects that rely on just one person.
And the big problem with this is that it is an ongoing job.
Software isn't just a thing you write once, and that's that.
You got to maintain it.
Computers change. Operating systems change.
New processors are released.
New kinds of computers come out,
and thus we have to keep our software up to date or it rots.
And someone needs to oversee all of these small little updates.
It's not the most glamorous work.
Most open source volunteers want to be contributing to new projects,
not looking after old ones.
So for many years, the work of maintaining XZ falls to laissez.
Fast forward to 2021.
This is when the hacker or hackers calling themselves Gia Tan come on to the scene.
And here's what we know about how their ingenious plot unfolded.
This Gia Tan character basically appears out of nowhere
and soon starts suggesting some improvements to XZ, which is great.
This is how open source is supposed to work, right?
What makes it so special?
Strangers on the internet helping each other out.
Heartwarming.
But a few months later, laissez starts getting these emails from users of XZ.
They're complaining that laissez has been falling behind on maintaining XZ.
One of them is kind of nasty.
It's saying how sad it is that laissez clearly does not care about this project anymore.
Hey, this has been delinquent for a long time.
How come nobody's updated this?
When are you going to get to with that kind of thing?
That's pretty rude. I'm sorry.
Like this guy's doing it for free.
Well, you know, this is the, I guess this is one of the failure modes
of how society has consumed open source.
The overhead of having to deal with this stuff can become overwhelming.
Lassez tells these people, you know, I'm sorry, the work is going slow.
I'm dealing with some personal stuff right now.
But his critics are still not satisfied.
Someone suggests, why doesn't he just step down and let someone else manage this thing?
And pretty soon that's what laissez does.
He decides to pass the baton on to that new volunteer, Gia Tan.
Now Gia is going to be the one holding up that Jenga tower instead of laissez.
Amkar says what we know now is that Gia Tan is probably an invented personality.
But also these people harassing laissez, they too seem to be invented personalities.
People who were created just to convince laissez to pass that baton to Gia.
It was literally a social engineering attack.
Somebody basically running a long con and tricking laissez into doing things
and giving permission that they shouldn't have.
Gia takes over and over the course of the next few years,
Gia starts to make all these little changes to XZ.
Seemingly innocuous changes that start to turn XZ into a Trojan horse.
You see, a lot of programs depend on XZ, including a very important program called Open SSH.
It's basically the garage door opener for the internet.
It lets you remote control other computers.
Pretty much every web server is running it.
It is literally the thing that controls access to every server on the internet.
It is really important.
This garage door opener program is a really well guarded piece of software.
Everybody has their eye on it.
But what Gia Tan, or what the hacker group behind the identity known as Gia Tan,
had figured out was that if they could secretly sabotage XZ,
they could sabotage this garage door opener
and give themselves access to basically every important computer on the internet.
This was incredibly well orchestrated.
I think somebody should make a movie about this.
I mean, I'd definitely watch it. I'd watch it in IMAX.
Earlier this year, Gia starts pressuring the major open source operating systems
to use their new sabotaged version of XZ.
That's when they send emails to people like Richard from the top,
and the compromised XZ starts slowly spreading across the internet.
Now, the way this hack was eventually discovered is kind of by accident.
It was discovered by this programmer at Microsoft named Andreas Freund,
who works on open source software, actually.
A couple months ago, Andreas noted that the garage door opener software was acting kind of slow.
And he started picking it apart, and he pulled that thread,
and he eventually unpacked all the stuff we know now.
Andreas sends out an email about this.
He's like, hey, guys, I think one of the most important pieces of software in the world has been compromised.
And also, I'm pretty sure this is exactly how they did it.
When Omkar sees this email, he almost falls out of his chair.
My first reaction was, oh, my God, how many people have downloaded this?
Luckily, the sabotaged XZ was caught before it got widespread distribution
and mostly only got onto computers running experimental or beta software.
Can you run me through what the nightmare scenario would have been if Andreas hadn't caught this?
Nightmare scenario is it gets broad distribution.
Whoever Geotan is quietly logs into computers all over the Internet,
stealing money, your personal information.
I mean, anything, stealing your email.
It could have been anything.
Omkar says it was a pretty shockingly close call.
And it has started to make people reconsider the entire economic model of open source.
The open source movement succeeded beyond anybody's wildest dreams.
It started with these programmers who were writing code in their free time
because they thought it was fun or they wanted to make something cool
or they wanted to make the world a better place.
But over the last three decades, all those volunteers have built this efficient, decentralized,
maybe even beautiful system of writing software, software that became the foundation for the Internet.
Yeah, but out of this efficient and decentralized and beautiful system,
you also get the Jenga Tower problem
where one person can write a program that's so good it changes the world
and it leads to the whole world depending on that one person.
Omkar says the solution is not that open source software goes away,
but we have to reconsider how we treat the open source software community.
He says open source has become this incredibly valuable public good.
It's become like the pipes and sewers of the Internet.
And like any public good, there aren't really strong incentives for people to help maintain them.
Open source folks are all incentivized to work on the new shiny thing, right?
To build skyscrapers.
In the meantime, the less interesting projects that we're all relying on,
the proverbial sewer pipes, nobody's taking care of them.
And when the sewage backs up, we're all in trouble.
How many vulnerable programs like XZ are there?
Omkar says there could be a lot.
He and his colleagues are working on this giant census
to try and identify all the single little Jenga blocks holding up the Internet.
He says they expect to have new results later this year.
On our next episode, layoffs.
They happen all the time.
They're a business reality.
But of course, they can be really destabilizing.
Honestly, I felt like I was being swallowed by a sinking hole.
Like when this person lost his job, he and his husband had a lot of questions,
especially for the HR rep who handled the layoff.
Like, do you get training on how to be human in these conversations?
Those questions and more on our next episode.
This episode was produced by Emma Peasley and engineered by Sina Lafreda.
It was edited by Jess Jang and fact-checked by Sierra Juarez.
Alex Goldmark is our executive producer.
I'm Jeff Guo.
And I'm Nick Fountain.
This is NPR.
Thank you for listening.
NPR brings you the updates you need on the day's biggest headlines.
The Senate narrowly passed a debt ceiling bill that will prevent the country from defaulting on its loans.
Stories from across the world.
Knowing how to forage and to live with the land is integral to Ami's culture.
And down your block.
From CPR News, this is Colorado Matters.
And you can find all of that and more in your pocket.
Download the NPR app today.
And a special thanks to our funder, the Alfred P. Sloan Foundation, for helping to support this podcast.
Hey, it's Ayesha Roscoe from NPR's Up First podcast.
I'm one of thousands of NPR Network voices coming to you from over 200 local newsrooms across the country.
We bring all Americans closer together through free and independent journalism, music, politics, culture, and so much more.
The NPR Network.
What you hear changes everything.
Learn more at npr.org slash network.
