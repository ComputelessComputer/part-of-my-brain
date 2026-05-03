---
type: "meeting"
started_at: "2026-05-01T08:37:24.813Z"
ended_at: "2026-05-01T09:47:09.472Z"
location: "Seoul"
source: "ad-hoc"
---
## Transcript
**Speaker 1 - 00:00**
We're in the this design, and if I click, like, um, date number 21 or something, then naturally I would expect, like, this left side daily note view to be, like.
**Speaker 2 - 00:12**
So, uh, yeah, it's true. It's true.
**Speaker 1 - 00:14**
Yeah. Uh, it.
**Speaker 2 - 00:15**
And, and this was, like, my main problem when I started, uh, uh, as you can see in, uh, Slack, uh, thread, when I wrote about, like, okay, we decided to go this way, like, calendar and contacts should be very small, uh, and narrow views, and, uh, don't need to show any stuff, like, anything time blocks related. This was my main conc ern about how to show calendar right now . And, uh, we discuss ed it with John on our previous thing, th ings, that it's not like a best way and not the right way to show calendar this way because it's now become more like task-related than, like, just date. And, uh, time blocks related, I would say.
**Speaker 1 - 01:17**
Mm-hmm.
**Speaker 2 - 01:18**
So honestly. Have, like, a right solution right her e. So we can just brainstorm around it, uh, through us, and, uh, figure out what's the best way to do this.
**Speaker 1 - 01:31**
I think, like, I just want to kind of, like, stop you guys there and then just kind of, like, lay out , like, how we can, like, work in par allel lanes for, like, both the design as well as the development work. So basically, I think, lik e, you like, Artem and I are going to b e, like, just doing some brainstorms about, like, how the user interface would look like by prototyping a lot of stuff and then try to actually see if this makes sense. Like, if it's actu ally usable. Like, we should actually tr y out the prototype, right, Artem? And also, like, in terms of , like, development, I think , like, apart from, lik e, actually looking at, like, how the user interface evolves over time, as , like, Artem and I am just , like, experimenting with a lot of stuff , like, I just think that we should try to, like, start off from the most primitive parts, which is basically the daily notes, and then just not try to think much about , like, the calendar as well as , like, other views. Like, the context and all that . And I'm, like, doing during our conversation, we had, like, some I k ind of mentioned that we shouldn't be implement ing something that isn't really complete yet. Like, the design spec and all of that, like, if we're still in a brainstorming phase, like, that should not be kind of, like, started out. Like, I know that we love to kind of , like, just try stuff out , but it's just best to kind of, like, kind of , like, have that switch off for a bit. And I think it's our j ob, Artem as well, as well as our job to kind of, like, explic itly state that these are some designs that are still in, like, the exploration phase, and we do , like, kind of, like, state that, but we need to be more deliberately stat Mm-hmm.ing
**Speaker 2 - 03:28**
Mm
**Speaker 1 - 03:28**
th
**Speaker 2 - 03:28**
-hmm. Mm-hmm.
**Speaker 1 - 03:29**
ose parts so that, like, you know, I guess, like, Yujong and something is not getting confused about th ose things. To kind of, like, summarize what I've just said, I think, like, like, these are all great designs, but , like, for now, I just think that we should just, like, only focus on making the , like, the editor
**Speaker 2 - 03:50**
Daily
**Speaker 1 - 03:51**
as well
**Speaker 2 - 03:51**
not
**Speaker 1 - 03:51**
as
**Speaker 2 - 03:51**
es.
**Speaker 1 - 03:51**
, like, the daily notes interface really, really great, and then we just know that we're going to be going with the convention that , like, there's going to be the main pane and then the subpane, right? And, like, there's not going to b e, like, the third pane not, like, a third pane that's going to be opening up. We're just going to go with, like, if you for examp le, like, if you have, like, a daily notes open and then like a task like a chat log open ed up and then you kind of, like, interact once you start interacting with, lik e, the artifact, then like the daily notes gets collapsed like how Artem prot otyped. So I think, like, we should try to kind of, like, like Artem, we should be trying to, like, spur a lot of stuff, but lay out those kind of fundament al principles just like the two-pane design. I think that would kind of complement with that . And then deliver those parts to Yujong as well as something. Like, that's my two cents,
**Speaker 2 - 04:51**
Mm
**Speaker 1 - 04:51**
but.
**Speaker 2 - 04:51**
-hmm.
**Speaker 1 - 04:53**
Yeah, Yujong? Like,
**Speaker 2 - 04:56**
Yeah.
**Speaker 1 - 04:56**
seems
**Speaker 2 - 04:56**
I'm
**Speaker 1 - 04:56**
l
**Speaker 2 - 04:56**
ag
**Speaker 1 - 04:56**
ike
**Speaker 2 - 04:56**
ree. I'm agree
**Speaker 1 - 04:57**
se
**Speaker 2 - 04:57**
here.
**Speaker 1 - 04:57**
ems like you're thinking about some stuff some stuff right now. Got anything to say? Uh, I-I-I'm just t ouching this because I was implementing calend ar sync, and there should be some kind of way to list events someway or, like, control someway. So that's why I tryna bring that part in Mm-hmm. . And yeah, so that's why. And, and I also had no-not aware that this is kind of a Right, right. ver y raw pro-prototype, and , um, yeah, at the at the time, it looks very M lmike-hmm. good idea, solid. So I try implement it, and I found some kind of Mm-hmm., lik e, um, edge cases that I haven't tho ught about, but you guys already did. So that's why I tryna bring it in. I-if it's just a, a very raw prototype, then I can just move on and do, do, like, other If stuff. that's the case for just , like, synchronization, like the calendar events, then I think we should just, like, utilize the settings if that makes sense.
**Speaker 2 - 05:59**
Yeah.
**Speaker 1 - 05:59**
And I just think that, lik Okay.e,
**Speaker 2 - 06:01**
Yeah.
**Speaker 1 - 06:01**
we shouldn't try
**Speaker 2 - 06:01**
I,
**Speaker 1 - 06:02**
yep, go ahead.
**Speaker 2 - 06:04**
oh, and I would suggest that maybe we shouldn't like have calendar view at first for first , uh, release. Maybe in the future, we'll be found some related problems that we want to figure to somehow fix by this calendar. But for now, h
**Speaker 1 - 06:27**
H
**Speaker 2 - 06:27**
m
**Speaker 1 - 06:27**
mm.
**Speaker 2 - 06:27**
m, I'm not sure.
**Speaker 1 - 06:32**
Cool. All right. I
**Speaker 2 - 06:34**
So
**Speaker 1 - 06:34**
think that c
**Speaker 2 - 06:35**
what
**Speaker 1 - 06:35**
le
**Speaker 2 - 06:35**
do
**Speaker 1 - 06:35**
ars
**Speaker 2 - 06:35**
you
**Speaker 1 - 06:35**
it
**Speaker 2 - 06:35**
th
**Speaker 1 - 06:35**
up
**Speaker 2 - 06:35**
ink?
**Speaker 1 - 06:35**
. Okay. Cool. All right. Does that clear things up for you, Yujong? And also, um, by, uh, inter view, you mentioned, like, daily note as a, like, main 100% focus. I, I, I, um , I uh, understand there's the focus, but also the calendar sync was also the one of the item on the our current sprint, and Mm it-h'smm. not really directly, like, 100% con like, constrained in the da ily note area because daily note is just a , like, um, U I, UI sur face to show it . But, like, the cal endar sync kind of involve, like, this kind of , like, little bit of the calendar or , like, settings. So Mm-hmm. like, you mean so my understanding is, like, I already kind of al-almost folded up the calendar sync, but consider ing the, um, lik e, our focus is daily note kind of statement, if that's the , like, strong case, then, like, calend ar sync is kind of out of scope? No, Tha- ath calat'send wharat no, no, the calendar syn c is definitely? inside our scope for the sprint right now, but it's just that , like, I don't know, lik e, if you guys realized, but, like, if you like, I don't think most of o ur users actually go inside the cal endar view, and Artem kind of, like, extracted some, like, you know, stats from that, and there's, like, like, very, very low percentage of us ers actually kind of opening
**Speaker 2 - 08:14**
Ye
**Speaker 1 - 08:14**
that
**Speaker 2 - 08:14**
ah.
**Speaker 1 - 08:14**
up . And, like, from our previous design, like, where we had, like, the left sidebar, like, I think, like, rarely anyone kind of, like, scrolls down to kind of view past notes. Like, people would rather search or rather just , like, use the chat directly. And I just think that , like, it's important to utilize the daily notes v iew as
**Speaker 2 - 08:38**
Mm-hmm.
**Speaker 1 - 08:39**
and then kind of, like, have those app ropriate meetings being for, like, event s being synced for, like, you know, kind of, like, embedded inside the note, like, the notes directly. Not, like, have, like, a dedicated view for that, if that makes sense. So, lik Oke,ay. y Soep. I so I you mean you mean, like, da ily note as a primary interface but not limit ing functionality but , like, if Exact anyly. functionality can be backed by the daily note UI, then we should do it, do it. But, like, this experiment ation is not a daily note surface, so we should kind of defer it, right? Right. Exactly. Okay. Okay. I, Cool. I think that yeah. Cool. You got you got any other questions or, like, want to sta No.y for the sync?
**Speaker 2 - 09:24**
Ye ah. I,
**Speaker 1 - 09:26**
Or you can just leave
**Speaker 2 - 09:27**
I
**Speaker 1 - 09:27**
right now.
**Speaker 2 - 09:27**
usually if no. Look. I, I change, uh, not change. I descri bed, uh, this layout a little bit on Figma, like, how we split scre ens and, uh, you can check it out . And I thought about maybe use 50/50, uh, for splitting, like, without any additional complex, uh, rules. Like, first screen split only, like, one -third of the window, and then, like, they split kind of continuously to, like, one-third to two-thirds. So I believe we can just split, 50/ 50 here. And also, other th ing about considering layout , we discussed with John, was that maybe on la on wider resolution s, we could show chat consistently op en. I'm not sure. I still didn't get into it. I didn't I don't have, like, uh, answers here. I don't have, like, the right resolution where we should move past this point because, like, for, for now, I mostly prot otyping in a window around, like, 900, uh, pixels wid e. And , uh, it's very comfortable both in , like, one window and two windows, like, 50/5 0. But maybe over this point over, like, um , 900 pixel s, we could show, like, some sort of, like, constantly open chat. I, I will add it, uh, but also, like, just tell you that I have, uh, updates on it on Figma. So if you want to check, uh, and have questions, just.
**Speaker 1 - 11:15**
Okay.
**Speaker 2 - 11:15**
Ask me.
**Speaker 1 - 11:16**
So before I leave, u h, do, do you have a we briefly talked about, like, nested pag e. Um, and I think it was very clear before, like, even a year ago, you, you said, like, we, we won't support, like, very nested page, like, maybe a single depth of page. It's a , like, enough. Are we still , um, keeping that kind of , uh, design , meaning, like, daily notes, and we go into the, like, page that is subpage of daily note, then from there, we cannot go, like, more deeper? We can't? That's the, like, constraint that we wanna make?
**Speaker 1 - 12:04**
I think we don't need to concept of folders. For chart. Just because of the fact that, like, we're not focusing on , like, like, so, like, there's there's some under lying principles for this. Like, I just think that , like, people should not be organizing stuff themselves.
**Speaker 2 - 12:23**
Hmm.
**Speaker 1 - 12:24**
Right? And giving, like, the option to actually, like, utilize fold ers, then you k ind of confront this, like, dilemma that , oh, like, should we kind of, like, constrain, lik e, the levels to kind of be opinionated about, like, the st ructure and all that? But then, like, it kind of, like, restricts, like, the flexibil ity, right? So, like, my thought is, like, it's just not just don't give that in the first place. And then and then, lik e, in the backend, somehow magically index or just organize that into, like, chartpedia.
**Speaker 2 - 13:02**
Hmm. But, but I, I agree that, like, folders kind of redundant. Um,
**Speaker 1 - 13:07**
M
**Speaker 2 - 13:07**
I
**Speaker 1 - 13:07**
m
**Speaker 2 - 13:07**
think
**Speaker 1 - 13:07**
-hmm.
**Speaker 2 - 13:07**
I was very against folder from day one. But
**Speaker 1 - 13:10**
Right.
**Speaker 2 - 13:11**
my, my original question is, like, by design, by our dat abase design, it is, um, a page have a, like, multiple child and parent kind of relation. So
**Speaker 1 - 13:22**
Right.
**Speaker 2 - 13:22**
it can be, like, infinitely nested, like, without the folder, right? It can be nested, nested, nested. And, like, my question is, like, should we support that kind of infinite nesting or, well, we are not going to do it, that kind of stuff?
**Speaker 1 - 13:37**
Mm-hmm. Good question. So, like, I guess, like, this is a different question then.
**Speaker 2 - 13:46**
Yeah.
**Speaker 1 - 13:55**
I think it's, like, it's kind of, like, very natural for a user to actually kind of, like, mention or embed such a page inside, like, an arbitrary arbitrary pag e.
**Speaker 2 - 14:09**
Yeah.
**Speaker 1 - 14:09**
Right? So I
**Speaker 2 - 14:10**
Ye
**Speaker 1 - 14:10**
do
**Speaker 2 - 14:10**
ah.
**Speaker 1 - 14:11**
agree on that, but I don't th ink, like, we should save the structure, like, that, if that makes sense. So, like, it would be, lik e, the pages are kind of saved in a different different I don't know. Like, you don't you'll figure that out, like. But, like, you get what I'm saying, right? Um, The so by design, in, in, um, we can support , like, arbitrary infinite depth , but I'm just saying, lik e, like, like you said, I, I think for user perspective, it is very natural to , like, ex like, keep, keep going in, ke ep, keep nesting for between and nest ing, like, two or three or four or five depth. R Butight,. like, we can always simply, but , um, if you think about in editor, like, daily note perspectiv e, John, you and I talk about , like, if, uh, for every page can have a tas k, and if a task is included in the daily note, then we expose this task of a subpage to a daily note, right? Exact Andly. , and, and if we support , like, infinite depth, then how should we support that , um, task exposing ? Like, are we support, like, are we exposing just the single depth, or, like, are we supporting, like, infinite depth? And all the time, are, are you following, right? Uh.
**Speaker 2 - 15:41**
Yeah. Yeah. I just I don't have any
**Speaker 1 - 15:45**
You know,
**Speaker 2 - 15:46**
uh, I. Opinion on, uh, architecture. It feels natural for me, actually, to have nested pages. And I believe it 's totally on user here, but what we need to support here is some sort of inner navigation I mean, like, back and forth buttons that we already have.
**Speaker 1 - 16:05**
So I guess, like, y ou
**Speaker 2 - 16:06**
We
**Speaker 1 - 16:06**
know,
**Speaker 2 - 16:06**
don't
**Speaker 1 - 16:06**
lik
**Speaker 2 - 16:06**
have
**Speaker 1 - 16:06**
e, from
**Speaker 2 - 16:06**
th
**Speaker 1 - 16:07**
from, like, a technical perspectiv
**Speaker 2 - 16:08**
em.
**Speaker 1 - 16:09**
e, like, they're trying to ab stract the user stuff and, like, the worst-case scenario that I think would would be, like, you have, like, these five levels of , like, nested pages, and then each of them has like a task. Task. Right? Yeah. And then like the question is, how are you going to be exposing these nest like these series of like task cha ins inside the daily notes? That's like the question, right? I guess. Yeah. Honestly, I haven 't kind of like, you know, thought of it that way. I haven't really overcomplicated this. Stuff. I just think that . Simple is the best , you know. So like, you know, I'll just think about this and then like why don't we talk about this later? Like after Okay. the design thing. Yep. All right. Sounds Yeah. good. Cool. Yeah. Talk soon, man. Yep. Oh, R10. All right. You got the stage, man.
**Speaker 2 - 17:09**
So I. I was thinking about th is, stuff of moving our task from yesterday, that's not done,
**Speaker 1 - 17:21**
Mm-hmm.
**Speaker 2 - 17:21**
kinda interesting. Uh, and complex.
**Speaker 1 - 17:26**
Right.
**Speaker 2 - 17:28**
How to share screen and share entire screen. Yay. I, I, I do some stuff on the page. So we
**Speaker 1 - 17:39**
Mm
**Speaker 2 - 17:39**
will
**Speaker 1 - 17:39**
-hmm.
**Speaker 2 - 17:40**
just brainstorm with you, uh, like, on the go.
**Speaker 1 - 17:45**
Gotcha.
**Speaker 2 - 17:46**
Um, I have two ideas in my mind. I'm not sure that we need to move tasks from yesterday, to be honest. Just, like, just move them here. And . On the un-un- unless user wants want this, like, unless , uh, they specifically decided to move this task. But what I'm thinking about is some sort of suggestion and maybe it could be a good, like, Starter starting point for Charlie, like,
**Speaker 1 - 18:38**
Mm-hmm.
**Speaker 2 - 18:38**
uh, you open I, I have two thought two things. In my mind . One is , like, this Charlie block with some sort of suggestion, and . Give me a second to take stuff from . I want to take this block. Some sort of suggestion and . Summary from , like, hey, you have three like, hey, you have three unfinished . Tasks from yesterday. One. Two, move them there. And it's, like, Charlie first interac tion, like, some sort of and we can put the there's these tas ks and give you as a user opportunity to do this stuff, like, press . Press yes and n o, and just if you press yes, we move them
**Speaker 1 - 19:52**
Mm-hmm.
**Speaker 2 - 19:52**
we. We remove this block, we remove, like, uh, message, but, uh, left — Left only the task itself. Themselves. And I, I thought about first and thought, like, it's it's okay. But what I don't like here is that it's kinda performative for m e. Like, you know, it's, it's something that every designer will think when when they uh, thinking about , like, AI helping in day-to-day basis. And
**Speaker 1 - 20:31**
Mm-hmm.
**Speaker 2 - 20:33**
. The second s-stuff that I don't like here is that it still. Feels kinda invasive. So in stead of that, I thought maybe we'll we alre ady have, uh, all instrument s for, for distribution. This tasks. And basically, they leave behind you so maybe we could move you m ove yesterd ay page up a little bit. In that case, and. Right here, something like one, two, bring — Unfinished tasks. Tw o. New day
**Speaker 1 - 21:30**
M
**Speaker 2 - 21:30**
to
**Speaker 1 - 21:30**
m-hmm.
**Speaker 2 - 21:31**
the new day. For example, I don't know.
**Speaker 1 - 21:33**
Mm-hmm.
**Speaker 2 - 21:35**
And. Some buttons here. Um, I started to think that actually this app Charlie anything button is , hmm. Not the right solution here beca use it removes a lot of good interaction points. But do you understand what I'm saying?
**Speaker 1 - 21:55**
Mm-hmm.
**Speaker 2 - 21:58**
And we can show here these buttons as well. Move. Or dismiss. Like, if you want to see these tas ks, we can, like, I don't know, for ex ample, just give you opportun ity to scroll down and see them.
**Speaker 1 - 22:20**
I want to stop you off there
**Speaker 2 - 22:21**
Or
**Speaker 1 - 22:21**
and and
**Speaker 2 - 22:21**
somehow
**Speaker 1 - 22:22**
and ask ask a ques tion.
**Speaker 2 - 22:24**
.
**Speaker 1 - 22:24**
Real quick. So like do you
**Speaker 2 - 22:26**
S
**Speaker 1 - 22:26**
th
**Speaker 2 - 22:26**
ure
**Speaker 1 - 22:26**
ink
**Speaker 2 - 22:26**
. Sure, sure, sure.
**Speaker 1 - 22:27**
do you think like there's for the second design, do you think the . Like what do you call it? Because l ike the prompt should be like sticky on like the bottom side or like is this something that's showing just like naturally by scrolling? Because like from this design, it seems like it needs to be exposed at all times, right?
**Speaker 2 - 22:59**
Mm-hmm. Yeah, you're right.
**Speaker 1 - 23:05**
Right . Because like my thought was like if if then like you you start decre asing the height of the window then you would have to like in order to kind of like show like the content of like like let's say today's note. And it starts over
**Speaker 2 - 23:18**
M
**Speaker 1 - 23:19**
fl
**Speaker 2 - 23:19**
m
**Speaker 1 - 23:19**
ow
**Speaker 2 - 23:19**
-hmm.
**Speaker 1 - 23:19**
ing then the the like the like the the container that's wrapp ing around like the content should like needs to be like scrollable which in that like in from my understanding isn't really natural because then we'll have like two scrollable areas, right?
**Speaker 2 - 23:37**
Yeah.
**Speaker 1 - 23:48**
Hmm.
**Speaker 2 - 23:51**
Or we can — Merge them. Into something like. Charlie related. Like,
**Speaker 2 - 24:06**
open this button.
**Speaker 1 - 24:07**
Mm-hmm.
**Speaker 2 - 24:08**
And tell you, like, you have three three unfinished tasks. From yesterday.
**Speaker 2 - 24:24**
Bring them to. The . I'm not sure the right
**Speaker 1 - 24:32**
Mm-h
**Speaker 2 - 24:32**
word
**Speaker 1 - 24:32**
mm.
**Speaker 2 - 24:33**
ing here, actually. And the but ton, again, so in this case, we have, like, sticky usual interface and, uh, maybe — And it appears from usual place for yesterday. Like, it appears from from the bottom where yesterday lives right now.
**Speaker 1 - 24:55**
Mm-hmm.
**Speaker 2 - 24:56**
And it it could work , probably. I don't like in this constru ction only that we don't show you task specifically.
**Speaker 1 - 25:07**
Mm-hmm.
**Speaker 2 - 25:08**
Um, but I I want to raise a different question here. And
**Speaker 1 - 25:15**
Yep.
**Speaker 2 - 25:15**
, uh, this question more about , like, hmm, do we need this moving tasks to today ? Uh, solution at the first place. Because in. My experience, i- it's I I I understand the probl em. I understand that if you did n't finish something, uh, we should still, like, show you that you have. This task on you. And it's the right construction for usual to-do lists. Like, when you have everything, uh, on one page, it's a under standable. Like, I ne ed to see what's what things I didn't finish. But in daily note, and in daily note construction, where each new day gives you a new focus.
**Speaker 1 - 26:22**
Mm-hmm.
**Speaker 2 - 26:22**
Areas and
**Speaker 1 - 26:23**
Mm-hmm.
**Speaker 2 - 26:24**
new , h mm, problems to solve, and ideas to create,
**Speaker 1 - 26:30**
Yep.
**Speaker 2 - 26:31**
I'm not su re that it's the right solution.
**Speaker 1 - 26:34**
I get what you're saying. Yeah.
**Speaker 2 - 26:35**
And
**Speaker 1 - 26:36**
Tell.
**Speaker 2 - 26:36**
yeah, and I I I can't bring you any good , um, data here. And I need to speak with some people who
**Speaker 1 - 26:47**
Mm-hmm.
**Speaker 2 - 26:49**
who is very task-heavy people. I I need to speak with you, like, for example, here. I have only my experien ce and opinion, and my experience and opinion in Filo and in , uh, current , uh, chart. Which day in the task is a bit mostly frustrating things for me.
**Speaker 1 - 27:10**
Right.
**Speaker 2 - 27:10**
Uh,
**Speaker 1 - 27:10**
Right.
**Speaker 2 - 27:10**
it's I I open it and I see, like, uh, bring new, um, prototype to to the guys about some stuff. I understand that actually I just didn 't check it out check it out or it just become a much bigger task than, like, at first and
**Speaker 1 - 27:30**
Hmm.
**Speaker 2 - 27:31**
just a simple to-do list. Um, and I need to have a some time for this, and I need to , like, split it or, lik e, change it.
**Speaker 1 - 27:42**
Right
**Speaker 2 - 27:42**
H
**Speaker 1 - 27:42**
.
**Speaker 2 - 27:42**
mm, so this is what I want to discuss.
**Speaker 1 - 27:47**
That's a really good point. And I think I kind of like feel that as well. Um, I just I
**Speaker 1 - 27:57**
It's a really tough question though.
**Speaker 2 - 28:08**
But maybe we can do something like this. Maybe we don't need to move them. We can say just . Delegate these tasks. Or something.
**Speaker 1 - 28:26**
Hmm.
**Speaker 2 - 28:36**
But all this feels — In my opinion, feels very Frustrating.
**Speaker 1 - 28:48**
Mm-hmm.
**Speaker 2 - 28:49**
But.
**Speaker 1 - 28:50**
I I I just think that like like if we do this like if we make this ch ange like by showing this like y ou got three unfinished tasks um . Which by the way like of those three I think there would be like like let's say just one of them is actually meaningful. But l ike
**Speaker 2 - 29:11**
Yeah.
**Speaker 1 - 29:11**
like two
**Speaker 2 - 29:12**
Yeah, it's
**Speaker 1 - 29:12**
is
**Speaker 2 - 29:12**
true.
**Speaker 1 - 29:12**
just like some brainstorming session or like whatever. Like it could be something that's just marginal, right ? Um, then it's just
**Speaker 2 - 29:21**
M
**Speaker 1 - 29:21**
not
**Speaker 2 - 29:21**
m-hmm.
**Speaker 1 - 29:21**
like it's not it's just not worth the time and effort to actually kind of like do it. Do do that, right? Um, so like I just think that like, you know, like like we said before like we have to be opinionated about like like how we design and I guess like the feeling that that we should be giving to users is that like, oh, like it's not creating a liability. Or anyth ing. It's just
**Speaker 2 - 29:47**
Yeah.
**Speaker 1 - 29:48**
something that's actually bringing clarity as well as . No. Feeling like I'm actually getting things done um so like in terms of that I think like triaging like if we could somehow magically triage like what needs to be done then like, you know, like I guess like it's it's up to the user to actually kind of like have like a shitload of lists like task items just like kind of like listed in a single day like explicitly can just like type stuff in like that. But like once that day's over I guess it's up to us to kind of like keep track of that in the background, right? And then actually
**Speaker 2 - 30:33**
Mm
**Speaker 1 - 30:33**
kind
**Speaker 2 - 30:33**
-hmm.
**Speaker 1 - 30:33**
of like ass ess, dude, is this worth the time and effort for you? Like or should I I know like just you you listed these stuff for me to kind of like take a look at it. But like I'm not going to be suggesting you to actually and I don't expect you to do all these stuff . And but like with all due respect like if you were to actually do like let's say five of them on the list of the 100 things that you' ve listed I think it 's worth like giving me like three of them to explore and then you should do these two because these seem to be like these seem to be kind of import ant. In some sense. So I gu ess like like you like you're trying to I think what you're trying to get at like consistent ly is like to be less inv asive and not creating these like not not increase the entropy as
**Speaker 2 - 31:38**
M
**Speaker 1 - 31:38**
let
**Speaker 2 - 31:38**
m
**Speaker 1 - 31:39**
's say
**Speaker 2 - 31:39**
-hmm.
**Speaker 1 - 31:39**
let's say that. Like not increasing the entropy um inside one's mind. So I get that. Hmm. Hmm.
**Speaker 2 - 32:02**
Yeah, at least, least, least. And, um, we can one. Two, bring them to the current day. You could delay them to me. And there should be some buttons. It's actually I. It's worth it because it both shows Charlie's productivity and, um , it doesn't feel like two mechan istic here. We don't show you just everything for the sake of performative. Uh, performative task del egation. Like, we don't show you, like, 2 0 tasks you should you just forget to checked out. We can just as k Charlie to track your progress and . Uh, on the start of each d ay, ask about it . Like, even not, like, just ask about, uh, you have some unfinished business , but we can just ask about , I don't know, I see that , um, you have a. PRs or tasks that not, I don't know, checked. Out yesterday, want me to check them out. So
**Speaker 1 - 33:46**
Yeah.
**Speaker 2 - 33:46**
it's basically not just . Number of tasks, but it could be also — Very active interaction with Charlie and what I believe it would be the most a. Recurrent interaction with Charlie. For the users, because in my experience and in my experience of other people that I worked with and speak, uh, about, uh, Tasks and, uh, to-d os and lists, a lot of people just , for some reason, didn't, uh, check everything out in the end of the day. And we And they will probab ly every day interact with some Charlie screen here. Asking, like, I see that you have someth ing or, like, I saw that you — Create a task and , uh, finished it or, like, delegated to someone and didn't check it out.
**Speaker 1 - 35:00**
Mm-hmm.
**Speaker 2 - 35:01**
It's a good—it's a good suggestion. I believe. Uh, about tri aging the right stuff and show it . We even could—I, I don't like here only one thing. Is it that if we giv e, give everything to the you or to the AI and, uh, it will cost us some—some tok ens if it will be, like, very recurrent t ask that happens on, like, thousands of users every day that Charlie goes to list and understand, like, okay, I see this and that. But what we can do, we can optimize it a little bit. We can, like, g ive— like, I don't know, three possible solu tions here. Like, uh, one is we found important stuff , uh, from a lot of noise. And give this message or, like, we found some stuff that finished and go — Integrations, but, uh, didn't, like, finished and — In charm? I don't know. And this is the second option. What do you think?
**Speaker 1 - 36:27**
So is this like more of like a like logic question or like more of a design question?
**Speaker 2 - 36:34**
I guess both .
**Speaker 1 - 36:40**
Hmm.
**Speaker 2 - 36:41**
First of all, about , uh, this possible solution. And the approach. And second, about, like, in terms of logic, how it sounds.
**Speaker 1 - 36:53**
Hmm. I see the idea. I mean like I'm I'm open to both I guess right now. Um
**Speaker 2 - 37:03**
Yeah. We can drop it into you, John and Bean.
**Speaker 1 - 37:07**
M
**Speaker 2 - 37:07**
And
**Speaker 1 - 37:07**
m-hmm.
**Speaker 2 - 37:07**
, uh, discuss it, uh, in Slack together.
**Speaker 1 - 37:10**
Yeah. Yeah. That sounds good.
**Speaker 2 - 37:11**
B ecause—because, yeah, hmm, me and you, we both, uh, have agreement that probably it's not the right solution to just put everything —uh, right. And users, uh, editor and not every task worth, uh, moving to, like, to today.
**Speaker 1 - 37:33**
Mm-hmm.
**Speaker 2 - 37:35**
Like, I even for. My day-to-day basis, I have some things in my things tree on m
**Speaker 1 - 37:44**
Hmm.
**Speaker 2 - 37:45**
y, uh, iPhone that I. Never finished and they always unchecked for and move for today, each new day. And it's mostly, like, things like—I don't know—pay water bills, for example.
**Speaker 1 - 38:02**
Right. R
**Speaker 2 - 38:03**
I
**Speaker 1 - 38:03**
ight.
**Speaker 2 - 38:03**
just
**Speaker 1 - 38:03**
Exactly.
**Speaker 2 - 38:03**
— I just forget about them. I just— I see them, like, ah, yeah, okay, sure, I need to do that. And I go, uh, into a prov ider and pay everything and —and I didn't back and check it. I just —there. Sometimes when I feel bor ed, I just open it and click on them all and few myself superior, but
**Speaker 1 - 38:25**
Hmm.
**Speaker 2 - 38:26**
most of the time it's just here. I need to delete this feature. Actually. H mm. So yeah. And I even don't have the right metric here to—to count. To be honest. Like, we can count —
**Speaker 1 - 38:45**
Mm-hmm.
**Speaker 2 - 38:47**
Some every end about, like, accepting or declining Char lie's interaction on us—on tasks, maybe. But if we move task each, like, un—unfinished task to the new day, it's kind of hard to implement the right event to track that user deletes them. Because I believe we could n't track , like, content in—in the editor as events. So if you just move th
**Speaker 1 - 39:23**
Mm-hmm.
**Speaker 2 - 39:24**
em. Hmm.
**Speaker 2 - 39:30**
Or we can — Do basically what, uh, we do right now, just suggest only triaged important stuff. And give accept decline near each of them.
**Speaker 2 - 39:53**
Let me, uh, make just —just our friends for this. Even don't need some prototypes generally. I believe we can have simple warframes. Here and bring these two solution s. Here. First, the first one would be about , like, Char lie asking you and suggest you to, like, delegate them. And, uh, second , Charlie brings it, like, into your editor and
**Speaker 1 - 40:23**
Mm-hmm.
**Speaker 2 - 40:23**
, uh, you can accept and decline them, but in both case, it will be like triaged from all the noise important stuff. Maybe even free region, uh, by Charlie somehow. Because on. Not really. I don't know. So yeah.
**Speaker 1 - 40:47**
Um like
**Speaker 2 - 40:47**
But I do—I
**Speaker 1 - 40:49**
go ahead.
**Speaker 2 - 40:50**
— Yeah, I believe it's not like a problem about just moving tasks from yesterday. It
**Speaker 1 - 40:57**
M
**Speaker 2 - 40:57**
's
**Speaker 1 - 40:57**
m
**Speaker 2 - 40:57**
actu
**Speaker 1 - 40:57**
-hmm.
**Speaker 2 - 40:57**
ally a big. Um, interaction point because if we —uh —try to, like, just . I f—if—if—if we think that Charlie will be proactive and bring you stuff into your editor in the future, we—it—it basically the same interaction. And it's, uh, question about
**Speaker 1 - 41:27**
Mm-hmm.
**Speaker 2 - 41:28**
two possible ways. Uh, lik e, we give editor ful ly for user
**Speaker 1 - 41:37**
Y
**Speaker 2 - 41:37**
or
**Speaker 1 - 41:37**
ep.
**Speaker 2 - 41:37**
we make it, like, shared space.
**Speaker 1 - 41:42**
Artem, what do you think about like actu ally like m like creating an experience where Char lie uh learns like would you prioritize ? So what I mean by that is like like I'm I'm normally us uh I'm using Evec AI for the um for my email inbox these days. And it's basically like a Tinder for emails. Like you can swipe right to l
**Speaker 2 - 42:07**
Ye
**Speaker 1 - 42:07**
ike
**Speaker 2 - 42:07**
ah, I sa
**Speaker 1 - 42:07**
mark
**Speaker 2 - 42:07**
w it
**Speaker 1 - 42:07**
that
**Speaker 2 - 42:07**
. Yeah.
**Speaker 1 - 42:08**
it's done and then like sw ipe left to kind of like mark it as like I'm gonna be doing it later. And and also you can just like swipe it downward s to mark it as low importance . I was thinking like
**Speaker 2 - 42:21**
M
**Speaker 1 - 42:21**
if
**Speaker 2 - 42:21**
m-hmm.
**Speaker 1 - 42:22**
like what if we kind of surface lo like not only tasks but like like let's say like emails or whatever and som etimes there are tricky on es right? That that I just think that like if if there are obvious ones like for examp le if it's past like a certain due date then there's a problem right? If if something's like about you know regarding your bank ac count that y our bank is going to be like you know like fucked up because it's like SVB or something you know. I don't know. But like um those obvious ones like excluding them like there are certain like there are ones in the gray area I guess like you need to kind of l ike kind of explicitly state this is low importance y ou know. And also there are stuff like that changes over time as well right? Like you might think that some task was important at a certain period of time but then like as time passes by you might kind of like depriorit ize that because like things might change. Like just like how like like how our start our startup is right? So um um in that regard I I think like what if we show like like Char lie um show like a modal and then like use like the keyboard like the left and right key to kind of like appro ve like let's say like mark as import ant. Or like you know
**Speaker 2 - 43:56**
Mm-hmm.
**Speaker 1 - 43:57**
add this like this this card that and then you'll be able to kind of re ally like swiftly go through like I guess like a list of ten ten stuff right? Like whether you wanna keep it or not. And then let's just say you start keeping things um. Or like five days straight and then you didn't complete them. I don't then this might be an indicator for like the AI to actually say that dude you've been just like stashing the like these three things for like the past five days but you haven't done shit. I didn't I don't think this is important. Like I think this is just like creating some like cognitive overload for you. I'm just gonna be discarding it for you. What do you think? And then just like if you approve that on like the fifth day it just it's just gone. But it will be like stay ing on whatever like daily not es that you've like written it ri written it in. So like it doesn't go away but like it's not being surfaced if that makes sense.
**Speaker 2 - 45:03**
It's a good idea.
**Speaker 1 - 45:07**
Yeah. So like that's a that 's a like a quick idea that I had on my mind but
**Speaker 2 - 45:13**
Ye
**Speaker 1 - 45:13**
.
**Speaker 2 - 45:13**
ah, let me try it as well.
**Speaker 1 - 45:14**
Mm-hm
**Speaker 2 - 45:15**
It
**Speaker 1 - 45:15**
m.
**Speaker 2 - 45:15**
's like a little more complicated than just moving stuff here and there, but
**Speaker 1 - 45:20**
Right.
**Speaker 2 - 45:22**
yeah. I can try it and show it.
**Speaker 1 - 45:24**
Right right.
**Speaker 2 - 45:25**
So bas— basically, it—it could be just some sort of, um, cards. Inside the , like, Charlie model, for example.
**Speaker 1 - 45:36**
Mm-hmm.
**Speaker 2 - 45:37**
That will have — Like, tasks itself. Or maybe, like, some summariz ation of the same task that user writes in each day. Like, for example, if user writes, like, "Don't forget to speak with Diana about fin ances," or, like,
**Speaker 1 - 45:58**
Mm-hm
**Speaker 2 - 45:58**
"C
**Speaker 1 - 45:58**
m.
**Speaker 2 - 45:58**
heck— check the finances with Diana," or, lik e, I don't know, whatever. Charlie could, like, get all this from history, understand this is basically about the same stuff, and the user continuously writ es it. So, like, do you w ant to make it recurrent? Do y ou want to, like, put it in —in. Your daily note ?
**Speaker 1 - 46:24**
Bro
**Speaker 2 - 46:24**
Or, lik
**Speaker 1 - 46:24**
l
**Speaker 2 - 46:24**
e,
**Speaker 1 - 46:24**
ike
**Speaker 2 - 46:24**
if user just writes something,
**Speaker 1 - 46:26**
M
**Speaker 2 - 46:26**
lik
**Speaker 1 - 46:26**
m-hmm.
**Speaker 2 - 46:27**
e, feels like, I don't know, our daily current us ers is low today. Like, our da ily current users is above average.
**Speaker 1 - 46:38**
Artem I had like a c
**Speaker 2 - 46:39**
Char
**Speaker 1 - 46:39**
razy
**Speaker 2 - 46:39**
lie
**Speaker 1 - 46:39**
tho
**Speaker 2 - 46:39**
will
**Speaker 1 - 46:40**
ught. Crazy thought right now. Um
**Speaker 2 - 46:42**
—
**Speaker 1 - 46:42**
mind if I share my screen?
**Speaker 2 - 46:46**
Sure thing. St
**Speaker 1 - 46:48**
Ye
**Speaker 2 - 46:48**
op
**Speaker 1 - 46:48**
ah
**Speaker 2 - 46:48**
sh
**Speaker 1 - 46:48**
ye
**Speaker 2 - 46:48**
aring.
**Speaker 1 - 46:48**
ah yeah. Just like a simple thing. But what if we kind of like have those things as li as like cards and it shows up on like the bottom bottom edge and like it just like kind of like surfac es like card by card and you kind of like swipe it. Like I it's some crazy idea. Um that I'm just throwing but
**Speaker 2 - 47:10**
N
**Speaker 1 - 47:10**
.
**Speaker 2 - 47:10**
o, it's—it's good. And—and—and this metap hor is very notebook-related metaphor.
**Speaker 1 - 47:17**
Right. And I I I think I re
**Speaker 2 - 47:19**
It's a physical object.
**Speaker 1 - 47:21**
right. And I think I reckon l ike you kind of l ike implemented something similar with your like previous projects right? I I'm not
**Speaker 2 - 47:32**
Ok
**Speaker 1 - 47:32**
su
**Speaker 2 - 47:32**
ay.
**Speaker 1 - 47:33**
re. I
**Speaker 2 - 47:33**
I
**Speaker 1 - 47:33**
'm
**Speaker 2 - 47:33**
'
**Speaker 1 - 47:33**
not
**Speaker 2 - 47:33**
m not
**Speaker 1 - 47:33**
sure
**Speaker 2 - 47:33**
sure.
**Speaker 1 - 47:33**
but um I think you have one in your portfolio. Last time I saw it. Not sure but. Not well it might be different but you get the point right?
**Speaker 2 - 47:46**
No, it—yeah, it's a good idea. It's a good idea. So it's —it's just becomes a more complex question than just what if we —how we will show tas ks. Because it's now become like a platform for learning and a platform of— for Charlie to understand you based on recurrent stuff.
**Speaker 1 - 48:09**
Right.
**Speaker 2 - 48:09**
And maybe user don't ne ed in this case to constantly receive the same, like, "Do you want to move this from yesterd ay?"
**Speaker 1 - 48:20**
Mm-hmm.
**Speaker 2 - 48:21**
Let me tr y this. Let me—this one I should prototype definitely. I' m not—I'm not sure that just one screen will enough to under stand.
**Speaker 1 - 48:30**
Yeah
**Speaker 2 - 48:30**
But
**Speaker 1 - 48:30**
totally.
**Speaker 2 - 48:31**
, uh, Yeah, I—I'll do that.
**Speaker 1 - 48:37**
Sounds good.
**Speaker 2 - 48:39**
Um, okay. What else I want to discuss with you? Uh, simple interaction point. Hm m, I just , uh, made this stuff we spoke about , like, what if user selects everything and, uh, how—and dec ides to delegate th
**Speaker 1 - 49:04**
M
**Speaker 2 - 49:04**
em.
**Speaker 1 - 49:04**
m-hm
**Speaker 2 - 49:04**
And
**Speaker 1 - 49:04**
m.
**Speaker 2 - 49:04**
it's—the easiest solution here, basically, I copied it from various of , uh, editors. You have just some floating, u h, button near the selection, and it's easy. But what I started to think about is, uh, some sort of interaction with , um.
**Speaker 2 - 49:29**
Notes, text notes here, and how they should . Work in terms of , like. Selecting them. What I mean, this is one of, uh, like, uh, interaction stuff. Like, for example, uh, it's my kind of personal, but no worries. If
**Speaker 1 - 49:54**
Can't re
**Speaker 2 - 49:54**
I
**Speaker 1 - 49:55**
ad it.
**Speaker 2 - 49:57**
— Okay. If I add here some—wow, it's actually bringing a lot of mess here. Sh it.
**Speaker 1 - 50:07**
Yikes.
**Speaker 2 - 50:07**
Don't like it. So if I add this stuff, and it transforms —uh, into a link. When I select it, it transforms back to just, uh, items.
**Speaker 1 - 50:23**
Right.
**Speaker 2 - 50:25**
And, like, hmm, markdown . What do you think? Should we do the same for our ed itor? Or should we just show, um,
**Speaker 1 - 50:46**
Hmm.
**Speaker 2 - 50:46**
Notes? Like, you—you wrote them, and you can change them only by deleting something. Uh, by deleting something, I mean. That if I, like, Decide to change —I—I can change this number only by pressing on it. But if I start to delete it, if I press backspace near this,
**Speaker 1 - 51:16**
Mm
**Speaker 2 - 51:16**
we
**Speaker 1 - 51:16**
-h
**Speaker 2 - 51:16**
rem
**Speaker 1 - 51:16**
mm.
**Speaker 2 - 51:16**
ove the note—the note, uh, related configur
**Speaker 1 - 51:22**
M
**Speaker 2 - 51:22**
ation
**Speaker 1 - 51:22**
m-hmm.
**Speaker 2 - 51:23**
and just show it as a number. Like,
**Speaker 1 - 51:26**
M
**Speaker 2 - 51:26**
like
**Speaker 1 - 51:26**
m
**Speaker 2 - 51:26**
this.
**Speaker 1 - 51:26**
-hmm.
**Speaker 2 - 51:29**
Or if it —
**Speaker 2 - 51:38**
I'm not sure how you did it in Filo actually, beca use I forget it about, uh, about the Filo before we —I. You just did a demo. Okay.
**Speaker 1 - 51:50**
Yep.
**Speaker 2 - 51:50**
It—it totally makes sense.
**Speaker 1 - 51:53**
It's just similar to Notion.
**Speaker 2 - 51:56**
Yeah.
**Speaker 1 - 51:57**
But I guess like w+we could do like potentially is something like like you were to s like you hit backspace and then you show like like a l ike a prompt or like a alert di alogue thing you wanna remove this format but. Hmm. I just don't think that's like a natural experience. Right? Because l ike you kn
**Speaker 2 - 52:26**
Yeah.
**Speaker 1 - 52:26**
ow you're typing stuff in and like whenever you're like hitting backspace or whatever and then something just pops up. I think that's a bit intrusive right? So. I don't know. I just l ike I I don't think like you know there's any problem with like re-removing the chip t like just um as a whole. I I'm not actu ally sure with how to convert ing that into a plain text and then um you start to edit it.
**Speaker 2 - 53:02**
Mm-hmm. Yeah. Okay. Let's keep the, uh, deleting the whole then. It's not a big problem, I believe.
**Speaker 1 - 53:12**
Got it. Okay.
**Speaker 2 - 53:16**
And what else I want to show you and discuss here are— Ah, no. It's not here. So I under stand what you spo—what you said about this one, and it's—it's true. And you're right totally. And I will change it. Uh, what do you think about all this, like, flow? Like, this states and
**Speaker 1 - 53:41**
Mm-hmm.
**Speaker 2 - 53:41**
is it an understandable ? You're—you're the only one who reacts on this. It's kind—kind of sad.
**Speaker 1 - 53:53**
I think like people are
**Speaker 2 - 53:53**
Ye
**Speaker 1 - 53:53**
bus
**Speaker 2 - 53:53**
ah,
**Speaker 1 - 53:53**
y.
**Speaker 2 - 53:54**
because —yeah, I understand. I just —it's actually took me so much time that I felt, like, maybe I just should —I wipe code it all from scratch. Just to make this prot otype
**Speaker 1 - 54:10**
M
**Speaker 2 - 54:10**
in
**Speaker 1 - 54:10**
m
**Speaker 2 - 54:10**
F
**Speaker 1 - 54:10**
-hm
**Speaker 2 - 54:10**
ig
**Speaker 1 - 54:10**
m.
**Speaker 2 - 54:10**
ma was too much.
**Speaker 1 - 54:15**
Mm-hmm.
**Speaker 2 - 54:15**
But yeah, uh, it —it has three states.
**Speaker 1 - 54:21**
Yep
**Speaker 2 - 54:22**
D
**Speaker 1 - 54:22**
.
**Speaker 2 - 54:22**
ifferent stat es. One is, like, thinking block behind it. One is, uh, very small and, uh, like, like a, uh, subtle— subtle loader. That appe
**Speaker 1 - 54:37**
Yep
**Speaker 2 - 54:37**
ars
**Speaker 1 - 54:37**
.
**Speaker 2 - 54:38**
only for checkl ists and, uh, bullet and other kind of lists bec ause I'm not sure that it—it's a good solution to m ove text to the left or—oh, sorry, to the right if you have just a plain text working on
**Speaker 1 - 55:00**
Mm-hmm.
**Speaker 2 - 55:01**
. And, uh, and this carried with different states. Like, searching, doing, blah, blah, blah. At first, I thought it's a lot, but now I'm thinking that actually it's fine.
**Speaker 1 - 55:18**
Mm-hmm. I mean let's see. Let's take a look at it again.
**Speaker 1 - 55:31**
All right. Mm-hmm.
**Speaker 1 - 55:37**
Oh. Oh I see what you did with the task item. That's super nice.
**Speaker 1 - 55:50**
Oh that's gorgeous.
**Speaker 2 - 55:56**
Just afraid that it could be too much.
**Speaker 1 - 56:02**
Reading a meeting.
**Speaker 1 - 56:13**
Mm
**Speaker 2 - 56:13**
And
**Speaker 1 - 56:13**
-hmm.
**Speaker 2 - 56:13**
ideally, it should just , like, should—should be different animation here. Like, some sort of appearing from after the, uh, cursor, after the Charlie's cursor. But again, it was hard to do in F igma. I mean,
**Speaker 1 - 56:30**
H
**Speaker 2 - 56:30**
it
**Speaker 1 - 56:30**
mm.
**Speaker 2 - 56:30**
—it's a real—it —it's —it's something that I can do, but I don't want to spend the whole day on this.
**Speaker 1 - 56:38**
Mm-hmm.
**Speaker 2 - 56:39**
Animation.
**Speaker 1 - 56:42**
Hmm.
**Speaker 2 - 56:43**
And, uh, I underst—understand about this one. Like, I even don't think , uh, now that I should make this block the. The sharp and, uh, bright. Maybe we should stay in this case.
**Speaker 1 - 57:00**
Question. Um so you showed like the task that n+needed to be done and like how Charlie is perceiving those tasks. And
**Speaker 2 - 57:12**
Yeah.
**Speaker 1 - 57:13**
within their cap like the extended carrot right?
**Speaker 2 - 57:16**
Yeah.
**Speaker 1 - 57:17**
So technically l ike so coffee with Masha today is like you you approve it to be con verted into a like
**Speaker 2 - 57:30**
R
**Speaker 1 - 57:31**
a
**Speaker 2 - 57:31**
emating.
**Speaker 1 - 57:31**
ca l ike a
**Speaker 2 - 57:31**
Yeah.
**Speaker 1 - 57:32**
calendar e+event or like a meeting right? Then
**Speaker 2 - 57:35**
Yeah.
**Speaker 1 - 57:36**
— What if we like expand that into like nested items? Could we do that as well? Like g I just it just seems like to have like a full visibility of like the things that should be done that or that will be done from that approval kind of like gives you more visibility whereas like right now
**Speaker 2 - 57:57**
Hmm.
**Speaker 1 - 57:58**
it's kind of like all cascaded right? So.
**Speaker 1 - 58:04**
So I think
**Speaker 2 - 58:04**
Ye
**Speaker 1 - 58:04**
I
**Speaker 2 - 58:04**
ah.
**Speaker 1 - 58:04**
think
**Speaker 2 - 58:05**
Ye
**Speaker 1 - 58:05**
there
**Speaker 2 - 58:05**
ah.
**Speaker 1 - 58:05**
's a d
**Speaker 2 - 58:06**
I—
**Speaker 1 - 58:06**
there are pros and cons to these like designs but like I just wanna kind of explore as much as possible so.
**Speaker 2 - 58:14**
I guess I did it
**Speaker 1 - 58:18**
Hmm.
**Speaker 2 - 58:18**
. Yeah. I thought about this and
**Speaker 1 - 58:22**
Y
**Speaker 2 - 58:22**
wh
**Speaker 1 - 58:22**
ep
**Speaker 2 - 58:22**
at
**Speaker 1 - 58:23**
.
**Speaker 2 - 58:23**
I didn't like about, uh, this stuff is that . What if —uh, I—I can't figure out the right . Number of stuff. I mean, what we should do? It should be just, uh, one item that constantly changes, or it should be, like, some sort of checking—checklist from AI that should appear here, like, it's done or not
**Speaker 1 - 58:55**
Hmm.
**Speaker 2 - 58:56**
. And if it's done, lik e, should it still sta y in user's input? In—in us er's note?
**Speaker 1 - 59:07**
Mm-hm
**Speaker 2 - 59:08**
And
**Speaker 1 - 59:08**
m.
**Speaker 2 - 59:08**
what makes me moving out of this idea from this idea is that I thought, okay, it's —it—it makes sense in terms of, like, AI working. On the same — Level as you, lik e, in—in the same structure as you, and use the same tools as you us e,
**Speaker 1 - 59:32**
Mm
**Speaker 2 - 59:32**
just
**Speaker 1 - 59:32**
-hmm.
**Speaker 2 - 59:32**
more effective, probab ly. But what if there will be more than one active task? And you just delegate, lik e, create a meeting, and after that, you just write some stuff about , like, I don't know, check out the Figma pricing and delegate this one. We will show you two different items that con—right now . Delegated . And each of these items will just generate some new blocks under it.
**Speaker 1 - 01:00:11**
Right.
**Speaker 2 - 01:00:12**
And it felt kind of no—noisy for me. It f elt like I
**Speaker 1 - 01:00:18**
Mm
**Speaker 2 - 01:00:18**
have
**Speaker 1 - 01:00:18**
-hmm.
**Speaker 2 - 01:00:18**
an editor space where I just write some
**Speaker 1 - 01:00:20**
Mm
**Speaker 2 - 01:00:21**
st u
**Speaker 1 - 01:00:21**
-h
**Speaker 2 - 01:00:21**
ff
**Speaker 1 - 01:00:21**
mm.
**Speaker 2 - 01:00:21**
and AI just creates some new, uh, sub-block and everything moves down. And that's why I moved from this idea.
**Speaker 1 - 01:00:32**
Got it. So basic
**Speaker 2 - 01:00:32**
Maybe
**Speaker 1 - 01:00:33**
ally
**Speaker 2 - 01:00:33**
it's actually not a big problem.
**Speaker 1 - 01:00:35**
—
**Speaker 2 - 01:00:35**
I don't know.
**Speaker 1 - 01:00:36**
So I guess like you kinda like excluded that based on some extreme conditions that we might run into
**Speaker 2 - 01:00:44**
Yeah.
**Speaker 1 - 01:00:44**
right?
**Speaker 2 - 01:00:45**
Yeah.
**Speaker 1 - 01:00:45**
Um yeah it makes sense I guess. But then like the question is like a+also like like we could delegate a lot of these things at the same time. Do you think like
**Speaker 2 - 01:00:57**
Yeah.
**Speaker 1 - 01:00:58**
there could be multi ple Char lie character like carrots? I just I'll just call it Charlie carrots. Like Charlie carrots appearing on the daily note. Or like I don't know like like obviously I think that we we should kinda like separate like the carrot color from like your carrot and Charlie's carrot. To k
**Speaker 2 - 01:01:20**
Yeah.
**Speaker 1 - 01:01:20**
inda like distinguish it. But like let's say and I don't know if you've looked at this project called Click y. It's by this dude called Far za. Like it's it ba it's basically l ike it like a desktop assistant um where it follows your cursor
**Speaker 2 - 01:01:38**
Re
**Speaker 1 - 01:01:38**
around
**Speaker 2 - 01:01:38**
—re
**Speaker 1 - 01:01:39**
.
**Speaker 2 - 01:01:39**
use the cursor. Yeah.
**Speaker 1 - 01:01:40**
Ye
**Speaker 2 - 01:01:40**
I
**Speaker 1 - 01:01:40**
ah
**Speaker 2 - 01:01:40**
—
**Speaker 1 - 01:01:40**
yeah yeah yeah.
**Speaker 2 - 01:01:41**
I—I see the demo, but I—it—it was, like, under waitlist or something. I didn
**Speaker 1 - 01:01:46**
M
**Speaker 2 - 01:01:46**
't
**Speaker 1 - 01:01:46**
m
**Speaker 2 - 01:01:46**
che
**Speaker 1 - 01:01:46**
-h
**Speaker 2 - 01:01:46**
ck
**Speaker 1 - 01:01:46**
mm.
**Speaker 2 - 01:01:46**
it out.
**Speaker 1 - 01:01:47**
Yeah I I just like I just wanna kinda like like use that analogy and like 'cause like it kinda like spins open like a n a new cursor for like different tas ks that you kinda like um like delegate stuff to Clicky. So like for example um like there's like bl ue red green you know cursors.
**Speaker 2 - 01:02:10**
Mm
**Speaker 1 - 01:02:10**
That
**Speaker 2 - 01:02:10**
-hmm. M
**Speaker 1 - 01:02:10**
that
**Speaker 2 - 01:02:10**
m-hmm.
**Speaker 1 - 01:02:11**
just
**Speaker 2 - 01:02:11**
Mm
**Speaker 1 - 01:02:11**
that
**Speaker 2 - 01:02:11**
-hmm.
**Speaker 1 - 01:02:11**
just like is like you know pinned at the top right side. To kinda like indicate these are are are l ike different tasks. That are being like you know um being run at the same time. So like similar to that like I was just thinking like if we should we have different colors for like different tasks that's being delegated to Charlie or somehow or or like
**Speaker 2 - 01:02:34**
It
**Speaker 1 - 01:02:34**
it
**Speaker 2 - 01:02:34**
's a
**Speaker 1 - 01:02:34**
co
**Speaker 2 - 01:02:34**
n
**Speaker 1 - 01:02:34**
uld
**Speaker 2 - 01:02:34**
ice idea, actually. Yeah.
**Speaker 1 - 01:02:36**
uh-huh. Or it could be like just like we could just use like um some dedicated palette that just like you know be kind of l ike revolve
**Speaker 2 - 01:02:45**
Mm
**Speaker 1 - 01:02:45**
around
**Speaker 2 - 01:02:45**
-hmm.
**Speaker 1 - 01:02:46**
. Or or like we could just like use like a like a gray scale or something right ? Like it could be a lot of options but or just we could just be monotone. Just like right now.
**Speaker 2 - 01:02:59**
It's a good idea. And I also —what if we will have not only different palette, but may be, like, create some—I— I will create some simple icons for sub-agents, like, if Charlie—like, delegate something to research. Agent or, like, delegate something to code agent.
**Speaker 1 - 01:03:21**
Mm mm ye
**Speaker 2 - 01:03:22**
I
**Speaker 1 - 01:03:22**
ah
**Speaker 2 - 01:03:22**
'
**Speaker 1 - 01:03:23**
it
**Speaker 2 - 01:03:23**
m
**Speaker 1 - 01:03:23**
mak
**Speaker 2 - 01:03:23**
not
**Speaker 1 - 01:03:23**
es
**Speaker 2 - 01:03:23**
sure
**Speaker 1 - 01:03:23**
sens
**Speaker 2 - 01:03:23**
if
**Speaker 1 - 01:03:23**
e.
**Speaker 2 - 01:03:23**
we will have such things, but, uh, we can create them as well. And, lik e, you will see that right now, this one is doing some sort of research , and that one just writing, uh, bullet points for you. After
**Speaker 1 - 01:03:39**
Yep.
**Speaker 2 - 01:03:39**
the meeting,
**Speaker 1 - 01:03:40**
Yep totally. Yeah it makes sense. Um
**Speaker 2 - 01:03:45**
let me tr y it. Let me try, uh, multiple carats. And, uh, see how it looks like because maybe it will fe el too—too much. Too much. And I'll try different palette plus, uh, icons. If we'll have som e. Agents. Even we—we'll have not some agents. Still, Char lie will delegate stuff to Dev in, for example, for—for coursework or cloud c ode.
**Speaker 1 - 01:04:15**
right.
**Speaker 2 - 01:04:16**
From our integr ation and, uh, it was—it works to show, like, right now, like, uh, coursework working on it.
**Speaker 1 - 01:04:24**
Yeah and like if we have like multiple carrots I guess like what we could do is like l ike not show everything with like the b ubble all together but like like let's say instead of like hav ing the carrot in like the front of like the task list. Like have it at the end and then just like show l ike an ellipsis. Like the three dots um
**Speaker 2 - 01:04:42**
Yeah.
**Speaker 1 - 01:04:43**
let's say just like moving around. And then look when y ou hover over it like just kinda like shrinks it. Then it becomes like the the turn form. Like we could like there could be multiple possibilities right ? Like um I just think that like like you said like it might be too much if you show like a lot of these information at the same time. But it's it is important to kinda like show like the statuses um in a very intuitive format.
**Speaker 2 - 01:05:12**
Yeah. It's true. It's true. I'll do that.
**Speaker 1 - 01:05:15**
All right that was good. Oh yeah Artem I th
**Speaker 2 - 01:05:20**
So
**Speaker 1 - 01:05:20**
ink I
**Speaker 2 - 01:05:20**
I'll
**Speaker 1 - 01:05:21**
yeah go ahead. Go ahead first.
**Speaker 2 - 01:05:23**
— I guess we're done here, and I just want to say there 's a lot of things to
**Speaker 1 - 01:05:28**
Mm-hmm.
**Speaker 2 - 01:05:29**
catch up with.
**Speaker 1 - 01:05:31**
Yeah I mean like we I think there's a lot of things to explore. Um and we can um honest ly I think I'll just give you the the whole weekend for the for for these stu ff. Like this like what we talk ed about I think is like a big chunk of work right? Um but before we go um like I was thinking like if you co uld if by the end of your day kind of suggest l ike what like what like the daily note editor and like how like the editor should be styled and all those stuff . Um could you kinda like create like a V1 document? Or like it doesn't need to be like a solid document in like Google Docs or any thing.
**Speaker 2 - 01:06:16**
Yeah. Sure
**Speaker 1 - 01:06:16**
R
**Speaker 2 - 01:06:16**
.
**Speaker 1 - 01:06:16**
ight?
**Speaker 2 - 01:06:16**
Sure.
**Speaker 1 - 01:06:17**
L
**Speaker 2 - 01:06:17**
Sure.
**Speaker 1 - 01:06:17**
ike you get what I'm saying right ? Like it ju I think like it just needs to be like a Figma page or something that like l ike Seungbin and Yoojung can kinda like go go and take a look at
**Speaker 2 - 01:06:25**
Look at it.
**Speaker 1 - 01:06:26**
right
**Speaker 2 - 01:06:26**
Ok
**Speaker 1 - 01:06:26**
?
**Speaker 2 - 01:06:26**
ay.
**Speaker 1 - 01:06:27**
And like so so then like you know like I think it's important for us to k inda like explore. And then k inda consolidate into like
**Speaker 2 - 01:06:35**
And now we'll wait until something came.
**Speaker 1 - 01:06:36**
right right right. At the same time so like so then like they can follow up
**Speaker 2 - 01:06:42**
S
**Speaker 1 - 01:06:42**
.
**Speaker 2 - 01:06:42**
ure. Sure. S ure. Yeah. I tried, like, I—I played a few with the phones a little b it, uh, this week and tried —no,
**Speaker 1 - 01:06:49**
Right
**Speaker 2 - 01:06:49**
I
**Speaker 1 - 01:06:49**
.
**Speaker 2 - 01:06:49**
—I mean, we have a guest as our main phone in our brand, and I tried to use it as a— our editor phone, and, uh, it felt miserably. I mean, it 's still a wonderful phon e. It's still a, like, a very pretty typeface. But it—like, for example, it doesn't have an italic. And if it doesn't have italic, you can just, like, press Command + I on sel ected text
**Speaker 1 - 01:07:16**
Mm-hmm.
**Speaker 2 - 01:07:17**
so I decided, okay, let's move with, uh, just simple system font, I guess. Because we don't want also narrow our language options. Like, if you have a lot of not es on Korean, I believe we should just show you your system phone. Even if it's not good. But I don't kn ow much good multilanguage fonts. We have not, or it's kind of
**Speaker 1 - 01:07:46**
Mm-hmm.
**Speaker 2 - 01:07:47**
ugly. For example, so ye ah, I—I'll do that, and I also— because I—I already have most of stuff figured out on my site. I just need to be written and
**Speaker 1 - 01:07:59**
Yeah.
**Speaker 2 - 01:08:00**
, uh, showed up.
**Speaker 1 - 01:08:01**
I just like y ou know like it's like just take them take this into account I guess. Like the part early users are gonna be mostly like you know speaking English and they're gonna be using English. But like for us to dog food it's gonna be l ike it requires Kirill I guess. L ike languages like the Russian language. As well as like
**Speaker 2 - 01:08:20**
I
**Speaker 1 - 01:08:20**
Kore
**Speaker 2 - 01:08:20**
don't
**Speaker 1 - 01:08:20**
an.
**Speaker 2 - 01:08:20**
use it mostly.
**Speaker 1 - 01:08:22**
You don't use that? Ok ay. Um then I guess just try to stick with English then. Like if we had to prioritize. But like I I I I do think that there will be a good option. Um out there in the market.
**Speaker 2 - 01:08:38**
Yeah. I'll check it.
**Speaker 1 - 01:08:39**
Co
**Speaker 2 - 01:08:39**
Che
**Speaker 1 - 01:08:39**
ol.
**Speaker 2 - 01:08:39**
ck it.
**Speaker 1 - 01:08:40**
Um
**Speaker 2 - 01:08:40**
Okay. Sure. I—I'll do that. I'll do that. I'll do that, and, uh, write in the end of the day, like, guys, this is an explic it description of, like, different elements. Sure thing.
**Speaker 1 - 01:08:51**
all right sounds good. All right enjoyed the talk today Artem.
**Speaker 2 - 01:08:56**
Also, one thing. Your background is reversed. You need to check it out.
**Speaker 1 - 01:09:03**
Thank you. Appreciate that. All right cheers man.
**Speaker 2 - 01:09:09**
See you.

