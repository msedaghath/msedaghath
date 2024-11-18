---
title: "transcribe"
---
Summarize notes from my last meeting with my supervisors : " I can let it run and you can later. I have it with my notes. What did you use from Microsoft? This is just notes from the Apple. And it gives the transcribe automatically. But maybe one thing, how you can organize it is from the task they are doing or what they are used for. The other thing is where they are running on. Maybe this. What we do as a collect system is because we try to collect everything together in one piece of software. In our case, this would be OctoPrint. And OctoPrint is getting all these sensor signals? Yes. Because OctoPrint is running on a Raspberry Pi 4. And with Serial, it is getting everything layer by layer, and it sends the G code and moderates it. And the sensor is connected to this Raspberry? Yes. Yes. And how is Octoprint connected to everything? Yeah. We have, for example, we have a we have a committee detection in our drying boxes for each print filament that we have. And they are connected by eTool to the to the Raspberry system. But these data, they are all always connected to one certain printer, or? I tried to have a graph for it, like how it is working and how the data is collected. So after the 3D printing, this would be the view of a controlled data connection monitoring and then different machine learnings that are working. This is not important. This is just a cleaning note I wrote. And I just had for the collection... Obsidian. cleaning note I wrote. And I just had, like, for the collection. Obsidian. Yes, obsidian. And from the framework, we can collect the data or the OctoPrint. And I have some data on OctoPrint. But everything I wrote was, like, dividing them into different, like, temperature, bed, or nozzle. And then nozzle position and the axis and the movement of the handles. And then the camera fit. For controlling, I didn't have. But we we have no okay Milad already did this so but but like do you have everything and no no no I don't have everything and there are lots of things missing and this is mostly from the paper we were writing so I gathered what data it was important but they did also acoustic yes that's the thing there are external sensors that they use so emission uh acoustic sensor was as an external that you can install temperature what type of temperature we have at least four yes one is okay every single temperature you can get so but then you have additional systems. But I have a problem. I'm sorry. If you are gathering the temperature outside of the 3D printer, then it is not a fixed temperature. We can have the room temperature, but it is not such a solid data. The room is big, the temperature is there. You will have to do this with every single signal. If there comes an additional signal, but you will have to do this with every single signal. If there comes an additional signal, then it needs to be added. So, yeah, and then you have to say, okay, this one is just for this room, because maybe you can just learn something for this certain setup. Okay. For this printer. Okay. So, actually what you need. And it is with every printer. You can, you can, you will need metadata, so data about the data. So you will need a database who is describing you every sensor and where he's positioned and what is he doing and what is his resolution, what is his measurement uncertainties. Sure, you need something like a tag that you put on it and say, oh, you're a measuring system from, let's say, NI, and I have a quality of, let's say, 10 hertz or 10 kilohertz or whatever. And this should be organized also in a database because these are commercial devices you are buying and you don't have to write it down again and again and again. You just have to link it to the right device. Yeah, the thing what we are doing here is because we are building our print systems ourselves, we don't want to have a lot of... Yeah, but... Then you have a new instant office, but maybe you build the system two times or three times or four times. Yeah, something like that. So it's better to organize it in this way because some devices, maybe a temperature sensor will occur a couple of times. Yeah, that's true. This one, that's why it's maybe better to organize it this way. So you have temperature, you have vibrations? Vibrations, the printer printer printing vibrations. What? The printer has a vibration sensor. That's the reason why I said we have to have something for the printer. We have temperature in certain ways 1, 2, 3, at least 3 temperature sensors that we have. We have vibration R in X, Z and Y direction we have that. We have positioning sensor. Let's say it's S and X, Y and Z. And this don't have to be complete in your task. You just have to do a couple of them and then you have to show how to integrate a new one. Yeah, so because obviously you can't get everything everybody used 100 years ago. No, but I just want to show you what we are in the moment trying to build if we build a new system. This is something we will have. Because except for the acoustic stuff, because it's always a bad thing. We would like to have it on the system to have, for example, pre-maintainance problems. But you can get the same information about fending ball rings, bearings. We can have that over the detection of the acceleration and the currency, especially at the moment let's say for the Z-direction. Yeah, but we will set up this database and then we can calculate even how big our requirements for storage is. We have here the currency for the motors, motors, all motors, that means we have... Currency and voltage, or? Voltage too, sure. We have that for these directions, We have that for the extruder. Extrude, we have this for. These are the positions. These are the positions. This is acceleration. This is position. The nozzle? Yes. Nozzle. Nozzle. Nozzle. Nozzle. Nozzle, yeah. Wow. You're not very good. You're not just very good in LLMs, you're also very good at printers. So basically we have this printer intern sensor rig, and we have this out... This intern... and basically, but you could say everything else, i.e. "



We can connect them and they are all.

  

O more or less anotherocol for.

  

Exchanging sense of information Basically.

  

It makes things easier.

  

I I don't I don't know maybe no, but maybe this is one maybe if I if this is good this is a good way to organize this now I guess it's not I guess it's not because it is too much.

  

What is for Sw printing it's a standard at all.

  

For organizing data, for for organizing data in in manufacturing processes, for example.

  

Yeah, but maybe I would you have another one, you could take MQTT.

  

We would use thatQTT.

  

That's what we use normally.

  

So you have to think about protocols.

  

This one is a different issue.

  

I that's that part of I am good, that part I'm good.

  

For you, we think about, we do it normally in a way that we say we have a job.

  

We have a job, Job means we print a part.

  

It's a job.

  

All these things have a certain lap and time that goes into these job.

  

So we have a job that will be stored with a CID model maybe in addition to the G code, um and then we store all the stuff we need together into this it is this container.

  

The container that we would like to use the moment it's just an idea that we are talking about because we want to build a print system, so we need to store this data anyway.

  

And our idea would to use that CDF.

  

This is a framework for restoring whatever.

  

And it's huge, you can store about a param or even more, but it's it's also something like the photocol.

  

It's a database.

  

A set of software libraries and square machine and independent data form as support creation access and sharing area oriented scientific data..

  

This one is good.

  

Transportation so basically you have to plate somewhere and then you have to have to get the way.

  

This there's also belongs to the drop raw.

  

You can't define it, or you could say you could you could you could say um obviously a job is finished when the plate is out of the box because then it's ready for a new job.

  

And you can say the job starts, starts at the same moment the play is ready to go and the system says you are done.

  

So you could so you could say you to put the the job and then that's how it works.

  

Exactly.

  

This is more octoprint does octoprint is basically the system for us that container that controls all the stuff that does and go off drops.

  

And does drop one job one, then we have to do things in between.

  

Logistics, we say.

  

So in the video step, logistic in our case in this loggistic, then we will prepare for the next.

  

This is part of the job.

  

There's part of the job part of the job.

  

This preparation like how did you play and couldn't look if it's clean.

  

It's target logistics.

  

You see, it's it's not completely down.

  

Maybe Maybe I should do it like that.

  

Uh, and we have to do it after it, and we have to do it before. .

  

So, maybe it have an inspection or something like this?

  

We have an inspection.

  

Sure.

  

That that's part of the of the of the post job, that's say cost.

  

I I missed that part.

  

And now we have preparation done, we can go to drop too.

  

Then we would have this whole job whatever it is, then we have logistics, and then we have preparation for the next, and in it like that.

  

And the thing is that's just for printer one .

  

Printer A. But we have printer B, for example, too.

  

And there isnected somehow.

  

And this is something up to print also needs to do.

  

It has a we have to prepare horstics.

  

O is this?

  

Organizing it for scheduling it?

  

It octop is also capable of triggering?

  

Yes, it can do that.

  

Then maybe occ a right system, here for doing everything extended by plan to do that, but it's capable of we have to look up a couple of dimensions.

  

Dimension to have process all the other stuff done in in in the process visions that the process vision and the data, or is third one is maybe the problem vision.

  

No, you need a problem to solve, of course.

  

I have a question until now, I'll the papers I was looking so they were around the RNN CNN detecting they t or I had the system to connect with the multiple printers and get the print history and logs and it can also control and start the jobs on the different printers at the same time.

  

But since the last week I'm working a little bit more around the idea of LLMs on how they work, actually, because they are from the companies was promised to me that we are gonna cooperate with Ziemens in airlineen to have their industrial copilot, that is, the new Olympic.

  

Is the Microsoft system from for semens I know.

  

Yes, yes.

  

So they wanted to give us the access then we can feed the data from the printers to them and then they take something.

  

But they said it is not ready..

  

I mean, it's it's still in the in the doing .

  

But uh since the last paper, so I'm I just want to know if uh should I focus on yes, uh something like this, like in like the data would be correlated and somehow, like LLM three different large language models to monitor and control three different things.

  

But yeah I guess I guess I should not hear about the where I'm sending the data.

  

Because you can treat them all the same, because if you do if you different things.

  

It's not because no like this one is okay or not just supervised, then you can you can do like you can organize the data or you can maybe do en detection or something like this.

  

The second thing is, you do supervised learning , then usually you have to you have an organ something which is labeling the data.

  

Exactly.

  

So should should I look to this foreign like uh to provide learning or should I look at the other for zero shots?

  

To parameters and maybe you could say, okay, I will use this information.

  

I want to use this this this information and then provide, maybe the next I for the next step, but I can this is not true, and so we don't what kind of we have.

  

So if I want to go simple, I can say we can have just a labend data from what we are collecting.

  

So all the data that we are collecting besides, we would just label it as the print was successful or unsuccessful.

  

We don't provide the percent or how they would accuracy or any provide for the neighbor or you a spot for a lot of labels, we want to labels, you don't even know how you want to label.

  

Bin but also it can be it can also that it's not only one state.

  

There's a couple of states.

  

A of classes at the same time.

  

So there can be two defects at the same time, you?

  

It can have a deviation?

  

And it has spaghetical at the same time...

  

So this one would be multiclass, multilabeled.

  

We don't know you have to you in the database needs needs to be capable of doing to like this..

  

So and some so maybe you have or you want to take as words, maybe you want to do a visual description that somebody is saying um if there are a whole mouse that text is just like it's just like you have a language and then they are trying to like get this one out or like you have a human observer who's who's just who's just like giving a text for the quality and maybe we want to do I don't know, but is it going with?

  

So, I I would just simplify.

  

The first word we talked about, we talked I think once a around the.

  

So we want the we need the framework as the title we selected for the paper, we can just go with the framework.

  

It is a framework, we will collect the data, we will connect to the printers, we will collect the data any kind of data, and we will prefer a data set.

  

And then you can be generic because this data collection generic and what do because you about protocols or data and stuff like this, and you can do at the end one example, then you show maybe how you on one example of where you prove how you can use this for a machine and you do something very easy.

  

So extract the pictures and detector an, you know, detectector or something like this.

  

So this is a thing there.

  

We are building a framework, a tool kit to collect the data, so generally completely then we we can select what are the kind of the data and everything, but the important is like, it iseneric.

  

We can have access to the external internal sensors and everything at the same time. , you could start collect all the.

  

Sure, because we could start, you know, you know, thereoprint, I don't know if there's an aut for it, I don't you can say what you prefer.

  

But is it reallyeneric?

  

Is it just working for or is it working for That's what I so octopri is basically good until the commercial like bamb lab gives access also, but it doesn't give the food API suggest about how generic is your is I understand this problem is that, for example, maker doesn't give you anything.

  

It just says, I'm a printer, I take parts or a code and that's it.

  

And the rest is fine for you.

  

In research,za is one research printer and it's but this is your decision, you can say it's it's just generic, but we have to use we have to use octopel.

  

This one is okay.

  

Use because otherwise we don't get all this information.

  

Frame is one thing.

  

I did this.

  

I searched in thecholar, how many papers there ever about like using Perza and it is around 8000 that there are using it anything else I research, I said Bambola search and nant nant, what is it?

  

One that burns a lot to get some but like now you have you have a different things you think about.

  

Think about standards.

  

You are using you obviously you you're thinking about this pen.ization of the data.

  

Maybe this container idea that's.

  

This is like container idea.

  

So he has star nuts, then maybe you you can talk about problems.

  

So it this one anability detection and so on.

  

Time serious prediction , um classification, um control, optimization.

  

So things like this, but you don't have to speak about them, you just you just no this one is John picked up data.

  

Give the last minute is the will be very, very huge on.

  

And we have all these things together.

  

Octoprint can do this as a second printainer, saying, least I have some information about the logistics, and priest stuff and all the stuff that can have also influence to your job quality .

  

But the main stuff you have is in job.

  

And so you have an organization into jobs.

  

It's a jobs are generic in that case that they are natural ended and started by what they are.

  

And the next step is, because the next person comes if the economics come and then they say, I don't this one, because this one, you can't use a printer.

  

And then put them at the end is something we do an after and we are already thought about how to do at aristics starting that can do job selection and can do in the same time if preparation and slicing for each printer that is capable of doing the job.

  

The problem that it is not optimization of the single printing process.

  

Optimization of the whole workflop of the air of truck flow or how energy flow or how you what you call it.

  

This one is also possible.

  

But but this this this is just a sequence,inery because it's you have this one um a data of kind a kind data of, then you on the relation of natural thing.

  

There is the natural scale for all this stuff that has a has a scale scale here is time.

  

So much cool things because you could take information, what is here and compress it to a like like like you do you can read a book I can read a book and the whole sentence of the whole book.

  

I can formulate as a back.

  

This is what and this vector 81 or 90 dimensions.

  

It could be more as a professor about this like exactly working on the multi dimensional det on how is it like if I want to collect the data, from Manitoba.

  

So I'm in contact with him, he said that I can maybe help you to have good structure for the victor that you want to provide as a data.

  

Data and we presentation to find a number and maybe or multimensional room and data, a picture transfer to a place somewhere here in in the room, just a number, and then we have a different number and then we can have a differentances and then we can identify problems, and then we can understand what you and but it's not what we are thinking about now and and this is a certain time, and we can do this, and this and this, then we can organize it and then we can do intelligence with this. But this is just . It's. 

  

