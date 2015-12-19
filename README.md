Building BrooklynJS
===================

[BrooklynJS][brooklynjs] is a monthly JavaScript event that takes place in Brooklyn, New York. From its start in November 2013 until this was written in December 2015, BrooklynJS had showcased 102 speakers and 15 musical guests for thousands of attendees, who along with 45 sponsors helped raise over $36,000. It grew alongside a new community of JavaScripters that has become one of the most vibrant in the world.

This is [my][jedschmidt] story of how BrooklynJS came to be.

Prologue
--------

My BrooklynJS story begins in 10 timezones away in Tokyo, where I was living in 2013. My girlfriend's startup had decided to move their product team to New York City, so we packed up our stuff and moved to Brooklyn.

Though I was a bit sad to leave one of my favorite cities in the world, I was also excited to live in a city where I could hobnob with JavaScript heroes; [John Resig][jeresig] in Park Slope, [Jeremy Ashkenas][jashkenas] in Brooklyn Heights, and [Ryan Dahl][ryah] in Williamsburg.

But by the time I arrived, [Brooklyn's JavaScript meetup][bkjs] had come to an end after [its organizer][marcocarag] moved to Queens (or maybe because they couldn't top a [Brian Leroux][brianleroux] [drinkup][bkjs2013]?), and the [Manhattan equivalent][nycjs], which I had [once attended][nycjs2010] and enjoyed three years prior, had been taken over by a Sencha Touch meetup complete with the ultimate in event code smells, ["webinars"][nycjswebinar].

So aside from a handful of small company-specific events, there wasn't much of a local JavaScript scene in New York. But I knew there was elsewhere; shortly after landing in New York, I started a conference crawl that took me to some amazing events over the summer of 2013:

- [TXJS][txjs], my favorite regional JavaScript conference, run by [noted identity thief][jedjs] [Alex Sexton][slexaxton],
- [JSConf][jsconf], the conference that kicked off the modern JavaScript community as we know it, run by [Chris Williams][voodootikigod],
- [JSConf EU][jsconfeu], JSConf's European cousin, then run by [Malte Ubl][cramforce], [Holger Blank][hblank], and [Jan Lehnardt][janl],
- [RejectJS][rejectjs], JSConf EU's first-born son, run by [Robin Mehner][rmehner], and
- [CSSConf EU][cssconfeu], JSConf EU's little sister, run by [Kristina Schneider][kriesse] and [Michael Pfeiffer][m_p_pfeiffer].

Each one felt a little like two months of summer camp compressed into a weekend, a bunch of edutaining activities interspersed with [jokes][introcss] and [singing][disneyjs]. And when they would end, I'd feel a little sad to return home and leave those distant micro-communities behind. So I decided to find a way to bring the fun back to New York City.

Start
-----

Along my conference travels over the summer, I kept bumping into [Brian J Brennan][brianloveswords], one of Brooklyn's finest humans, who also wanted to bring the feels of a JSConf-type event back home. By 2013, Brian and I had been to a lot of tech events, but only to attend or speak, and not to organize. Since organizing a big conference with the production value of those in the JSConf family seemed like more work than we wanted to take on, we hatched a plan to take the fun of a JSConf event, shrink it down to 8.33333-ish percent of its original size, and spread it across every month of the year. And since Brian and I lived a short walk away from each other, we decided to give our event a local feel and call it _BrooklynJS_. In November of 2013, Brian [registered the domain][icann], and I created [our riff][logo] on Chris William's [JS logo][logojs] and set up [a website][first commit] in the flavor of an [MTA schedule][mta].

Venue
-----

We looked at a few prospective venues, including a bootcamp code school and some startup offices, but settled on the [upstairs room][61upstairs] at [61 Local][61local], a pub in Cobble Hill down the street from my apartment. Though we didn't really know it at the time, choosing 61 Local was one of the best decisions we made. Not only did it help set us apart from the usual tech meetup ambiance of pizza and Coors under fluorescent lights, but it also freed us of the awkwardness of holding an event in a office of a tech company. Companies that host meetups see their role as somewhere between charity, in which venue availability can disappear at the first sign of a hiring freeze or more important event, and opportunism, in which recruiters use their captive audience to foist awkward pitches and boring in-house tech talks.

Having our event in a space unencumbered by the agenda of our host meant that we had more freedom to control the tone and personality of our event, to make it more engaging such as by adding music and comedy. But perhaps more importantly, it also presented a symbiotic relationship in which we bring a diverse crowd of a hundred thirsty developers (as in software, not as in Wall Street, an important distinction in New York City) in exchange for a creative space that we can call our own once a month.

Having a win-win relationship like this was one of the biggest factors in the success of the event. Because our interests were mutually aligned, 61 Local was happy to set aside the space on the same day every month, and would schedule and invoice us accordingly, reducing the busywork of running a meetup in a potentially ephemeral venue. And keeping the event timing predictable in both time (third Thursday of the month) and space (61 Bergen Street) also made it easier for other related events to slot in around us without conflict, and for us to dependably book out-of-town speakers in advance.

More specifically to our setup, 61 Local has been an incredible partner. From [the local CSA][localroots] to [their calendar full of interesting events][61events], you can tell they're wired for community. Get there early enough and you can see laptoppers in the morning give way to parents in the afternoon and then professionals in the evening, enjoying their [rotating roster][drinklocal] of local craft beer, kombucha, and soda.

61 Local's focus on their community has made it easier for us to focus on ours. When their Internet buckled under the load of a hundred nerds, they installed FiOS and a new WiFi endpoint. When their kitchen strained under the load of a hundred mouths, they created a [custom branded menu][61menu] optimized for throughput to keep their kitchen running. So while we often receive complaints that the venue is [too][toosmall1] [small][toosmall2] for the size of the audience we attract, I can't imagine moving. And besides, we'd rather see more events than bigger ones.

Talks
-----

The core of a BrooklynJS event consists of five lightning talks of ten minutes each, preceeded by an intro in which the emcees give some context for the event.

```
+-------+ +====+ +====+ +====+ +====+ +====+
| intro | |talk| |talk| |talk| |talk| |talk|
+-------+ +====+ +====+ +====+ +====+ +====+
```

Talk proposals are entirely open, and take place on GitHub via a pull request, starting the day after the previous month's event. To submit a talk, speakers insert their name and talk title into [our website source][indexhtml], and add a description in the body of the pull request. Two weeks before each month's event (and the day before tickets go on sale), we choose five talks from the outstanding pull requests by merging in [our choices][chosentalks] (and dealing with the inevitable merge conflicts).

Using an open format for talk submissions has worked out well. Having more talks than the average meetup would require more grunt work to curate manually, and we're constantly delighted by the high quality of unexpected proposals from new and returning speakers.

Once in a while we'll exercise a little bit of curation and cajole interesting speakers into submitting, so that the lineup is one we think our attendees will enjoy, but [even JavaScript celebrities need to submit a pull request][eichpr]. For first-time speakers uncomfortable with submitting a public pull request, we also offer out-of-band advice and coaching (via Twitter DM, Slack channel, or in-person) before the pull request, so that there's no risk of getting rejected publicly.

Sometimes we'll try to steer people to topics that are likely to be more successful based on our audience. This usually means keeping things from getting too specific, such as talks on tool A (such as testing) for framework B (such as Angular), which would appeal only to a limited section of attendees.

For talks that are not chosen, we give the speaker a code to buy a reserved ticket to the event anyway. This is by far the most reliable way to get often scarce tickets, and is also a cheap and convenient way for us to increase the number of talks from which to choose.

Social
------

Another one of The Good Parts™ of a JSConf event that we wanted to emulate was the "hallway track", where attendees can interact informally outside of scheduled content. So again we took a cue from Chris Williams, and tacked a [beer.js][beerjs] to the end of our event.

```
+-------+ +----+ +----+ +----+ +----+ +----+ +=========+
| intro | |talk| |talk| |talk| |talk| |talk| | beer.js |
+-------+ +----+ +----+ +----+ +----+ +----+ +=========+
```

Our choice of venue made this easy, as talks take place upstairs from the bar, far enough to be out of earshot but still in the same building. With the usual conference room meetup format, presentations and conversation can only happen in serial, which is unfortunate when many attendees [come for the social][nolanbeverajs].

While we had intended only to give folks an opportunity to mingle after the talks, having a less structured mode of interaction came with other benefits. For example, we were able to avoid the inevitable attendee attrition that takes place at meetups in which attendees post-game at a separate venue. Having a social track also makes it easier for us to accomodate folks that had to stay late at work or couldn't get a ticket but still want to hang out.

We did, however, tweak the "beer.js" brand a little bit to make it our own. Specifically, we took out the "beer". Since the use of alcohol at tech events can be a tricky issue, we wanted to avoid naming our hallway track after it. Also, when it comes to Brooklyn, attendees are just as likely to be avoiding gluten as they are alcohol, and with all the great [kombucha][kb] and [soda][soda] the borough offers, we wanted to be more inclusive.

Thankfully, resident pun expert [Willman Duffy][willmanduffy] [came up][willmanbeverajs] with an amazing JavaScript-specific rebrand: **bevera.js**. It's so clever; I hope it catches on elsewhere.

```
+-------+ +----+ +----+ +----+ +----+ +----+ +===========+
| intro | |talk| |talk| |talk| |talk| |talk| | bevera.js |
+-------+ +----+ +----+ +----+ +----+ +----+ +===========+
```

Music
-----

As any good web developer knows, the best way to keep users engaged is to minimize the time they spend waiting. The same is true of meetups, and critically so for ones with multiple talks straddled by minutes of the awkward dance of getting arbitrary slideshow software on arbitrary laptops to work with the venue's projector setup. In our case, a few minutes of downtime in each of six gaps between blocks could add up around 20 minutes, or two talks worth of time.

To get around this, we tried two technical solutions. The first was to buy a monitor switcher, so that we could plug in two laptops at the same time and switch between them. This didn't work at all due to the cramped space we have for speakers and the latency in having the projector detect each laptop just made things more awkward. The second was to use an Apple TV and have speakers use AirPlay, but this too suffered from poor latency over the network, not to mention requiring Macs to work and allowing only speakers on the device.

So instead of trying to minimize the downtime, we masked it with music. Starting with our second event, each BrooklynJS has featured a musical guest surrounding all five talks with six musical interludes.

```
       + = = = = = = = = = = = = = = = = = = = +
       |          musical interludes           |
+-------+ +----+ +----+ +----+ +----+ +----+ +-----------+
| intro | |talk| |talk| |talk| |talk| |talk| | bevera.js |
+-------+ +----+ +----+ +----+ +----+ +----+ +-----------+
       |                                       |
       + = = = = = = = = = = = = = = = = = = = +
```

This worked out well for reasons beyond just mitigating downtime. Musical interludes give the audience a chance to decompress after the mindblow of hearing speakers try to cram half an hour of content into a 10-minute talk, and give us a chance to surface the hidden talents of developers in our community.

Once our first guinea pig musical guest (my barbershop quartet, [The Four Fives][fourfives]) survived, we then searched for musical talent within our pool of speaker alumni, where we uncovered [Vince Allen][vinceallenvince]'s slide guitar, [Helen Hou Sandí][helenhousandi] and her husband Adrián's keyboard and clarinet duo, and [Mani Nilchiani][mani_art]'s chill acoustic covers. We also cast the net a little wider within the community to find [Thorsten Lorenz][thlorenz]'s jazz guitar, [Adam Sontag][ajpiano]'s Tin Pan Alley keyboard, [Pascal Balthrop][pascalpp]'s eclectic [small-town band][balthropalabama], and [Stephanie Morillo][radiomorillo]'s soulful R&B. And who could forget [John K. Paul][johnkpaul]'s stirring rendition of [I've Been Workin' on a Rails App][railsapp].

As [our budget][budgetjs] grew, we decided to dedicate a small slice of it to also attract other musical acts in the borough. Being in Brooklyn really helped here, as we were able to land some unique acts, including [Bathtub Jen and the Henchmen][bathtubjen], [Bachtopus][bachtopus], [Zac Zinger][zaczinger], [Jess Ledbetter][jessledbetter], and [Toot Sweet][tootsweet]'s Mary Spencer Knapp.

I think adding music to the event was the most effective thing we did to form our own identity. It set the tone of our events apart. BrooklynJS started to feel less like a meetup and more like a variety show.

Coworking
---------

Five months into its existence in March 2014, BrooklynJS had neared its final form, but there was still one more thing to add. Even though we were packing a lively crowd of 100 people into a space designed for 60 all evening, that same space was empty for the rest of the day. So we struck a good deal with 61 Local where we got to use the space for the entire day, and they got to cater our lunch, and created [Boroughgramming][boroughgramming] (not to be confused with [Brogramming][brogrammer]).

```
                             + - - - - - - - - - - - - - - - - - - - +
                             |          musical interludes           |
+===================+ +-------+ +----+ +----+ +----+ +----+ +----+ +-----------+
|  boroughgramming  | | intro | |talk| |talk| |talk| |talk| |talk| | bevera.js |
+===================+ +-------+ +----+ +----+ +----+ +----+ +----+ +-----------+
                             |                                       |
                             + - - - - - - - - - - - - - - - - - - - +
```

Boroughgramming is an all-day coworking session that starts at 10am with bottomless [Oslo Coffee][oslocoffee] and [a catered lunch][bgramminglunch], and ends with the main BrooklynJS event. Attendees bring a laptop and something to work on, and we bring WiFi, outlets, chairs, and tables. We usually take a quick break after lunch to go around the room and talk about what we're working on, and duck out for ice cream at [Van Leeuwen][vanleeuwen] in the afternoon. Usually the crowd is split between folks working remotely and folks working on open source or side projects. It's a great place to swap project advice, since there's a good chance that there's a developer there who's deeper into your platform than you are.

For me, Boroughgramming is where the BrooklynJS community really started to gel. Since attendees are equal parts regulars and first-timers, the vibe is familiar without being stale, comfortable without being clubby. As enjoyable as I find the evening BrooklynJS event, the more relaxed nature of Boroughgramming makes it a better venue to seek project feedback and get honest opinions on new libraries and frameworks.

Sponsors
--------

TODO

Sponsees
--------

TODO

Tickets
-------

TODO

Speakers
--------

TODO

Organizers
----------

Siblings
--------

TODO

[brooklynjs]: http://brooklynjs.com
[jedschmidt]: https://twitter.com/jedschmidt
[jeresig]: https://twitter.com/jeresig
[jashkenas]: https://twitter.com/jashkenas
[ryah]: https://www.quora.com/What-happened-to-Ryan-Dahl
[bkjs]: http://www.meetup.com/Brooklyn-Javascript
[marcocarag]: https://twitter.com/marcocarag
[brianleroux]: https://twitter.com/brianleroux
[bkjs2013]: http://www.meetup.com/Brooklyn-Javascript/events/69811692
[nycjs]: http://www.meetup.com/NYC-JS
[nycjs2010]: https://groups.google.com/forum/#!topic/nycjs/6IaHPoT6WhY
[nycjswebinar]: http://www.meetup.com/NYC-JS/events/220456591
[txjs]: https://2013.texasjavascript.com
[jedjs]: https://slexaxton.github.io/Jed
[slexaxton]: https://twitter.com/slexaxton
[jsconf]: http://2013.jsconf.us
[voodootikigod]: https://twitter.com/voodootikigod
[jsconfeu]: http://2013.jsconf.eu
[cramforce]: https://twitter.com/cramforce
[hblank]: https://twitter.com/hblank
[janl]: https://twitter.com/janl
[rejectjs]: http://2013.rejectjs.org
[rmehner]: https://twitter.com/rmehner
[cssconfeu]: http://2013.cssconf.eu
[kriesse]: https://twitter.com/kriesse
[m_p_pfeiffer]: https://twitter.com/m_p_pfeiffer
[introcss]: https://www.youtube.com/watch?v=KKM71-YeJp8
[disneyjs]: https://www.youtube.com/watch?v=o7OE1uas2yg
[brianloveswords]: https://twitter.com/brianloveswords
[icann]: https://whois.icann.org/en/lookup?name=brooklynjs.com
[first commit]: https://github.com/brooklynjs/brooklynjs.github.io/commit/fea182f8223ea7930d197f02a0f6e0ce0aa0f122
[61upstairs]: http://61local.com/private-events
[61local]: http://www.61local.com
[logo]: https://github.com/brooklynjs/brooklynjs.github.io/blob/master/logo/logo.png
[logojs]: https://github.com/voodootikigod/logo.js
[mta]: http://www.mta.info/schedules
[drinklocal]: http://61local.com/drink
[61menu]: https://twitter.com/61local/status/601119293053476865
[toosmall1]: https://twitter.com/brianvan/status/474922156392849409
[toosmall2]: https://twitter.com/mmwtsn/status/665190033725374464
[indexhtml]: https://github.com/brooklynjs/brooklynjs.github.io/blob/master/index.html
[eichpr]: https://github.com/brooklynjs/brooklynjs.github.io/pull/213
[chosentalks]: https://github.com/brooklynjs/brooklynjs.github.io/issues?q=label%3Aaccepted
[61events]: http://61local.com/events/month
[localroots]: http://localrootsnyc.org
[beerjs]: https://github.com/beerjs/meta
[nolanbeverajs]: https://twitter.com/nolanlawson/status/634579495983423488
[kb]: http://www.kombuchabrooklyn.com
[soda]: http://www.brooklynsodaworks.com
[willmanduffy]: https://twitter.com/willmanduffy
[willmanbeverajs]: https://twitter.com/jedschmidt/status/615595098605232129
[fourfives]: https://www.youtube.com/playlist?list=PLkByX1-Zh4Eu86cuVTwhiLTg2HD0Ci5sb
[thlorenz]: https://twitter.com/thlorenz
[ajpiano]: https://twitter.com/ajpiano
[pascalpp]: https://twitter.com/pascalpp
[radiomorillo]: https://twitter.com/radiomorillo
[vinceallenvince]: https://twitter.com/vinceallenvince
[helenhousandi]: https://twitter.com/helenhousandi
[mani_art]: https://twitter.com/mani_art
[balthropalabama]: https://twitter.com/balthropalabama
[johnkpaul]: https://twitter.com/johnkpaul
[railsapp]: https://www.youtube.com/watch?v=0sgUgqPPxoo
[bathtubjen]: http://www.jenniferharder.com/bathtub.html
[bachtopus]: http://bachtopus.bandcamp.com
[zaczinger]: http://www.zaczingermusic.com
[jessledbetter]: https://jessledbetter.bandcamp.com
[tootsweet]: https://tootsweetmusic.bandcamp.com
[boroughgramming]: https://twitter.com/boroughgramming
[brogrammer]: https://en.wikipedia.org/wiki/Brogrammer
[oslocoffee]: http://www.oslocoffee.com
[bgramminglunch]: https://twitter.com/brooklyn_js/status/578591024076967936
[budgetjs]: https://github.com/brooklynjs/brooklynjs.github.io/blob/master/budget.js
[vanleeuwen]: http://www.vanleeuwenicecream.com/
