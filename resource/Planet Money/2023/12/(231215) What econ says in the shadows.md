---
title: (231215) What econ says in the shadows
date: 20231215
tags: #PlanetMoney
citation: “Planet Money,” _NPR_, 2 Juni 2023. [https://www.npr.org/podcasts/510289/planet-money](https://www.npr.org/podcasts/510289/planet-money) (diakses 4 Juni 2023).
---


----
# Points

- 

----
# Article
https://www.npr.org/2023/12/15/1197956091/econ-job-market-rumors-ip-addresses
Economics Job Market Rumors is a website that's half a job information Wiki, where people post about what's going on inside economics departments, and half a discussion forum, where anyone with an internet connection can ask the economics hive mind whatever they want. All anonymously. 

What econ says in the shadows
December 15, 20239:31 PM ET

By 

Mary Childs

, 

Alexi Horowitz-Ghazi

, 

Keith Romer

, 

Willa Rubin
26-Minute Listen

    Download

    Transcript

Economics Job Market Rumors webpage on a laptop screen.
Willa Rubin/NPR

Economics Job Market Rumors is a website that's half a job information Wiki, where people post about what's going on inside economics departments, and half a discussion forum, where anyone with an internet connection can ask the economics hive mind whatever they want. All anonymously.

People can talk about finding work, share rumors, and just blow off steam. And that steam can get scaldingly hot. The forum has become notorious for racist and sexist posts, often attacking specific women and people from marginalized backgrounds.
Planet Money
Economics, Sexism, Data

Last year, economist Florian Ederer and engineer Kyle Jensen discovered a flaw in the way the site gave anonymity to its users. The flaw made it possible to identify which universities and institutions were the sources of many of the toxic posts on the site. And helped answer a longstanding question that's dogged the economics profession: was the toxicity on EJMR the work of a bunch of fringey internet trolls, or was it a symptom of a much deeper problem within economics itself?

This episode was hosted by Mary Childs and Alexi Horowitz-Ghazi. It was produced by Willa Rubin with help from James Sneed and Sam Yellowhorse Kesler. It was edited by Keith Romer and engineered by Josh Newell. Fact-checking by Sierra Juarez. Alex Goldmark is Planet Money's executive producer.

Help support Planet Money and get bonus episodes by subscribing to Planet Money+ in Apple Podcasts or at plus.npr.org/planetmoney.

Always free at these links: Apple Podcasts, Spotify, Google Podcasts, the NPR app or anywhere you get podcasts.

Find more Planet Money: Facebook / Instagram / TikTok / Our weekly Newsletter.

Music: Universal Music Production - "Sangria Spice," "Pop Only Knows," and "Come To Life"

# Transcribe
https://www.npr.org/transcripts/1197956091
SYLVIE DOUGLIS, BYLINE: This is PLANET MONEY from NPR.

(SOUNDBITE OF COIN SPINNING)

ALEXI HOROWITZ-GHAZI, HOST:

Economist Florian Ederer tells the story of how he got pulled into a fight over an anonymous economics message board as a sort of string of happenstances. The first was one day last spring.

FLORIAN EDERER: The real catalyzing event in all of this is just a conversation with my friend Kyle Jensen, who is not an economist.

MARY CHILDS, HOST:

Kyle Jensen is an engineer with experience writing computer code. He lectures at Yale's School of Management, and that day, the two of them were taking a stroll around New Haven. Kyle had recently sat in on some econ seminars, and he was telling Florian how aggressive the conversation had gotten.

KYLE JENSEN: And I told him, look, we have a relatively aggressive tone in seminars, but there's much, much more aggressive behavior in economics. You should read the type of stuff that gets said on the internet about various people. And he said, what do you mean, what gets said on the internet? People discuss economists on the internet? I said, well, there's this platform called Econ Job Market Rumors.

HOROWITZ-GHAZI: Economics Job Market Rumors - one half of the website is a sort of job information wiki where people anonymously post about what's going on inside the black box of economics departments. The anonymity lets academic insiders pass on information without fear of professional consequences - stuff that's directly relevant to people applying for jobs.

EDERER: About which universities have sent out invites for interviews or which have given offers out or even who has been receiving those offers.

CHILDS: The other half of the website is a discussion forum where anyone with an internet connection can ask the economics hivemind whatever they want - also anonymously.

HOROWITZ-GHAZI: Which made it pretty popular. Economics is this notoriously hierarchical field. It can be hard to navigate for people outside the elite echelons of academia, and this place was democratizing potentially useful information.

CHILDS: People also post rumors about things like harassment or plagiarism. You can find out what people really think about some powerful famous economist and their work or about your peers or yourself.

HOROWITZ-GHAZI: Or you could just blow off some steam.

EDERER: There is more willingness to voice that discontent on an anonymous platform.

HOROWITZ-GHAZI: It's kind of an emotional labor market.

EDERER: Yeah. I think so, yeah. It's where people will go and vent.

HOROWITZ-GHAZI: And all that venting can get scaldingly hot. Debates over academic papers can spill over into outright attacks - sometimes even threats. Florian himself has gotten roasted on there.

CHILDS: And the econ jobs board has become most notorious for its sexist and racist posts, often attacking specific women and people from marginalized backgrounds. A famous paper back in 2017 actually demonstrated that statistically, on the site, women are disproportionately discussed with unprofessional and lewd terms.

HOROWITZ-GHAZI: Florian explains the site's whole deal to Kyle, and when Kyle gets home, he pulls up the website. And at first, scrolling through all these anonymous posts, he's just kind of shocked by how gnarly some of them are. But here is the next happenstance. When he looks at the website, he sees something Florian hadn't.

CHILDS: To give posters anonymity, the site was assigning them a kind of code name for each thread they posted in - these four character ID numbers, but those super secret code names are in a format instantly recognizable to anyone with programming experience like Kyle.

JENSEN: To me, it was immediately obvious how those usernames are put together.

CHILDS: How do you feel when you solve a little puzzle like this?

JENSEN: Oh, I'm super into puzzles, for sure. I just...

CHILDS: (Laughter).

JENSEN: ...This wasn't very - a very long puzzle.

(SOUNDBITE OF MUSIC)

CHILDS: Hello, and welcome to PLANET MONEY. I'm Mary Childs.

HOROWITZ-GHAZI: And I'm Alexi Horowitz-Ghazi. The story of the Econ Job Market Rumors website gets to this kind of fundamental tension about the internet. When you allow people to be anonymous online, you give them the freedom to share all the things they maybe couldn't otherwise but also to say things they maybe really shouldn't.

CHILDS: And because the posters on the jobs board are anonymous, no one could really say for sure - was all this toxicity just the work of a bunch of fringy internet trolls? Or was it a symptom of a much deeper problem within economics itself?

HOROWITZ-GHAZI: Today on the show, Florian and his colleagues discover that all the clues they need to answer that question have been sitting out in the open all along, and what they find sends a shockwave through the profession.

(SOUNDBITE OF MUSIC)

CHILDS: So engineer, not economist, Kyle Jensen has just started poking around on the Econ Job Market Rumors site, and he's noticed that the format of the anonymous four-character code names the website is assigning to its users look extremely familiar.

HOROWITZ-GHAZI: The website seems to be using an algorithm called a hash to transform some piece of information about every poster - he thought probably their IP address - to generate these code names.

CHILDS: There are a couple popular algorithms Kyle suspects the site may have used to do this, so he calls up his economist friend Florian, asks for his IP address and proposes a test.

JENSEN: Let me see if I can guess what your username would be knowing what your IP address is.

HOROWITZ-GHAZI: He asks Florian to make a new post in a particular thread on the website. His plan is to enter the threads ID number, along with Florian IP address, into a series of the most commonly used hashing algorithms.

CHILDS: And sure enough, on the second algorithm he tries with just Florian's IP address and the topic he was posting about, Kyle is able to guess the theoretically anonymous four-character code name the site had assigned to him.

JENSEN: So it really - what didn't take very long.

CHILDS: This is just fun for you? This is just like a little Sunday morning puzzle that you're doing?

JENSEN: Yeah. I thought it was interesting. Yeah, for sure. I thought it was interesting. But also, it was a super obvious thing.

HOROWITZ-GHAZI: And the super obviousness of this puzzle, Kyle says, revealed something huge about the site - that whoever had set it up back in the late 2000s had not taken one of the most basic precautions when it comes to using one of these hashing algorithms. They forgot to add salt.

JENSEN: Which just means you sprinkle a little bit of other data in there. That kind of obscures where those posts are made from. And the lack of a salt meant that it was feasible for us to do some statistics on these usernames.

CHILDS: Those statistics could potentially point to which IP addresses were responsible for each individual comment on the site.

HOROWITZ-GHAZI: And while Kyle found all of this mildly amusing in a Sunday-morning-puzzle kind of way, when he explained what was going on to Florian, Florian immediately sees they might have something much bigger on their hands, a kind of treasure trove of data hiding in plain sight.

CHILDS: Because the anonymity that had cloaked the toxic speech on the econ jobs board seemed like it might unravel with the application of a little statistical analysis, an analysis they could then convert into the only language economists seem to understand - an academic research paper.

HOROWITZ-GHAZI: What were you setting out to do with this paper? What was the plan?

EDERER: I think we wanted to just document who posts on Econ Job Market Rumors. I had heard this criticism before saying, oh, you know, it's just people that are not relevant to the center of the profession. It's just disenfranchised people who are unhappy at low-ranking universities. They're posting all that information on there, and that's why we should just ignore it. And I think what I wanted to know is, well, is that really true?

HOROWITZ-GHAZI: So it's like, are all of these toxic posts attributable to a few rotten apples kind of in the periphery...

EDERER: Exactly.

HOROWITZ-GHAZI: ...Of the discipline, or does this rot go all the way to the top?

EDERER: Exactly.

CHILDS: So now it is math time. Florian ropes it another friend - a mathy one - Paul Goldsmith-Pinkham of Yale. Kyle had figured out the easy way to crack the code on a single post, but now they will have to do it at scale. They will need to do a version of that puzzle to every comment on the site.

HOROWITZ-GHAZI: Which is an enormous task. For every comment, there's a starting pool of 4.3 billion potential suspects, 4.3 billion possible IP addresses in the world that could have been responsible. So they're going to have to do that short, obvious puzzle a preposterous 3 quadrillion times. That's quadrillion with a Q.

EDERER: On our very first attempt, it took us 230 hours.

HOROWITZ-GHAZI: Wait, the first time you crunched these numbers, it took 10 days?

EDERER: Yeah, exactly. The first time, it took 10 days. Yeah. But just - once you program it, the code runs, and you just wait.

HOROWITZ-GHAZI: And what happens when it's done? Is there, like, a toaster...

CHILDS: Ding.

EDERER: Yeah.

HOROWITZ-GHAZI: ...Sound?

EDERER: Yeah. No, it just sends - yeah - it sends you a message that the code that you ran is completed.

CHILDS: But that completed code still doesn't answer the question of which IP address was responsible for any given post because once those calculations are done, Florian and the team are still left with around 65,000 IP addresses that could have conceivably left any single comment - 65,000, down from 4.3 billion, but still.

HOROWITZ-GHAZI: So the next part of the process is to take these 65,000 possible IP addresses for one single comment and to cross-reference them with the 65,000 possible IP addresses for every other comment across the site over the course of a week. If an IP address is on the list of possibilities for one comment and then again on the list of possibilities for another and then another, it becomes more and more statistically likely that you found a real IP address that was the source of multiple comments. Those super posters are the signal in the mathematical noise.

EDERER: Then you have - for about 67% of all posts on Econ Job Market Rumors, you have an IP address associated with it, and then you can start the analysis.

HOROWITZ-GHAZI: IP addresses for two-thirds of all the posts on the site, which Florian and his colleagues could now plug into a sort of IP address directory.

CHILDS: These directories help narrow down which zip code a given IP address has come from. They're not super accurate for locating an exact physical address within a city, but...

EDERER: What is very, very accurate is the allocation to particular institutions 'cause they tend to have IP addresses specifically allocated to them and that very, very rarely change. And so that allows actually the identification of universities very, very easily.

CHILDS: And when they narrowed it down to look at just the bad posts, the racist and sexist stuff, what they found was that the toxic posts on Econ Job Market Rumors were very much coming from within the house of economics, from institutions across the discipline.

EDERER: It's not that all the rotten apples are in one barrel, but there's at least one rotten apple in every single barrel. It's just everywhere.

HOROWITZ-GHAZI: Including many of the top institutions in the field, places like Stanford, Harvard, UChicago, even the Federal Reserve. All of them seem to have contributed toxic comments to the Econ Jobs board.

CHILDS: It might be someone using the library computer, or it might be someone writing policy suggestions or who will go on to work in the next presidential Cabinet. To Florian, this seemed like an important enough finding that he was willing to risk stirring the hornet's nest.

HOROWITZ-GHAZI: Did you imagine that your work might put you in kind of direct confrontation with this online forum?

EDERER: No, I never imagined this. You know, my work is on antitrust economics, but I do enjoy confrontation a little bit. So when I started doing this project, I was very much aware that I was going to take on anonymous hoards. But, you know, sticks and stones can break your bones, but words will never hurt me.

HOROWITZ-GHAZI: After the break, Florian reveals what he's found out about the ugly id of economics to economics itself, and everyone freaks out.

(SOUNDBITE OF MUSIC)

HOROWITZ-GHAZI: So Florian and his team found that toxic posts on Econ Job Market Rumors are coming from everywhere in economics. They're going to present their paper at a big conference put on by the National Bureau of Economic Research.

CHILDS: And ahead of the presentation, Florian tweets out a little teaser. He posts an abstract of the paper, which says that they've managed to identify the majority of posts on the site, including ones that they have categorized as toxic, and that a lot of the posts are coming from universities.

EDERER: This was, by far, the most viral post I ever put out on Twitter. I think it got something close to 2 million views and reached well, well, well beyond economics.

HOROWITZ-GHAZI: And the economics world itself freaks out - in particular, a lot of those individual posters on Econ Job Market Rumors, including this one tenured professor who we are going to call Terry. Terry asked that we not reveal his identity, his real name or voice, so we're going to use a voice actor for him. He says he's worried there would be professional repercussions for having posted on the site, even though, he assures us, he is, quote, "a nobody."

JULIAN RING: (As Terry) I'm not, like, this super famous person. I mean, most people in the field don't even know who I am, so...

CHILDS: Terry found out about the econ jobs board over a decade ago. And he says, under the site's alleged cloak of anonymity, he had passed along some insider-y information about his academic department's hiring decisions. And, he says, he also engaged from time to time in some light political trolling.

RING: (As Terry) It wasn't racist or misogynist, but, like, I've made some posts where I sound like a right-wing extremist. It's kind of like a Stephen Colbert.

HOROWITZ-GHAZI: Which meant that when he read Florian's tweet, Terry was extremely distressed. Terry feared that if his posts were unmasked, people wouldn't understand that he'd been joking and that there might be real professional consequences.

RING: (As Terry) I was very stressed. I was feeling dread because I had no idea, like, what information they had, what they were going to release, what their timeline was.

HOROWITZ-GHAZI: For people who had posted on the econ jobs board, the worry seemed to be, if Florian and his team can identify specific universities where some of the toxic posts were coming from, could they also identify specific people who had made the posts? Were they going to be doxxing people who'd posted?

CHILDS: And this worry was exacerbated when, in a leaked early draft of the researchers' presentation slides, one slide showed the IP address of one anonymous user that the authors had managed to identify - the site's administrator.

HOROWITZ-GHAZI: The econ jobs board itself was inundated with hundreds of comments puzzling, worrying and fuming about the paper. People were speculating about how Florian and his co-authors got ahold of this information, whether this project might fall afoul of academic ethics rules or if it might even be illegal.

CHILDS: And they're freaking out not just because some of them had posted racist, sexist stuff but because some of them had also posted all sorts of other kinds of sensitive information in which they, say, trash talked their boss or posted about a mental health crisis, even about considering suicide - stuff they posted because they believed they were anonymous.

HOROWITZ-GHAZI: So this past July, when the day finally comes for Florian and Paul to present their findings, everyone is watching - from people who'd been harassed and attacked on the jobs board to frequent posters fearing they were about to be doxxed. When Florian and Paul arrive at the Royal Sonesta Hotel in Cambridge, Mass., to present the paper, they discovered they've accidentally worn matching suits...

(SOUNDBITE OF ARCHIVED RECORDING)

CATHERINE: Welcome, everyone. OK...

HOROWITZ-GHAZI: ...And that they will have a packed audience.

(SOUNDBITE OF ARCHIVED RECORDING)

CATHERINE: I just wanted just to mention something a little bit different.

CHILDS: There is a reporter in the room. The session is also being streamed on YouTube.

(SOUNDBITE OF ARCHIVED RECORDING)

CATHERINE: You know, we often sort of feel like we're just us in the room, but actually, there may be quite a few people watching.

CHILDS: More than 2,000 people have tuned in, which is pretty high for an academic conference session.

(SOUNDBITE OF ARCHIVED RECORDING)

CATHERINE: So with that warning ahead, let me give the stage over to Florian.

EDERER: Thank you very much, Catherine (ph). Thank you very much, everybody, for coming.

HOROWITZ-GHAZI: Florian introduces the paper...

(SOUNDBITE OF ARCHIVED RECORDING)

EDERER: A very important topic for everybody in this room and for everybody in our profession - namely, toxic speech in economics.

HOROWITZ-GHAZI: ...And puts up on the screen behind him screenshots from the econ jobs board - examples of useful posts on the site, like...

(SOUNDBITE OF ARCHIVED RECORDING)

EDERER: How to run nonlinear least squares with fixed effects...

HOROWITZ-GHAZI: ...Mini tutorials economists offer up to each other...

(SOUNDBITE OF ARCHIVED RECORDING)

EDERER: ...Make your Stata graphs more beautiful....

CHILDS: And then he puts up examples of the bad stuff - posts with sexist language and racial slurs. And then he delivers the headline finding of their study.

(SOUNDBITE OF ARCHIVED RECORDING)

EDERER: That these posts here come from IP addresses at Harvard, at Stanford, at Yale, at Chicago and even the NBER headquarters at 1050 Mass. Ave.

HOROWITZ-GHAZI: Florian goes on to explain to the audience the whole story - how they'd figured out the site's method for anonymizing posters...

(SOUNDBITE OF ARCHIVED RECORDING)

EDERER: A allocation scheme that did not use a salt...

HOROWITZ-GHAZI: ...The tragicomic lack of salt...

(SOUNDBITE OF ARCHIVED RECORDING)

EDERER: ...The random secret that sort of gets added to the stuff that is...

HOROWITZ-GHAZI: ...And how they used statistics to identify which institutions these toxic posts were coming from.

(SOUNDBITE OF ARCHIVED RECORDING)

EDERER: ...And that was also in plain sight for more than a decade.

CHILDS: As Terry and the thousands of other viewers watch from around the world, it gradually becomes clear that this was as much as Florian and Paul were going to reveal - just the names of universities and government offices - no names of individual posters. They had IP addresses but nothing more granular.

HOROWITZ-GHAZI: And IP addresses are not people. To even try to link an IP address to an individual, somebody would need to sift through tons of posts to collect biographical clues and triangulate them, and that was just not part of the paper.

CHILDS: And as for that slide identifying the site administrator's IP address, the only reason the researchers had been able to get that one was because of a special setting the admin had used for one year that allowed the researchers to link all of those posts together. Also, the researchers took out that slide for their final presentation.

HOROWITZ-GHAZI: Instead of doxxing anonymous econ jobs board users, what they are doing is kind of doxxing the profession of economics itself.

(SOUNDBITE OF ARCHIVED RECORDING)

EDERER: This is pervasive. It's everywhere, and I think we should not look away. Thank you very much for your time.

PAUL GOLDSMITH-PINKHAM: Great. So as we were doing before, line up at the mics, and we'll take...

CHILDS: Are a lot of questions and comments. People ask about the terms they'd used in the paper.

(SOUNDBITE OF ARCHIVED RECORDING)

UNIDENTIFIED ATTENDEE #1: Power users and power laws are, like, not showing up in your data.

CHILDS: Some of the questions are more technical, about methodology.

(SOUNDBITE OF ARCHIVED RECORDING)

UNIDENTIFIED ATTENDEE #2: So any changes on this behavior 'cause this is about...

HOROWITZ-GHAZI: Some people just want to express their gratitude to Florian and his colleagues for helping bring this problem out into the open.

(SOUNDBITE OF ARCHIVED RECORDING)

UNIDENTIFIED ATTENDEE #3: I don't have a question. I just want to say thank you.

CHILDS: Others want to take the findings into the real world.

(SOUNDBITE OF ARCHIVED RECORDING)

UNIDENTIFIED ATTENDEE #4: There is a petition out there that has been signed by almost a thousand people who have had slanderous comments made about them on the website. If you are one of these people or you know...

CHILDS: That petition started by a professor at UC San Diego asked the American Economic Association to explore ways to identify those responsible for the worst posts, the threats and libel - stuff that is legally actionable - so that the people who posted it could be held actually responsible.

HOROWITZ-GHAZI: And then after this flurry of comments and just a little over 50 minutes, the presentation comes to an end.

(SOUNDBITE OF ARCHIVED RECORDING)

GOLDSMITH-PINKHAM: Thank you very much for all your time and all your questions.

EDERER: Thank you.

CHILDS: It has now been five months since that presentation. For all the hubbub this summer, not a lot has changed. None of the universities whose IP addresses showed up as the top 14 sources for toxic posts seem to have taken any official action. We emailed them to ask, and the few that did respond sent over statements about being disappointed or not tolerating harassment.

HOROWITZ-GHAZI: Since news of the paper dropped, the econ jobs board administrator has changed how usernames are given out on the site. Posters are now assigned the name of a famous economist instead of a four-character code name.

CHILDS: A lot of people still posting on the site, along with its administrator, see this paper in the context of freedom of speech and censorship. They point out that there are real societal benefits to anonymity for exposing things like wrongdoing, corruption, plagiarism, and that there's a cost to undoing anonymity.

HOROWITZ-GHAZI: For his part, Florian Ederer says it was never his intention to destroy the site. He just wants economics to find a better way to talk to itself. As for doing more to de-anonymize the toxic posters, Florian does not see that as his role.

EDERER: I think at that point, you're just veering too much into doxxing, I think. And then I'm - I have just bigger ethical concerns. Would it be a net positive to expose the worst actors on that platform? Perhaps. But you know, in economics, we tend to think of trade-offs, and, you know, it's - it is a trade-off, maybe, that I'm not willing to make at this point.

CHILDS: Florian does acknowledge that his work may have opened the door for others who view those trade-offs differently.

HOROWITZ-GHAZI: Terry, the anonymous econ job rumors poster who watched Florian presentation with bated breath - the whole thing has not convinced him to quit the Economics Job Market Rumors site, or EJMR, as he calls it.

RING: (As Terry) I think EJMR is bad for the econ profession. I think it's bad for society. I think the econ profession would be better without EJMR, right? So if I could like, you know, wave a magic wand and make it go away, like, I would do that. But, like, whether I visit the site or not, the site's going to exist. And so that's kind of why I continue to visit the site.

CHILDS: Though he does now use a service that disguises his IP address, just in case.

(SOUNDBITE OF MUSIC)

HOROWITZ-GHAZI: Argentina has a new president who campaigned on the promise to dollarize his country - make the U.S. dollar their new national currency. An economist says there could be one big upside.

UNIDENTIFIED ECONOMIST: It's like tying yourself to the mast so as to not go towards the sirens' call.

AMANDA ARONCZYK, BYLINE: And the sirens' call is print more pesos.

NICK FOUNTAIN, BYLINE: Exactly.

ARONCZYK: Print more pesos.

UNIDENTIFIED ECONOMIST: Right. Exactly.

CHILDS: Why dollarize, how to do it, and will it even work? That's on the next PLANET MONEY. You can email us at planetmoney@npr.org, or we are on some of the social media platforms at @planetmoney.

HOROWITZ-GHAZI: Today's episode was produced by Willa Rubin, with help from James Sneed and Sam Yellowhorse Kesler. It was edited by Keith Romer, engineered by Josh Newell and fact-checked by Sierra Juarez. Alex Goldmark is our executive producer.

CHILDS: Huge thank you to Catherine Tucker at MIT and to NPR One producer Julian Ring for voicing Terry. I'm Mary Childs.

HOROWITZ-GHAZI: And I'm Alexi Horowitz-Ghazi. This is NPR. Thanks for listening.

Copyright © 2023 NPR. All rights reserved. Visit our website terms of use and permissions pages at www.npr.org for further information.

NPR transcripts are created on a rush deadline by an NPR contractor. This text may not be in its final form and may be updated or revised in the future. Accuracy and availability may vary. The authoritative record of NPR’s programming is the audio record.

----

**(Adam Davidson):**

**(Laura Conaway):**


**faster whisper:**
Support for NPR and the following message come from the Kauffman Foundation, providing
access to opportunities that help people achieve financial stability, upward mobility, and
economic prosperity, regardless of race, gender, or geography.
Kauffman.org.
This is Planet Money from NPR.
Economist Florian Ederer tells the story of how he got pulled into a fight over
an anonymous economics message board as a sort of string of happenstances.
The first was one day last spring.
The real catalyzing event in all of this is just a conversation with my friend, Kyle Jensen,
who is not an economist.
Kyle Jensen is an engineer with experience writing computer code.
He lectures at Yale's School of Management.
On that day, the two of them were taking a stroll around New Haven.
Kyle had recently sat in on some econ seminars, and he was telling Florian how aggressive
the conversation had gotten.
I told him, look, we have a relatively aggressive tone in seminars, but there's much, much
more aggressive behavior in economics.
You should read the type of stuff that gets said on the internet about various
people.
He said, what do you mean, what gets said on the internet?
People discuss economists on the internet and said, oh, there's this platform called
Econ Job Market Rumors.
Economics Job Market Rumors.
One half of the website is a sort of job information wiki where people anonymously
post about what's going on inside the black box of economics departments.
The anonymity lets academic insiders pass on information without fear of professional
consequences.
If that's directly relevant to people applying for jobs.
About which universities have sent out invites for interviews or which have given offers
out or who has been receiving those offers.
The other half of the website is a discussion forum where anyone with an internet connection
can ask the economics hive mind whatever they want, also anonymously.
Which made it pretty popular.
Economics is this notoriously hierarchical field.
It can be hard to navigate for people outside the elite echelons of academia.
And this place was democratizing potentially useful information.
People also post rumors about things like harassment or plagiarism.
You can find out what people really think about some powerful famous economist and
their work or about your peers or yourself.
Or you could just blow off some steam.
There is more willingness to voice that discontent on an anonymous platform.
It's kind of an emotional labor market.
I think so.
Yeah.
It's where people will go and vent.
And all that venting can get scaldingly hot.
Debates over academic papers can spill over into outright attacks.
Sometimes even threats.
Florian himself has gotten roasted on there.
And the Econ jobs board has become most notorious for its sexist and racist posts, often attacking
specific women and people from marginalized backgrounds.
A famous paper back in 2017 actually demonstrated that statistically on the site, women are
disproportionately discussed with unprofessional and lewd terms.
Florian explains the site's whole deal to Kyle.
And when Kyle gets home, he pulls up the website.
And at first, scrolling through all these anonymous posts, he's just kind of
shocked by how gnarly some of them are.
But here is the next happenstance.
When he looks at the website, he sees something Florian hadn't.
To give posters anonymity, the site was assigning them a kind of code name for
each thread they posted in, these four character ID numbers.
But those super secret code names are in a format instantly recognizable to anyone
with programming experience, like Kyle.
To me, it was immediately obvious how those usernames are put together.
How do you feel when you solve a little puzzle like this?
Oh, I'm super into puzzles for sure.
This wasn't a very long puzzle.
Hello and welcome to Planet Money.
I'm Mary Childs.
And I'm Alexi Horowitz-Ghazi.
The story of the Econ job market rumors website gets to this kind of fundamental
tension about the internet.
When you allow people to be anonymous online, you give them the freedom to
share all the things they maybe couldn't otherwise.
But also to say things they maybe really shouldn't.
And because the posters on the jobs board are anonymous, no one could really say
for sure, was all this toxicity just the work of a bunch of fringy internet trolls?
Or was it a symptom of a much deeper problem within economics itself?
Today on the show, Florian and his colleagues discover that all the clues they
need to answer that question have been sitting out in the open all along.
And what they find sends a shockwave through the profession.
Support for this podcast and the following message come from WISE, the app that makes
managing your money in different currencies easy.
With WISE, you can send and spend money internationally at the mid-market
exchange rate.
No guesswork and no hidden fees.
Learn more about how WISE could work for you at WISE.com.
So engineer, not economist, Kyle Jensen has just started poking around on the
Econ Job Market Rumors site.
And he's noticed that the format of the anonymous four-character codenames
the website is assigning to its users look extremely familiar.
The website seems to be using an algorithm called a hash to transform
some piece of information about every poster.
They thought probably their IP address to generate these codenames.
There are a couple popular algorithms Kyle suspects the site may have used to
do this.
So he calls up his economist friend Florian, asks for his IP address and
proposes a test.
Let me see if I can guess what your username would be,
knowing what your IP address is.
He asks Florian to make a new post in a particular thread on the website.
His plan is to enter the thread's ID number along with Florian's IP address
into a series of the most commonly used hashing algorithms.
And sure enough, on the second algorithm he tries with just Florian's IP address
and the topic he was posting about, Kyle is able to guess the theoretically
anonymous four-character codename the site had assigned to him.
So it really, what didn't take very long?
This is just fun for you.
This is just like a little Sunday morning puzzle that you're doing.
Yeah, I thought it was interesting.
Yeah, for sure, I thought it was interesting.
But also, it was a super obvious thing.
And the super obviousness of this puzzle, Kyle says,
revealed something huge about the site.
That whoever had set it up back in the late 2000s had not taken one of
the most basic precautions when it comes to using one of these hashing
algorithms.
They forgot to add salt.
Which just means you sprinkle a little bit of other data in there.
That kind of obscures where those posts are made from.
And the lack of a salt meant that it was feasible for
us to do some statistics on these usernames.
Those statistics could potentially point to which IP addresses were
responsible for each individual comment on the site.
And while Kyle found all of this mildly amusing in a Sunday morning
puzzle kind of way, when he explained what was going on to Florian,
Florian immediately sees they might have something much bigger on their hands.
A kind of treasure trove of data hiding in plain sight.
Because the anonymity that had cloaked the toxic speech on the econ
jobs board seemed like it might unravel with the application of
a little statistical analysis.
An analysis they could then convert into the only language economists
seem to understand, an academic research paper.
What were you setting out to do with this paper?
What was the plan?
I think we wanted to just document who posts on econ job market rumors.
I had heard this criticism before of saying, it's just people
that are not relevant to the center of the profession.
It's just disenfranchised people who are unhappy at low ranking universities.
They're posting all that information on there and
that's why we should just ignore it.
And I think what I wanted to know is, is that really true?
So it's like, are all of these toxic posts attributable to a few rotten apples,
kind of in the periphery of the discipline, or
does this rot go all the way to the top?
Exactly.
So now it is math time.
Florian ropes in another friend, a mathy one, Paul Goldsmith Pinkham of Yale.
Kyle had figured out the easy way to crack the code on a single post, but
now they will have to do it at scale.
They will need to do a version of that puzzle to every comment on the site.
Which is an enormous task.
For every comment, there's a starting pool of 4.3 billion potential suspects.
4.3 billion possible IP addresses in the world that could have been responsible.
So they're gonna have to do that short, obvious puzzle a preposterous
three quadrillion times.
That's quadrillion with a Q.
On our very first attempt, it took us 230 hours.
Wait, the first time you crunched these numbers, it took 10 days?
Yeah, exactly.
It's the first time it took 10 days.
It's just once you program it, the code runs and you just wait.
And what happens when it's done?
Is there like a toaster sound?
Yeah, it sends you a message that the code that you ran is completed.
But that completed code still doesn't answer the question of which
IP address was responsible for any given post.
Because once those calculations are done, Florian and
the team are still left with around 65,000 IP addresses
that could have conceivably left any single comment.
65,000 down from 4.3 billion, but still.
So the next part of the process is to take the 65,000 possible IP addresses
for one single comment and to cross-reference them with these 65,000
possible IP addresses for every other comment across the site over the course of a week.
If an IP address is on the list of possibilities for one comment and
then again on the list of possibilities for another and then another,
it becomes more and more statistically likely that you found a real IP address
that was the source of multiple comments.
Those super posters are the signal in the mathematical noise.
Then you have for about 67% of all posts on EconJob Market Rumors,
you have an IP address associated with it.
And then you can start the analysis.
IP addresses for two-thirds of all the posts on the site,
which Florian and his colleagues could now plug into a sort of IP address directory.
These directories help narrow down which zip code a given IP address has come from.
They're not super accurate for locating an exact physical address within a city, but.
What is very, very accurate is the allocation to particular institutions.
Because they tend to have IP addresses specifically allocated to them and
that very, very rarely change.
And so that allows actually the identification of universities very,
very easily.
And when they narrowed it down to look at just the bad posts,
the racist and sexist stuff.
What they found was that the toxic posts on EconJob Market Rumors
were very much coming from within the house of economics,
from institutions across the discipline.
It's not that all the rotten apples are in one barrel, but
there's at least one rotten apple in every single barrel.
It's just everywhere.
Including many of the top institutions in the field.
Places like Stanford, Harvard, UChicago, even the Federal Reserve.
All of them seem to have contributed toxic comments to the EconJobs board.
It might be someone using the library computer.
Or it might be someone writing policy suggestions.
Or who will go on to work in the next presidential cabinet.
To Florian, this seems like an important enough finding that he was willing to
risk stirring the hornet's nest.
Did you imagine that your work might put you in kind of direct
confrontation with this online forum?
No, I never imagined this.
My work is on antitrust economics, but
I do enjoy confrontation a little bit.
So when I started doing this project, I was very much aware that I was
going to take on anonymous hoards.
But, you know, sticks and stones can break your bones, but words will never hurt me.
After the break, Florian reveals what he's found out about the ugly
id of economics to economics itself.
And everyone freaks out.
Hey, it's Kenny Malone with a quick but very sincere thank you
to our Planet Money Plus supporters and anybody else listening who
donates to public media.
After all, public media means you, the public, support it.
Everything you hear from the NPR network really cannot exist without your
contributions.
And for anybody listening who isn't a supporter yet, right now is a great time
to change that.
For you to get invested in creating a more informed public that is, after
all, our whole mission at NPR.
That's why we're here.
If you like perks, well, Planet Money Plus offers sponsor-free listening and
also bonus episodes of the show featuring extended interviews, behind the
scenes content and more.
And if you want to make a tax-deductible donation to your favorite station or
stations in the NPR network, that is fantastic as well.
What really matters is that you are part of the community that makes this
work possible.
Journalists across the NPR network need resources to do their best work.
And those resources have a cost.
Microphones, laptops, safety gear, software, and whatever amount you can
pitch in really does make a difference.
So please give today at donate.npr.org slash Planet Money.
You can also explore NPR Plus at plus.npr.org.
And thank you.
So Florian and his team found that toxic posts on econ job market
rumors are coming from everywhere in economics.
They're going to present their paper at a big conference put on by the
National Bureau of Economic Research.
And ahead of the presentation, Florian tweets out a little teaser.
He posts an abstract of the paper, which says that they've managed to
identify the majority of posts on the site, including ones that they have
categorized as toxic and that a lot of the posts are coming from
universities.
This was by far the most viral post I ever put out on Twitter.
I think it got something close to 2 million views and reached well, well,
well beyond economics.
And the economics world itself freaks out.
In particular, a lot of those individual posters on econ job
market rumors, including this one tenured professor who we are going
to call Terry.
Terry asked that we not reveal his identity, his real name or voice.
So we're going to use a voice actor for him.
He says he's worried there would be professional repercussions for having
posted on the site.
Even though he assures us he is, quote, a nobody.
I'm not like a super famous person.
I mean, most people in the field don't even know who I am.
So Terry found out about the econ jobs board over a decade ago.
And he says under the site's alleged cloak of anonymity, he had
passed along some insidery information about his academic
department's hiring decisions.
And he says he also engaged from time to time in some light
political trolling.
It wasn't racist or misogynist, but like I've made some posts where I
sound like a right wing extremist.
It's kind of like a Stephen Colbert.
Which meant that when he read Florian's tweet, Terry was
extremely distressed.
Terry feared that if his posts were unmasked, people wouldn't
understand that he'd been joking and that there might be real
professional consequences.
I was very stressed.
I was feeling dread because I had no idea like what information they
had, what they were going to release, what their timeline was.
For people who had posted on the econ jobs board, the worry seemed
to be if Florian and his team can identify specific universities
where some of the toxic posts were coming from, could they also
identify specific people who had made the posts?
Were they going to be doxing people who'd posted?
And this worry was exacerbated when, in a leaked early draft
of the researcher's presentation slides, one slide showed the IP
address of one anonymous user that the authors had managed to
identify, the site's administrator.
The econ jobs board itself was inundated with hundreds of
comments, puzzling, worrying, and fuming about the paper.
People were speculating about how Florian and his co-authors
got a hold of this information, whether this project might
fall afoul of academic ethics rules, or if it might even be illegal.
And they're freaking out not just because some of them had
posted racist, sexist stuff, but because some of them had also
posted all sorts of other kinds of sensitive information, in
which they say trash-talked their boss or posted about a
mental health crisis, even about considering suicide.
Stuff they posted because they believed they were anonymous.
So this past July, when the day finally comes for Florian
and Paul to present their findings, everyone is watching.
From people who'd been harassed and attacked on the jobs board,
to frequent posters fearing they were about to be doxed.
When Florian and Paul arrive at the Royal Sonesta Hotel
in Cambridge, Massachusetts, to present the paper, they
discover they've accidentally worn matching suits.
Welcome, everyone. OK.
And that they will have a packed audience.
I just wanted just to mention something a little bit different.
There is a reporter in the room.
The session is also being streamed on YouTube.
You know, we often sort of feel like we're just us in the room.
But actually, there may be quite a few people watching.
More than 2000 people have tuned in, which is pretty high
for an academic conference session.
So with that warning ahead, let me get the stage over to Florian.
Thank you very much, Catherine.
Thank you very much for everybody for coming.
Florian introduces the paper.
A very important topic for everybody in this room
and for everybody in our profession, namely toxic speech in economics.
And puts up on the screen behind him screenshots from the Econ jobs board.
Examples of useful posts on the site, like how to run nonlinearly squares
with fixed effects, mini tutorials economists offer up to each other.
To make your state of graphs more beautiful.
And then he puts up examples of the bad stuff.
Posts with sexist language and racial slurs.
And then he delivers the headline finding of their study.
These posts here come from IP addresses at Harvard, at Stanford,
at Yale, at Chicago, and even the NBR headquarters at 1050 Massif.
Florian goes on to explain to the audience the whole story.
How they'd figured out the site's method for anonymizing posters.
A allocation scheme that did not use the salt.
The tragicomic lack of salt.
It's a random secret that sort of gets added to the stuff that is.
And how they use statistics to identify which institutions
these toxic posts were coming from.
And I was also in plain sight for more than a decade.
As Terry and the thousands of other viewers watch from around the world,
it gradually becomes clear that this was as much as Florian and Paul
were going to reveal.
Just the names of universities and government offices.
No names of individual posters.
They had IP addresses, but nothing more granular.
And IP addresses are not people.
To even try to link an IP address to an individual,
somebody would need to sift through tons of posts
to collect biographical clues and triangulate them.
And that was just not part of the paper.
And as for that slide identifying the site administrator's IP address,
the only reason the researchers had been able to get that one
was because of a special setting the admin had used for one year
that allowed the researchers to link all of those posts together.
Also, the researchers took out that slide for their final presentation.
Instead of doxing anonymous Econ jobs board users,
what they're doing is kind of doxing the profession of economics itself.
This is pervasive.
It's everywhere.
And I think we should not look away.
Thank you very much for your time.
Great. So as we were doing before, line up at the mics.
There are a lot of questions.
And comments.
People ask about the terms they'd used in the paper.
Power users and power laws are like not showing up in your data.
Some of the questions are more technical about methodology.
So any changes on this behavior?
Some people just want to express their gratitude
to Florian and his colleagues for helping bring this problem out into the open.
I don't have a question.
I just want to say thank you.
Others want to take the findings into the real world.
There's a petition out there that has been signed by almost a thousand people
who have had slanderous comments made about them on the website.
If you are one of these people or you know...
That petition, started by a professor at UC San Diego,
asked the American Economic Association to explore ways to identify those responsible
for the worst posts, the threats and libel, stuff that is legally actionable,
so that the people who posted it could be held actually responsible.
And then after this flurry of comments and just a little over 50 minutes,
the presentation comes to an end.
Thank you very much for all your time and all your questions.
Thank you.
It has now been five months since that presentation.
For all the hubbub this summer, not a lot has changed.
None of the universities whose IP addresses showed up as the top 14 sources
for toxic posts seem to have taken any official action.
We emailed them to ask, and the few that did respond sent over statements
about being disappointed or not tolerating harassment.
Since news of the paper dropped, the Econ jobs board administrator
has changed how usernames are given out on the site.
Posters are now assigned the name of a famous economist
instead of a four-character code name.
A lot of people still posting on the site, along with its administrator,
see this paper in the context of freedom of speech and censorship.
They point out that there are real societal benefits to anonymity
for exposing things like wrongdoing, corruption, plagiarism,
and that there's a cost to undoing anonymity.
For his part, Florian Ederer says it was never his intention
to destroy the site.
He just wants economics to find a better way to talk to itself.
As for doing more to de-anonymize the toxic posters,
Florian does not see that as his role.
I think at that point, you're just veering too much into doxing, I think.
And then I have just bigger ethical concerns.
Would it be a net positive to expose the worst actors on that platform?
Perhaps, but in economics, we tend to think of trade-offs.
It is a trade-off, maybe, that I'm not willing to make at this point.
Florian does acknowledge that his work may have opened the door
for others who view those trade-offs differently.
Terry, the anonymous econ job rumors poster
who watched Florian's presentation with bated breath,
the whole thing has not convinced him to quit
the economics job market rumors site, or EJMR, as he calls it.
I think EJMR is bad for the econ profession.
I think it's bad for society.
I think the econ profession would be better without EJMR, right?
So if I could, like, you know, wave a magic wand and make it go away,
like, I would do that.
But, like, whether I visit the site or not, the site's going to exist.
And so that's kind of why I continue to visit the site.
Though he does now use a service that disguises his IP address, just in case.
Argentina has a new president who campaigned on the promise to dollarize his country,
make the U.S. dollar their new national currency.
An economist says there could be one big upside.
It's like tying yourself to the mast so as to not go towards the siren's call.
And the siren's call is print more pesos, print more pesos.
Right, exactly.
Why dollarize? How to do it?
And will it even work?
That's on the next Planet Money.
You can email us at planetmoney.npr.org
or we are on some of the social media platforms at atplanetmoney.
Today's episode was produced by Willa Rubin with help from James Snead and
Samuel Horace Kessler.
It was edited by Keith Romer, engineered by Josh Newell,
and fact-checked by Sierra Juarez.
Alex Goldmark is our executive producer.
Huge thank you to Katherine Tucker at MIT and to NPR One producer
Julian Ring for voicing Terry.
I'm Mary Childs. And I'm Alexi Horowitz-Ghazi.
This is NPR. Thanks for listening.
And a special thanks to our funder, the Alfred P. Sloan Foundation,
for helping to support this podcast.
