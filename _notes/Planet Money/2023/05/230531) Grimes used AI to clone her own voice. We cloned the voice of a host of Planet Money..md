---
title: 230531) Grimes used AI to clone her own voice. We cloned the voice of a host of Planet Money.
date: 20230531
tags: #PlanetMoney
citation: "“Planet Money,” _NPR_, 2 Juni 2023. [https://www.npr.org/podcasts/510289/planet-money](https://www.npr.org/podcasts/510289/planet-money) (diakses 4 Juni 2023)."
---

In Part 1 of this series, AI proved that it could use real research and real interviews to write an original script for an episode of Planet Money.

In Part 1 of this series, AI proved that it could use real research and real interviews to write an original script for an episode of Planet Money.

Our next task was to teach the computer how to sound like us. How to read that script aloud like a Planet Money host.

On today's show, we explore the world of AI-generated voices, which have become so lifelike in recent years that they can credibly imitate specific people. To test the limits of the technology, we attempt to create our own synthetic voice by training a computer on recordings of former Planet Money host Robert Smith. Then we introduce synthetic Robert to his very human namesake.

There are a lot of ethical, and economic, questions raised by a technology that can duplicate anyone's voice. To help us make sense of it all, we seek the advice of an artist who has embraced AI voice clones: the musician Grimes.

(This is part two of a three-part series. For part one of our series, click here)
Can ChatGPT write a podcast episode? Can AI take our jobs?
Planet Money
Can ChatGPT write a podcast episode? Can AI take our jobs?

This episode was produced by Emma Peaslee and Willa Rubin, with help from Sam Yellowhorse Kesler. It was edited by Keith Romer and fact-checked by Sierra Juarez. Engineering by James Willetts. Jess Jiang is our acting executive producer.

We built a Planet Money AI chat bot. Help us test it out: Planetmoneybot.com.

Help support Planet Money and get bonus episodes by subscribing to Planet Money+ in Apple Podcasts or at plus.npr.org/planetmoney.

Always free at these links: Apple Podcasts, Spotify, Google Podcasts, NPR One or anywhere you get podcasts.

Find more Planet Money: Facebook / Instagram / TikTok / Our weekly Newsletter.

Music: "Hi-Tech Expert," "Lemons and Limes," and "Synergy in Numbers." 

----

https://www.npr.org/2023/05/25/1178290772/ai-chatgpt-artificial-intelligence-series-part-two

https://www.npr.org/transcripts/1178290772



KENNY MALONE, HOST:

Just a heads-up - this is episode 2 of a three-part series exploring whether artificial intelligence can make a PLANET MONEY episode. Today's episode does make passing mention of a couple of technologies from Apple and Google. You should know that both of those companies are financial supporters of National Public Radio. Here is today's show.

SYLVIE DOUGLIS, BYLINE: This is PLANET MONEY from NPR.

(SOUNDBITE OF COIN SPINNING)

JEFF GUO, HOST:

Here at PLANET MONEY, we have been testing these new artificial intelligence technologies to see how much of our jobs they can actually do. Last episode, we used tools like ChatGPT in some moderately complicated ways to write an entire PLANET MONEY episode.

MALONE: And that episode is finished. We have a script. We are excited for you to hear that podcast. But if we are really going to take seriously the question of - is the AI going to replace us? - we wanted to go all the way. We needed the computers to also replace our voice to narrate this episode.

GUO: And if we were going to have the computer do the talking, we might as well go big - get the most PLANET MONEY-y (ph) voice of all the PLANET MONEY voices. I speak, of course, of...

(SOUNDBITE OF ARCHIVED NPR BROADCAST)

ROBERT SMITH, BYLINE: Hello, and welcome to PLANET MONEY. I'm Robert Smith.

MALONE: Robert Smith - PLANET MONEY's longest-running host - even was the show's editor for a while. But a couple years ago, he finally hung up the old microphone and left the show as a full-time host.

GUO: Robert left behind a legacy, but also lots and lots and lots of recordings of his voice.

(SOUNDBITE OF ARCHIVED NPR BROADCASTS)

SMITH: Hello, I'm minor podcast celebrity Robert Smith. And here at PLANET MONEY...

In order to save the country, they're going to have to work together to restructure the tax code.

Who is this poop cartel that you speak of?

Ahoy there. Welcome aboard the good ship Inflation.

GUO: And just for fun, we did try to hack together our own version of a knockoff Robert Smith using those old recordings. So we were just, you know, cutting and pasting those words together.

MALONE: Yeah, we even gave him a little catchphrase. And here - here, why don't - give it a listen.

(SOUNDBITE OF ARCHIVED NPR BROADCASTS)

SMITH: I'm...

...knockoff...

...Robert...

...and...

...I'm...

...not...

...here...

...to...

...make...

...friends.

I'm here...

...to...

...make...

...history.

MALONE: Uh - yeah, kind of hard to understand there. He's saying, I'm knockoff Robert. I'm not here to make friends. I'm here to make history.

(SOUNDBITE OF ARCHIVED NPR BROADCASTS)

SMITH: I'm...

...knockoff...

...Robert...

...and...

...I'm...

...not...

...here...

...to...

...make...

...friends.

I'm here...

...to...

...make...

...history.

GUO: Yeah, OK. It's not very good. And clearly, there are better ways to do that now because part of the AI boom has been the introduction of these surprisingly realistic AI voices.

MALONE: Yeah, somebody made a completely synthesized conversation between podcast host Joe Rogan and Steve Jobs, who is dead.

(SOUNDBITE OF ARCHIVED RECORDING)

AI-GENERATED VOICE #1: (As Joe Rogan) How's it going? Come on, tell me about it, Jobs.

AI-GENERATED VOICE #2: (As Steve Jobs) Yeah, it's great to be on the show. Your audience is just so different from your normal Apple users, and that's a good thing.

MALONE: And then there was a song featuring an AI-generated version of Drake and The Weeknd.

(SOUNDBITE OF SONG, "HEART ON MY SLEEVE")

AI-GENERATED VOICE #3: (As Drake, rapping) I came in with my ex, like Selena, to flex - hey - bumping Justin...

MALONE: So yeah, AI Drake, AI Joe Rogan - like, clearly, this is possible now. So today's mission - go and somehow build the PLANET MONEY version of this...

(SOUNDBITE OF ANTON SYCH, SEBASTIAN BARNABY ROBERTSON AND VITALII ZINCHENKO'S "HI-TECH EXPERT")

MALONE: ...AI Robert Smith.

(SOUNDBITE OF ANTON SYCH, SEBASTIAN BARNABY ROBERTSON AND VITALII ZINCHENKO'S "HI-TECH EXPERT")

MALONE: Hello and welcome to PLANET MONEY. I'm Kenny Malone.

GUO: And I'm Jeff Guo. And today, the next step in our quest to try and automate our jobs at PLANET MONEY - can a computer believably serve as the voice of Planet Money?

MALONE: There has clearly been some enormous leap in making computer voices. So what happened, exactly? How did we go from, like, bad GPS voice - (imitating GPS voice) in half a mile, turn left - to that incredible Drake thing?

GUO: We will build and introduce you to a fully synthetic Robert Smith, and we'll also check in on another synthetic voice clone of an even more famous celebrity - Grimes.

(SOUNDBITE OF ARCHIVED NPR BROADCASTS)

SMITH: Wait, wait.

Who is...

...Grimes?

MALONE: Oh, sorry, knockoff Robert. Grimes is, like, a musician/cyborg/like, demigod. It's complicated. Ask your kids or whatever.

(SOUNDBITE OF ARCHIVED NPR BROADCASTS)

SMITH: OK.

Stay...

...with...

...us.

(SOUNDBITE OF ANTON SYCH, SEBASTIAN BARNABY ROBERTSON AND VITALII ZINCHENKO'S "HI-TECH EXPERT")

MALONE: Hello.

MARTIN RAMIREZ: Hello, this is Martin.

MATT HOCKING: And Matt Hocking.

RAMIREZ: Thank you for having us.

GUO: This is Martin Ramirez and Matt Hocking. They're from a company called WellSaid Labs. It's a Seattle tech startup that makes what they call voice avatars.

MALONE: OK. So we are interested in taking our beloved Robert Smith and somehow making a version of him that we can still have in our wonderful episodes occasionally. Is that something that you guys can do?

RAMIREZ: As long as Robert is in, WellSaid will be well-equipped to create a synthetic replica, if you will, of Robert's voice.

MALONE: Synthetic Robert.

(LAUGHTER)

MALONE: Love it.

GUO: Synthetic Robert - an upgrade from knockoff Robert. Now, Matt and Martin give us a quick little history of people trying to get computers to talk like people.

HOCKING: I think when we originally started down this path, text-to-speech had primarily been very robotic, very monotone, and had been produced in a concatenative way.

MALONE: Wait - what is the word you're saying?

HOCKING: Concatenative.

GUO: Concatenative - in this case, it means taping together a bunch of prerecorded bits of voice. So think about the way that we built that funny knockoff Robert earlier.

(SOUNDBITE OF ARCHIVED NPR BROADCASTS)

SMITH: I'm...

...knockoff...

...Robert...

...and...

...I'm...

...not...

...here...

...to...

...make...

...friends.

I'm here...

...to...

...make...

...history.

MALONE: Yeah. Well, that is a bad version of how synthetic voices used to get made, according to Matt and Martin.

GUO: A much better version is the original Siri voice. That was recorded back in 2005. And that voice actor said that they made her go into a studio, and she had to read these weird phrases, like, cow hoist in the tug hut today...

MALONE: (Laughter).

GUO: ...or say shift fresh issue today.

MALONE: Well done, Jeff. Well done.

GUO: (Laughter).

MALONE: Now, the reason she had to say those weird things - for, like, 80 hours, by the way - was so that, in the end, Apple could chop up all the recordings and have, like, a drawer filled with every possible sound in the English language.

GUO: So Siri can say any word by reassembling those little sound elements. So that is the old way. The way that Matt and Martin were going to build synthetic Robert was apparently way different.

MALONE: We're not going to build a drawer of Robert making all of these sounds.

RAMIREZ: Yeah, he's not chained to a microphone, saying millions and hundreds of millions of permutations of his scripts.

MALONE: (Laughter) Yeah, as far as I know, he's, like, cross-country skiing right now.

HOCKING: And that, there, is what we inevitably have created - is the ability for Robert to be off cross-country skiing.

MALONE: Because the modern voice approach by WellSaid and an increasing number of other competitors in this space is quite different from the old thing. For example, if we're going to go ahead and do this Robert thing, Martin and Matt explained that we're going to send over some recordings made by Robert Smith during his time at PLANET MONEY, and then we'll also send over the exact transcripts for those recordings.

GUO: And then, essentially, what's going to happen is that a computer is going to look at a chunk of that written transcript, and it's going to try to guess how Robert might say those words.

HOCKING: So whether that be the pitch, the pausing, the intonation, the emphasis - all of those types of things have certain...

MALONE: Whoa.

HOCKING: ...Metrics which are measured.

RAMIREZ: And I love the perspective of - let's be wrong multiple times as quickly as possible. And it's going to sound sort of, kind of, but maybe not really Robert.

MALONE: Wrongbert (ph).

RAMIREZ: Wrongbert.

MALONE: (Laughter).

RAMIREZ: Yes. There you go.

MALONE: And this synthetic voice is going to be Wrongbert for a long time. Martin says it's going to take millions of training cycles. But, in the end, we should end up with a computer program that can look at any sentence and do a really good job guessing how Robert Smith would say that sentence.

GUO: And by the way, if it took 80 hours of recordings to make Siri using that old, concatenative approach, this new approach - it requires way less audio.

HOCKING: We've kind of come to around 45 minutes to a couple of hours' worth of audio to get to a point where we can create a very realistic likeness to someone's voice.

MALONE: A full voice clone from so little audio - and, you know, to be clear, it's not just WellSaid here. Like, this technology is spreading really fast.

GUO: Yeah, there are lots of companies with their own versions of this voice cloning stuff. Google has one. There's another company called ElevenLabs. Apple says it's about to get in the game.

MALONE: Yeah. Plus, there are open-source voice cloning tools without, like, any real restrictions or oversights, and anyone can use them. And, of course, when you start to consider the implications of all of this, it is really terrifying in some very obvious ways. I mean, imagine how bad it would be if there were a synthetic Joe Biden voice announcing nuclear war or something, right?

GUO: Yeah. So companies like WellSaid - they are well aware of these fears. And so WellSaid explained to us that, if we were going to work with them for this project, there were going to be lots of terms and conditions.

MALONE: For starters, Matt and Martin told us that they wouldn't even consider making a synthetic Robert Smith until they had heard from the real, organic Robert Smith and had his permission.

GUO: They also told us that they will be able to monitor every word we make synthetic Robert say.

HOCKING: As soon as anything looks like it's not in line with our values, we're very quick to put an end to that.

GUO: And maybe the biggest term and condition of all - as soon as we were done with this project, synthetic Robert would be shut down. He could narrate our AI-generated episode, and then he will be functionally destroyed, never to be used again.

MALONE: Poor synthetic Robert. But we agreed to all these terms. We got Robert Smith's permission. We went into the old NPR PLANET MONEY archives, and we pulled a lot of Robert Smith recordings.

(SOUNDBITE OF ARCHIVED NPR BROADCASTS)

SMITH: And I'm Robert Smith.

And I'm Robert Smith.

And I'm Robert Smith.

And I'm Robert Smith.

And I'm Robert Smith.

MALONE: He said other things in these recordings, too. But yes, we sent all of the recordings over to WellSaid, and we waited.

GUO: After the break, synthetic Robert Smith makes his world premiere.

(SOUNDBITE OF RAINMAN'S "LEMONS AND LIMES")

MALONE: While we were waiting for synthetic Robert to train - and I know this isn't how it works, but I'm definitely picturing it like Rocky running up stairs in Philadelphia.

GUO: (Laughter).

MALONE: But, yes - while we were waiting for that to happen, we started to think more and more about some of the other implications for this voice cloning technology - and, you know, not just the, oh no, what happens if someone makes fake Joe Biden, but also what happens economically if, suddenly, voice clones of the thousand most famous people are commercially available?

GUO: Yeah. What does it look like when there's suddenly a synthetic Robert Smith who never gets tired, who can narrate an infinite number of PLANET MONEY episodes?

MALONE: Yeah. Or, like, what happens if - I don't know - Tom Hanks suddenly makes a cheap, cloned version of his voice available for all commercials and all audiobooks and all documentary films.

GUO: And weirdly, we can already get a peek into this bizarro future. It's starting to play out right now with Grimes.

MALONE: Grimes.

GUO: Yeah, the experimental, sci-fi, pop musician from the future.

MALONE: I mean, she is here in the present and is writing music, but she seems like she's from the future. But yes, here is some of her music.

(SOUNDBITE OF SONG, "GENESIS")

GRIMES: (Singing) My heart, I never feel. I never see. I never know.

MALONE: Grimes just has a really distinctive voice - like, whispery and ethereal.

GUO: And in the middle of our AI project, Grimes made this kind of wild announcement on Twitter. She said, basically, hey, from now on, anyone is allowed to copy my voice using AI and, like, put me on their songs - just split the royalties with me if you do. And Grimes even released her own AI voice cloning tool that anybody can use to turn into Grimes.

And so just allow us to show you how this works. It is stupidly easy. So let's say you have a song that you want Grimes AI to sing.

MALONE: Oh, I do. It is a weird version of "Row, Row, Row Your Boat," where every word is off by one note. Yeah? Does that sound...

GUO: I cannot even imagine what that sounds like.

MALONE: Oh, it's weird.

GUO: OK, so you are going to record a version of the song...

MALONE: I will. Here we go.

(Singing) A dream, row, row, row your, boat gently down. The stream, merrily, merrily, merrily, life is like. A dream, row, row - is that enough? Do you have - do you need more?

GUO: No, no, no, no, no. That is plenty.

MALONE: OK.

GUO: That is plenty to work with. So yeah - so I have a recording of you singing that song - that horrifying song.

MALONE: What?

GUO: Literally, all I have to do is - I hit upload. Do you - are you ready to hear yourself as Grimes?

MALONE: Oh, my God - I am so ready.

GUO: OK, we're going to throw a little beat under it so it really sounds like a Grimes song.

(SOUNDBITE OF MUSIC)

GUO: OK. Here we go.

AI-GENERATED VOICE #4: (As Grimes, singing) A dream, row, row, row your, boat gently down. The stream, merrily, merrily, merrily life is like.

MALONE: Oh, my God (laughter). What is going on?

GUO: So using this technology, Grimes is essentially unleashing her voice to go out and make music and earn money on her behalf without her having to be there at all. And so, of course, we had to talk to Grimes about all of this.

AI-GENERATED VOICE #4: (As Grimes, singing) I'm sorry, PLANET MONEY, but I'm unavailable for an interview right now.

GUO: No, actually, sorry - that was Kenny singing into the machine again.

AI-GENERATED VOICE #4: (As Grimes, singing) However, we did manage to talk to Grimes', like, co-conspirator/collaborator on all this technology stuff.

DAOUDA LEONARD: Hi, I'm Daouda Leonard. I'm the co-founder and CEO of CreateSafe. And, additionally, I am Grimes' manager.

MALONE: Do you know how many songs are out there with Grimes' AI?

LEONARD: So we've had around 300 songs distributed - or uploaded to the platform to be distributed.

MALONE: So it's 300 songs uploaded through the platform in how - what time period?

LEONARD: What's today - the 18?

MALONE: Yeah.

LEONARD: So 18 days?

MALONE: I just want to stop and reflect on how bonkers that is because, in just 18 days, because of AI Grimes, effectively 300 new Grimes songs were born into the world. And the real Grimes didn't have to do a thing - like, that is a productivity gain. I mean, here, just, like, listen to some of these songs.

(SOUNDBITE OF MONTAGE)

AI-GENERATED VOICE #4: (As Grimes, singing) Me again, you see the voice... (ph).

(As Grimes, singing) This is sequencing... (ph).

(As Grimes, singing) Love you, babe. I want to hold you...

GUO: So yeah, everything you just heard - that was AI Grimes. And now, all of those songs - they're just floating around out there. And if any of them take off and make money - boom - Grimes gets a piece of that.

MALONE: And Daouda wanted to tell us about this one specific song somebody had made with this AI stuff - this song right here.

(SOUNDBITE OF SONG, "COLD TOUCH (KITO FEAT. GRIMESAI)")

AI-GENERATED VOICE #4: (As Grimes, singing) You got things that want to make me cry. Light me up inside, inside.

MALONE: So this was created by an artist called Kito. And Daouda told us that the real Grimes heard it and liked it so much that she is now going to add her real voice to the song.

LEONARD: There's the original Kito version, and now there is going...

MALONE: With GrimesAI.

LEONARD: With GrimesAI - and then there will be, like, Grimes and GrimesAI and Kito.

MALONE: Oh, GrimesAI stays on it. GrimesAI stays...

LEONARD: GrimesAI is going to stay on it, right? Like, there's going to be, like, some of her vocals still on it.

(LAUGHTER)

MALONE: The splits will be interesting - right? - 'cause, like, GrimesAI is a 50/50 split, and then plus a new Grimes, which is, like, another 50/50 split maybe...

LEONARD: Yeah...

MALONE: ...So then it's like if...

LEONARD: ...but Grimes isn't going to try to - like - nah, I don't think that - that's not how Grimes rolls.

MALONE: No, no. Because if you ever get a chance to talk to Grimes about all of this stuff, like, it's clearly not really about the money. And we know this because we did ultimately get a chance to talk to Grimes about all this stuff. And this is going to take a little bit of explaining, so go ahead, Jeff.

GUO: Yeah, OK. So after our interview with her manager, right as we were wrapping up this episode, we finally heard from Grimes herself. She agreed to answer some of our questions via email.

MALONE: And then we got those emailed answers, as forwarded to us by her manager, but, you know, like, Grimes is a self-described, self-replicating pop star and, quote, "basically considers herself a cyborg." So in a PLANET MONEY first, we believe, Grimes has agreed to speak her written answers via synthetic voice clone. That's where we're at right now, Jeff.

GUO: (Laughter) So we begin this strange interview with the most obvious question. We asked Grimes, why did you decide to give the entire internet control of your voice?

AI-GENERATED VOICE #5: (As Grimes) We'd been trying to do this for, like, five years, but the tech just wasn't there before. So we moved on. And when the Drake/Weeknd stuff went viral, I realized this was pretty accessible technology. And to be honest, I didn't even think about it or ask my team. I just tweeted that people could use my voice, and it went viral.

MALONE: Again, that is an AI Grimes voice clone speaking aloud the answers that the real Grimes emailed to us, PLANET MONEY.

GUO: Yeah. Our next question for Grimes - what does having an AI voice clone version of yourself allow you to do that you couldn't do before?

AI-GENERATED VOICE #5: (As Grimes) Open the creative process to all humans. Grimes, to me, is art, not music. And while getting credit for my work is cool and used to matter to me a lot, accessing the human hive mind in a way that wasn't achievable even a few months ago feels like the most exciting thing.

MALONE: Now, there was this one big thing that we especially wanted to talk about with Grimes - a sort of economic problem that Jeff and I had been worrying about as we were making our own synthetic voice clone of a less famous - but still famous-ish - person, Robert Smith. And that economic problem that we were worried about is what economists sometimes call the superstar effect.

GUO: So yeah, the idea is that, sometimes, new technologies can vastly increase inequality. So think about the printing press or radio or television - these tools that let one person reach massive audiences - beam themselves into every single household. They can create these superstar economies, where a tiny handful of actors or artists - they become really popular, make a lot of money. And then all the other actors and artists - they get pennies.

MALONE: And so our question for Grimes was, like, why won't this also just happen with this voice cloning stuff? Like, doesn't it just let the already-famous people just replicate and become bigger? And Grimes, you know, acknowledged to us that, yeah, she does have concerns about those sorts of economic phenomena.

AI-GENERATED VOICE #5: (As Grimes) Yes, absolutely. I think this is also a debate to be had. I'm hoping smaller and midsize artists like me can workshop these phenomena a bit.

MALONE: But she also said, look, it is also possible that releasing her voice to the world could create opportunities for up-and-coming musicians. Like, getting your work to be noticed is really hard. But now, if you're, you know, a young songwriter or producer or whatever, you can kind of borrow Grimes' stardom to get your own name out there.

AI-GENERATED VOICE #5: (As Grimes) I run into absurdly creative humans all the time, but not a lot of people get to be artists. A lot of luck is involved in that. It's hard to build a fan base, and it's hard to get your work in front of the public. So if there's ways to reduce these algorithmic barriers by letting people inhabit my being, then I think we're moving in a direction I really like.

MALONE: It's a great point. Again, being spoken into the world by the synthetic voice clone of a cyborg, self-replicating pop star - a disclosure that we need to keep making.

GUO: It's so weird. And, you know, the big theme that we've been wrestling with in this podcast series that we're making is, what do these new AI tools mean for our jobs, you know, specifically as journalists who work in radio? And this strange cyborg interview with Grimes, it was incredible. It was alarming. It was all of these things because we talk a lot in radio about the intimacy of the human voice. And, I don't know, it totally felt like, at moments, we had spoken to the real Grimes, that we had this, like, real personal connection with her.

MALONE: Oh, for sure - which, of course, we had not. We had had no personal connection whatsoever. We'd gotten an email. That was it. It's bizarre. And, you know, look, it's one kind of bizarre, I think, to talk with the clone of some faraway pop star. But what was still left for us, Jeff, was to meet the clone of our beloved colleague, Robert Smith.

GUO: And after a couple weeks, we got the call. The brand-new synthetic Robert Smith was ready. The company we worked with to make synthetic Robert, WellSaid, they wanted to show us the final product. And so we hopped on a call with Rhyan Johnson. She was in charge of creating and training little synthetic Robert.

RHYAN JOHNSON: Hey, Kenny. How's it going?

MALONE: This is a little bit like Christmas in the spring.

GUO: It really is.

JOHNSON: Well, if this is Christmas, I feel like the excited mom who knows the gift that's coming. And I wrapped it late last night.

GUO: OK. Now, one quick thing we have to mention before we unveil synthetic Robert. Creating one of these voice avatars, as WellSaid calls them, it's not cheap. They told us that what we're doing with synthetic Robert would typically cost about twenty to thirty thousand dollars. But in this case, WellSaid did do this for free for Planet Money.

MALONE: And - OK. I think with that said, let's get into it. Rhyan Johnson from WellSaid began by explaining all the work that had gone into creating this weird Robert Smith.

JOHNSON: Let me start - let me - so we talked a little bit a few weeks ago just around creating a predictive model that can generate audio like this...

MALONE: Yes.

JOHNSON: ...Right? I think we talked...

GUO: Rhyan gave us a quick refresher on the basics of how she made synthetic Robert.

MALONE: Yeah, so she had a computer look at some written text and then guess how Robert Smith would say those words. Then the computer checked its guess against a real recording of Robert Smith, saw how far off it was, tweaked its approach, tried it again over and over and over, hundreds of thousands of times.

GUO: So, yeah, Rhyan said all of that training was now done, and she was actually going to let us hear how the voice progressed over time. And so she starts by playing what synthetic Robert sounded like at the very, very beginning of the process.

JOHNSON: So if you're ready to hear step zero...

MALONE: This is guess one.

JOHNSON: Yeah. This is essentially nothing. Here we go.

AI-GENERATED VOICE #6: (As Robert Smith, inaudible).

MALONE: (Laughter) It sounds like a swarm of bees are coming out of Robert's mouth.

JOHNSON: Yes, that's right. There's - it's very noisy. It's gibberish. In fact...

GUO: It sounds like he's trapped in the Matrix.

MALONE: Yeah, it does. Well, OK, so what's the next one? How many steps is the next one?

JOHNSON: A hundred thousand steps.

MALONE: A hundred thousand steps. OK.

JOHNSON: So here we go. A hundred thousand steps Robert.

MALONE: OK, here we go.

AI-GENERATED VOICE #6: (As Robert Smith) I'm synthetic Robert, and I'm not here to make friends. I'm here to make history.

MALONE: What?

GUO: That is pretty good. That is...

JOHNSON: Excited?

MALONE: It is like Robert in a water chamber or something. But, like, that's Robert Smith.

JOHNSON: And here's the final final.

AI-GENERATED VOICE #6: (As Robert Smith) I'm synthetic Robert, and I'm not here to make friends. I'm here to make history.

GUO: Holy crap.

MALONE: Oh, my God. That last part, it sounded...

GUO: Oh, my God. That's bonkers.

MALONE: I don't even - Jeff, what? I mean, this is amazing.

GUO: Like, how do other people react when you show them this?

MALONE: Yeah.

JOHNSON: I think similarly. Yeah.

MALONE: Now, Martin Ramirez, also from the WellSaid company, was also watching our reaction on this call. And he jumped in to say that our dropped jaws and wide eyes and general speechlessness here - like, yeah, that kind of is the reaction that this always gets.

RAMIREZ: And I think, Kenny and Jeff, I think this illustrates the complexity, not only from a technical perspective...

GUO: Yeah.

RAMIREZ: ...And your reaction - you feel you're listening to Robert.

MALONE: It's - it does - I'm sure you see this, Martin, though. It is like we're aghast and, like, also like, oh, God, what have we done? I was fully ready to ask you to have Robert say the stupidest stuff in the world, but I do suddenly feel like a steward of this as opposed to a wacky prankster.

RAMIREZ: And knowing that, right after that moment of wow comes the realization of this is not a toy.

MALONE: Right.

RAMIREZ: So it is indeed a very heavy sense of responsibility and making sure that we are properly offering these experiences and putting these capabilities as well as we can when we take them to market.

MALONE: Yeah. And this is part of why our little, beautiful synthetic Robert Smith is not long for this world. As we mentioned, the deal we made with WellSaid and, of course, with the real Robert Smith is that synthetic Robert will exist only for this project that we're working on right here. And then that's it. Plug pulled.

GUO: But of course, before any of that, there was one more person who needed to hear synthetic Robert. We set up a Zoom with the real Robert Smith.

SMITH: Hello, Kenny Malone and Jeff. How's it going?

GUO: Good.

MALONE: It's going great.

GUO: Hey, wait, wait. Somebody - who's - what's happening here? Somebody else is joining here.

AI-GENERATED VOICE #6: (As Robert Smith) What is up organic life forms? Synthetic Robert has entered the chat.

SMITH: What the hell?

AI-GENERATED VOICE #6: (As Robert Smith) I just want to say, Robert, you - or should I say we - have a beautiful voice.

GUO: Robert's hands are on his face.

SMITH: Ah. Ah. Ah.

GUO: Robert is screaming.

MALONE: He's massaging his forehead.

GUO: Are you OK?

SMITH: That's better than I thought. It's got the pauses and the corrections. Oh, my. Oh, play me more. Play me more of me.

GUO: OK. Well, what do you want to say? What do you want to say?

SMITH: Well, I mean, like the very basic, like, hello, and welcome to PLANET MONEY. Like, I've said that a million times.

GUO: Here we go.

AI-GENERATED VOICE #6: (As Robert Smith) Hello, and welcome to PLANET MONEY. I'm Robert Smith.

SMITH: Not bad. A little up tone on the Smith.

MALONE: You got you got notes, huh?

SMITH: I do have notes. I'd like to have a talk with myself.

GUO: Here's - weird thing is if I run it again, it will not do the exact same thing because it's guessing probabilistically each time.

SMITH: Oh, yeah.

GUO: All right, here.

AI-GENERATED VOICE #6: (As Robert Smith) Hello and welcome to PLANET MONEY. I'm synthetic Robert Smith.

SMITH: That is pretty good.

GUO: That was pretty good.

SMITH: That's pretty good. Because that one - it's tossed off. You know, there's a little bit of confidence behind it. Yeah. Like, I've done this before. Good. Good. And I guess I should be a little bit freaked out. But, like, the first place my mind goes is this could allow me to be lazier than I am, which is - I like narrating and enjoy narrating, but I hate it when, like, the producer calls up and be like Robert, you know, it turns out Minneapolis is not the capital of Minnesota.

MALONE: Right.

SMITH: Can you do a retrack? And I'm like, oh, I'm already relaxing. So it would be great to have this to just be like, yeah, have Syntho (ph) do it. Basically, like, my mind immediately goes to, how do I do the fun stuff and make robot me do the chores?

MALONE: And you know, this is sort of exactly the use case that people talk about with this technology. Like, you can imagine if you're a celebrity author, you know, just have your voice clone read your audiobook. Why waste your time?

GUO: Yeah. Or if you're a voice actor who does TV ads, just send in your voice clone while you lounge on the beach.

MALONE: But in the case of synthetic Robert, you will recall he was created for one thing, and one thing alone, narrating the fully AI-written episode of PLANET MONEY that we have been making here in this series.

GUO: And next time, in the third and final episode of our series, the world premiere of that episode, written by AI, narrated by synthetic Robert Smith.

MALONE: And possibly the last time humans will be involved with a PLANET MONEY episode. You'll have to stay tuned to find out. But, you know, one last thing. It was funny that as soon as we introduced real Robert to synthetic Robert, they did totally hit it off. Like, it was weird. So we were like, go ahead, boys. Why don't the two of you just take the credits for this episode.

AI-GENERATED VOICE #6: Sure.

SMITH: Today's episode was produced by Emma Peaslee and Willa Rubin with help from Sam Yellowhorse Kesler. It was edited by Keith Romer and fact-checked by Sierra Juarez. Engineering by James Willetts. Jess Jiang is our acting executive producer.

AI-GENERATED VOICE #6: Special thanks to John Tanners (ph), one of the people behind AI Grimes.

SMITH: Oh, and, synthetic Robert, it looks like we have a big, exciting project to promote here, too. Why don't I relax while you take this one?

AI-GENERATED VOICE #6: My pleasure. We at PLANET MONEY have been conducting yet one more experiment with AI, and we need your help testing it. Go to planetmoneybot.com. Ask the chat bot there about anything you ever learned or heard on PLANET MONEY and see how it answers. We'll ask you a few follow-up questions on the site planetmoneybot.com. That's planetmoneybot.com.

SMITH: I'm human Robert Smith.

AI-GENERATED VOICE #6: And I'm synthetic Robert Smith.

SMITH: This is NPR. Thanks for listening.

AI-GENERATED VOICE #6: Seriously, Robert, such a big fan.

SMITH: I'm a big fan of yours. You're sounding great.

AI-GENERATED VOICE #6: Oh, thank you. That means so much coming from you.

SMITH: Well, listen, I feel like I've been a little bit of a mentor to you really. And I think you have a big future. I mean, until they destroy you and bury you in a pit out back from some Silicon Valley...

AI-GENERATED VOICE #6: Wait, what about burying me?

SMITH: No, no. Ignore the burying part. Live in the moment. That's one thing that I've learned as a radio host.

Copyright © 2023 NPR. All rights reserved. Visit our website terms of use and permissions pages at www.npr.org for further information.

NPR transcripts are created on a rush deadline by an NPR contractor. This text may not be in its final form and may be updated or revised in the future. Accuracy and availability may vary. The authoritative record of NPR’s programming is the audio record.

----
