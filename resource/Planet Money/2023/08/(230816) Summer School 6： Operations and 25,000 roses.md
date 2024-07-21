---
title: (230816) Summer School 6： Operations and 25,000 roses
date: 20230816
tags: #PlanetMoney
citation: “Planet Money,” _NPR_, 2 Juni 2023. [https://www.npr.org/podcasts/510289/planet-money](https://www.npr.org/podcasts/510289/planet-money) (diakses 4 Juni 2023).
---


----
# Points

- 

----
# Article
https://www.npr.org/2023/08/16/1194249897/summer-school-operations-capacity-variability-newsvendor-model
"It's difficult to control everything," says our guest professor for this week, Santiago Gallino. "What is not difficult is to plan for everything." Today we venture into the sphere of business that masters the planning, and backup planning: operations management. 

Summer School 6: Operations and 25,000 roses
August 16, 20235:15 PM ET

By 

Robert Smith

, 

Alex Goldmark

, 

Max Freedman
32-Minute Listen

    Download

    Transcript

Planet Money Summer School
NPR

"It's difficult to control everything," says our guest professor for this week, Santiago Gallino. "What is not difficult is to plan for everything." Today we venture into the sphere of business that masters the planning, and backup planning: operations management.

It's more than just predicting a bottleneck and imagining a solution, because there's always a bottleneck to clear. It's about modeling, and weighing the costs of messing up vs. missing out. For instance, take a newspaper vendor who has to decide how many newspapers to sell tomorrow morning. Do they buy fewer, knowing that they'll sell out–and then miss out on potential revenue from papers not sold? Or do they order more than they expect to sell, just in case–and eat the cost of a few unsold papers? This type of trade-off applies to all kinds of businesses, and Gallino talks us through how to choose.

The only certainty in this life is uncertainty. But we are certain you will come out of this episode feeling better prepared for your future business. And fortunately, there are no bottlenecks in podcasting.

The series is hosted by Robert Smith and produced by Max Freedman. Our project manager is Julia Carney. This episode was edited by Alex Goldmark and engineered by James Willetts. The show is fact-checked by Sierra Juarez.

Help support Planet Money and get bonus episodes by subscribing to Planet Money+ in Apple Podcasts or at plus.npr.org/planetmoney.

Always free at these links: Apple Podcasts, Spotify, Google Podcasts, NPR One or anywhere you get podcasts.

Find more Planet Money: Facebook / Instagram / TikTok / Our weekly Newsletter.

Music: Universal Production Music - "Lost Situation," "Vision," "Pyramid Thoughts," "Wandering Around," and "Growling Sax Surf"; Audio Network - "Reflected Colours" and "Sweet Valentine."
# Transcribe
https://www.npr.org/transcripts/1194249897
SYLVIE DOUGLIS, BYLINE: This is PLANET MONEY from NPR.

(SOUNDBITE OF BRICE MONTESSUIT AND CHARLES CASTE-BALLEREAU'S "LOST SITUATION")

ROBERT SMITH, HOST:

Welcome back, everyone, to PLANET MONEY Summer School, MBA edition - the only business school where free is not a dirty word. I'm Robert Smith. Today we are leaving the classroom for a field trip. We'll travel halfway around the world to a romantic farm and then to the least romantic place we can think of - our local supermarket checkout line - because today we are talking about operations management. The people who work in operations are the unsung heroes of any business. They are the optimizers of a business, the waste police. They keep the factory line moving quickly, the supply chain unbroken and the lines at Disneyland so twisting and confusing that you don't even know how long you've been waiting. Today on the show, we will show you the tools that the operations gurus use to keep the world spinning smoothly. In fact, our professor this week arrived with his clipboard and stopwatch in hand. He teaches operations at the Wharton School at the University of Pennsylvania. Santiago Gallino, thanks for teaching the class today.

SANTIAGO GALLINO: Oh, my pleasure. Thank you very much for having me.

SMITH: So one of the things I love about operations is how concrete it is. So, for instance, I just bought a cup of coffee from Starbucks. But in terms of operations, just getting a cup of coffee in my hand is incredible when you think about it. You've got to start with...

GALLINO: The coffee beans - you need to ship them to arrive on time with good quality. You need to be ready to put that coffee beans into the right machine with the right specification.

SMITH: And then you need to have all sorts of things arrive at the same time - the milk, the sugar, the cups, the baristas.

GALLINO: The baristas need to be there. The staff need to be scheduled on time, ready to manage the capacity that you expect.

SMITH: And when I walked into the Starbucks, like, I had to know where to stand. There was one line. There was two cashiers. There were people running back and forth.

GALLINO: Exactly. A coffee store that is well run is a store when everybody knows what to do all the time, and they are not trying to figure that on the fly.

SMITH: Does it drive you nuts when you go into a restaurant or a store as an operations person?

GALLINO: Many times, many times it does. But that is a signal that there is room for opportunity to improve.

SMITH: (Laughter) That is the kind way to put it. But we live in a world of chaos where anything can happen at any time. Is it too difficult to try and control everything?

GALLINO: I think it's difficult to control everything. What is not difficult is to plan for everything. And that's why operations management is embracing the uncertainty and making sure that you have a plan, that you are taking into account the different ranges of things that can happen. You need to know that it takes between three and five seconds to make a burger under certain conditions. There are some days where it's colder, and brewing the coffee can take longer - when somedays it's super hot and that will change. And you need to be aware of those changes. So I don't think you need to only fight uncertainty and randomness. You need to embrace it and manage it.

SMITH: There's something empowering and almost Zen-like about the operations outlook of the world. You see the uncertainty. You measure the uncertainty. You manage the uncertainty. We'll bring back Santiago in a few minutes after we listen to our first case study. You think you feel pressure on Valentine's Day? We'll have the story of a man who has to get 25,000 roses from Ecuador to his flower shop in New York City by February 14 after the break.

(SOUNDBITE OF MUSIC)

SMITH: Our first operations case study is one where a broken supply chain can lead to a broken heart. It's a story about roses on Valentine's Day. Lots of businesses have this kind of make-or-break moment. I'm thinking toys on Christmas or fireworks on the Fourth of July. You need an ace operations person to make sure that the product absolutely, no excuses, arrives on time. In this classic episode, we met Jan Ooms who owns a flower shop called Roses and Blooms in Manhattan. Valentine's Day is his moment.

(SOUNDBITE OF ARCHIVED NPR BROADCAST)

JAN OOMS: If you really make a big mistake for Valentine's Day, it would cost us so much money that we would not be able to make it back up for the rest of the year. So we have to really carefully plan this holiday.

STACEY VANEK SMITH: So how much is a dozen roses on February 14?

OOMS: It's about $80.

VANEK SMITH: And how much is it on February 15?

OOMS: It's $48.

VANEK SMITH: So that's almost double.

OOMS: That's almost double, yes.

SMITH: When Stacey Vanek Smith and I met Jan in early 2015, he had just made a huge gamble. He had ordered 25,000 roses to sell on Valentine's Day from one single farm outside Quito, Ecuador. In this story, listen for what operations people call variability. Which part of the process is uncertain, and how do you plan for it?

(SOUNDBITE OF ARCHIVED NPR BROADCAST)

VANEK SMITH: It's 36 days until Valentine's Day.

SMITH: And Jan Ooms has bet everything on this one farm to deliver the goods. And it's actually pretty unusual in the flower business to do this. I mean, normally a flower shop will wait until February and will basically go to one of these big flower distributors, say, what have you got? What are your prices? But Jan says the problem is you never know what the answer is going to be.

VANEK SMITH: Jan wanted to avoid all that, so he locked his price in early - $1.40 per rose. But that also means that his entire Valentine's Day is resting on one farm 4,000 miles away.

OOMS: You know, we cannot be too optimistic yet. Of course, the last four weeks are very critical.

VANEK SMITH: Do you get nervous?

OOMS: Yes, absolutely. Yeah. It's nerve-wracking because not only is it hard to get the roses. It's also hard to get them out and, you know, get them a long time and get all the work done.

SMITH: In this business, anything can happen. And this year, unfortunately, it does. The temperature started to drop in the Andes, started to get chilly there, and thunderstorms rolled in, which meant the roses were in danger.

VANEK SMITH: I got on a plane and went to Ecuador to see what the farm was going to do about it.

UNIDENTIFIED PERSON: Welcome to Quito. The local time is 15 minutes...

VANEK SMITH: It's 21 days until Valentine's Day. The Cayambe Valley is at the foot of a huge volcano. It's incredibly lush here. Everything is bright green. These huge mountain peaks surround us. And this is where Jan Ooms' roses are growing.

Here we are.

JUAN TORRI: Yes.

VANEK SMITH: And I'm met at the farm by the owner, Juan Torri. Just looking at the roses - he shows them to me - they look fine. They're really deep, this deep blood red. And they're all covered in these little mesh socks, which they put on the roses to hold the petals together.

TORRI: Right now we are looking at the red roses we are producing that is coming for Valentine's.

VANEK SMITH: And how many roses are here altogether?

TORRI: For Valentine's, we will produce around 3 million roses.

VANEK SMITH: Wow. That's a lot. That's a lot of roses.

TORRI: Yes. That's a lot of roses.

SMITH: What you should know is that cold weather doesn't kill roses. It throws off the timing. There's this whole art to picking a rose at just the right time for the optimal amount of blooming.

VANEK SMITH: And any other time of year, you can just wait until the roses are perfect for their destination and snip - good to go. But Valentine's Day season, there is this really tight schedule. You have to harvest before February 6 in order to get those roses shipped off. There's very little wiggle room.

TORRI: Not sure that the rose will bloom in time. It depends a lot on weather.

VANEK SMITH: And this is the moment when they call Hector.

HECTOR ROACHA: (Speaking Spanish).

VANEK SMITH: Hector the plant engineer - 20 years of experience growing roses.

ROACHA: (Speaking Spanish).

VANEK SMITH: Hector is this nervous, wiry guy. He wears an enormous watch that keeps track of moon cycles and weather reports. He can actually look at a rose and tell exactly how many days it will be until it blooms. He shows me this. He points to this super-tiny little red bud.

ROACHA: (Speaking Spanish).

VANEK SMITH: So in eight days, this will open.

ROACHA: (Speaking Spanish).

VANEK SMITH: You're sure, totally sure.

ROACHA: (Speaking Spanish).

VANEK SMITH: Hector has all of these crazy tricks that he can use to speed the roses up or slow the roses down. For instance, if it's too hot and the roses are ahead of schedule, Hector can turn on huge fans and block the roses from the sun to cool them down a little bit. If the roses are behind schedule, if they're not opening fast enough, Hector will use plant hormones and potassium to speed the roses up.

SMITH: But there is a limit.

VANEK SMITH: There is a limit. Hector says using all the tricks he has, he can speed the roses up or slow the roses down by four days.

ROACHA: (Speaking Spanish).

VANEK SMITH: So has it ever happened that the roses haven't been on time?

ROACHA: (Speaking Spanish).

VANEK SMITH: 2008. It was a really warm winter, and the roses were growing way too fast. They were 10 days ahead of schedule. Hector worked all of his magic. He kept the sides of the tent open. He put on huge fans to cool the roses down. He did everything he could, but in the end, the roses opened five days early. And for Hector, this was awful. He just had to sit there and watch all of these roses open and then get cut and sold at these super-bargain prices, less than half of what they normally would have gotten. And a lot of them were just thrown away.

SMITH: This year everyone on the farm is worried about the opposite problem. It is too cold. The roses might bloom too late. But the owner of the farm, Juan Torri, says the result is just the same as in 2008.

TORRI: We will throw away the roses. It will be a disaster. It's like we have sacrificed five months of work.

VANEK SMITH: While we're talking, you might have heard the thunder in the background. This cold wind starts to blow through the rose bushes. Workers start running along the sides of the greenhouses, rolling down the plastic walls to keep the roses warm.

So is it going to rain? I heard rumbling.

TORRI: Yeah, maybe. Yeah. It's - I think it will rain.

VANEK SMITH: Is that good or bad?

TORRI: Yeah, that's not good.

VANEK SMITH: While I'm standing there talking to Juan, Hector, the plant engineer, takes off running in a total panic. It's the last time I see him, actually. I have to go back to New York.

SMITH: We checked back in with the farm eight days before Valentine's Day, and they blew their February 6 deadline. But Hector had been working his magic, and they managed to get the roses to just the right level of bloom by February 7 - one day late. Luckily, the rest of the process has been designed with at least a little bit of wiggle room.

VANEK SMITH: Back in New York, Jan Ooms is really relieved to hear this. A week is enough time to get the roses to New York. But of course, Robert, the hurdles have just begun. Twenty-five thousand roses still have to be transported 4,500 miles to New York.

SMITH: You know, I'd always thought that all of the roses got here in these giant cargo planes that probably smell really good packed to the rafters with roses. But I guess, apparently, they have to be a little bit more flexible than that. And you're never sure when the roses will be ready or how big the orders are or where they have to go. So they came up with a really novel solution. The roses travel the same way we do - on commercial flights through Miami.

VANEK SMITH: The roses catch their scheduled flight on February 9. They arrive at JFK on February 10 at 2 a.m. By 6:30, the huge boxes are stacked in the middle of Jan's store.

Good morning.

OOMS: Good morning. How are you?

VANEK SMITH: Good. How are you doing?

OOMS: Good.

VANEK SMITH: It's early.

OOMS: It is definitely early. Yeah.

VANEK SMITH: T-minus four days until Valentine's Day. Jan Ooms drags the first box into the back room.

Do you get nervous before you open up the boxes of roses before you see them?

OOMS: I always am, yes. It's a lot of possibilities when it goes wrong.

SMITH: Although Jan solved all the logistical hurdles, he still doesn't know what the flowers look like. There's anything that could have happened out there. The roses could have been left on the tarmac in Miami - got all wilted.

VANEK SMITH: They could have frozen in the delivery truck on the way to the shop.

SMITH: And I hear sometimes customs agents looking for drugs or whatnot go into the boxes of roses and - what? - they just toss them everywhere.

VANEK SMITH: They, like, bash them on a table seeing if drugs or little bugs fall out.

SMITH: So you can imagine the drama as Jan watches one of his employees pull out a ceremonial box cutter to open the box.

VANEK SMITH: This is it. The moment of truth.

(SOUNDBITE OF BOX BEING CUT)

VANEK SMITH: What do you think?

OOMS: They look good.

VANEK SMITH: And you're happy with these roses?

OOMS: I'm very happy with the roses. They look good. They look really, really good. I'm a happy guy.

VANEK SMITH: Jan and his staff quickly get to work. They trim the stems of the roses, and they immediately put them in this hydrating solution. It's amazing. These roses have traveled thousands of miles. They haven't had any water at all for days, and they look beautiful. They look really good.

SMITH: And this, right here, is the reason why we give roses on Valentine's Day. And I know I always thought that it was some sort of tradition that went back hundreds and hundreds of years. But as we talked to people, they were like, oh, oh, no, you know, people on Valentine's Day used to give things like sweet violets - these little fragile flowers that were grown locally.

VANEK SMITH: Right, except for once Valentine's Day became a big business, flower shops needed a flower that they could order in bulk. And because it's in February, they needed a flower they could order from the other side of the world. And there aren't that many flowers that can stand up to that kind of abuse.

SMITH: Roses were the perfect choice - pretty much indestructible. We didn't just set up this global transportation chain in order to get this traditional flower, roses. We actually started to like roses because they were optimized for the global transportation chain. They were the flower that worked best with the planes and the boxes and the farms.

VANEK SMITH: Once Jan got his roses, once they'd been through all the planes and boxes and everything, they cost him about $4.30 each. And that's a good deal this year. Because it was so cold, there aren't that many roses on the market. Jan says he saved about 30% per rose.

SMITH: And one day before Valentine's Day, T-minus-1, they were ready for customers.

KEN STURM: How much - are they just all the same price? There are dozens, and they're priced the same?

VANEK SMITH: Ken Sturm comes into Roses and Blooms to get a bouquet of flowers for his wife. He's checking out all these roses in the big refrigerator there, and he's a little shocked by the $80 price tag. That's how much it is for a dozen roses this year. But he says he doesn't really have a choice.

STURM: If you bring home anything else, you're seen as a cheapskate.

SMITH: Of course, he could have explained to his wife all the logistics that went into the flowers or that the roses are this beautiful sign of brilliant plant engineering and transportation efficiency.

VANEK SMITH: But really, Ken is just hoping to hear one thing.

STURM: So I might get - oh, they're beautiful - that beautiful kind of embellishment. That's all.

VANEK SMITH: That's what you're hoping for from your wife?

STURM: I am.

VANEK SMITH: The beautiful?

STURM: Yes, exactly.

(SOUNDBITE OF MUSIC)

SMITH: It was a happy ending for the couples of Manhattan and a happy ending for those of us who are learning operations. Despite all the weather chaos, the flowers got there when they needed to get there. Our operations guru is already taking notes to see how Jan could make the supply chain even more efficient the next time. We'll bring him back after the break.

(SOUNDBITE OF MUSIC)

SMITH: We are back with our operations professor, Santiago Gallino, who's been grimacing a little bit. I know your heart was racing while listening to the flowers episode.

GALLINO: Indeed.

SMITH: So in the story we just heard, the flower-seller, Jan Ooms - he didn't necessarily care about all of the steps in the process. He just wanted the flowers on Valentine's Day. But he did make a lot of crucial decisions here that sort of affect the final outcome. Maybe we should go through those, you know?

GALLINO: Yes, I think the first decision he made is how many flowers to order.

SMITH: Yeah, 25,000, if I remember correctly. Yeah.

GALLINO: That's correct. And you can ask, what - was that the right number? The key here is that he doesn't know for sure how many he's going to sell. And so what he needs to think is how much it will cost him - every flower that is not sold that he bought.

SMITH: That he throws away.

GALLINO: That is a cost, and he needs to take that into account. However, he also needs to take into account how much money he will lose for every customer that walks in and says, hey, I want roses. Oh, I don't have any more. I sold out. Well, that's also money on the table. And if these two numbers are not symmetric, then he will probably need to be more aggressive in how much he wants to order.

SMITH: That's a fascinating idea because the roses only cost a few dollars, you know, and if you were to throw away a few dollars, that's nothing, right? But every lost sale could cost him 30, 40, $50 in lost sales. So what you're saying, as an operations guy, is maybe order 30,000?

GALLINO: Exactly. You know, he can see that the money that he's not actually making because he ran out of roses is as painful as the money he's throwing away if he is left with roses at the end of Valentine's season.

SMITH: And there's a name you teach in business school for this conundrum of lost sales.

GALLINO: That's right. That's right. That thing is one of the most exciting concepts - is the news vendor model.

SMITH: News vendor as in the dudes who sell the newspapers on the street corners.

GALLINO: Exactly because that guy used to have exactly the same problem, where every newspaper that you need to throw away is way cheaper than not selling a newspaper during that day.

SMITH: OK, so the news vendor model is one way to deal with the variability of the world. You can't predict the exact demand, so you just figure out which way will essentially cost you less. But there is another way, listening to the story again, that Jan could have dealt with variability, which is to have more than one farm - to have more than one country, more than one airplane, more than one supply line.

GALLINO: That's exactly right. And I think you point to one of the aspects of this decision that creates tension. You want to be efficient, but you also want to be flexible. And you can get flexibility by trying to find other sources for the same product sometimes. And say, well, why he's not going to find a second producer from Colombia? Well, because if he split the order, the order is going to be more expensive.

SMITH: Sure, yeah.

GALLINO: And that is going to be less efficient - 100%. But it's going to be more flexible because if the winter is too strong in one country and the summer is too hot in the other - well, that maybe balances things out, and you will still have your roses. If you put all your eggs in one basket, it might be very efficient - not very flexible.

SMITH: And that's a technical operations term - eggs in one basket?

GALLINO: (Laughter) Yes, I guess it is.

SMITH: (Laughter) Speaking of eggs all in one basket, our next story is about the supermarket checkout line.

(SOUNDBITE OF MUSIC)

SMITH: Operations people are obsessed with lines. Think about it. Customers want to buy something. Stores want to sell something. And a long line is standing in the way of everyone's happiness. Customers are bored and annoyed. The cashier at the front of the line is overworked. MBAs call this a bottleneck, but as you listen to this story, think about how fixing a bottleneck, like a supermarket checkout line, can just create more bottlenecks, create more annoyance. This story is from 2016, and it's hosted by Jacob Goldstein and Nick Fountain.

(SOUNDBITE OF ARCHIVED NPR BROADCAST)

NICK FOUNTAIN: Goldstein, the other day, you and I went to Walmart.

AUTOMATED VOICE: Welcome to Walmart.

JACOB GOLDSTEIN: We got peppers, apples, bread. I got a Halloween card.

FOUNTAIN: We were there 'cause we're doing a story about self-checkout.

GOLDSTEIN: Yeah, we wanted to find out, could we make it through self-checkout one time - just one time - without getting some kind of error message from the machine?

FOUNTAIN: We were there with Howard Schneider. He lives a couple of blocks away from this particular Walmart, and we were shopping there with him because he's kind of an expert on self-checkout.

AUTOMATED VOICE: Touch the item to purchase.

HOWARD SCHNEIDER: It was Fuji, right?

AUTOMATED VOICE: Move your Fuji apples to the bag.

FOUNTAIN: Everything was going fine until we hit the red bell peppers.

SCHNEIDER: Maybe it's under red. I don't know.

FOUNTAIN: So you're scrolling through the pages, looking for the right thing.

SCHNEIDER: No red peppers?

GOLDSTEIN: Could it be B for bell pepper?

SCHNEIDER: Nope. No peppers.

FOUNTAIN: It was not B for bell peppers.

SCHNEIDER: Doesn't even say what to do, so then you're stuck here right now. Doesn't even say get help or anything.

GOLDSTEIN: And Fountain, we'd probably still be standing there trying to figure this out but for the fact that Howard went and got a store employee who walked over and saved us by typing in the code for peppers. She just knew the number in her head.

SCHNEIDER: The fact that the - we have to call the attendant to process this little order is a failure. Really, it shouldn't happen, and the machine should deal with situations like that.

FOUNTAIN: And why is self-checkout a big deal to you?

SCHNEIDER: Because I invented it, right? Why wouldn't it be?

(SOUNDBITE OF MUSIC)

SMITH: We're going to skip ahead in the story of how Howard Schneider created the self-checkout machine. In a nutshell, he was a doctor and an inventor, and he wanted to make something like an ATM but for supermarket lines. He perfected the scanning part, the scale that weighs your items and accuses you of stealing things. But he couldn't get a store to install the damn thing.

(SOUNDBITE OF ARCHIVED NPR BROADCAST)

GOLDSTEIN: He gets a meeting at a New England supermarket chain called Stop and Shop. So he drives down. He gives this presentation in this boardroom full of people, and at the head of the table, there's this executive who everybody's looking to.

SCHNEIDER: This old guy's sitting at the head of a table and, you know, he says, son, do you know why people shop at Stop and Shop? I said, no. He says, because of our people, because of our people. And then everybody around the table starts nodding their head. And he says, do you think people want to come in and speak to your machine? Do you know anything about retail? Do you know anything? And he says, I don't think it's for us. And then everybody around the table nodded their head, and I drove back to Montreal with my tail between my legs. And it was just a horrible feeling, thinking, this is the stupidest thing I've ever done. Nobody will ever like it or ever use it.

GOLDSTEIN: But Howard keeps loading his machine into the back of this rented Ryder truck, keeps going to supermarket trade shows. And eventually, he gets a meeting with a supermarket chain called Price Chopper. It's based in upstate New York.

SCHNEIDER: The head person actually saw the machines. And you know what he said? He looked at it. He says, I like it. Let's do it. And guess what? After that, everybody's very nice.

FOUNTAIN: The CEO says, we're not going to buy the machines from you, but you can use one of our stores in upstate New York as a real-world experiment.

GOLDSTEIN: And on August 5, 1992, grocery store shoppers use what may be, depending on your definition - I mean, we - what we are going to call the first fully automatic self-checkout machines.

FOUNTAIN: When Howard gets to the supermarket that day, he sees that there are protesters there. It's the cashiers' union. They're saying, these machines are taking our jobs. Howard read us this quotation from a union rep at the time. And the union rep basically said this thing that I think about all the time - these machines are forcing customers to do more work.

SCHNEIDER: Quote, "maybe if the customers come early, they can unload the truck and stock the shelves," unquote.

GOLDSTEIN: Well, I mean, like, there is a serious question underneath it - right? - which is like, are these machines taking people's jobs?

SCHNEIDER: But the answer is very anticlimactic. Let me tell you what happened in Price Chopper. The machines went in. People used them, and they didn't work. It crashed. It stopped working. And then people had shopping carts half unloaded and everything stopped.

FOUNTAIN: The store is full of angry shoppers. And Howard, he's just sitting there in the middle of all this chaos, unscrewing the back of the machine so that he can restart it. And the union, they figure they've got nothing to worry about. They pack up their protest and leave.

GOLDSTEIN: Howard stays up all night sitting there in the grocery store fixing the code. He says he can still remember smelling the cinnamon buns they are baking in the back of the store while he's sitting there trying to figure out what's wrong. And the next day, his machines didn't crash, but the shoppers and the machines, they still needed a lot of handholding. In fact, they need so much help that Howard has to invent something else. He has to invent the person who stands there next to the self-checkout machines, helping the customers and fixing the machines.

SCHNEIDER: We drilled some holes in the cabinet so that if you had to reset the machine, you could just stick the long screwdriver in...

(LAUGHTER)

SCHNEIDER: ...And hit the reset button. So we gave him a long screwdriver. And he was very friendly, very nice with people. And he would like - he'd help them through the orders. And that made a huge difference.

(SOUNDBITE OF MUSIC)

SMITH: And so the self-checkout machine was born, along with the employee standing next to it to actually make it work.

(SOUNDBITE OF MUSIC)

SMITH: Since that moment, the self-checkout machine has muddled along. Howard Schneider eventually sold his idea and his company, and the self-checkout machine slowly started to move into grocery stores. Now a little more than half of consumers report using self-checkout every week. Was this an operations triumph or an example of moving from one inefficient process to another? We'll have our professor weigh in after the break.

(SOUNDBITE OF MUSIC)

SMITH: We are back with our professor today, Santiago Gallino. Santiago, you specialize in retail operations. So I can ask you the question I just have to ask you. These self-checkout machines seem to be everywhere, and yet we hate them. I hate them. How can this be? Who can stop this?

GALLINO: I am with you. I'm with you, Robert. By transferring this to customers, the retailer is saving a lot of money because the retailer has two expenses that go to the top of the list - inventory and staff. And if they can reduce one of those, they are going to do it. They are reducing the staff expense because you and I are doing the job.

SMITH: Should we have just said no?

GALLINO: That's one option.

SMITH: (Laughter).

GALLINO: We could all stop using it. And so then they will actually start to pull back. But we are in a rush, and it turns out that it actually helped to get things flowing and increase the capacity.

SMITH: It turns out it is faster? We accept it because it's faster?

GALLINO: Yes, I think that the reason why we accept that is because if you show up to the checkout process and there is a real cashier, and you need to wait for that person - or there is an empty self-checkout, the temptation is too big. You will go for it because you want to get out of there fast.

SMITH: Even if I don't like the process of checking out.

GALLINO: That's right. It's painful, but for the companies, it's cost effective. And I think operations is getting the right balance. You want efficiency. You want to move along in the process, but you want to also keep your customer happy and your employees happy as well.

SMITH: So let's talk about lines for a moment because I think where a lot of us encounter operations problems is as we're standing in a very, very, very long line, moving slowly, and we start to think - what is going on here? So I'll ask you - if you're standing in a line, if it's taking too long, what is going on?

GALLINO: Well, there are two reasons why we can have a line, especially if it's a long line. One is that we have more demand than capacity. That means that we have less cashiers than we actually need.

SMITH: Because maybe we went to the grocery store after work, and there's just - everybody's shopping at the same time.

GALLINO: That's right. But there is another reason that goes together with this that is that you can have a line when you have enough capacity, but there is a lot of variability.

SMITH: Variability, what does that mean?

GALLINO: Well, imagine that you show up to the grocery store, and in front of you there is this person that takes every product very slowly to the cashier.

SMITH: Yes, yes, I know them.

GALLINO: Or if you are in front of the self-checkout and you happen to be behind me, and I start to mess things up - and you are rolling your eyes, and I'm adding variability to the process.

SMITH: Variability to the process because once you have variability, then there's going to be these - I guess the technical term is bottleneck.

GALLINO: The bottleneck is the step in the process with the smallest capacity. You are going to start to experience a bottleneck because you have now less capacity than the demand you need to serve.

SMITH: Now, it seems like a lot of people are experimenting with different forms of lines. I mean, we heard about the self-checkout machine, but there's the system that they use in Trader Joe's - if you've ever been there - which is it's one long line and like 30 cashiers. But then there's a lot of places that have different lines for different people. What is the best way to shorten a line?

GALLINO: Well, those dedicated lines for 30 cashiers are trying to reduce variability. And if you think about it, that will give you a more consistent line, even if it's a longer one. But you really don't care because you have enough capacity - 30 cashiers - to deal with that one long line.

SMITH: So if there's one slow cashier and if I have to pick a cashier, I might pick the slow cashier. But if you have all these different cashiers in one line, then it's probably not going to slow everybody else down.

GALLINO: On average, you're going to be better, and that average is helping you with the variability.

SMITH: Professor Santiago Gallino from the Wharton School, thank you so much for being our professor today.

GALLINO: Thank you very much, Robert. It was a pleasure.

SMITH: It was efficient.

GALLINO: Indeed.

(SOUNDBITE OF MUSIC)

SMITH: And our professor has left us with some vocabulary words that you can practice while waiting in long lines. The first one is the news vendor model. This is the calculation you should do when you think about how much product to order. What will it cost to throw away an extra newspaper you don't sell versus the money you will lose if you run out of the product? We also have this vocabulary - two things that can create long lines, capacity and variability. Do you have enough staff to help the customers? That's capacity. But variability means that one slow customer can grind the whole line to a halt. This creates our last vocabulary word - the bottleneck. Of every part of the process, which one is the slowest, the one with the longest line forming behind it? That's your bottleneck and fixing that can speed up the whole process.

(SOUNDBITE OF MUSIC)

SMITH: We are two weeks away from the end of Summer School, and we'll have our graduation episode then, including actual business pitches from actual PLANET MONEY listeners like you. We'll also open our final exam online. If you pass it, we will send you something that in a very dim room might look a lot like a business school diploma. You've all earned it.

Our Summer School series is produced by Max Freedman. Our project manager is Julia Carney. This episode was edited by our executive producer, Alex Goldmark, and engineered by James Willetts. The show was fact-checked by Sierra Juarez. I'm Robert Smith. This is NPR. Thanks for listening.

Copyright © 2023 NPR. All rights reserved. Visit our website terms of use and permissions pages at www.npr.org for further information.

NPR transcripts are created on a rush deadline by an NPR contractor. This text may not be in its final form and may be updated or revised in the future. Accuracy and availability may vary. The authoritative record of NPR’s programming is the audio record.

----

**(Adam Davidson):**

**(Laura Conaway):**


**faster whisper:**
Support for NPR and the following message come from the Kauffman Foundation,
providing access to opportunities that help people achieve financial stability,
upward mobility, and economic prosperity, regardless of race, gender, or geography.
kauffman.org.
This is Planet Money from NPR.
Welcome back everyone to Planet Money Summer School, MBA edition.
The only business school where free is not a dirty word.
I'm Robert Smith.
Today, we are leaving the classroom for a field trip.
We'll travel halfway around the world to a romantic farm
and then to the least romantic place we can think of,
our local supermarket checkout line.
Because today, we are talking about operations management.
The people who work in operations are the unsung heroes of any business.
They are the optimizers of a business, the waste police.
They keep the factory line moving quickly, the supply chain unbroken,
and the lines at Disneyland so twisting and confusing
that you don't even know how long you've been waiting.
Today on the show, we will show you the tools that the operations gurus use
to keep the world spinning smoothly.
In fact, our professor this week arrived with his clipboard and stopwatch in hand.
He teaches operations at the Wharton School at the University of Pennsylvania.
Santiago Galino, thanks for teaching the class today.
Oh, my pleasure. Thank you very much for having me.
So one of the things I love about operations is how concrete it is.
So for instance, I just bought a cup of coffee from Starbucks.
But in terms of operations, just getting a cup of coffee in my hand
is incredible when you think about it.
You got to start with the coffee beans.
You need to ship them to arrive on time with good quality.
You need to be ready to put that coffee beans
into the right machine with the right specification.
And then you need to have all sorts of things arrive at the same time.
The milk, the sugar, the cups, the baristas.
The baristas need to be there.
The staff needs to be scheduled on time,
ready to manage the capacity that you expect.
And when I walked into the Starbucks, like, I had to know where to stand.
There was one line. There was two cashiers.
There were people running back and forth.
Exactly. A coffee store that is well run is a store
when everybody knows what to do all the time.
And they are not trying to figure that on the fly.
Does it drive you nuts when you go into a restaurant
or a store as an operations person?
Many times. Many times it does.
But that is a signal that there is room for opportunity to improve.
That is the kind way to put it.
But we live in a world of chaos where anything can happen at any time.
Is it too difficult to try and control everything?
I think it's difficult to control everything.
What is not difficult is to plan for everything.
And that's why operations management is embracing the uncertainty
and making sure that you have a plan, that you are taking into account
the different ranges of things that can happen.
You need to know that it takes between three and five seconds
to make a burger under certain conditions.
There are some days where it's colder and brewing the coffee
can take longer, when some days it's super hot and that will change.
And you need to be aware of those changes.
So I don't think you need to only fight uncertainty and randomness.
You need to embrace it and manage it.
There's something empowering and almost zen-like
about the operations outlook of the world.
You see the uncertainty, you measure the uncertainty,
you manage the uncertainty.
We'll bring back Santiago in a few minutes
after we listen to our first case study.
You think you feel pressure on Valentine's Day?
We'll have the story of a man who has to get 25,000 roses
from Ecuador to his flower shop in New York City by February 14th.
After the break.
Support for this podcast and the following message come from Wyse,
the app that makes managing your money in different currencies easy.
With Wyse, you can send and spend money internationally
at the mid-market exchange rate.
No guesswork and no hidden fees.
Learn more about how Wyse could work for you at Wyse.com.
Our first operations case study is one where a broken supply chain
can lead to a broken heart.
It's a story about roses on Valentine's Day.
Lots of businesses have this kind of make-or-break moment,
thinking toys on Christmas or fireworks on the 4th of July.
You need an ace operations person to make sure that the product,
absolutely no excuses, arrives on time.
In this classic episode, we met Jan Oems,
who owns a flower shop called Roses and Blooms in Manhattan.
Valentine's Day is his moment.
If you really make a big mistake on Valentine's Day,
it would cost us so much money that we would not be able
to make it back up for the rest of the year.
So we have to really carefully plan this holiday.
So how much is a dozen roses on February 14th?
It's about $80.
And how much is it on February 15th?
It's $48.
So that's almost double.
That's almost double, yes.
When Stacey Vanik-Smith and I met Jan in early 2015,
he had just made a huge gamble.
He had ordered 25,000 roses to sell on Valentine's Day
from one single farm outside Quito, Ecuador.
In this story, listen for what operations people call
variability, which part of the process is uncertain
and how do you plan for it?
It's 36 days until Valentine's Day.
And Jan Oems has bet everything on this one farm
to deliver the goods.
And it's actually pretty unusual
in the flower business to do this.
I mean, normally a flower shop will wait until February
and will basically go to one
of these big flower distributors, say, what have you got?
What are your prices?
But Jan says the problem is you never know
what the answer is going to be.
Jan wanted to avoid all that,
so he locked his price in early, $1.40 per rose.
But that also means that his entire Valentine's Day
is resting on one farm 4,000 miles away.
You know, we cannot be too optimistic yet.
Of course, the last four weeks are very critical.
Do you get nervous?
Yes, absolutely.
It's nerve-racking because not only is it hard
to gather roses, it's also hard to get them out
and, you know, get them all on time
and get all the work done.
In this business, anything can happen.
And this year, unfortunately, it does.
The temperature started to drop in the Andes,
started to get chilly there,
and thunderstorms rolled in,
which meant the roses were in danger.
I got on a plane and went to Ecuador
to see what the farm was going to do about it.
Welcome to Quito.
The local time is 15 minutes.
It's 21 days until Valentine's Day.
The Cayambe Valley is at the foot of a huge volcano.
It's incredibly lush here.
Everything is bright green.
These huge mountain peaks surround us.
And this is where Jan Umze's roses are growing.
Here we are.
Yes.
And I met at the farm by the owner, Juan Torre.
Just looking at the roses, he shows them to me,
they look fine.
They're really deep, this deep blood red,
and they're all covered in these little mesh socks,
which they put on the roses to hold the petals together.
Right now we are looking at the red roses
we are producing that is coming for Valentine's.
And how many roses are here all together?
For Valentine's, we will produce
around three million roses.
Wow, that's a lot.
That's a lot of roses.
Yes, that's a lot of roses.
What you should know is that
cold weather doesn't kill roses.
It throws off the timing.
There's this whole art to picking a rose
at just the right time
for the optimal amount of blooming.
And any other time of year,
you can just wait until the roses
are perfect for their destination.
And snip, good to go.
But Valentine's Day season,
there is this really tight schedule.
You have to harvest before February 6th
in order to get those roses shipped off.
There's very little wiggle room.
Not sure that the rose will bloom in time.
It depends a lot on weather.
And this is the moment when they call Hector.
My name is Hector Olavacha.
Hector, the plant engineer.
20 years of experience growing roses.
I have 20 years of experience in roses.
Hector is this nervous, wiry guy.
He wears an enormous watch
that keeps track of moon cycles and weather reports.
He can actually look at a rose
and tell exactly how many days
it will be until it blooms.
He shows me this.
He points to this super tiny little red bud.
So in eight days, this will open.
You're sure?
Totally sure.
Hector has all of these crazy tricks
that he can use to speed the roses up
or slow the roses down.
For instance, if it's too hot
and the roses are ahead of schedule,
Hector can turn on huge fans
and block the roses from the sun
to cool them down a little bit.
If the roses are behind schedule,
if they're not opening fast enough,
Hector will use plant hormones
and potassium to speed the roses up.
But there is a limit.
There is a limit.
Hector says using all the tricks he has,
he can speed the roses up
or slow the roses down by four days.
So has it ever happened
that the roses haven't been on time?
2008.
It was a really warm winter
and the roses were growing way too fast.
They were 10 days ahead of schedule.
Hector worked all of his magic.
He kept the sides of the tent open.
He put on huge fans to cool the roses down.
He did everything he could,
but in the end, the roses opened five days early.
And for Hector, this was awful.
He just had to sit there
and watch all of these roses open
and then get cut and sold
at these super bargain prices,
less than half of what they normally would have gotten.
And a lot of them were just thrown away.
This year, everyone on the farm
is worried about the opposite problem.
It is too cold.
The roses might bloom too late,
but the owner of the farm, Juan Torre, says
the result is just the same as in 2008.
While we're talking,
you might've heard the thunder in the background.
This cold wind starts to blow through the rose bushes.
Workers start running along the sides of the greenhouses,
rolling down the plastic walls
to keep the roses warm.
So is it gonna rain?
I heard rumbling.
Yeah, maybe.
Yeah, I think it could rain.
Is that good or bad?
Yeah, that's not good.
While I'm standing there talking to Juan,
Hector, the plant engineer,
takes off running in a total panic.
It's the last time I see him, actually.
I have to go back to New York.
We check back in with the farm
and they're eight days before Valentine's Day
and they blew their February 6th deadline.
But Hector had been working his magic
and they managed to get the roses
to just the right level of bloom by February 7th,
one day late.
Luckily, the rest of the process has been designed
with at least a little bit of wiggle room.
Back in New York,
Jan Ummes is really relieved to hear this.
A week is enough time to get the roses to New York,
but of course, Robert, the hurdles have just begun.
25,000 roses still have to be transported
4,500 miles to New York.
You know, I'd always thought that all of the roses
got here in these giant cargo planes
that probably smell really good,
packed to the rafters with roses.
But I guess apparently they have to be
a little bit more flexible in that.
You're never sure when the roses will be ready
or how big the orders are or where they have to go.
So they came up with a really novel solution.
The roses travel the same way we do
on commercial flights through Miami.
The roses catch their scheduled flight on February 9th.
They arrive at JFK on February 10th at 2 a.m.
By 6.30, the huge boxes are stacked
in the middle of Jan's store.
Good morning.
Good morning, how are you?
Good, how are you doing?
Good.
It's early.
It is definitely early, yeah.
T minus four days until Valentine's Day.
Jan Ummes drags the first box into the back room.
Do you get nervous before you open up the boxes
of roses before you see them?
I always am, yes.
It's a lot of possibilities when it goes wrong.
Although Jan solved all the logistical hurdles,
he still doesn't know what the flowers look like.
There's anything that could have happened out there.
The roses could have been left on the tarmac in Miami,
got all wilted.
They could have frozen in the delivery truck
on the way to the shop.
And I hear sometimes customs agents
looking for drugs or whatnot
go into the boxes of roses and what?
They just toss them everywhere.
They bash them on a table,
seeing if drugs or little bugs fall out.
So you can imagine the drama
as Jan watches one of his employees
pull out a ceremonial box cutter to open the box.
This is it, the moment of truth.
What do you think?
They look good.
And you're happy with these roses?
I'm very happy with the roses.
They look good.
They look really, really good.
I'm a happy guy.
Jan and his staff quickly get to work.
They trim the stems of the roses
and they immediately put them in this hydrating solution.
It's amazing.
These roses have traveled thousands of miles.
They haven't had any water at all for days
and they look beautiful.
They look really good.
And this right here is the reason
why we give roses on Valentine's Day.
And I know I always thought
that it was some sort of tradition
that went back hundreds and hundreds of years,
but as we talk to people,
they're like, oh, oh no.
People on Valentine's Day used to give
things like sweet violets,
these little fragile flowers that were grown locally.
Right, except for once Valentine's Day
became a big business,
flower shops needed a flower
that they could order in bulk.
And because it's in February,
they needed a flower they could order
from the other side of the world.
And there aren't that many flowers
that can stand up to that kind of abuse.
Roses were the perfect choice,
pretty much indestructible.
We didn't just set up this global transportation chain
in order to get this traditional flower roses.
We actually started to like roses
because they were optimized
for the global transportation chain.
They were the flower that worked best
with the planes and the boxes and the farms.
Once Jan got his roses,
once they'd been through all the planes
and boxes and everything,
they cost him about $4.30 each.
And that's a good deal this year
because it was so cold,
there aren't that many roses on the market.
Jan says he saved about 30% per rose.
And one day before Valentine's Day,
T minus one, they were ready for customers.
How much are they just all the same price?
There are dozens and they're priced the same.
Ken Sturm comes into Roses and Blooms
to get a bouquet of flowers for his wife.
He's checking out all these roses
in the big refrigerator there.
And he's a little shocked by the $80 price tag.
That's how much it is for a dozen roses this year.
But he says he doesn't really have a choice.
If you bring home anything else,
you're seen as a cheapskate.
Of course, he could have explained to his wife
all the logistics that went into the flowers
or that the roses are this beautiful sign
of brilliant plant engineering
and transportation efficiency.
But really, Ken is just hoping to hear one thing.
So I might get, oh, they're beautiful,
that beautiful kind of embellishment.
That's what you're hoping for from your wife?
I am.
The beautiful.
Yes, exactly.
It was a happy ending for the couples of Manhattan
and a happy ending for those of us
who are learning operations.
Despite all the weather chaos,
the flowers got there when they needed to get there.
Our operations guru is already taking notes
to see how Jan could make the supply chain
even more efficient the next time.
We'll bring him back after the break.
We are back with our operations professor,
Santiago Galino, who's been grimacing a little bit.
I know your heart was racing
while listening to the flowers episode.
Indeed.
So in the story we just heard,
the flower seller, Jan Umms,
he didn't necessarily care about
all of the steps in the process.
He just wanted the flowers on Valentine's Day.
But he did make a lot of crucial decisions here
that sort of affect the final outcome.
Maybe we should go through those, you know?
Yes, I think the first decision he made
is how many flowers to order.
Yeah, 25,000 if I remember correctly, yeah.
That's correct.
And you can ask, was that the right number?
The key here is that he doesn't know for sure
how many he's gonna sell.
And so what he need to think is
how much it will cost him
every flower that is not sold, but he bought.
That he throws away.
That is a cost and he need to take that into account.
However, he also need to take into account
how much money he will lose
for every customer that walks in
and says, hey, I want roses.
Oh, I don't have anymore, I sold out.
Well, that's also money on the table.
And if these two numbers are not symmetric,
then he will probably need to be more aggressive
in how much he wants to order.
That's a fascinating idea
because the roses only cost a few dollars.
And if you were to throw away a few dollars,
that's nothing, right?
But every lost sale could cost him 30, 40, $50
in lost sales.
So what you're saying as an operations guy
is maybe order 30,000?
Exactly.
He can see that the money
that he's not actually making
because he ran out of roses
is as painful as the money he's throwing away
if he is left with roses at the end of Valentine's season.
And there's a name you teach in business school
for this conundrum of lost sales.
That's right, that's right.
That I think is one of the most exciting concepts
is the news vendor model.
News vendor as in the dudes
who sell the newspapers on the street corners.
Exactly, because that guy used to have
exactly the same problem
where every newspaper that you need to throw away
is way cheaper than not selling a newspaper
during that day.
Okay, so the news vendor model
is one way to deal with the variability of the world.
You can't predict the exact demand.
So you just figure out
which way will essentially cost you less.
But there is another way,
listening to the story again,
that Jan could have dealt with variability,
which is to have more than one farm,
to have more than one country,
more than one airplane,
more than one supply line.
That's exactly right.
And I think you point to one of the aspects
of this decision that creates tension.
You want to be efficient,
but you also want to be flexible.
And you can get flexibility
by trying to find other sources
for the same product sometimes.
And you say, well,
why he's not going to find
a second producer from Colombia?
Well, because if he split the order,
the order is gonna be more expensive.
Sure, yeah.
And that is going to be less efficient, 100%.
But it's gonna be more flexible
because if the winter is too strong in one country
and the summer is too hot in the other,
well, that may be balance things out
and you will still have your roses.
If you put all your eggs in one basket,
it might be very efficient, not very flexible.
And that's a technical operations term,
eggs in one basket?
Yes, I guess it is.
Speaking of eggs all in one basket,
our next story is about the supermarket checkout line.
Operations people are obsessed with lines.
Think about it.
Customers want to buy something.
Stores want to sell something.
And a long line is standing in the way
of everyone's happiness.
Customers are bored and annoyed.
The cashier at the front of the line is overworked.
MBAs call this a bottleneck.
But as you listen to this story,
think about how fixing a bottleneck,
like a supermarket checkout line,
can just create more bottlenecks,
create more annoyance.
The story is from 2016
and it's hosted by Jacob Goldstein and Nick Fountain.
Goldstein, the other day, you and I went to Walmart.
Welcome to Walmart.
We got peppers, apples, bread.
I got a Halloween card.
We were there because we're doing a story
about self checkout.
Yeah, we wanted to find out,
could we make it through self checkout one time,
just one time,
without getting some kind of error message from the machine.
We were there with Howard Schneider.
He lives a couple blocks away
from this particular Walmart.
And we were shopping there with him
because he's kind of an expert on self checkout.
Touch the item to purchase.
It was Fuji, right?
Move your Fuji apples to the back.
Everything was going fine
until we hit the red bell peppers.
Maybe it's under red, I don't know.
So you're scrolling through the pages,
looking for the right thing.
Red peppers?
Could it be B for bell pepper?
No, no peppers.
It was not B for bell peppers.
It doesn't even say what to do,
so then you're stuck here right now.
Doesn't even say get help or anything.
And Fountain, we'd probably still be standing there
trying to figure this out.
But for the fact that Howard went
and got a store employee who walked over
and saved us by typing in the code for peppers.
She just knew the number in her head.
The fact that we have to call the attendant
to process this little order is a failure.
Really, it shouldn't happen.
And the machine should deal with situations like that.
And why is self checkout a big deal to you?
Because I invented it.
Why wouldn't it be?
We're gonna skip ahead in the story
of how Howard Schneider created
the self checkout machine.
In a nutshell, he was a doctor and an inventor
and he wanted to make something like an ATM,
but for supermarket lines.
He perfected the scanning part,
the scale that weighs your items,
and the machine that accuses you of stealing things.
But he couldn't get a store to install the damn thing.
He gets a meeting at a New England supermarket chain
called Stop and Shop.
So he drives down, he gives this presentation
in this boardroom full of people.
And at the head of the table,
there's this executive who everybody's looking to.
This old guy sitting at the head of a table
and he says, son,
do you know why people shop at Stop and Shop?
I said, no.
He says, because of our people.
Because of our people.
And then everybody around the table
starts nodding their head.
And I think people wanna come in and speak to your machine.
Do you know anything about retail?
Do you know anything?
And he says, I don't think it's for us.
And then everybody around the table nodded their head.
And I drove back to Montreal
with my tail between my legs.
And it was just a horrible feeling,
thinking this is the stupidest thing I've ever done.
Nobody will ever like it or ever use it.
But Howard keeps loading his machine
into the back of this rented Ryder truck,
keeps going to supermarket trade shows.
And eventually he gets a meeting
called Price Choppers, based in upstate New York.
The head person actually saw the machines.
And you know what he said?
He looked at it, he says, I like it.
Let's do it.
And guess what?
After that, everybody's very nice.
The CEO says, we're not gonna buy the machines from you,
but you can use one of our stores in upstate New York
as a real world experiment.
And on August 5th, 1992,
grocery store shoppers use what may be,
depending on your definition,
what we are gonna call
the first fully automatic self checkout machines.
When Howard gets to the supermarket that day,
he sees that there are protesters there.
It's the cashier's union.
They're saying, these machines are taking our jobs.
Howard read us this quotation
from a union rep at the time.
And the union rep basically said,
this thing that I think about all the time,
these machines are forcing customers to do more work.
Quote, maybe if the customers come early,
they can unload the truck and stock the shelves, unquote.
Well, I mean, like there is a serious question
underneath it, right?
Which is like, are these machines taking people's jobs?
But the answer is very anti-climactic.
Let me tell you what happened to Price Chopper.
The machines went in, people used them,
and they didn't work.
It crashed.
It stopped working and then people had shopping carts
half unloaded and everything stopped.
The store is full of angry shoppers
and Howard, he's just sitting there
in the middle of all this chaos,
unscrewing the back of the machine
so that he can restart it.
And the union, they figure they've got nothing to worry about.
They pack up their protest and leave.
Howard stays up all night,
sitting there in the grocery store, fixing the code.
He says he can still remember smelling the cinnamon buns
that are baking in the back of the store
while he's sitting there trying to figure out what's wrong.
And the next day, his machines didn't crash.
But the shoppers and the machines,
they still needed a lot of handholding.
In fact, they need so much help
that Howard has to invent something else.
He has to invent the person
who stands there next to the self-checkout machines,
helping the customers and fixing the machines.
We drilled some holes in the cabinet
so that if you had to reset the machine,
you could just stick the long screwdriver in
and hit the reset button.
So we gave him a long screwdriver.
And he was very friendly, very nice with people
and he'd help them through the orders
and that made a huge difference.
And so the self-checkout machine was born
along with the employee standing next to it
to actually make it work.
Since that moment,
the self-checkout machine has muddled along.
Howard Schneider eventually sold his idea and his company
and the self-checkout machines slowly started
to move into grocery stores.
Now a little more than half of consumers report
using self-checkout every week.
Was this an operations triumph
or an example of moving
from one inefficient process to another?
We'll have our professor weigh in after the break.
We are back with our professor today,
Santiago Galino.
Santiago, you specialize in retail operations.
So I can ask you the question.
I just have to ask you.
These self-checkout machines seem to be everywhere
and yet we hate them.
I hate them.
How can this be?
Who can stop this?
I am with you.
I'm with you, Robert.
By transferring these to customers,
the retailer is saving a lot of money
because retailer has two expenses
that go to the top of the list,
inventory and staff.
And if they can reduce one of those,
they are gonna do it.
They're reducing the staff expense
because you and I are doing the job.
Should we have just said no?
That's one option.
We could all stop using it
and so then they will actually start to pull back.
But we're in a rush
and it turns out that it actually helped
to get things flowing and increase the capacity.
It turns out it is faster.
We accept it because it's faster.
Yes.
I think that the reason why we accept that
is because if you show up to the checkout process
and there is a real cashier
and you need to wait for that person
or there is an empty self-checkout,
the temptation is too big.
You will go for it
because you want to get out of there fast.
Even if I don't like the process of checking out.
That's right.
It's painful,
but for the companies it's cost effective.
And I think operations is getting the right balance.
You want efficiency,
you want to move along in the process,
but you want to also keep your customer happy
and your employees happy as well.
So let's talk about lines for a moment
because I think where a lot of us
encounter operations problems
is as we're standing in a very, very, very long line,
moving slowly and we start to think,
what is going on here?
So I'll ask you, if you're standing in a line,
if it's taking too long, what is going on?
Well, there are two reasons why we can have a line,
especially if it's a long line.
One is that we have more demand than capacity.
That means that we have less cashiers
than we actually need.
Because maybe we went to the grocery store after work
and there's just everybody's shopping at the same time.
That's right.
But there is another reason that goes together with this
that is that you can have a line
when you have enough capacity,
but there is a lot of variability.
Variability, what does that mean?
Well, imagine that you show up to the grocery store
and in front of you, there is this person
that takes every product very slowly to the cashier.
Yes, yes, I know them.
Or if you are in front of the self-checkout
and you happen to be behind me
and I start to mess things up
and you are rolling your eyes
and I'm adding variability to the process.
Because once you have variability,
then there's going to be these,
I guess the technical term is bottleneck.
The bottleneck is the step in the process
with the smallest capacity.
You are going to start to experience a bottleneck
because you have now less capacity
than the demand you need to serve.
Now it seems like a lot of people are experimenting
with different forms of lines.
I mean, we heard about the self-checkout machine.
But there's the system that they use in Trader Joe's,
if you've ever been there,
which is it's one long line and like 30 cashiers.
But then there's a lot of places
that have different lines for different people.
What is the best way to shorten a line?
Well, those dedicated lines for 30 cashiers
are trying to reduce variability.
And if you think about it,
that will give you a more consistent line,
even if it's a longer one,
but you really don't care
because you have enough capacity, 30 cashiers,
to deal with that one long line.
So if there's one slow cashier,
and if I have to pick a cashier,
I might pick the slow cashier.
But if you have all these different cashiers in one line,
then it's probably not going to slow everybody else down.
On average, you're going to be better.
And that average is helping you with the variability.
Professor Santiago Galino from the Wharton School,
thank you so much for being our professor today.
Thank you very much, Robert, it was a pleasure.
It was efficient.
Indeed.
And our professor has left us with some vocabulary words
that you can practice while waiting in long lines.
The first one is the news vendor model.
This is the calculation you should do
when you think about how much product to order.
What will it cost to throw away an extra newspaper
you don't sell versus the money you will lose
if you run out of the product?
We also have as vocabulary two things
that can create long lines, capacity and variability.
Do you have enough staff to help the customers?
That's capacity.
But variability means that one slow customer
can grind the whole line to a halt.
This creates our last vocabulary word, the bottleneck.
Of every part of the process,
which one is the slowest,
the one with the longest line forming behind it?
That's your bottleneck.
And fixing that can speed up the whole process.
We are two weeks away from the end of summer school
and we'll have our graduation episode then
including actual business pictures
from actual Planet Money listeners like you.
We'll also open our final exam online.
If you pass it, we will send you something
that in a very dim room might look a lot
like a business school diploma.
You've all earned it.
Our summer school series is produced by Max Friedman.
Our project manager is Julia Carney.
This episode was edited by our executive producer,
Alex Goldmark and engineered by James Willis.
The show is fact-checked by Sierra Juarez.
I'm Robert Smith.
This is NPR.
Thanks for listening.
Support for NPR and the following message
come from Carnegie Corporation of New York.
Supporting innovations in education,
democratic engagements and the advancement
of international peace and security.
More information is available online at carnegie.org.
And a special thanks to our funder,
the Alfred P. Sloan Foundation
for helping to support this podcast.
