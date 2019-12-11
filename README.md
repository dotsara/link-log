# Stuff I looked up this month

I look stuff up all the time for lots of different reasons. I'm going to try to keep track of it. 

<!-- dates are Sunday to Saturday -->

## 2019

### December

* "precarity": came up in Jia Tolentio's Guardian article, ["Athleisure, barre and kale: the tyranny of the ideal woman"](https://www.theguardian.com/news/2019/aug/02/athleisure-barre-kale-tyranny-ideal-woman-labour) (2 August 2019), 
   > But today, in an economy defined by precarity,…
   - [From Wikipedia](https://en.wikipedia.org/wiki/Precarity): Precarity is a precarious existence, lacking in predictability, job security, material or psychological welfare. The social class defined by this condition has been termed the _precariat_. 
      * Naturally(!), the word showed up again 2 hours later, this time in Anil Dash's ["'Link in Bio' is a slow knife"](https://anildash.com/2019/12/10/link-in-bio-is-how-they-tried-to-kill-the-web/)
   
   
### November

* "No true Scotsman", an appeal to purity ([Wikipedia entry](https://en.wikipedia.org/wiki/No_true_Scotsman)). Stumbled across it in [a reply to Anil Dash by Jessica Price w/r/t who's labeled as "not real Christians", etc.](https://twitter.com/Delafina777/status/1198769656531570688) and to be fair: I understood it immediately because of the way Jessica used it (hooray for context). The fuller definitions and examples made looking it up worth it. 

### October

* Difference(s) between `.forEach` and `.map` in Javascript. The crucial bit is this: `.forEach` doesn't return anything, `.map` returns a new array. They both let you do something to each item in an array, but only one gives back.
* The difference between postfix and prefix unary operators, specifically incrementing. The [MDN docs on Increment(++)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators#Increment) did the best job explaining it for my brain. 
   - **postfix** returns the value _before_ doing the work
   - **prefix** returns the value _after_ doing the work.
   
### July

* Watching the 2019 Track & Field Outdoor Championships and I think this is the first time I've _watched_ the long-distance events and for the men's 5000m, the runner's started in 2 groups. I found [a little about _how_ these races start](https://www.liveabout.com/olympic-distance-running-rules-3258720#mntl-sc-block_1-0-12) (~65% of the field in one group, the rest in another ahead of them) but not _why_. 🤔

### June

* [The difference between `describe` and `context` in Rspec](http://lmws.net/describe-vs-context-in-rspec) (via coworker)

## 2018


### November

* Why do I suddenly have to enter my SSH password every time I do something in Terminal with git/GitHub?
   - Because in an update to Sierra the default behavior--defaulting to saving passwords in the Keychain--was reversed and now you must turn it on deliberately in the SSH config file. [OpenSSH updates in macOS 10.12.2](https://developer.apple.com/library/archive/technotes/tn2449/_index.html) (via [StackOverflow](https://stackoverflow.com/questions/10032461/git-keeps-asking-me-for-my-ssh-key-passphrase#comment74279267_41576222))

### 22-29 July

* **chondromalacia** Oh! Runner's knee. Ha. Full name: chondromalacia patella. That just rolls right off the tongue, doesn't it. [Info from Cedars-Sinai](https://www.cedars-sinai.edu/Patients/Health-Conditions/Chondromalacia.aspx)
   > The patella is covered with a layer of smooth cartilage, which normally glides across the knee when the joint is bent. 
   >
   > The pain is caused by an irritation of the undersurface or patella of the kneecap as the kneecap rubs against one side of the knee joint, irritating the cartilage surface.
   
   Oof. Just reading that makes my teeth hurt. 
   
### 01-07 July

* I've been watching tennis for a number of years, but I don't know and haven't looked up what the Open Era is.
   - [Britcannica.com : tennis : history, Professional and open tennis](https://www.britannica.com/sports/tennis#ref29707). 
      Ah, so prior to 1968 there just weren't tournaments where professionals and amateurs could compete openly. 
      
      > Although the traditional tournament circuit was avowedly amateur, leading players were paid substantial guarantees “under the table” in addition to expenses. For more than four decades there was discussion of having “open” competition between amateurs and pros to end the hypocrisy of “shamateurism,” but proposals were always defeated by conservative elements within the International Lawn Tennis Federation (ILTF—later the ITF). 


### 13-19 May

* Emails and tweets have been flying around about the [General Data Protection Regulation (GDPR)](https://www.eugdpr.org/) going into effect on 25 May 2018, so it's time to read up.
   - Official site: https://eugpdr.org
      * Ooooooh: 
         > Arguably the biggest change to the regulatory landscape of data privacy comes with the extended jurisdiction of the GDPR, as it applies to all companies processing the personal data of data subjects residing in the Union, regardless of the company’s location. 
   - [What is GDPR, and why should designers care?](https://www.fastcodesign.com/90171699/what-is-gdpr-and-why-should-designers-care) (via [@jgarber](https://twitter.com/jgarber/status/997158084463267846))
   - [Wikipedia's GDPR entry](https://en.wikipedia.org/wiki/General_Data_Protection_Regulation)
   
### 04-10 February

* My friend [Tiff](https://twitter.com/tifferh) has a tradition of keeping us updated on the comings and goings of the booze cruise and cruise ship traffic when she's with her family in Mexico. 
   - [staysails](https://en.wikipedia.org/wiki/Staysail)
   - mizzencourse: the lowest sail on the [mizzenmast](https://en.wiktionary.org/wiki/mizzenmast) (obviously!) 
* segfaults, or [segmentation faults](https://en.wikipedia.org/wiki/Segmentation_fault), or When Things Go Terribly Wrong


   I hang out in our `#tech-ops` channel at work because tech ops is not my purview, but Ben always provides lots of detail for historical record which turns out to be super useful for someone like me who likes to look things up. 🤓
   
## 2017

### 27 November-02 December

* Nope! I was pretty wrong last week with my conclusions about how the `NodeList` was being used and that business about `item`. It hadn't clicked--until this week, watching the _rest_ of the exercises video where Wes walks through the solutions--that the way the chained methods are working is they're taking what all the arrow functions automatically return as their input and declaring variable names for them as they go. 


   I mean, it seems pretty obvious when I say it like that. I understand how chained methods work, but I _wasn't_ thinking of this that way on my first trip through. Oof. 
   
   Well, I learned some stuff then and now. So. 


### 20-26 November

* I'm working through the [ES6 for Everyone](https://github.com/wesbos/es6.io) course and in the answer file for the first exercise, it shows `Array.from(document.querySelectorAll('[data-time]'));`
   - first up, `Array.from`--I think this might be the first time I'm seeing it? From MDN: "[The `Array.from()` method creates a new `Array` instance from an array-like or iterable object.](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/from)). Cool! pass it a thing, get an array. Got it. 
      * interestingly, my first pass at the same line was: `const videos = document.getElementsByTagName('li');` hilariously (to me), both return the exact same array-of-objects. Ha!
   - next up… all the stuff available to `document`. I… I just don't know all these off the top of my head. We've been using [RubyMine](https://www.jetbrains.com/ruby/) at work, lately, and with all the hinting things turned on it's much less painful to find what's available, I like it. That said, I haven't seen `querySelectorAll` before!
      * Oohhhh, so my version and the answer version aren't, in fact, returning the same array of objects. They just _look_ the same in Chrome's console. What the answer is returning is a `NodeList` ([MDN details](https://developer.mozilla.org/en-US/docs/Web/API/NodeList)) and _actually_! seeing that `item` is a thing that you get with a `NodeList` helps me understand code further down in the answer file where it's using `item`.
         - I was super confused about the use of `item` because it hadn't been defined or instantiated and it looked like the singular thing you'd use in a loop, but where it's used doesn't _look_ like a loop *and* the thing (`const`) we're working on is called `items`. So 🤔. But now I think I got it. Woo!
      * So I see why you'd use what's in the answer file: because you want what's available to a `NodeList`. Cool. 
      * [Using querySelector on Elements](https://developer.rackspace.com/blog/using-querySelector-on-elements/): I'm… probably going to have to read that & mess around with it a few times. 
   - oh, also, I was wondering about where `item.dataset` comes from, but `data` set is just the collection of `data-` prefixed attributes on elements. Neat! I didn't realize they would get rolled up that way, but that's handy.
  
### 13-19 November

* My contribution to Friendsgiving on Thursday next is applesauce ([my favorite thing to make](https://www.americastestkitchen.com/recipes/364-simple-applesauce)) and a cocktail and _obviously_ I'm going to choose a gin cocktail and surprising precisely no one my first thought was: a French 75! 💕
   - [Behind the Drink: the French 75](https://www.liquor.com/articles/behind-the-drink-the-french-75/)
      * naturally, almost every recipe I've found today has slightly different amounts of each ingredient.
   - I'm also thinking I'll "just" go with a [Bowie Knife](http://playboysfw.kinja.com/bowie-knife-a-pink-cocktail-for-all-you-manly-men-1532819388): partly because most people don't know it and partly because there's just 1 version of the recipe (from _Playboy_ of all places). 👩🏽‍🔬

### 06-12 November

* I've got a plan to make candles this season and I've noticed the trend toward (a) wooden wicks and (b) actively pointing out the use of soy wax, so… I'm reading up:
   - I admit I didn't realize paraffin is / can be [petroleum-based](https://en.wikipedia.org/wiki/Paraffin_wax)
   - Are paraffin wax candles dangerous? (apart from the fire hazard, that is)
   
      This [CNN article from 2009](http://www.cnn.com/2009/HEALTH/08/21/candles.air.pollution/index.html?_s=PM:HEALTH) is the most balanced take I've found so far. Balanced because it cites a [South Carolina State University study](https://www.scsu.edu/news_article.aspx?news_id=832) and doesn't hide or downplay that (a) there's still _some_ debate (as ever) and (b) it is possible to mitigate the accumulation of the unwanted chemicals.
* In reading that SCSU study, the following made me curious:

   > Massoudi’s research stems from a desire to address a possible public health concern, boost the American agricultural economy and promote sustainability.
   
   > The candles emissions study is funded by 1890 Research & Extension, a federal and state funded program that helps ensure SC State achieves its land-grant mission of improving the lives of limited resource individuals, families and communities through research, teaching and service.
   - Background on [the 1890 Research and Extension Program](http://www.scsu.edu/1890/1890background.aspx)
   - A little more [detail about the Second Morrill Act of 1890](https://en.wikipedia.org/wiki/Morrill_Land-Grant_Acts#Expansion), particularly aimed at the former Confederate states. "This act required each state to show that race was not an admissions criterion, or else to designate a separate land-grant institution for persons of color." I think I can be forgiven for being deeply sketpical on _this_ point at _that_ point in history, _however_. SCSU is an HBCU, so.
   
### 23-29 October

* Why do we (Americans, anyway) pronouce "reveille" as "REH-va-lee"? Every time I see it, I hear it (in my head) the French way (guttural _r_ and all) and it takes a beat to remember the other way.
   - [Oxford English Dictionary entry for _reveille_ (n)](http://www.oed.com.ezproxy.spl.org/view/Entry/164685?redirectedFrom=reveille#eid)
   - [How to pronounce "reveille" in UK & US English](http://dictionary.cambridge.org/us/pronunciation/english/reveille)
   - Conclusion: After 5 minutes' research, I've no idea why we say it the way we do outside the way pronounciations in US English migrate away from British English. (I like the UK version! "re-VELL-ee")

### 09-15 October

* Scylla & Charybdis: you'd think as a lit major (and a fan of the _Percy Jackson_ series!) these wouldn't be names I'd have to look up, but here we are, friends; here we are. So, today we learned that they're both sea monsters, [one on the rocks](http://www.theoi.com/Pontios/Skylla.html) (Scylla) and [one with a whirlpool](http://www.theoi.com/Pontios/Kharybdis.html) (Charybdis), and they stayed across from each other.
   - what prompted me to look them up is this from _What Works for Women at Work_ by Joan C. Williams and Rachel Dempsey:
   
      > "Savvy is a threshold requirement for women. We have to be astute enough to tack back and forth, navigating between the Scylla of being "too feminine" (and so liked but not respected) and the Charybdis of being "too masculine" (and so respected but not liked)."
      
      
### 02-08 October

* "aguanile": started listening to the [For Puerto Rico Por Puerto Rico](https://open.spotify.com/user/spotify/playlist/37i9dQZF1DWVJYaFlGP5hP?si=c1mrxq3l) and had _no_ idea what the title of the Marc Anthony song, "Aguanile" meant (I mean, I _did_ know it's not pronounced "a-gwa-nyull", heh). Anyhow, I found what seems to be [a pretty good answer at spanishdict.com](http://www.spanishdict.com/answers/111008/from-the-marc-anthony-song-aguanile-word-im-asking-about-is-aguanile). Neato!

   
### 25 September-01 October

* Who in the world would ban _Green Eggs and Ham_!?

   Oh, China did it: [Banned Books Week: Green Eggs and Ham](https://www.nypl.org/blog/2013/09/24/banned-books-week-green-eggs-and-ham)
* What _is_ happening when your ears "pop"? 

   A-ha! [Pressure equalization](https://gizmodo.com/why-your-ears-pop-and-what-to-do-if-they-dont-505598950), that makes sense.
   
### 04-10 September

* [HTTP Status Codes](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status): you might think after so many years making my living via the Internet I know these by heart, but you would be _wrong_, friendo!
   - [favorite code: `418: I'm a teapot`](https://tools.ietf.org/html/rfc2324)
   
      > Any attempt to brew coffee with a teapot should result in the error code "418 I'm a teapot". The resulting entity body MAY be short and stout.


### 28 August-03 September

_Cross-country season is back in full-swing, so my available brain power to remember to look up random things is rather diminished._

* **starboard**, _n._ I know _that_ it's the right side (facing forward) of a ship, but I was always forgetting to look up the why.

   > This side of the ship was so called with reference to the single side rudders used in early Germanic ships, which were typically suspended on the right side of the vessel (for comfortable use by a right-handed helmsman).
   From the _Oxford English Dictionary_.


### 21-27 August

_A bit of a light week because cross-country season started and now occupies a significant portion of my brain_

* [portage](https://www.merriam-webster.com/dictionary/portage): _noun_ "the carrying of boats or goods overland from one body of water to another or around an obstacle (such as a rapids)" [Lori's post about an upcoming trip](https://www.instagram.com/p/BYJbDfOHsXf/?taken-by=theoriginal10cent) got me to look it up because I've never heard it in this context before. Neato! (We have Portage Bay in Seattle, but I never looked it up!) 🚣‍♀️

### 14-20 August

* I was telling [Jason](@jgarber623) about the occasional game of 6 Degrees of [Ciarán Hinds](http://www.imdb.com/name/nm0001354/) that @tiffehr and I sometimes play. And he challenged me to go from Hinds to… **Carrot Top**. Honestly, I wasn't sure I'd be able to do it. But 5 minutes later… 😎

   Carrot Top _The Aristocrats_ > Chris Rock _The Fresh Prince of Bel Air_ > Will Smith _Wild, Wild West_ > Kenneth Branagh _half the movies in his career_ > Emma Thompson _Harry Potter & the Deathly Hallows_ > Ciarán Hinds
   
   💥
   
   
### 07–13 August

* Welsh pronunciation guides: I'm knee-deep into the second season of [_Hinterland_](http://www.bbc.co.uk/programmes/b03sgfbz) and decided to look up a guide to help with the signs in the show. (I've heard Caernarfon pronounced tons of times on [_Secrets of Great British Castles_ ](https://www.netflix.com/title/80095866) and but it takes a couple of seconds for my brain to spin up. Every time.)
   - [Pronouncing Welsh Place Names …and their meaning](http://www.cyclingwales.co.uk/welsh.html) (Ha! "coed cwmglas" was in an episode I watched last night)
   - [A guide to Welsh pronunciation](http://www.go4awalk.com/fell-facts/welsh-language-pronunciation.php)
   
---

* cleaning silver… I know _that_ you can clean silver jewelry with tin foil, boiling water, and baking soda, but almost none of the articles & blog posts touting the technique explain why. 😩 Philadelphia Museum of Art to the rescue! [Hands-Free Silver "Polishing"](http://www.philamuseum.org/booklets/7_44_85_1.html?page=2)

   It's an electrochemical reaction doing the heavy lifting. The baking soda makes it easier for electrons to move between the silver & aluminum and the aluminum reduces the silver sufide (tarnish) back to silver and produces aluminum sulfide in the process. Why boiling water? Makes the whole process go faster! Nifty.

* _permille_ ‰: I don't know how I've been a type nerd this long and never come across the permille, or indeed thought harder about the components of the word "per-_cent_" :flushed: Of course it only has one 0 in the divisor! Oy.

   Came across it in [The Loveliest Living Fossil](https://www.typography.com/blog/the-loveliest-living-fossil) by Jonathan Hoefler.
* [Monument to the Third International (Tatlin's Tower)](https://en.wikipedia.org/wiki/Tatlin%27s_Tower): listening to an episode of [No Such Thing as a Fish](http://qi.com/podcast), this tower came up and I couldn't remember ever hearing about it or having seen it. The hosts on NSTAAF remarked on its double-helix design predating the discovery of DNA's structure by several decades, but what I find interesting is [this discussion about spirals](https://thecharnelhouse.org/2015/03/24/tatlins-tower/) and how they relate to/function as a metaphor for the repetition of capitalism. Huh! 

---

* _Boricua_: a Puerto Rican, especially one living in the United States. 
   Listening to [Code Switch](http://www.npr.org/sections/codeswitch/2017/07/26/539368829/stretch-bobbito-on-race-hip-hop-and-belonging) last weekend, Bobbito reminded me I've heard this word a bunch of times (like in the middle of ["Jenny from the Block"](https://www.youtube.com/watch?v=dly6p4Fu5TE#t=3m5s)!) and always forget to look it up, but this time I remembered!
   
   Mystery solved! (:
   
--- 
   
* I always mix up which type of soil produces blue and pink hydrangeas, [Farmer's Almanac to the rescue](https://www.almanac.com/plant/hydrangea)! Low pH below 5.5 (acidic): blue; higher pH over 5.5 (more base): pink. (White flowered hydrangeas aren't affected by the soil's pH.)


### 31 July–04 August

* Subaru's "pzev" badge on their vehicles (was behind one this morning on the way to work). Ah, "partial zero emissions vehicle".
   - [What is a PZEV?](https://www.thoughtco.com/pzev-partial-zero-emissions-vehicle-85335)
   
      > PZEVs run on gasoline, yet offer extremely clean emissions with zero evaporative emissions.
   - Origin story: California's zero emission vehicles mandate, PZEVs are a compromise (and hard to type correctly).
   - Heh, one of the other sources I found was mostly a huffy rant about the California Air Resources Board, sooo no link for them.

---

* [HTMLHint](https://github.com/yaniswang/HTMLHint/wiki/About): saw it in a commit for a big upcoming project.
   - That about statement is… it could be better, but I like the way they're using the repo's wiki for the documentation. 👍
* [Transpiling ES6](https://css-tricks.com/transpiling-es6/): ran through their Babel section just to see how it does things.
   - We end up in such weird places with the names of related / similar tools: Gulp, Brocoli, Brunch. Honestly.
* [**heteroglossia**](https://en.wikipedia.org/wiki/Heteroglossia) from the phrase "a heteroglossic wonderland" (which goes straight on to [the band name list](https://github.com/dotsara/is-the-name/blob/master/README.md)).

   The intro on this isn't as good as it could be, but I think this bit in the first section gets at the meat in heteroglossia (and provides support for the relationship to code switching):
   
   > Extending his argument, Bakhtin proposes that all languages represent a distinct point of view on the world, characterized by its own meaning and values. In this view, language is "shot through with intentions and accents" (1981: 324), and thus there are no neutral words. Even the most unremarkable statement possesses a taste, whether of a profession, a party, a generation, a place or a time. To Bakhtin, words do not exist until they are spoken, and that moment they are printed with the signature of the speaker.
   >
   > Bakhtin identifies the act of speech, or of writing, as a literary-verbal performance, one that requires speakers or authors to take a position, even if only by choosing the dialect in which they will speak.

---

* Google search: "github markdown code wrap"
   I've always hated that code blocks in Markdown with long lines scroll out of view; occasionally, I'll break them manually, but sometimes I'm saving code that I don't understand, so I'd rather _not_. Anyway, apparently it's not a thing. 🙄 Well, it's a thing with a browser extension, but it's not a built-in thing, yet.
   * [how to line wrap long lines inside markdown code blocks in github & gitlab issues? (StackOverflow)](https://stackoverflow.com/questions/41238148/how-to-line-wrap-long-lines-inside-markdown-code-blocks-in-githubgitlab)
   * [github-pre-utility](https://github.com/yoheimuta/github-pre-utility)
* ⬆️ related! [linguist `languages.yml`](https://github.com/github/linguist/blob/master/lib/linguist/languages.yml): GitHub uses Linguist to detect languages & do the syntax highlighting, this is the list of which keywords are valid. 

---

* **proprioception**: "…is the sense of the relative position of one's own parts of the body and strength of effort being employed in movement" ([Wikipedia](https://en.wikipedia.org/wiki/Proprioception)), from [Digging Deeper: Stretching](https://www.elitefts.com/education/rehab-recovery/digging-deeper-stretching/)
* `pushInsteadOf`, `insteadOf` in a coworker's `~/.gitconfig`: https://git-scm.com/docs/git-config#git-config-urlltbasegtinsteadOf
   - I'm not sure I interact with open-source repos often enough for this to be useful for me, but still, nifty.
   
--- 

* Is Donkey Kong a gorilla…? Turns out, no, an [ape-like creature](https://en.m.wikipedia.org/wiki/Donkey_Kong)
