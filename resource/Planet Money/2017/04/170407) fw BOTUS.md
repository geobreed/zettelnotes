---
title: 170407) BOTUS
date: 20170407
tags: #PlanetMoney
citation: "“Planet Money,” _NPR_, 2 Juni 2023. [https://www.npr.org/podcasts/510289/planet-money](https://www.npr.org/podcasts/510289/planet-money) (diakses 4 Juni 2023)."
---

On today's show, we get in on the future of investing. We build an automated stock-trading bot. It analyzes the twitter feed of President Donald Trump, then trades stocks with real money. Our money. You can follow our bot on twitter, @BOTUS.

All across Wall Street, humans are being replaced by computers. Even the people who make decisions about which stocks to buy and sell are being replaced by computer programs, by bots.

To understand what goes on inside a stock-picking bot, we at Planet Money built our own.

Bots are cheaper than stock-picking humans. They're less emotional and more disciplined. They can process more information at once. They are doing things like scanning social media for consumer trends and counting the number of cars parked in Wal-Mart parking lots, then using that to trade.

Our bot is doing something seemingly simple: It looks at President Trump's Twitter feed, and when he tweets about a company, it trades stocks, with real money. Because the official Twitter handle of the president of the United States is @POTUS, we named our bot @BOTUS, bot of the United States. There's $1,000 on the line invested by the staff members of the Planet Money podcast from their personal funds. Follow along, and track whether we're making money or losing it.
Sponsor Message

Music: "Rapture" and "Now Son." Find us: Twitter/ Facebook. Subscribe to our show on iTunes or PocketCast.

See what BOTUS has been up to lately:
Tweets by BOTUS

The Fine Print: This is for real. All decisions on buying and selling stocks are made automatically by BOTUS, a computer program. BOTUS makes trades by analyzing tweets from @realDonaldTrump to recognize when he mentions a publicly traded company. BOTUS also measures the sentiment using VADER Sentiment Analysis. If BOTUS decides a tweet is positive, it will buy the stock mentioned in the tweet; if BOTUS decides the tweet is negative, it will sell the stock short. BOTUS will hold the position for 30 minutes, then get out. BOTUS was built with Tradeworx and trades through the Interactive Brokers platform.
When Trump Tweets, This Bot Makes Money
Technology
When Trump Tweets, This Bot Makes Money



----

https://www.npr.org/sections/money/2017/04/07/522897876/meet-botus-planet-money-s-stock-trading-twitter-bot

https://www.npr.org/transcripts/522897876



ALEX GOLDMARK, HOST:

We've been working on this episode for a long while. We had it ready to go. And then, like the rest of the world, we got news that President Trump had ordered missile strikes in Syria. Today's show is in part about responding to unpredictability, and we thought of changing the whole show based on the news. But then we thought, actually, it is completely in the spirit of this episode to hit publish on it just as it was originally prepared. Here we go.

Last week, the biggest investment firm in the world laid off a bunch of its top stock pickers and replaced them with computer programs. This is happening all over Wall Street. Firms are moving away from having humans decide what stocks to buy and sell and towards having humans program computers and then letting the computers decide what to buy and sell. Computers are cheaper than humans. They are more disciplined. They can think about more things at once. Like, they can scan Facebook for trends, they can count the number of cars in Wal-Mart parking lots, and then use all that to figure out what stock to buy and sell and do it automatically. This is the way the world is going. This is what the stock market is becoming.

And I want in. I want to see this world from the inside. I want to build a machine that will buy and sell stocks for me automatically based on some cold, hard data out there in the world, no wild human emotions. And I want my machine to do it based on the tweets of President Donald J. Trump.

(SOUNDBITE OF BEN SUMNER, GLENN HERWEIJER AND KONSTANTINOS PAPALEXOPOULOS SONG, "RAPTURE")

GOLDMARK: Hello and welcome to PLANET MONEY. I'm Alex Goldmark.

JACOB GOLDSTEIN, HOST:

And I'm Jacob Goldstein. Today on the show PLANET MONEY builds a robot, a bot to trade stocks with real money.

GOLDMARK: We have no idea what will happen.

(SOUNDBITE OF BEN SUMNER, GLENN HERWEIJER AND KONSTANTINOS PAPALEXOPOULOS SONG, "RAPTURE")

GOLDSTEIN: So there is a thing that often happens when President Trump tweets about a company. When he says something positive about a company, the stock price tends to go up, at least for a little while. When he says something negative, the stock price tends go down.

GOLDMARK: So here's what I want to do. I want to build a computer program that monitors President Trump's tweets. And when he says something nice about a company, we buy that company's stock. And when President Trump tweets something negative about a company, we will sell that company's stock short. What that just means is that we will set ourselves up to make a profit if the stock price goes down.

GOLDSTEIN: If you've listened to PLANET MONEY for a while you know that we sometimes make investments with our own money. Not with NPR's money, but, like, my money, your money, our personal money. And we do this so we can, you know, get into the world for real, feel how the world works.

GOLDMARK: Got to have skin in the game. For this project, I did some math and I figured out that I needed $100 from each member of PLANET MONEY to make it work. So I went around the office with my pitch, starting with Noel King.

NOEL KING, BYLINE: Terrific. This is a great idea.

GOLDMARK: Great idea, right?

KING: Yeah.

GOLDMARK: OK, so you're in?

KING: Yeah, yeah, yeah. How much do I owe you?

GOLDMARK: One hundred dollars.

KING: Wait, you really need 100 bucks from me? That's not going to happen. I pay rent in New York. I'm not giving you a $100.

GOLDMARK: You'll get it back and then some.

KING: And then some. Yeah, all right, I'll break your kneecaps.

GOLDMARK: That is roughly how it went all around the office. Jacob, I'm going to play you the tape of when I pitched it to you.

We are going to build a stock trading bot that will trade off of Donald Trump's tweets. You know how he does these tweets?

GOLDSTEIN: Everything that I have learned about economics suggests to me that that's not going to work.

GOLDMARK: OK, but let me tell you why...

I was undeterred.

GOLDSTEIN: You did get my $100. But let me just explain myself briefly. My basic view of the world is if there's some way to make money out there somebody's already doing it. Somebody's already got their Trump bot. I don't believe that we can build a better Trump bot.

GOLDMARK: But we're going to try.

GOLDSTEIN: Sure. No, look, obviously I'm in. I'm not in it for the money. I'm in it for the ride, for the delight.

GOLDMARK: And I gladly took your skeptical $100. I got my $1,000 from my other skeptical colleagues. I took everybody's money, I put it in a trading account. And then I did the one more very important thing before we could get started. I named our bot.

GOLDSTEIN: Go on.

GOLDMARK: Our bot will be called BOTUS.

GOLDSTEIN: I see what you did there.

GOLDMARK: B-O-T-U-S. So you know how the president's Twitter handle...

GOLDSTEIN: POTUS, president of the U.S.

GOLDMARK: The official Twitter handle, yeah. BOTUS, bot of the United States.

GOLDSTEIN: OK.

GOLDMARK: B-O-T-U-S.

GOLDSTEIN: OK. It's good. Yeah. I'm kind of proud of it. But now you've got to, like, build the thing, right? Now you've got to make the machine.

GOLDMARK: So I found some professional help. I found a company that builds bots and helps other companies with their trading technology. It is called Tradeworx with an X...

GOLDSTEIN: Of course there's an X.

GOLDMARK: ...At the end of it. Their office is in New Jersey, about 90 minutes outside of New York City on a commercial strip. It's, like, very low key. I went there to meet with Mani Mahjouri, their head of investing. He runs a whole team of people making all kinds of bots. And he is very secretive about what those bots do, but he explained to me the essence of trading with bots.

MANI MAHJOURI: You know, if you take a simple idea and do it 3,000 times four times a year, it doesn't have to be right that - it can be, like, just slightly right, you know? And over time it's like a casino except you're the house.

GOLDSTEIN: Yeah, we only have to be right, like, 51, 52 percent of the time, right? We can be wrong a lot as long as we're right a little more often than we're wrong. And we make a lot of bets, we'll make a lot of money.

GOLDMARK: You're starting to come around.

GOLDSTEIN: OK, slightly less skeptic.

GOLDMARK: I like that. So I told him my idea, to get a bot to read Trump's tweets and then buy and sell stocks based on that. And he said first problem - can the computer read Trump's tweets? Can it figure out whether the president is saying something nice or saying something mean?

MAHJOURI: This is - this is the - this is more than just positive and negative words. This is a computer actually determining the sentiment of a tweet. You can type any sentence in and it will give you a sense of what the sentiment is.

GOLDMARK: And this is just an algorithm you have lying around the office.

MAHJOURI: More or less.

GOLDSTEIN: Computers have gotten much better at doing this kind of thing over the past few years. It's called sentiment analysis. And companies use it a lot with social media to figure out how people feel about movies and new products and whatever.

GOLDMARK: It's so common now that Mani and his team had already done a little test by the time I showed up. They had run hundreds of Donald Trump's tweets through this algorithm, this computer program that they use to find the sentiment. And then when I got there it was time for us humans to check the computer's work, to see how often it found the right answer.

MAHJOURI: Do you want to pull up our scores?

GOLDMARK: Sure.

So let me give you an example, Jacob. The computer, it read this tweet from January. Quote, "Toyota Motor said will build new plant in Baja, Mexico, to build Corolla cars for U.S. No way," exclamation mark - and that's in caps - "build plant in U.S. or pay big border tax."

GOLDSTEIN: My gut check says that is negative.

GOLDMARK: Humans say negative, computers say negative.

GOLDSTEIN: OK, so the algorithm got this one right.

GOLDMARK: It got a lot of them right. We looked through the list, one after another after another, and almost every time the algorithm got it right.

MAHJOURI: And a really interesting thing about Donald Trump is those algorithms work really well because he uses words like bad and sad and great, you know, and they always mean what he means them to mean. So from that perspective he makes it really easy for computers.

GOLDSTEIN: He's not subtle.

GOLDMARK: Easy for a computer to read, which means our trading bot, BOTUS, passed the first test. I was feeling pretty good and so was Mani.

MAHJOURI: Yeah, this is definitely doable.

GOLDMARK: So that was a few weeks ago. And after I left their offices that is when the real work started, when they got down to making BOTUS. And Mani handed over the project to one of his programmers, a person named Camilo Jimenez. And it started out fine. Camilo did what he usually does when he's researching. He started in his home office at a little wood desk in his bedroom. He keeps it simple.

CAMILO JIMENEZ: It's just my laptop, coffee and notepad. That's basically it.

GOLDMARK: Laptop, notepad and some coffee. That's what you need.

JIMENEZ: Yeah, that's all you need.

GOLDMARK: OK.

JIMENEZ: Sometimes Red Bull, yeah.

GOLDSTEIN: Sometimes Red Bull.

GOLDMARK: Yeah.

GOLDSTEIN: Classic - sort of a parody of a coder.

GOLDMARK: Except he's a physicist by training, so not such a classic programmer.

GOLDSTEIN: So - OK, so we already know that the bot can tell nice from mean. What's, like, the next step?

GOLDMARK: The next thing he has to be able to do is be able to tell what company Trump is tweeting about.

GOLDSTEIN: That one sounds, like, relatively easy to me.

GOLDMARK: Nope.

JIMENEZ: That's very hard. That's easy for a human. That's very hard for a computer because the text could include either the name of a person or the company or the product and you have to link that to a company.

GOLDMARK: So is Donald Trump just saying he ate an apple for lunch or is he talking about Apple computers?

JIMENEZ: Correct. That's a really good case.

GOLDMARK: So this is what making a bot is, puzzle solving over and over. For something like Apple stock versus apple the food, Camilo had to do something to train our bot to tell them apart. So he added what's called a context algorithm, right? He had our bot, our little bot read a whole bunch of financial articles about Apple the company and learn the kinds of things, the kind of words and phrases and topics associated with the company Apple.

GOLDSTEIN: Uh-huh (ph). Cupertino. Steve Jobs. Tim Cook. iPhone.

GOLDMARK: Exactly.

GOLDSTEIN: Uh-huh.

GOLDMARK: And the things that are not associated with the company but with apple the food.

GOLDSTEIN: Crunchy. Mushy. Delicious.

GOLDMARK: Our bot might accidentally short Red Delicious.

GOLDSTEIN: I actually would short Red Delicious. I think that would be a great call. I still think it's overvalued.

GOLDMARK: I'm long on Fuji. OK, our bot, it can now tell the difference.

GOLDSTEIN: But what about Honeycrisp?

GOLDMARK: We're - let's get back on task here. Focus. Focus on our bot, OK? Our bot can tell the difference between apple the fruit and Apple the the company.

GOLDSTEIN: OK.

GOLDMARK: Right? It's a victory. Now, there are a few types of companies that were especially hard to deal with. One of them that's worth talking about - Trump tweets about the media all the time, but that's because he is commenting on the media. He's not saying, like, I am threatening to put some tax on newsprint...

GOLDSTEIN: Right.

GOLDMARK: ...That will affect the business.

GOLDSTEIN: He's saying, I don't like the story that was on the newsprint.

GOLDMARK: Right. And it usually doesn't affect the stock price of a media company. So Camilo decided media companies - not in our trading universe.

GOLDSTEIN: This is interesting to me because this is like the human decision making, right? So, you know, we proposed this thing as like, well, it's just going to be a machine. But once you actually have to make the machine, you have to tell the machine how to think. The machine in this case is not exactly thinking for itself, right? Camilo is the - is a human being and he is setting up a set of decisions based on his - Camilo's - human judgment.

GOLDMARK: Well, it's a mix of his judgment and the computer's. The machine really is making decisions. It is learning about Apple. It is interpreting language. It's just that in some places humans have stepped in and said some puzzles, they would just take way too long to solve. Not worth it. For instance, I want to give you this one. I love it. There is this one company that the bot could not recognize. You want to guess what it was?

GOLDSTEIN: I'm very excited. I have - give me a clue.

GOLDMARK: It is very close to Donald Trump physically and emotionally.

GOLDSTEIN: Is it Boeing? They make Air Force One.

GOLDMARK: No. Here is Camilo's boss, Mani, again.

MAHJOURI: We - in our production algorithm we won't trade the company Tiffany's 'cause the computer can't tell when Trump is talking about his daughter and when he's talking about the actual company.

GOLDSTEIN: Oh, right, Tiffany Trump, the lesser-known Trump daughter.

GOLDMARK: And Tiffany's the jeweler, which is just down the block from Trump Tower on Fifth Avenue. Our bot, it will not trade Tiffany's. That's the decision they made, which is fine. No big deal.

GOLDSTEIN: So OK, our machine, or BOTUS-to-be, it can A, tell when the president is being positive or negative, saying nice things or mean things. And B, it can figure out what companies the president is tweeting about.

GOLDMARK: The last thing we have to tell it is how soon after the tweet to buy - and how long do we hold it for?

GOLDSTEIN: OK.

GOLDMARK: Do we buy it and keep it?

GOLDSTEIN: No.

GOLDMARK: Do we buy it and sell it right away?

GOLDSTEIN: Yes.

GOLDMARK: OK. But right away - what does that mean? This is not an obvious question. So Mani sets up a test. He makes a simulation of the stock market, the whole stock market in the past few months. He adds in Trump's tweets and then he runs our bot through that. So it's like going back in time to see what our bot would have done if it had existed a few months ago.

GOLDSTEIN: And to be clear, our bot did not exist a few months ago. This is not trading with real money. This is just a test.

GOLDMARK: He runs it over and over again, tweaking the variable of when to buy and when to sell each time he runs it.

MAHJOURI: I was in my office at my desk, late for dinner and worried about that. And - but I remember sitting there and saying, you know, here are some options, you know, that we could try. We could try holding it overnight. We can try holding it for a little while. You know, we can try holding it for days.

GOLDMARK: What his simulation pointed to was get in and get out relatively fast. But it's not like the exact number of minutes mattered all that much.

MAHJOURI: You know, and so that made us feel good because that made us say, like, well, it's not like if I hold this thing for 30 minutes there's something magic about 30 minutes or if I hold it for 40 minutes there's something broken. It turned out that what mattered most was, you know, getting reasonably close to when the tweet happened, you know, and trying to get out by the end of the day.

GOLDMARK: So that is what BOTUS will do. When Donald Trump tweets about a company, BOTUS will buy a stock right away. Not in milliseconds like some high-speed trading bots that you might have heard about, just, you know, pretty much right away. It'll take, like, a few seconds, and then 30 minutes after that the bot will sell. We'll be out. The last time I talked to Mani he showed me this chart. He showed me how much money we would have made if we had launched right after the election. To be clear, we did not launch then. This is just, again, his simulation. It's more like the ad for our bot than the report card.

OK, so now I'm looking at a chart of how much money we're going to make. And what it looks like is you - it flatlines and then it shoots up really fast. Presumably, I guess, that's when there's a tweet and we make money. And then there's another flatline for a while. And then it shoots up again. Oh, there's one where it goes down. Oh, there's two where - there's a couple where it goes down. But overall it looks like we are on the slow and steady path towards riches on this chart. Am I interpreting it right?

MAHJOURI: You are interpreting it optimistically right, yes.

GOLDMARK: (Laughter) That's what I do when I'm investing. I'm not a very good investor.

But Mani said it did pass the bar for him, that if it were his bot he would start trading real money.

MAHJOURI: You know, we're - we feel good about the strategy. You know, and...

GOLDMARK: Can you say that with a little more confidence? You're...

MAHJOURI: I can't.

GOLDMARK: You're saying it to me like...

MAHJOURI: I can't, no, because...

GOLDMARK: Like you don't really believe it.

MAHJOURI: No, no, no, I just - I don't want to overstate - I don't want to understate the risk and I don't want to overstate the benefit of doing something like this. I just feel like, you know, it's not - we haven't scientifically proven anything.

GOLDSTEIN: I like this guy. Like, I respect this guy. I - it actually gives me more confidence that he is skeptical, that he's like, well, we don't really know. Maybe it's fluky. I mean, that is what he's saying here. And, like, that makes me like him more.

GOLDMARK: What was really interesting about talking with him about strategy is that he's very clearly driven by the scientific method, that he wants to pose a hypothesis and test it, follow the data. But he understands that that has major limitations because if you wait around for the data to be just right you're going to miss a lot of opportunities.

GOLDSTEIN: That is absolutely true. You have just described my life.

MAHJOURI: You know, there's just a practical aspect of it, which is, you know, like, so, you know, if you had this as an option, you know, to invest some of your money in, like, doesn't this seem like a good bet?

GOLDMARK: Yes. Today, at the moment we publish this podcast, we are pushing go on our bot, BOTUS.

GOLDSTEIN: It will start trading real money, our real money.

GOLDMARK: So if you are listening to this podcast it means the machine is live.

(SOUNDBITE OF PODINGTON BEAR'S "NOW SON")

GOLDMARK: You can follow BOTUS in the real world. How to do it after this.

(SOUNDBITE OF PODINGTON BEAR'S "NOW SON")

GOLDMARK: BOTUS is more than a stock trading bot. It also tweets. You can follow @BOTUS on Twitter, @B-O-T-U-S. And you will see every trade that we make, how we're doing, plus a few other little surprises we put in there.

GOLDSTEIN: And once BOTUS starts trading you will also be able to follow along on our website, npr.org/planetmoney.

GOLDMARK: We genuinely don't know what's going to happen. We could make money. We could lose money. Trump could stop tweeting about companies.

GOLDSTEIN: Perhaps the least interesting option for us.

GOLDMARK: But if there is something interesting we will let you know about it on the website, on the Twitter account and right here on the podcast.

GOLDSTEIN: Today's show was produced by Sally Helm and edited by Bryant Urstadt.

GOLDMARK: Big thanks to Mani and Camilo and everyone at Tradeworx who helped build our bot and then endured all of my questions in the weeks after. And to Interactive Brokers, who let us set up a very small trading account without charging us extra fees, also Kevin McPartland and Robert Mata and the folks at the NPR visual and digital teams.

GOLDSTEIN: If you're looking for something else to listen to, try Up First. It's NPR's newest podcast. It is a daily news show hosted by some of the biggest names at NPR - David Greene, Steve Inskeep, Rachel Martin. It's called Up First. And you can find it at npr.org/podcasts, on the NPR One app or wherever you get your podcasts. I'm Jacob Goldstein.

GOLDMARK: And I'm Alex Goldmark. Thanks for listening.

(SOUNDBITE OF PODINGTON BEAR'S "NOW SON," BELL)

GOLDSTEIN: Footnotes.

GOLDMARK: Footnotes. We got some footnotes. OK, footnote number one. One detail of those tweets that the computer analyzed to figure out which were positive and which were negative. The most negative of all of the tweets scored by the computer, it was about "Saturday Night Live." It goes @NBCNews is bad, but "Saturday Night Live" is the worst of NBC. Not funny. Cast is terrible. Always a complete hit job. Really bad television.

GOLDSTEIN: Bad. Terrible. Really bad. Worst.

(SOUNDBITE OF BELL)

GOLDMARK: Footnote number two. Number two, on Tiffany's the company and Tiffany's the stock, Donald Trump's daughter is reportedly named after Tiffany's the company. And Trump bought the air rights over Tiffany's the store, which is what enabled him to build Trump Tower as tall as it is. Boom.

(SOUNDBITE OF PODINGTON BEAR'S "NOW SON")

Copyright © 2017 NPR. All rights reserved. Visit our website terms of use and permissions pages at www.npr.org for further information.

NPR transcripts are created on a rush deadline by an NPR contractor. This text may not be in its final form and may be updated or revised in the future. Accuracy and availability may vary. The authoritative record of NPR’s programming is the audio record.

----

**faster whisper:**
Last week, the biggest investment firm in the world laid off a bunch of its top stock pickers and replaced them with computer programs.
This is happening all over Wall Street.
Firms are moving away from having humans decide what stocks to buy and sell and towards having humans program computers and then letting the computers decide what to buy and sell.
Computers are cheaper than humans. They are more disciplined. They can think about more things at once.
They can scan Facebook for trends. They can count the number of cars in Walmart parking lots and then use all that to figure out what stock to buy and sell and do it automatically.
This is the way the world is going. This is what the stock market is becoming.
And I want in.
I want to see this world from the inside. I want to build a machine that will buy and sell stocks for me automatically based on some cold hard data out there in the world.
No wild human emotions.
And I want my machine to do it based on the tweets of President Donald J. Trump.
Hello and welcome to Planet Money. I'm Alex Goldmark.
And I'm Jacob Goldstein.
Today on the show Planet Money builds a robot, a bot, to trade stocks with real money.
We have no idea what will happen.
Support for Planet Money and the following message come from Wonder Capital.
Wonder Capital's online investment platform allows you to invest in solar energy projects across the U.S., earn up to 8.5% annually while diversifying your portfolio and combating global climate change.
In fact, investors like you financed 40 large scale solar projects in 2016, offsetting the CO2 emissions from 2.8 million pounds of burned coal.
Create an account for free at wondercapital.com slash planet money.
So there is a thing that often happens when President Trump tweets about a company.
When he says something positive about a company, the stock price tends to go up, at least for a little while.
When he says something negative, the stock price tends to go down.
So here's what I want to do. I want to build a computer program that monitors President Trump's tweets.
And when he says something nice about a company, we buy that company stock.
And when President Trump tweets something negative about a company, we will sell that company stock short.
What that just means is that we will set ourselves up to make a profit if the stock price goes down.
If you've listened to Planet Money for a while, you know that we sometimes make investments with our own money, not with NPR's money, but like my money, your money, our personal money.
And we do this so we can, you know, get into the world for real, feel how the world works.
Gotta have skin in the game. For this project, I did some math, and I figured out that I needed $100 from each member of Planet Money to make it work.
So I went around the office with my pitch, starting with Noelle King.
Terrific! It's a great idea.
Great idea, right?
Yeah.
Okay, so you're in?
Yeah, yeah, yeah. How much do I owe you?
$100.
Wait, you really need $100 from me? That's not gonna happen. I pay rent in New York. I'm not giving you $100.
You'll get it back, and then some.
And then some, yeah. All right, I'll break your kneecaps.
That is roughly how it went all around the office. Jacob, I'm gonna play you the tape of when I pitched it to you.
We are going to build a stock trading bot that will trade off of Donald Trump's tweets. You know how he does these tweets?
Everything that I have learned about economics suggests to me that that's not gonna work.
Okay, but let me tell you why I was undeterred.
You did get my $100, but let me just explain myself briefly.
My basic view of the world is if there's some way to make money out there, somebody's already doing it.
Somebody's already got their Trump bot. I don't believe that we can build a better Trump bot.
But we're gonna try?
Sure. No, look, obviously I'm in. I'm not in it for the money. I'm in it for the ride, for the delight.
And I gladly took your skeptical $100. I got my $1,000 from my other skeptical colleagues.
I took everybody's money. I put it in a trading account.
And then I did the one more very important thing before we could get started.
I named our bot.
Go on.
Our bot will be called BOTUS.
I see what you did there.
B-O-T-U-S. So you know how the president's Twitter handle?
POTUS, president of the U.S.?
The official Twitter handle, yeah. BOTUS, bot of the United States.
Okay.
B-O-T-U-S.
Okay, that's good. Yeah, I'm kind of proud of it. But now you gotta like build the thing, right?
Now you gotta make the machine.
So I found some professional help.
I found a company that builds bots and helps other companies with their trading technology.
It is called TradeWorks with an X at the end of it.
Their office is in New Jersey about 90 minutes outside of New York City on a commercial strip.
It's like very low key.
I went there to meet with Mani Majori, their head of investing.
He runs a whole team of people making all kinds of bots.
And he is very secretive about what those bots do.
But he explained to me the essence of trading with bots.
You know, if you take a simple idea and do it 3,000 times, 4 times a year,
it doesn't have to be right. It can be like just slightly right.
And over time, it's like a casino, except you're the house.
Yeah, we only have to be right like 51, 52% of the time, right?
We can be wrong a lot, as long as we're right a little more often than we're wrong.
And we make a lot of bets, we'll make a lot of money.
You're starting to come around.
I'm slightly less skeptical.
I like that.
So I told him my idea to get a bot to read Trump's tweets and then buy and sell stocks based on that.
And he said, first problem, can the computer read Trump's tweets?
Can it figure out whether the president is saying something nice or saying something mean?
This is more than just positive and negative words.
This is a computer actually determining the sentiment of a tweet.
You can type any sentence in and it will give you a sense of what the sentiment is.
And this is just an algorithm you have lying around the office, more or less.
Computers have gotten much better at doing this kind of thing over the past few years.
It's called sentiment analysis.
And companies use it a lot with social media to figure out how people feel about movies and new products and whatever.
It's so common now that Monty and his team had already done a little test by the time I showed up.
They had run hundreds of Donald Trump's tweets through this algorithm, this computer program they use to find the sentiment.
And then when I got there, it was time for us humans to check the computer's work to see how often it found the right answer.
Do you want to pull up our scores?
Sure.
So let me give you an example, Jake.
The computer, it read this tweet from January.
Quote, Toyota Motor said we'll build new plant in Baja, Mexico to build Corolla cars for U.S.
No way! Exclamation mark, and that's in caps.
Build plant in U.S. or pay big border tax?
My gut check says that is negative.
Humans say negative, computers say negative.
OK, so the algorithm got this one right.
It got a lot of them right.
We looked through the list, one after another after another, and almost every time the algorithm got it right.
And a really interesting thing about Donald Trump is those algorithms work really well because he uses words like bad and sad and great.
And they always mean what he means them to mean.
So from that perspective, he makes it really easy for computers.
It's not subtle.
Easy for a computer to read, which means our trading bot, Bodus, passed the first test.
I was feeling pretty good, and so was Mani.
Yeah, this is definitely doable.
So that was a few weeks ago, and after I left their offices, that is when the real work started, when they got down to making Bodus.
And Mani handed over the project to one of his programmers, a person named Camilo Jimenez.
And it started out fine.
Camilo did what he usually does when he's researching.
He started in his home office at a little wood desk in his bedroom.
He keeps it simple.
Just my laptop, coffee, notepad.
That's basically it.
Laptop, notepad, and some coffee.
That's what you need.
That's all you need.
Okay.
Sometimes Red Bull, yeah.
Sometimes Red Bull.
Classic.
Sort of a parody of a coder.
Except he's a physicist by training, so not such a classic programmer.
Okay, so we already know that the bot can tell nice from mean.
What's like the next step?
The next thing he has to be able to do is be able to tell what company Trump is tweeting about.
That one sounds like relatively easy to me.
Nope.
That's very hard.
That's easy for a human.
That's very hard for a computer.
Because the text could include either the name of a person or the company or a product.
And you have to link that to a company.
So is Donald Trump just saying he ate an apple for lunch or is he talking about apple computers?
Correct.
That's a really good case.
So this is what making a bot is.
Puzzle solving.
Over and over.
For something like Apple stock versus Apple the food, Camillo had to do something to train our bot to tell them apart.
So he added what's called a context algorithm.
He had our bot, our little bot, read a whole bunch of financial articles about Apple the company and learn the kinds of things,
the kind of words and phrases and topics associated with the company Apple.
Cupertino, Steve Jobs, Tim Cook, iPhone.
Exactly.
And the things that are not associated with the company but with Apple the food.
Crunchy, mushy, delicious.
Our bot might accidentally short read delicious.
I actually would short read delicious.
I think that would be a great call.
I still think it's overvalued.
I'm long on Fuji.
Okay.
Our bot, it can now tell the difference.
But what about Honeycrisp?
Well, let's get back on task.
It's a harder case.
Focus.
Focus on our bot.
Okay.
Our bot can tell the difference between Apple the fruit and Apple the company.
Okay.
Right?
It's a victory.
Now there are a few types of companies that were especially hard to deal with.
One of them is we're talking about Trump tweets about the media all the time.
But that's because he is commenting on the media.
He's not saying like I am threatening to put some tax on newsprint that will affect the business.
He's saying I don't like the story that was on the newsprint.
Right.
And it usually doesn't affect the stock price of a media company.
So Camillo decided media companies not in our trading universe.
This is interesting to me because this is like the human decision making.
Right.
So, you know, we propose this thing as like, well, it's just going to be a machine.
But once you actually have to make the machine, you have to tell the machine how to think.
The machine in this case is not exactly thinking for itself.
Right.
Camillo is a human being and he is setting up a set of decisions based on his Camillo's human judgment.
Well, it's a mix of his judgment and the computer's.
The machine really is making decisions.
It is learning about Apple.
It is interpreting language.
It's just that in some places, humans have stepped in and said some puzzles.
They would just take way too long to solve.
Not worth it.
For instance, I want to give you this one.
I love it.
There is this one company that the bot could not recognize.
You want to guess what it was?
I'm very excited.
Give me a clue.
Give me a clue.
It is very close to Donald Trump physically and emotionally.
Is it Boeing?
They make Air Force One.
No.
Here is Camillo's boss, Mani, again.
In our production algorithm, we won't trade the company Tiffany's because the computer can't tell when Trump is talking about his daughter
and when he's talking about the actual company.
All right. Tiffany Trump, the lesser known Trump daughter.
And Tiffany's the jeweler, which is just down the block from Trump Tower on Fifth Avenue.
Our bot, it will not trade Tiffany's.
That's the decision they made, which is fine.
No big deal.
So, okay.
Our machine, our bonus to be, it can A, tell when the president is being positive or negative, saying nice things or mean things.
And B, it can figure out what companies the president is tweeting about.
The last thing we have to tell it is how soon after the tweet to buy and how long do we hold it for.
Okay.
Do we buy it and keep it?
No.
Do we buy it and sell it right away?
Yes.
Okay.
But right away, what does that mean?
This is not an obvious question.
So Mani sets up a test.
He makes a simulation of the stock market, the whole stock market in the past few months.
He adds in Trump's tweets and then he runs our bot through that.
So it's like going back in time to see what our bot would have done if it had existed a few months ago.
And to be clear, our bot did not exist a few months ago.
This is not trading with real money.
This is just a test.
He runs it over and over again, tweaking the variable of when to buy and when to sell each time he runs it.
I was in my office at my desk, late for dinner, and worried about that.
But I remember sitting there and saying, you know, here are some options that we could try.
We could try holding it overnight.
We could try holding it for a little while.
We could try holding it for days.
What his simulation pointed to was get in and get out relatively fast.
But it's not like the exact number of minutes mattered all that much.
You know, and so that made us feel good because that made us say like, well, it's not like if I hold this thing for 30 minutes,
there's something magic about 30 minutes or if I hold it for 40 minutes, there's something broken.
It turned out that what mattered most was, you know, getting reasonably close to when the tweet happened, you know,
and trying to get out by the end of the day.
So that is what Botus will do.
When Donald Trump tweets about a company, Botus will buy a stock right away,
not in milliseconds like some high-speed trading bots that you might have heard about, just, you know, pretty much right away.
It'll take like a few seconds.
And then 30 minutes after that, the bot will sell.
We'll be out.
The last time I talked to Mani, he showed me this chart.
He showed me how much money we would have made if we had launched right after the election.
To be clear, we did not launch them.
This is just, again, his simulation.
It's more like the ad for our bot than the report card.
Okay, so now I'm looking at a chart of how much money we're going to make.
And what it looks like is you flat lines and then it shoots up really fast.
Presumably, I guess that's when there's a tweet and we make money.
And then there's another flat line for a while.
And then it shoots up again.
Oh, there's one where it goes down.
There's two where it goes down.
There's a couple where it goes down.
But overall, it looks like we are on the slow and steady path towards riches on this chart.
Am I interpreting it right?
You are interpreting it optimistically right, yes.
That's what I do when I'm investing.
I'm not a very good investor.
But Mani said it did pass the bar for him.
That if it were his bot, he would start trading real money.
You know, we feel good about the strategy.
Can you say that with a little more confidence?
You're saying it to me like you don't really believe it.
No, no, no.
I just I don't want to overstate.
I don't want to understate the risk.
I don't overstate the benefit of doing something like this.
I just feel like, you know, it's not we haven't scientifically proven anything.
I like this guy.
Like I respect this guy.
It actually gives me more confidence that he is skeptical.
He's like, well, we don't really know.
Maybe it's fluky.
I mean, that is what he's saying here.
And like that makes me like him more.
What was really interesting about talking with him about strategy is that he's very clearly driven by the scientific method that he wants to pose a hypothesis and test it, follow the data.
But he understands that that has major limitations because if you wait around for the data to be just right, you're going to miss a lot of opportunities.
That is absolutely true.
You have just described my life.
You know, there's just a practical aspect of it, which is, you know, like, so, you know, if you had this as an option, you know, to invest some of your money in, like, doesn't this seem like a good bet?
Yes.
Today, at the moment we publish this podcast, we are push and go on our bot, BOTUS.
It will start trading real money, our real money.
So if you are listening to this podcast, it means the machine is live.
You can follow BOTUS in the real world.
How to do it after this support for this podcast and the following message come from the Economic Development Authority of Fairfax County, Virginia, home to more than 350 cyber companies and 8900 technology related firms.
Details at power of ideas dot org.
BOTUS is more than a stock trading bot.
It also tweets.
You can follow at BOTUS on Twitter at BOTUS and you will see every trade that we make, how we're doing, plus a few other little surprises we put in there.
And once BOTUS starts trading, you will also be able to follow along on our website and PR dot org slash money.
We genuinely don't know what's going to happen.
We could make money.
We could lose money.
Trump could stop tweeting about companies, perhaps the least interesting option for us.
But if there is something interesting, we will let you know about it on the website, on the Twitter account and right here on the podcast.
Today's show was produced by Sally Helm and edited by Brian Urstead.
Big thanks to Mani and Camilo and everyone at TradeWorks who helped build our bot and then endured all of my questions in the weeks after.
And to interactive brokers who let us set up a very small trading account without charging us extra fees.
Also Kevin McPartland and Robert Mata and to the folks at the NPR visual and digital teams.
If you're looking for something else to listen to, try up first.
It's NPR's newest podcast.
It is a daily news show hosted by some of the biggest names at NPR.
David Green, Steve Inskeep, Rachel Martin.
It's called Up First and you can find it at NPR dot org slash podcast on the NPR one app or wherever you get your podcasts.
I'm Jacob Goldstein.
And I'm Alex Goldmann.
Thanks for listening.
Footnotes.
We got some footnotes.
OK, footnote number one.
One detail of those tweets that the computer analyzed to figure out which were positive and which were negative.
The most negative of all of the tweets scored by the computer.
It was about Saturday Night Live.
It goes at NBC News is bad, but Saturday Night Live is the worst of NBC.
Not funny.
Cast is terrible.
Always a complete hit job.
Really bad television.
Bad.
Terrible.
Really bad.
Worst.
Footnote number two.
Number two.
On Tiffany's the company and Tiffany's the stock, Donald Trump's daughter is reportedly named after Tiffany's the company and Trump bought the air rights over Tiffany's the store, which is what enabled him to build Trump Tower as tall as it is.
Boom.
