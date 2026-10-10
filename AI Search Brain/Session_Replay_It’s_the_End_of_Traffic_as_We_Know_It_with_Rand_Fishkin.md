# Session Replay: It’s the End of Traffic as We Know It with Rand Fishkin

- Tab 1

00:05

Alright.

00:08

It's great when we get people coming in.

00:14

Are you, at the moment, you're in Seattle around?

00:17

In Seattle. Yeah.

00:19

At home. How about yourself?

00:22

Just in Sydney. Yeah.

00:24

I'm planning a holiday,

00:26

almost when I was in New Zealand a week ago,

00:28

but,

00:30

a friend actually actually offered up a a tiny home,

00:33

about 90 minutes here from Sydney, so I'm just gonna

00:35

go remote.

00:36

But I've never done solo before. That's my plan.

00:40

Just go and chill out.

00:42

Yeah. That sounds fun.

00:44

Yeah. Not too bad. We usually

00:47

try and stay in Seattle during the summer because

00:50

every other place on Earth is way too hot.

00:54

Yeah. But but it's it's so comparatively nice here.

00:58

Yeah. Exactly.

01:00

We just had Laura join. We'll just put another couple

01:02

minutes for

01:04

anyone else. Otherwise, it's a recorded session so we're posting

01:06

to the, the community.

01:08

But nearly

01:10

close to 200 people now, actually. So it's

01:13

it's getting pretty cool and pretty active.

01:15

Yeah. A muzzle tov.

01:17

Yeah. Thank you.

01:19

And we've had some great speakers. So

01:24

Wonderful.

01:25

That's where I'm going.

01:31

Yeah. I think when we originally were scheduled to do

01:34

this,

01:38

we were in Astoria, Oregon. And so I, I borrowed

01:41

Cyrus Shepherd's office

01:43

Yeah. Set up in there,

01:45

yeah, to, to give this talk. And then

01:48

and then, you know, waited there for 30 minutes, and

01:50

we canceled. So I was like, okay. No problem.

01:53

Yeah. Yeah. Sorry, man. Anyway, we're we're good good as

01:56

time.

01:58

I did I did find out though that Saris has

02:00

the worst office chair in the world.

02:03

It was so horrifying to sit on even for those

02:05

30 minutes that I,

02:07

immediately ordered him a new chair.

02:10

I was like, buddy.

02:12

Oh my god. This is this is your Christmas and

02:15

Hanukkah and birthday present. You just Yeah.

02:17

Kills me, but People are I'm like, I'm all about

02:20

chairs.

02:21

I'm sitting on an Aeron chair right now, and I

02:23

can't like, my, very,

02:26

lucky over at Fonda. We had some good chairs. So

02:30

Yeah, man. You gotta you gotta invest in the chair.

02:33

It's just

02:34

Hundred percent. Know. That's like

02:36

work 1 0 1

02:38

Yeah. I remember when COVID hit. There's a big logistics

02:42

exercise. Everybody picking up their co their, I was gonna

02:44

say COVID chair. The Aaron's taking them home. So,

02:51

anyways, I'm I'm mindful of your time. I think we

02:53

will kick off, and as stragglers come in,

02:56

we can,

02:58

yeah, just having the the participants listen, leaving comments in

03:01

chat.

03:03

Sounds good.

03:09

Cool. I'll, I'll do a little bit of an intro.

03:11

Not that you you need it.

03:13

But, yeah, Rand,

03:15

obviously, we've known each other a long time. I I

03:17

put out a LinkedIn post,

03:20

in 2006

03:21

I believe. I was, hanging out on,

03:25

search engine watch and, asking you questions about Internet marketing.

03:29

And,

03:30

little did I realize you were going to become

03:33

pretty much the most well known person,

03:36

not only in SEO, but across marketing. You are extremely

03:39

well known, and,

03:40

you've you've since founded several companies.

03:44

CEO, co the cofounder of SparkToro,

03:46

Lurtmau5,

03:47

obviously, Snackbar Studio,

03:49

and then previous life, Moz, which,

03:52

for all of us had such a huge impact,

03:54

on the industry. And and we're so thankful of, you

03:57

know, for all the blogging in the original days, like,

03:58

on ACM laws and then eventually the the epic conferences

04:01

and,

04:02

putting on a stage, which honestly has,

04:06

yeah, just really brought the industry together and, allowed us

04:08

to stay ahead. And I I think AI, socially, this

04:11

is very much inspired by, you know, the the path

04:13

that you you like for us, and,

04:16

we're just trying to do, you know, what we can

04:17

to help people through this massive shift in AI search.

04:20

And so I think your presentation today is going to

04:23

be

04:24

really useful for us, as as always. I've always,

04:28

I used to make the trek out from Sydney,

04:30

1st myself over to Seattle to go to to to

04:32

coast at MozCon.

04:34

And then, eventually, at some point, we had, like, you

04:36

know, cohorts of something like 10 people heading over just

04:39

to to learn from you in the in the

04:41

the squad. So,

04:42

yeah, very, very appreciative of your time today, Rand. And,

04:46

you know, please, guys, if you have any questions, throw

04:48

them in the chat. Otherwise, we've got a whole bunch,

04:50

for you, obviously.

04:51

Yeah, there's so much to learn. Thank you. Over to

04:54

you.

04:55

Yeah. Great.

04:56

Well, Jeremy, so,

04:58

you asked me to give this

05:01

presentation, which I'm gonna

05:03

pull up my screen.

05:05

Alright. So we can we can see that here. And

05:08

I've got,

05:09

we can hide this guy.

05:12

I've got a bunch to get through, so I'll I'll

05:14

just go quickly. And if you wanna interrupt me, go

05:17

right ahead.

05:19

And if we've got questions at the end, that's great

05:22

too. So

05:24

most of the folks who are, watching, listening will probably

05:27

know that Amanda Natividad and I,

05:30

wrote a new book called 0 Click Marketing, and it

05:32

it is because

05:34

it's not because I wanted to write a book. Dear

05:36

god.

05:38

Writing a book extremely painful and challenging, but but I

05:41

was convinced,

05:43

by Amanda and by our publishers that this,

05:47

epoch, this era

05:49

deserves and needs

05:51

sort of a a grounding to help folks understand what's

05:54

changed, why it's changed,

05:56

and what that means for digital marketing. So I'm gonna

05:59

I'm gonna give you a brief tour of that today.

06:03

1st I'm gonna take you through

06:05

the old way. Most of you on this call, I

06:07

suspect, probably remember what digital marketing was like for the

06:11

last 30 years, which which I sort of describe as,

06:13

like,

06:14

classic funnel

06:15

shaped digital marketing. Right? So, you know, you have your

06:18

top of the funnel where you get attention, you get

06:20

your 1st impressions, and then that that middle of the

06:23

funnel, right, which is where you turn attention and curiosity

06:26

into,

06:27

your attention about your brand. Right?

06:30

And then you try and turn that curiosity into demand

06:34

and overcome the objections that people might have so that

06:37

eventually you get a conversion.

06:39

And the idea was that at the top of the

06:41

funnel

06:41

for these 1st 30 years,

06:44

we earned attention through search and social and ads and

06:47

content and PR and and everything we did on the

06:49

web.

06:50

And then we drive as many people as possible to

06:53

our website

06:54

for the middle of funnel and bottom of funnel and

06:56

conversion process. Right? And that's where we turn visitors into

07:00

fans

07:01

and subscribers and eventually customers via your website and email

07:04

list.

07:07

And

07:10

all of this

07:11

all of this

07:13

is what people now want. Right? Like like, what is

07:17

happening today is that

07:20

this

07:21

world, this world that used to happen on your site,

07:24

is now

07:25

happening

07:27

in answers that come from search and responses from AI

07:29

tools and content from creators and threads on Reddit and

07:32

videos on YouTube,

07:34

even communities like ours, like like this 1

07:37

All of that stuff is happening in those places, not

07:39

on your site.

07:41

And that has completely changed how the funnel works. Like,

07:45

yes, people will still use your website to convert. Right?

07:47

There's all these stories of,

07:49

traffic down, revenue up. Right? Conversions up. But

07:53

this is just not it's not what the platforms want

07:55

because they can better monetize people when they keep them

07:58

on there.

07:59

And it's not what people want because we've been trained

08:02

to get accustomed to not having to click, not having

08:05

to go to anyone's site. So the you know, we

08:08

Amanda and I are kinda like that. Those 1st 30

08:10

years of the web, that's done.

08:13

You've probably seen graphs like this, tons of graphs like

08:16

this, this 1 from Google Search Console, right, which is

08:18

the idea that clicks keep going down, but impressions are

08:21

going up. So more and more people are

08:24

seeing my content just not on my website. They're seeing

08:28

it

08:28

in Google's results or in the AI overview or

08:32

across the social platforms.

08:34

And marketers have taken to calling this the alligator graph,

08:36

which I think is a great name. So it does

08:38

kinda look like an alligator, especially this 1 It's got

08:40

that crooked jagged teeth at the end there.

08:44

Wait. Jeremy, do you remind me, Australia, do you have

08:47

crocs or gators?

08:50

Crocodiles. Yeah. Yeah. Crocodiles. Okay. Okay. Alright. Well, gators, I

08:54

guess, that's the that's the American version.

08:57

Down under, we can call it the crocodile graph. And

09:00

this is not just you, by the way. Right? This

09:02

is if you're looking at this and you're kinda nodding

09:04

your head like, oh, yeah. I have noticed, a, traffic

09:06

is getting way harder to get, and b, traffic is

09:09

down despite me doing better and working harder than ever

09:13

before. You are not alone. This is study after study,

09:17

industry after industry. This 1 recently shared by by Cyrus

09:21

Shepherd, which I I came across from Daniel Stanica,

09:24

looking at 100 very successful blogs from literally 4 years

09:28

ago. Right? We're not talking about, like, 10 years or

09:30

something. This is this post COVID. Right? This is

09:34

blog universe definitely in the social media era, and yet

09:38

0.5 of these sites wiped out,

09:41

another

09:42

25 percent gutted or or declining.

09:47

Only a few. Only handful still growing their traffic. And

09:50

and that's mostly because they're brands beyond

09:53

the blog themselves.

09:56

Okay. There I I do wanna point something out. Whenever

09:59

I give this presentation, especially to folks outside of sort

10:01

of hardcore digital marketing world, a lot of people make

10:05

the assumption that search must be dying and that AI

10:08

is replacing it. And that's what's causing this whole change.

10:10

And that

10:11

that is not true at all. That is absolutely not

10:15

true. Well, with 1 caveat, 1 little caveat, but

10:18

you can look and see. Right? This is visits to

10:21

search traditional search engines. So Google,

10:24

Yahoo,

10:27

Bing, DuckDuckGo. Right? That's that's the big blue

10:31

here.

10:32

AI tools is in red. It's growing. It was 1.31

10:36

percent

10:37

last year. This year, it's 1.65

10:39

percent of all These are US devices,

10:43

that visited

10:44

1 or more of these tools 1 or more times.

10:47

And then ecommerce platform, so this would be like Amazon

10:49

or Etsy or eBay or Costco.

10:52

And,

10:54

man,

10:55

there's just no story. There's no story to be told

10:58

that AI is replacing search.

11:00

Traffic is absolutely shrinking. This, by the way, this, resource

11:04

I really appreciate from the Ahrefs folks. They they have

11:07

this panel of 75000

11:08

sites who've opted in to share all of their traffic

11:11

data. And so then you can see it all grouped

11:13

together, which is which is kinda great.

11:16

Essentially, what we're looking at is about a 10 percent

11:19

overall decline from what was probably the high watermark in

11:23

web traffic that was sent out

11:25

on the Internet, and that that is mostly driven by

11:27

Google.

11:30

Well, surely AI will save us.

11:32

No. No, my friend. I'm sorry to say

11:36

AI is not coming to save your traffic.

11:39

In fact, the the very, very opposite. So despite the

11:43

fact that I just showed that AI use is big

11:45

and growing, it used almost 10 percent as much as

11:47

search, you can see the traffic referrals are are 1

11:51

1 500th

11:52

of what search sends out. So So who is sending

11:54

it?

11:57

It is pretty

11:58

much organic search or no refer at all.

12:04

And then you, yeah, you can see organic social actually,

12:08

what, 20 times larger than AI tools,

12:10

yet social traffic gets no attention, and everyone is super

12:15

obsessed with how do I get traffic from chat g

12:17

p t.

12:19

I think I think most people are playing the wrong

12:21

game. They're getting they're getting biased by I don't think

12:24

it's digital marketers fault. I think it's executives who are

12:27

who all have AI derangement syndrome and just are super

12:31

obsessed with AI everything.

12:35

My my argument here is is that basically

12:38

well, I I don't think it's an argument. But what's

12:40

going on here

12:42

is that

12:43

when we search for things like, what are the best

12:45

real estate agents in Seattle? Well,

12:48

Google's basically trying to keep you on Google by just

12:51

answering that question.

12:53

Right?

12:54

And even when they send traffic out, it's going to

12:57

other Google properties.

12:59

The social web is

13:02

even worse if you can imagine it. Right? Essentially, inside

13:04

of Instagram, which is where more and more people are

13:06

turning for commercial activity of all kinds, even choosing real

13:09

estate agents,

13:11

that

13:12

is not sending any traffic anywhere.

13:15

I spoke at a real estate, conference recently and talked

13:19

to agents there who basically told me that

13:23

a lot of people,

13:24

especially younger buyers, are calling them up to spend, you

13:27

know, 1000002 million, 3000000 dollars on homes in Seattle because

13:30

that's the price of houses here.

13:33

And they do it off of TikTok without ever visiting

13:35

their website. Right? They hit their profile. They send a

13:38

DM. They're like, yo, dawg.

13:41

Let's buy a house. Right?

13:43

Hey. That

13:45

that that's commerce. That's how it's working.

13:48

There's no referral. There's no tracking that.

13:51

AI tools, which, as I mentioned, heavily used by about

13:54

20 percent of Americans and 30 percent of Europeans. I

13:57

apologize. I don't have Australia and New Zealand data, but,

14:00

that's something that Daedos is working on.

14:04

That

14:05

sends virtually no traffic out at all, which which I

14:07

think you all know. I I believe ChatGPT recently tripled

14:11

the amount of traffic that they send out, and it

14:13

is still

14:15

you know, it went it went from, like, nothing to

14:19

a little more nothing. It's really it's really quite pathetic.

14:22

YouTube, obviously, same story. Right? Reddit,

14:26

same story. Not 99 percent 0 click. Now Reddit used

14:28

to be a link platform. Jeremy, you and I remember

14:31

the days when you could get a bunch of traffic

14:32

from Reddit.

14:34

No more, my friend.

14:35

No more.

14:36

Alright. Why is this happening? What's go what's going on?

14:40

I'm I'm gonna talk through 3 sections here. I'll try

14:43

to do it in brief so that we leave some

14:45

time for q and a. But, essentially, rise of the

14:47

0 click web, then we'll talk about death of attribution,

14:51

which I I I think probably was always a myth,

14:54

but it kinda worked. You could, like, squint and make

14:56

it work for 15 years there. And then I'll talk

14:58

about how we fight back. So

15:00

0 click web.

15:02

This, is brand new data, which which,

15:05

some of you might have seen, and we we just

15:07

launched on SparkToro,

15:09

last week, couple weeks ago.

15:11

And,

15:13

essentially, this is what happens after

15:15

someone searches on Google in the United States. This is

15:18

a blended average of mobile and desktop, where mobile is

15:22

about 0.667 of all Google searches,

15:24

desktop about 0.333

15:26

So desktop is gonna be heavier in clicks, mobile lighter

15:29

in clicks.

15:30

You can see here, 32 percent of people click on

15:33

something,

15:34

but tragically more than 0.25 of those go right back

15:37

into Google's ecosystem.

15:39

YouTube, Google Maps, Google News, Google Images, another Google property.

15:43

6 percent paid, 66 percent organic, which which is what

15:47

we call sort of the open web. Right? Like, that's

15:49

open web referrals.

15:51

39 percent

15:53

of people who search do nothing. They they walk away.

15:56

They have no activity in their browser for the next,

15:59

like, whatever. I I think the the delay was, like,

16:02

10 minutes or something. Right? So they they they basically

16:04

don't do anything. 29 percent perform another search sometime in

16:08

the next few minutes. And that that,

16:11

is where we get our 68 percent 0 click searches

16:13

number. I I can't tell you whether those people performing

16:16

another search are refining the search they originally made or

16:19

whether they're in the grocery store and they're like,

16:22

what kind of flour do I need to make pizza

16:24

dough? And then, you know, they get the answer to

16:27

that, and then they search for and how old is

16:29

Tom Cruise? You know? Like, I don't know how related

16:32

these queries are. We we're not able to get that

16:34

data from the,

16:36

Clickstream panel,

16:38

but I can tell you that 68 percent of searches

16:41

result in no click on anything that comes up in

16:43

those results. And that means for every thousand US Google

16:46

searches, 232 clicks go to the open web. You might

16:48

remember that just 2 years ago, that number was about

16:51

350

16:52

So we have seriously

16:55

declined. You can see that here.

16:57

20 16

16:58

we had 45 percent 0 click searches. 20 26

17:01

68 percent. So

17:04

really, really significant growth. And the most significant growth has

17:07

come in the last 2 years when we grew a

17:09

full 8 percentage points,

17:12

in 0 click.

17:14

Now

17:15

the weird part of this is, we also this is

17:18

from, a research study we did last year with Datosys

17:21

data

17:22

where we looked at branded keywords and generic keywords and,

17:26

the searches that made up them. You can now see

17:28

this in Daedosis quarterly state of search reports, which I

17:31

urge you to check out. They're they're free to download

17:33

and,

17:34

quite comprehensive.

17:36

I also do a webinar every 0.25 with Eli Goodman,

17:38

the the founder,

17:40

on those

17:41

reports and sort of what's going on. But, basically,

17:45

what what these graphs are saying, what I'm trying to

17:47

show you here is that

17:49

0.5 of all people who search Google already know what

17:52

they want.

17:53

They're not searching for running shoes. They're searching for Nike.

17:57

You know, they're not searching for real estate agents. They're

18:00

searching for Joseph Goldberg, Seattle real estate agent. Like, it's

18:03

it's

18:05

we we perceive this growth in search

18:08

or,

18:09

you know, volume as being

18:12

transactional opportunities,

18:14

but, really, 0.5 of all people have already chosen what

18:18

they're gonna do. And so you have to be in

18:21

front of them before the search happens.

18:24

I really think this is your new home page. This

18:27

is our new home page, and we we treat it

18:29

that way, and we believe this is

18:33

sort of the the future of how people are gonna

18:35

perceive our brand.

18:37

Yes. Our homepage still matters. Yeah. You can go to

18:39

SparkToro and whatever, get a free report or sign up

18:41

or whatnot.

18:42

But Google has decided

18:45

that that these are our, you know, this is our

18:47

competitive space, Semrush and Answer the Public and

18:50

SimilarWeb and Ahrefs. Quite frustrating for us. Right? We're not

18:53

in the SEO space. We don't do, like, keyword data

18:56

stuff. So Semrush and Answer the Public and Ahrefs are

18:59

really not relevant. SimilarWeb is pretty relevant. SimilarWeb, I would

18:59

say, excellent, very

19:02

Similarweb is pretty relevant.

19:04

Similarweb, I would say, excellent. Very glad to be in

19:05

that in that thing. You can also see here. Right?

19:07

This is these

19:09

are really gonna nudge people to think about our brand

19:13

in a cost type of way.

19:15

Right? It it wouldn't it be so cool if I

19:18

could get people to, you know or Google to show

19:21

people also ask,

19:24

what types of data does SparkToro show, or what can

19:27

SparkToro tell me about my audience?

19:30

But, unfortunately,

19:31

not not getting that here. And I think these are

19:34

your home page as well. What AI says about you

19:38

is very much

19:41

influencing people.

19:44

I will point out recent studies have shown that,

19:46

what a the response AI gives

19:49

is

19:50

incredibly hyper personalized based on everything you've ever talked to

19:54

about it.

19:55

Almost no 1 anymore is getting,

19:58

what do you whatever you wanna call it, like, history

20:00

free AI responses.

20:02

And so your AI tracking tools that are telling you

20:05

what a

20:06

logged out 1st time,

20:08

you know, request from the API. Is there

20:12

almost certainly

20:13

way, way off of what actual human beings are seeing.

20:17

How how can you actually see what's in there?

20:20

Wait for Chat, GPT, and Claude to

20:23

to come out with some some analytics, I guess. I

20:26

I don't know. It's it's pretty nasty.

20:29

This is not just Google, by the way. Right? Like,

20:31

when when we talk about 0 click, it's not just

20:33

search and AI tools.

20:36

You know, a few years ago, in fact,

20:38

the folks at Facebook

20:40

realized

20:41

that by sending traffic out,

20:44

which they were becoming a major referrer, you know, back

20:46

in this is this is 12 years ago now. Right?

20:48

But Facebook was passing Google as a referrer of traffic

20:53

to major news sites in the United States.

20:57

That that was a wild era. This was an era

20:59

when you could chase Facebook traffic and reasonably do quite

21:03

well.

21:04

And then sort of the, you know, folks behind the

21:05

scenes were like, wait a minute. Wait a minute. We

21:08

already reach everyone on Earth. How are we gonna grow?

21:11

Oh, we need to keep more people on Facebook. Facebook

21:14

should be where you get your news, not

21:16

independent journalism and and and news sources.

21:20

That, of course, has gone wonderfully for world politics and

21:23

current affairs. So I I had us off to Facebook

21:26

for helping us enter this new era of peace and

21:29

prosperity.

21:32

Instead

21:34

of clicking, they realize what they really want.

21:37

Scrolling.

21:39

Let's just keep everyone scrolling.

21:42

Oh, there you go. Facebook referrals to

21:45

anybody, never mind news, but anybody have fallen off. Right?

21:48

Let's

21:50

stock bonuses, brah. If you if you get those stock

21:52

bonuses,

21:55

all we have to do is just just put a

21:57

little thing in our algorithm and it says, does your

22:00

post contain a link?

22:01

No visibility for you.

22:04

And this

22:05

this became the era we're in. Amanda and I did

22:08

a research study with

22:10

Really Good Data, see from Really Good Data,

22:13

last year no. Couple years ago where we looked at

22:15

0 click content across web platforms and their preferences and

22:19

basically

22:19

every major platform

22:22

with 1.5

22:23

exceptions,

22:24

Mastodon. And, technically, Blue Sky does not bias against links,

22:28

but their algorithm does reward things that get more engagement.

22:32

And turns out links get less engagement because people have

22:35

been trained not to click on things on social media.

22:37

They they wanna just stay in the platform they're on.

22:40

And so

22:41

it's really it's really just Mastodon

22:43

that's giving you that,

22:45

that old, you know, sort of Twitter, Facebook experience from

22:48

a dozen years ago.

22:51

Right now, what we are seeing actually need to update

22:54

this. What we need what we are seeing is that

22:56

when we test these out, and we've been doing a

22:58

bunch of tests more tests recently around this because we

23:01

we really wanna confirm it,

23:03

where we put up posts,

23:05

1 with a link, 1 with no link. This one's

23:06

on Facebook, but I do this test. You can see

23:08

me doing these tests all the time on LinkedIn, on

23:11

Twitter, on,

23:13

threads, which threads has become

23:15

considerably bigger than Twitter now. I think there are 500000000

23:19

users.

23:20

So just just wild. And we're seeing

23:23

not not 10 x, friends. We are seeing actually, I'm

23:26

gonna live update this so I don't, mess it up

23:28

in the future. There you go.

23:31

We're seeing 12 x the reach right now

23:36

with posts that contain no links.

23:39

That's that's pretty remarkable.

23:41

Also true, by the way, for Reddit, although a lot

23:44

of my Reddit posting is to I post a lot

23:46

to, like, data is beautiful and charts and graphs and,

23:49

like, some of the marketing subreddits.

23:51

And in those places, a lot of time, they do

23:53

require that you include a link, but no 1 ever

23:56

clicks it. It's more like a you know, it sits

23:58

under the post unless you unless you click in,

24:01

you're not gonna see it. Similar to YouTube.

24:04

I think these,

24:06

your social platform, these are your home page as well.

24:09

Remember I was showing you, like, you know, the real

24:11

estate agents who get found on Instagram?

24:14

Their their home page is essentially their Instagram profile page.

24:17

That is where buyers are determining

24:19

whether they are gonna use their services.

24:22

They're deciding based on their reels and their videos and

24:25

their photos and images and their description and what they

24:28

get when they click the more button.

24:30

That that is where it's happening.

24:33

Very, very different from,

24:35

oh, hey. You know, my my behavior my behavior, because

24:38

I I grew up in the, you know, early Internet,

24:42

is if I see something I'm interested on on Instagram,

24:45

I click the profile and I look for the link

24:47

and I go to their website.

24:49

And that is that is not how

24:52

a lot of folks are using it. I and I

24:54

don't think it's a generational thing. I see older folks

24:57

doing this, folks older than myself, who also view social

25:00

as essentially a 1 stop shop.

25:03

Alright. So let's talk about attribution

25:05

and measurement.

25:08

Friends, we and I say we,

25:10

very much including myself, Jeremy, you you mentioned all those,

25:13

all those years at Moz. I I spent 0.25 century

25:17

trying to convince executives to invest in digital channels and

25:20

move their budgets out of, you know, brand advertising,

25:24

Super Bowl ads, and,

25:26

billboards and television,

25:28

media you know, of all kinds.

25:31

And our big weapon in that fight was you can

25:33

measure it.

25:34

You can see every step along the way of every

25:37

journey, and you can say, hey.

25:40

Before,

25:41

you know, this is back in the most days. Right?

25:43

Before someone bought a subscription,

25:45

we could go and look in our analytics and be

25:47

like, okay. They visited an average of 10 posts. These

25:50

were the most influential posts on their behavior.

25:52

They tended to subscribe

25:54

7 months before they converted to a paid account. They

25:58

tended to run this many reports before they converted.

26:02

These were the channels that referred the traffic.

26:05

That's gone. That is

26:07

gone in the wind. Like, you you can't do anything

26:10

close to the kind of measurement that you used to

26:12

be able to do. But we trained

26:14

we trained these execs

26:16

that every conversion,

26:18

every sale could be attributed, put in these nice little

26:20

buckets, and then we could assign percentages

26:22

to each different 1 depending on on how we thought

26:25

it went. And it it went sideways because

26:29

of 3rd party cookies

26:30

stopping stopping functioning in every browser except Chrome. Right?

26:35

1st party cookies getting way less effective than they used

26:37

to be. Users manually blocking, tracking,

26:41

and and doing it with,

26:43

software. Right? These

26:45

all of the ad blockers that are installed on a

26:47

huge percent of machines across the world,

26:50

those don't just block ads. They block Google Analytics.

26:54

They block

26:55

almost every tracking technique you can imagine.

26:58

The browser fingerprinting

26:59

that, you know, we try and use in the United

27:02

States, that's illegal almost everywhere. You cannot do that outside

27:06

the US. A lot of Americans are like, oh, browser

27:08

fingerprinting. Yeah. Yeah. Yeah. Europe, forget about it. I don't

27:11

can you do it in Australia?

27:16

No. It's actually, yes. Same sort of issue issue here.

27:19

Yeah. Yeah. Yeah. I I mean, look, it should be

27:22

illegal. Right? But America is basically like, did you pay

27:25

the right politicians? You get whatever you want.

27:28

So, you know, apart from countries that have legalized bribery,

27:31

you cannot do this.

27:33

Essentially, the way I view it is

27:35

you can't really track someone before they've logged in. Once

27:38

they've o authed or given you a username and password,

27:41

email and password,

27:42

yes, then you can start to see their their patterns

27:44

of behavior on your site. Before that, no. Not not

27:48

really. Yeah. Like I mentioned, what's possible in the US?

27:51

Not possible most place. Oh, yeah. Here we go. Australia.

27:54

Oh, privacy act. There you go. No dice, friends.

28:00

I think, you know, if you if you haven't been

28:02

in this field very long or even or even if

28:03

you have, you might have forgotten how easy it used

28:06

to be to justify

28:07

those investments. Right? When you could basically point to, like,

28:10

hey. Look. We ranked number 12 for this keyword. We

28:13

got 4 conversions on it last week. So if we

28:15

move to number 2 we would get 40 time you

28:18

know, we get 80 conversions

28:20

next week.

28:21

Boss, can I have some money for SEO? Hell, yeah.

28:23

You can.

28:24

Right?

28:25

It's you know, what's vanishingly weird to me is how

28:28

much budget is getting assigned to AI visibility

28:32

when can't nobody

28:34

prove no conversions came from no AI.

28:36

It's it's wild. I mean, great. Like, I hope the

28:40

you know, hopefully, no 1 ever looks at the books,

28:43

but,

28:44

someday

28:45

someday someone might.

28:47

I think the problem is Google sort of learned that

28:49

their monopoly power was untouchable. I don't know I don't

28:52

know what sort of sweetheart deal they got with judge

28:54

Meta, but, when the anti remember that that Google lost

28:58

lost the antitrust case in the United States. Right? This

29:01

was a a case that was brought by the Trump

29:03

administration the 1st time. It was continued under Biden. It

29:06

was 1 of the few bipartisan

29:08

things that has happened in the American government in the

29:10

last 12 years.

29:12

And yet,

29:13

when judgment day came after the Department of Justice won

29:16

their case against Google proving that they intentionally

29:20

did things like manipulate,

29:22

their results to drive more clicks to ads and make

29:24

the results worse so that people would would click those

29:27

ads,

29:28

All sorts of shady stuff in monopoly power.

29:32

Do you know do you remember what the meta fine

29:34

was?

29:35

I say meta fine. The the judge meta's fine against

29:38

Google.

29:39

It was 2000000

29:42

dollars,

29:43

which which Google

29:44

made before the end of this sentence.

29:50

Yeah. So,

29:51

essentially, you know, Google sort of learned that they can

29:53

do all sorts

29:55

of sketchy stuff. Right? If they wanna conflate unbranded and

29:57

branded keywords,

29:59

if they want to turn your performance max campaign into

30:03

a money generator for them and and a loss machine

30:06

for you, if they wanna,

30:09

switch to less granular behavioral tracking and then and then

30:12

put that inside GA, right, to make

30:15

all the models that are unfavorable to Google's ads, like,

30:19

not possible to use in GA anymore

30:22

or literally make search results works to sell more ads.

30:24

This was this was from the,

30:27

Department of Justice case. Right? Here's the

30:30

the smoking gun as they like to call it. And

30:32

just nothing happened. Right?

30:35

So

30:36

when when I dig into our analytics this is Mark

30:38

Toro's analytics, I think, from last year. I was looking

30:41

at,

30:42

you know,

30:43

76

30:44

percent of all our visits come from direct. Like,

30:48

seem weird to you guys, especially when you when you

30:50

look at where they're going.

30:52

Like, these you are did someone really type in

30:56

spark toro dot com slash blog slash a I hyphen

30:58

generated hyphen content hyphen is hyphen the hyphen new hyphen

31:02

floor?

31:04

I can't see it. I don't think that happened. That

31:08

doesn't seem like a direct visit at all.

31:11

What's really going on?

31:13

Well, so we ran an experiment,

31:15

again, with Steve from Really Good Data, and you can

31:18

you can find the link in here. The presentation

31:20

will will include all the links

31:22

and found that entire networks are hiding referral data. If

31:26

you've ever gotten a visit from TikTok, no. You didn't.

31:29

Right? Like like, TikTok sends you

31:31

may send you traffic from the profile link just like

31:33

Instagram would, but

31:35

100 percent of that traffic is completely hidden. WhatsApp, hidden.

31:40

Discord, hidden. Mastodon, hidden. Slack, hidden. Facebook Messenger, for some

31:44

reason,

31:45

some 1 out of 4 times, they'll send a refer

31:47

string.

31:48

Instagram,

31:50

7 out of 10 times, they sent a refer string.

31:52

30 percent of the time, they didn't. There's no con

31:53

there was no consistency. It wasn't like the app did

31:55

it 1 way and the desktop version of the mobile

31:58

web version. Nope. Just just didn't. Same with LinkedIn. LinkedIn

32:01

is hiding more

32:02

stuff. Most of the AI refers this is some great

32:05

research, compiled by Will Critchlow over at SearchPilot.

32:09

And you can see that a bunch of theirs is

32:12

direct and dark.

32:13

Right?

32:15

I think this is why if you look at that

32:17

Ahrefs panel data again, that's the 75000 sites, you can

32:20

see that direct has gone to,

32:22

you know, over the they they don't show the previous

32:25

year. But over the last 2 years, basically, it went

32:27

from,

32:28

you know, below significantly below search to above search, and

32:31

now it is way above search. It is the number

32:34

1 refer by a by a mile,

32:36

direct type in.

32:38

And and they

32:39

they also

32:40

have unknown, which,

32:42

by the way, that's growing. Great.

32:45

I think that's just more direct.

32:47

Or direct should all be unknown. Right? Because we we

32:50

really we really don't know what that is.

32:54

So there's, there's this elephant in the room I wanna

32:56

talk about, which is

32:58

it's this quote, which I know has made its way

33:00

around the marketing universe, but I I think it is

33:02

still hugely important.

33:04

So this is Brian Chesky, the CEO of Airbnb on

33:07

an earnings call in 20 23

33:09

I believe.

33:11

And he's talking about the previous

33:13

2 or 3 years, basically, 20 20 21 22

33:17

And he's saying, like, hey. This what the pandemic showed

33:19

us is that we can take marketing down to 0

33:21

He says marketing, but he does not mean marketing. He

33:24

means advertising.

33:25

He means paid performance advertising,

33:27

just to be clear, and get 95 percent of the

33:30

same traffic as the year before.

33:33

And in context here,

33:35

by the way, Airbnb was showing that more than 30

33:38

percent of all their bookings,

33:42

claimed as a as attribution

33:45

a paid referral.

33:47

But, obviously, when they turned it off, only 5 percent

33:51

was incremental lift.

33:54

And the New York Times wrote about this, dug into

33:56

the numbers, and found exactly that in their docs. So

33:58

this was this is not a false quote. This is

34:01

this is actual truth from a public company CEO who

34:04

knew it was possible. Definitely not Elon Musk.

34:09

And I like to tell this story. For those of

34:12

you who've heard it before, I will tell it very

34:13

briefly.

34:14

So this, this pizzeria owner

34:17

in Milan, not real, by the way. This is a

34:19

parable. Remember? Parable. Fake story. Real real outcomes.

34:24

Real takeaways.

34:26

She

34:27

decides she wants to get some more business. And so

34:30

she hires 3 neighborhood scamps

34:32

around,

34:33

Northern Milano.

34:35

And she she gets these kids to pass out

34:38

flyers with a discount code for the pizzeria. And and,

34:41

of course, the flyers each have

34:44

a different color. So she knows when the flyers get

34:46

turned in by the customers,

34:48

which kid distributed it. So the, you know, green, red,

34:51

white, the colors of the Italian flag make it easy

34:54

on everybody.

34:55

Now after a couple of months,

34:59

she looks at the receipts and she's like, oh my

35:01

god.

35:02

The green flyer kid is crushing it. Like like, more

35:05

than 9 out of 10

35:06

new customers who are coming in with a flyer, coming

35:09

in with the green 1 we're getting the most sales

35:12

from them.

35:13

This kid's amazing.

35:14

The other 2 you're fired.

35:16

Green flyer kid, keep it up. Like, whatever you're doing,

35:19

keep doing it.

35:21

Then comes the end of the year. She sits down

35:23

with her accountant. They look over the books.

35:27

And the accountant's like, well, you know, the good news

35:29

is,

35:31

foot traffic's up a little bit. Sales are up a

35:33

little bit. But because of the discount code,

35:35

we're actually,

35:37

revenue wise, a little under where we were last year.

35:41

And the pizzeria owner is like, no. I can't believe

35:43

it. How is this possible? So many people are coming

35:46

in with the green flyer. I how could they be

35:50

it couldn't be that all those those people are are

35:52

not new customers.

35:54

So she's like, well, what's going on here? You know

35:56

what?

35:57

I gotta figure this out. I'm gonna I'm gonna

36:00

see what this kid is doing. So

36:02

she puts on a disguise

36:04

1 1 morning early,

36:06

and she follows the green flyer kid out of the

36:08

pizzeria,

36:09

and then she watches what he does.

36:12

And sure enough, you know, the kid with the green

36:14

flyer takes the big stack.

36:15

He walks out

36:17

onto the street, and then he

36:19

ducks into an alleyway around the corner from the pizzeria.

36:22

And he just watches.

36:24

He watches for anybody who's walking by the pizzeria.

36:27

If they look like they're walking toward the door,

36:30

he jumps out and hands them the flyer.

36:34

Because why would you work hard

36:37

to make

36:38

more sales

36:40

when you could just take credit for sales that were

36:42

already gonna happen,

36:45

AKA

36:46

Facebook and Google's motto.

36:48

And this is why I think

36:51

whenever I see this kind of thing, whenever you see

36:53

this, like, excellent ad targeting, right, I'm I'm scrolling through

36:56

my Reddit feed.

36:57

Spear and Mackay is a is a Canadian classic men's

37:01

fashion brand,

37:02

and I'm sort of like, yeah. I

37:05

You know, I have been sort of thinking that I

37:07

need some more linen shirts for the summer.

37:10

Not that this 1 is is too shabby either. But,

37:14

you know, how how did they figure that out? How

37:17

did they know that Spear and McKay was actually something

37:20

that that my stylist

37:21

recommended? I haven't visited I haven't even visited their website

37:24

yet. I probably was going to,

37:27

and that's what ad targeting knows. Because ad targeting has

37:31

seen journeys like yours 10000 times before, and so they

37:34

know to show it. Even if I scrolled past this,

37:37

never registered that I saw it, it had no impact

37:40

on me. Sometime in the next few months, I was

37:42

probably gonna go to their website, and I was probably

37:45

gonna buy a shirt anyway.

37:48

And Reddit's advertising team knows that.

37:51

So they get to take credit for it because they

37:53

can fingerprint my machine,

37:55

say he saw this ad, and then when the when

37:57

the transaction comes, they're like, view through conversion, baby. Look

38:01

at that. Reddit advertising works. Does it

38:04

was was I gonna buy that shirt anyway? Yes.

38:07

I probably was.

38:10

Alright. Big takeaway here. In 20 12 it was challenging,

38:14

but possible possible to measure and attribute,

38:17

I don't know, maybe 0.75

38:19

of digital marketing investments. But 20 26

38:23

yes. You can still measure a bunch of these touch

38:24

points individually.

38:26

But realistically assigning attribution in a world without 3rd party

38:30

cookies where,

38:31

direct traffic is the overwhelming majority, where keyword data is

38:35

not provided, where every platform makes you pay for any

38:38

data that you

38:39

want, forget about it. I have heard all the arguments

38:43

for econometrics,

38:45

you know, marketing mix modeling software, blah blah. I don't

38:48

believe it. I don't believe it anymore than Avinash Kaushik

38:50

does. I don't know if you saw his recent LinkedIn

38:52

post where he was like, nope. It's a pile of

38:55

baloney. They I think he might have used stronger words

38:57

than that.

38:59

Alright. Let's talk about how marketers can fight back in

39:02

these last few minutes.

39:06

So

39:09

you and I

39:10

know something that our data confirmed, our our SimilarWeb and,

39:13

study confirmed, which is that influence happens everywhere. Right? Like,

39:16

essentially,

39:17

people are being influenced

39:19

in all of these places on ecommerce sites and, yes,

39:22

in the news and media and publications that they read

39:25

and the entertainment platforms that they consume

39:28

and search engines and email and social.

39:33

And my contention is I this is not a a

39:36

scientific mathematical certainty,

39:40

but rather a representation

39:42

of what's going on, which is that for every visitor

39:44

who comes to your site,

39:46

1000 people learned about you and what you did

39:50

on some other platform that you don't control.

39:54

On social, through search, through AI,

39:57

through content platforms,

39:59

news, and media that they consume from friends, from storefronts,

40:03

from word-of-mouth,

40:05

from email.

40:07

And so you have to be present in those places.

40:11

My

40:12

I I am reversing

40:14

course

40:15

fully reversing course on 1 of the biggest things that

40:18

I told people to do for 20 years, which is

40:21

don't build on rented land.

40:23

Don't build your digital house on Instagram's platform, on LinkedIn's

40:26

platform, on Reddit's platform, on Twitter's platform.

40:30

Put all your effort into your own site and then

40:32

distribute your content in those places.

40:34

That was my

40:36

advice. It doesn't work anymore.

40:38

I'm changing my mind.

40:40

And I'm salty about it. I am pissed off that

40:43

basically within 3 months of Elon buying Twitter,

40:46

it became a useless channel for our marketing.

40:49

Like, we you can, you know, you can see what

40:51

Amanda and I used to get for SparkToro from Twitter

40:54

participation and engagement. And, essentially, within a few months of

40:57

him buying that platform,

40:59

it it went from a place where communities of all

41:01

kinds had all sorts of conversations to, you know, if

41:04

you're not, like, hating on trans people, there's just not

41:06

a lot of places or or promoting your AI tool.

41:09

Like, there's just not a lot of stuff to do

41:11

on Twitter. And so the, you know, conversation

41:14

just left.

41:16

A lot of marketing conversations come back on LinkedIn, which

41:18

I'm I'm grateful for.

41:20

But even though this went from a huge platform where

41:23

I made big investments to something useless,

41:27

I'm doing it again.

41:29

Any day, Microsoft could decide, hey. You know what? LinkedIn,

41:32

let's change how everything works there, and we'll ban Rand's

41:36

account. And, you know, it's not gonna work. Right?

41:38

Well,

41:40

I think,

41:41

realistically, the only choice I have is just to go

41:44

to all of these places

41:47

and build my digital platform on rented land, and I

41:50

I urge you to do the same.

41:52

This

41:52

these places have way more potential reach than your website

41:56

does.

41:57

Declining traffic and the opportunity to reach people just means

42:01

that, you know, maybe maybe if I'm lucky, we will

42:04

see 809

42:05

hundred views,

42:06

via Wistia Analytics

42:08

on a video that I put on a blog post

42:10

on SparkToro.

42:11

And that's 1 that does really well. A lot of

42:13

them are under 500 views.

42:15

My old whiteboard Fridays used to be, you know, 10020

42:18

thousand people would watch them on Moz's website.

42:21

No more.

42:23

It's all on YouTube or on LinkedIn or

42:26

on Reddit or on Instagram or TikTok,

42:29

all those places.

42:31

But we know we're reaching the right audience, and we

42:33

know we're getting that that penetration.

42:36

These are all rented land. Right? Like, my my threads

42:39

account, absolutely, my YouTube account,

42:42

my blue sky.

42:45

I'm gonna argue.

42:47

Might be controversial, but I'm gonna argue this is rented

42:50

land too.

42:52

Google itself is building your digital home on rented land,

42:56

and the opportunity, at least from a clicks perspective, absolutely

42:59

declined. But from an influence perspective, it does not. It

43:02

has only increased.

43:03

Alright. Number 2

43:05

there's only 1 own channel

43:07

where opportunity has not declined at all in the last

43:10

30 years.

43:11

Jeremy, you wanna guess what it is?

43:21

I don't know, actually.

43:22

It looks good.

43:27

It is

43:28

email.

43:29

Oh, interest yeah. I should've said that. Email email turns

43:33

out,

43:34

if you go all the way back in time, and

43:35

I did, I went I went back to 2005 That

43:38

was the those were the oldest studies I could find

43:40

showing what percent of people,

43:42

you know, read their email and what average open and

43:44

click through rates were.

43:47

And I I took all of these studies over all

43:50

these years, the best ones that I could find from

43:52

each year, and I built this graph.

43:54

So that the the sources of data are all over

43:56

the place. But

43:58

oh, and also note that this is,

44:01

this recent spike in open rates is Apple's

44:05

iOS

44:06

by default opening,

44:08

messages. It is not that open rates have gone significantly

44:11

up. You the click through rate is probably more indicative.

44:15

But, essentially,

44:17

people's use of email over the last 25 years has

44:21

not changed.

44:22

Has not changed.

44:24

And I know every generation, it's like, oh, man. You

44:27

know, Gen Xers, they're never gonna open email. Wait a

44:30

minute. Wait a minute. No. No. They did. But millennials,

44:32

they're gonna stop using email. Oh my gosh. They're using

44:35

email too. Well, Gen z, surely, they will not know.

44:37

They're starting to do it too. Don't worry. Gen Alpha's

44:39

coming. They're gonna I don't know, man. People just people

44:42

just like naming groups of people born in certain years.

44:46

I will say this, though.

44:48

You can probably spot that,

44:50

click through rates have dropped just a little bit even

44:53

though open rates have stayed pretty stable the last few

44:55

years. And I think that is just because

44:57

people are clicking less on everything. Like, we we like

45:00

to scroll now. We don't like to click. And so

45:03

you are seeing a slight decline.

45:05

It's slight, but it's there even in

45:08

email. So if you're trying to drive people to your

45:11

website via your,

45:13

emails,

45:14

I might rethink that. Amanda and I have started doing

45:17

way more 0 click email marketing, which is essentially

45:20

putting the content of the message that we're trying to,

45:24

send people directly into the email itself rather than trying

45:28

to say, like, hey. The latest edition of our blog

45:30

post is out. Come click it here. You know, that

45:32

kind of thing.

45:33

Alright. Number 3

45:35

I am recommending,

45:37

and I'm not alone,

45:39

that you drop traffic as a KPI. It was it

45:41

was always a vanity metric.

45:44

Instead,

45:45

you should be measuring the size of the audience and

45:47

and the reach and the interest that you're getting and,

45:50

of course, your sales. So it's it's kind of like

45:51

looking at the top of the funnel and the very

45:53

bottom, but not the middle so much.

45:56

Traffic's a fine secondary metric, but but it's a dumb

45:59

thing to optimize for unless you're actually selling CPM ads.

46:04

I I will point out what I what I mentioned

46:06

at the top of this, presentation, which is that traffic

46:08

and revenue are not the same thing. And there are

46:11

so many case studies from the last few years of

46:14

these 2 numbers just completely separating. Right?

46:17

Traffic up, traffic down, revenue up

46:20

is like the story of 24 25

46:23

You remember that HubSpot traffic apocalypse last year? Like, what

46:26

was that? Q 1 of,

46:28

25 And so, you know, when this when this happened,

46:32

all the oh my god. The you know, digital marketing

46:35

LinkedIn was, like,

46:36

up in arms. They're like, oh my god. How could

46:38

they do this? You know, they they screwed up all

46:40

their SEO with all their blog posts and everything.

46:45

But I was like, Did they? Because

46:48

they just released an earnings report, and it it sure

46:51

looks like they're doing amazing. Like, I don't I I

46:55

think this and this are not connected.

46:59

And,

47:01

you know, it turns out that

47:03

you don't need traffic to drive

47:07

revenue.

47:09

If you've noticed that your conversion rates are also rising,

47:12

that is no coincidence. It's because people are doing all

47:14

the things

47:16

that they

47:17

needed to do to investigate you and your brand and

47:20

figure out whether they wanted to buy from you. They

47:21

they're doing that before they ever reach your site.

47:24

This is my buddy, Scott Heimendinger.

47:26

Fantastic case study because he has yet

47:30

has yet to post a link anywhere

47:33

to his website, which is which I think is Seattle

47:36

Ultrasonics dot com.

47:37

Basically, he does YouTube videos. He does TikToks. He does

47:41

stuff on LinkedIn.

47:42

He does stuff on threads.

47:44

He's essentially, like, showing off the world's 1st ultrasonic handheld

47:49

chef's knife,

47:50

which is which is really cool. Like, it's a super

47:52

cool device, and it's about the same price as, like,

47:54

you know, a fancy Japanese knife. I I have,

47:57

1 downstairs, and it's it's become the 1 that I

47:59

use for most of my cooking.

48:04

And 2500

48:05

ultrasonic knives sold.

48:08

No no click driving at all.

48:11

Nothing. Right? Because Scott was basically like, I I think

48:14

I will hurt myself if I try and

48:17

put links in my posts and drive people specifically to

48:20

the site. I'm gonna show off all the cool things

48:23

it does and how amazing this tech is,

48:25

and then let people find me. And that that is

48:30

exactly what's happening on for all this. So if you

48:32

wanna measure this, right, if you're trying to be like,

48:34

hey, Rand. I cannot I cannot in good conscious just

48:36

be like, just trust me, boss. The conversion the sales

48:39

will come.

48:40

You can measure these things. Right? For any platform,

48:44

any source that you're you're using, you can measure audience

48:47

and reach and interest and sales. We we have a

48:50

blog post on on SparkToro where I talk about how

48:52

to build these, like,

48:54

dashboards that show the correlation between any different channel and

48:57

and how well sales are doing.

49:01

You can build those hard to measure dashboards yourself, and

49:03

then and then actually, AI is pretty darn good at,

49:08

interpreting and analyzing these.

49:10

Quite quite nice. Alatus Solis also has a wonderful framework

49:14

very similar to this, even more in-depth than this 1

49:17

with all sorts of metrics that includes the new,

49:21

new stuff you can measure through Google Search Console with

49:23

your platforms,

49:24

like Instagram and and Facebook and LinkedIn, etcetera,

49:28

YouTube, all that.

49:32

I'm gonna argue that if you choose channel investments based

49:35

on referral data,

49:37

you will become Google's fool.

49:39

And that is because all the things that happen in

49:42

all of these categories

49:46

turns into 1 of these.

49:48

And then who gets credit in the analytics?

49:52

I think when Google took keyword data away, it was

49:55

a nefarious ploy to hide the fact that they saw

49:58

that they were becoming

50:00

more of a navigational

50:02

source. Right? That 0.5 of the people who were coming

50:04

to Google already knew what they wanted, and Google

50:07

was figuring out, well, how can we monetize that more?

50:10

Wait. If people don't know what their users searched for,

50:14

then they'll have to put more budget into Google because

50:17

they'll assume that we were the driver

50:20

of all of that value as opposed to just a

50:22

middleman

50:23

for the Internet.

50:25

Number 4

50:26

you gotta find where your audience pays attention and then

50:29

go market to them there. This is obviously the, you

50:31

know, core reason that that SparkToro exists. But I I

50:34

really like this chart. This comes from Dana DiTomaso,

50:38

her her idea here. And, essentially, it's looking at where

50:41

people in your audience are paying attention. Right? So social

50:44

feeds, hundred and 45000 are reading industry websites, 110000

50:48

are subscribed to all the YouTube channels.

50:50

Right? So that's that's this inner circle. And then the

50:53

outer circle

50:55

is where you're putting budget.

50:57

And if things look a little weird like they do

50:59

on this chart,

51:01

you know, you're putting 33 percent of all your budget

51:04

against

51:05

1 sliver,

51:06

right, those those unbranded Google search keywords,

51:11

you might you might be making a mistake.

51:14

Right? It could be worth considering

51:16

whether you should be putting a lot more into email

51:18

newsletters, for example, or Google Discover or comparison sites

51:23

and,

51:24

yeah, whether some of these are overweighted.

51:29

My my final

51:31

last takeaway is just it I think we're moving away

51:33

from

51:34

traffic and attribution

51:37

and shifting to

51:39

influence,

51:40

judge through measurement and testing

51:42

and a lot of testing.

51:44

If you wanna win

51:46

in the years ahead, I I think what you're gonna

51:48

have to do is be in these places. Right? Be

51:51

where your audience is

51:55

and let brand affinity,

51:57

not links, drive the converting traffic

52:00

that's coming to you.

52:02

So, more about this in 0 click marketing, which is

52:05

coming this fall. And, Jeremy, thank you so much for

52:07

having me. I really appreciate it.

52:10

Awesome, Ryan. As always,

52:12

so much in that presentation there.

52:15

You did say running a book was tough and here

52:16

you are doing another 1 so I am looking forward

52:19

to that.

52:21

Don't get me wrong. It's a good book. I'm very

52:23

glad we put it together. But,

52:26

yeah, really,

52:28

really quite a challenging process to train just. Also challenging

52:31

because some of this stuff is changing all the time,

52:33

and so we had to try and find a way

52:35

to make

52:36

the advice and the examples

52:38

timeless and

52:40

not predict the future, but instead,

52:43

you know, recognize this sort of long long path that

52:46

we've been on for a decade

52:48

since, since all the big tech platforms figured out that

52:51

they can make more money by keeping us there.

52:53

Yeah.

52:55

So we had some some good questions in the in

52:57

the chat. I'll I'll ask,

52:59

just a quick 1 It's more like a,

53:03

just on the graphs, like, that you presented,

53:06

do AIOs and AI mode get grouped into the Google

53:10

organic search bucket versus AI tools like Chat, JBTO, or

53:12

Gemini? Do you know?

53:14

Yeah. Great question. Let's pull that up.

53:19

So in the blog post about that, I have got,

53:26

details on that. There we go.

53:30

So, yeah, essentially

53:32

essentially, what you're seeing here,

53:35

is

53:38

alright. So there we go.

53:41

The breakdown of searches again, session ends, goes to AI

53:44

mode,

53:45

clicks 1 or more times. So you can see that

53:48

AI mode is vanishingly tiny.

53:51

So a lot of people on mobile expand the

53:56

AI overview, but they don't follow-up with the click into

53:59

AI mode. That that seems to be extremely unpopular

54:03

still.

54:04

Granted, it's grown,

54:06

and it continues to grow. We we cover this in

54:08

the data state of search report

54:10

as well, but it's it's pretty tiny. The AI overview,

54:12

if that

54:14

so that little box when if someone expands it,

54:18

it is not considered a click because it doesn't change

54:20

the URL in any way.

54:22

So

54:24

you you could say, like,

54:26

oh, that shouldn't be counted as 0 click. I I

54:29

would argue it's still staying inside of Google's ecosystem and

54:32

not going anywhere, not even to another Google site.

54:36

But, yes, that's a that would count as

54:40

stays on the page.

54:43

Awesome.

54:44

I have a question from Sam who,

54:47

previously ran,

54:49

SEO at Amazon globally and also now is setting up,

54:52

SEO at AirOps.

54:54

So he says, his slides are showing lots of videos

54:57

in YouTube, Tube. I'm thinking

54:59

building a YouTube muscle is the big unlock for AEO

55:02

the next bit,

55:03

couple of years, 2 to 5 years. Reddit is struggling

55:05

to keep up with spam and filtering and won't be

55:07

the top source for LLMs.

55:09

Do you agree?

55:13

Oh, man.

55:14

You know what's really weird about,

55:18

about that generally is

55:22

if

55:26

if lots of people start recognizing that YouTube is a

55:29

great opportunity

55:31

to

55:32

influence or manipulate

55:35

AI tools,

55:36

they will start to change their behavior. You could already

55:38

see this with Reddit. Right? Like, Reddit,

55:40

you know, there's a bunch of examples of people who

55:42

are like, hey. I can post, like, 2 Reddit threads

55:45

that get 0 upvotes,

55:47

but

55:48

I can change chat g p t's responses with just

55:51

that. Like, that alone.

55:53

Well, you know, if that starts to happen with YouTube,

55:57

I I think they're gonna do what they did with

55:58

Reddit and and push it down a little more and,

56:01

you know, maybe maybe turn to LinkedIn more. Maybe they'll

56:04

it would not surprise me. I think I think the

56:06

the future case of this

56:10

is that a lot of these AI tools

56:14

start running short of data sources,

56:16

and it would not surprise me if they start creator

56:19

funds the same way TikTok has.

56:22

That seems

56:23

seems like a logical use of all those billions of

56:25

dollars is like,

56:26

hey. Here's a couple billion to sort of write for

56:29

these platforms.

56:31

People Magazine, which owns I can't even remember how many

56:34

dozens or hundreds of publications in the United States.

56:37

People magazine is essentially

56:40

just an AI tool feeder network at this point.

56:44

Like,

56:45

their their traffic is poorly monetized.

56:48

Traffic is down,

56:50

but revenue is hugely up because the AI tools pay

56:54

them

56:55

to license their content for training.

56:58

And they have essentially

57:00

charged their writers to become,

57:03

you know, an AI creation department.

57:07

Interesting.

57:08

Obviously,

57:09

you have a background building some software for traditional search

57:12

for for Moz and all the cool tools you built

57:14

over the years.

57:16

Sam had the question on your thoughts on the AEO

57:18

tool landscape, and I I likewise had the same question.

57:21

Like, what what's your thoughts around it? Like, what do

57:23

you think about the the the tools out there? Are

57:26

they incentivizing the right activity?

57:29

Yeah.

57:30

What do you mean?

57:34

Gosh. Let's see what

57:36

what I see here. I

57:39

trying to find a study for you, but, I recently

57:42

showed this on on LinkedIn. I'll I'll try and dig

57:44

it up

57:45

and send it to you. But I am

57:48

I am worried that the degree of personalization

57:51

and history

57:54

influencing

57:55

responses

57:56

means that

57:58

there is no reasonable way to measure

58:04

AI responses

58:07

that is

58:09

within

58:10

the realm of accurate.

58:12

Right? So, like,

58:15

I we use Gumshoe right now. Right? I I track,

58:18

our presence in Gumshoe. I I like the tool. I

58:21

like the UI.

58:22

I think that persona based approach is is solid. Right?

58:25

They try and, like, build these personas

58:28

of

58:28

of, like, our audience

58:30

who are actually gonna be asking these questions to AI.

58:33

And so they give them some context,

58:37

which should help with some of that personalization stuff.

58:40

But, man, I

58:42

I'm just not sold. I think until and unless,

58:46

you know, the major AI tools say, hey. We're gonna

58:48

release data on how often your brand showed up

58:51

in prompts

58:52

and in responses

58:55

until they actually do that and and in what with

58:57

what context. Right? Like, was it a positive mention? Was

59:00

it a negative mention? Were they comparing me against someone

59:03

else but unfavorably? Did they say accurate things about me,

59:05

inaccurate?

59:06

You know, presence alone is not

59:09

not that helpful,

59:10

given all the stuff that's in the response. So

59:14

I don't know. To me, it's

59:16

messy and uncertain and

59:19

growing my, you know, percentage

59:21

of,

59:23

visibility from 40 percent to 60 percent,

59:27

does that actually have an impact on my sales?

59:31

I think

59:32

I think not many people are asking that right now,

59:35

and that's a problem. And I don't think the tool

59:37

providers have a great solution to any of these

59:40

personalization

59:41

and and history biasing challenges that exist.

59:45

Sorry. I don't have better news.

59:47

No. I just shared the link, by the way, to

59:49

your research. I remember seeing that on LinkedIn.

59:53

Mike, who once been here in Milwaukee,

59:55

is asking, what's your bot take on the future of

59:57

website creators and publishers?

01:00:03

I think that people will still create for the web,

01:00:06

especially the social web. I think more of that activity

01:00:09

will move from

01:00:10

blogs and websites

01:00:12

to platforms.

01:00:16

That's Instagram, it's Reddit, but it's also Patreon or,

01:00:20

threads

01:00:21

or LinkedIn,

01:00:24

I think it's gonna be extremely

01:00:27

difficult

01:00:28

to monetize

01:00:29

content alone.

01:00:30

I think that almost almost everyone who wants to do

01:00:33

that at scale and have success is gonna need products

01:00:37

behind them.

01:00:38

And then the the content

01:00:39

is is essentially just

01:00:41

there to help

01:00:42

market the product.

01:00:45

I don't

01:00:47

I don't see a bright future for most publishers unless

01:00:51

you're People magazine and you're selling your data to AI

01:00:53

at scale.

01:00:56

You know, the New York Times, for example, right, has

01:00:59

is it

01:01:00

I think it it's it's more more than 0.5 It

01:01:02

might be 0.667 now of

01:01:05

all New York Times subscribers

01:01:06

never visit anything except games and recipes.

01:01:11

That's not a publisher. Right? They're just a they're just

01:01:14

a games platform with a vestigial

01:01:16

news arm. Like, they're not

01:01:18

they're not a newspaper,

01:01:21

and they're 1 of the only ones that's had, you

01:01:23

know, real success

01:01:26

monetizing.

01:01:27

So I

01:01:28

my my view is pretty dim on publishing

01:01:31

itself,

01:01:33

as being a path forward. I

01:01:35

do I agree that we need more news sources, more

01:01:38

local news, more

01:01:40

people doing journalism, more content creators. Yes. Do I love

01:01:44

that stuff? Absolutely.

01:01:46

Do I think it's gonna be,

01:01:50

possible to make a profit in it?

01:01:54

Not really.

01:01:56

Just, coming up to the hour. Do you have,

01:01:59

time for 2 more rapid, fire questions?

01:02:02

Yeah. So,

01:02:05

I'm really interested in your perspective here.

01:02:08

It's been a monopoly up until now with Google effectively,

01:02:11

running the show.

01:02:12

Where do you think it goes over the medium to

01:02:15

long term? Between a chat, TBT, call it Google kind

01:02:18

of

01:02:19

scenario, is it still gonna be, you know, a monopoly,

01:02:21

or do you think this is gonna change? Who do

01:02:23

you think is the long term or meetings long term

01:02:24

we're not here?

01:02:26

Yeah.

01:02:28

Let's see.

01:02:30

I think

01:02:31

Google is gonna keep doing well regardless of what anyone

01:02:34

else does, and that's because they've got

01:02:37

such

01:02:39

powerful infrastructure and relatively

01:02:41

cheap compute, and,

01:02:45

they

01:02:47

have an incredible business even if AI turns out to

01:02:50

be a bubble.

01:02:53

I think that

01:02:57

the pure AI tools are in big trouble

01:03:00

if and when the financial bubble around

01:03:03

AI pops, and

01:03:06

I don't know.

01:03:09

It seems

01:03:10

almost impossible that it won't at some point. There's just

01:03:14

there just isn't enough

01:03:17

revenue

01:03:19

being found. Right? You could see ChatGPT

01:03:22

sort of,

01:03:24

you know, making these revenue targets for 20 30 that

01:03:28

they they they don't have a snowball's chance in hell

01:03:31

of getting to 0.2 of that number.

01:03:34

And it's, like, it's sort of like everyone knows it,

01:03:36

but

01:03:37

they think that there's enough idiots out there who'll keep

01:03:40

propping up the,

01:03:41

you know, the market, and so they don't wanna pull

01:03:44

their money out yet either.

01:03:47

It's very much a a game of of chicken at

01:03:49

this point among,

01:03:52

financiers.

01:03:53

And so

01:03:54

I don't know. I hesitate to speculate on that stuff

01:03:56

because it's not technology.

01:03:58

It's not value. It's it's really what's going on,

01:04:02

you know, in the

01:04:04

behind the scenes bankers rooms.

01:04:08

I've obviously been impressed with Claude, like like almost everyone

01:04:11

has.

01:04:13

They are

01:04:15

almost the 3rd the size of ChatGPT at this point

01:04:18

in terms of usage in the US.

01:04:20

That's that's up from, like, you know, less than 0.1

01:04:23

a year ago.

01:04:26

They they could keep doing that. I I think they're

01:04:29

smart to focus on a few niches like

01:04:31

programming,

01:04:33

and a lot of professional use cases. ChatGPT is really

01:04:36

becoming the

01:04:37

market leader for, like, consumer

01:04:40

AI.

01:04:41

But

01:04:42

they're throwing,

01:04:44

you know, they're throwing trillions of dollars of compute around

01:04:47

to solve a problem that Apple seems to be miniaturizing

01:04:50

into your iPhone. So I I don't know. I

01:04:53

it just makes makes me real nervous. I'm I'm very

01:04:56

glad I have no money in the private markets of

01:04:58

AI.

01:05:00

And last question, Rand.

01:05:02

Obviously, you put forward the case for

01:05:04

the end of traffic.

01:05:06

What would falsify it and and what development would have

01:05:09

to occur effectively

01:05:10

to be the counterpoint to what you're saying?

01:05:15

Let's see. So, you know, I think

01:05:17

if the American government acted more like the EU, we

01:05:20

would see a

01:05:21

a wildly different world. Right? So because all these companies

01:05:25

are

01:05:26

US

01:05:27

based,

01:05:27

they can sort of,

01:05:32

ply their nefarious trade globally

01:05:35

with

01:05:36

while suffering, you know, a few big fines,

01:05:39

but

01:05:40

really no no significant

01:05:43

consequences.

01:05:44

You know, until the Department of Justice is willing to

01:05:46

be like, hey, Google. You engaged in an illegal monopoly

01:05:49

behavior where you sent all local searches to your own

01:05:53

property, Google Maps, and monetize them there. You're not allowed

01:05:56

to do that. Google Maps, you are now your own

01:05:58

independent company.

01:06:00

Right? And, like,

01:06:01

boom. Suddenly,

01:06:03

30 percent of all Google searches are happening in local

01:06:05

and, like, they're a major competitor. And,

01:06:07

wow, search is this, you know, much more competitive landscape.

01:06:12

Room for innovation

01:06:13

happens at

01:06:14

you know, if I if I were advising the DOJ,

01:06:17

I would tell them YouTube and Google Maps should be

01:06:20

their own companies,

01:06:23

and breaking up Google is the the only way to

01:06:26

create a competitive

01:06:27

market environment

01:06:29

inside of search.

01:06:31

Everyone who's like, oh, AI is gonna compete well, no.

01:06:34

It's it's clearly not. Google's Google searches per searcher have

01:06:38

not dropped 1 IOTA.

01:06:40

The most common behavior people have after using ChatGPT is

01:06:44

go to Google and perform a search.

01:06:48

Awesome, Rand. Honestly, thank you so much again for

01:06:52

your contribution to the narrative in a fast changing space.

01:06:55

Really looking forward to the book.

01:06:57

And and for those that are part of the community,

01:07:00

we also have a discount for Rand's tool alert mouse

01:07:02

in the members and perks section, so check it out.

01:07:05

Yeah. Big thanks again, and, great to reconnect. It's been

01:07:08

a while.

01:07:09

Yeah. Good to see you, Jeremy. Thanks for having me.

01:07:11

Thanks. Thanks, everybody.
