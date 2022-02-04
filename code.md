# Code-related things!

[&larr; back to the main log](README.md)

Mostly what's below are code snippets and commands, but I'm starting to include (Feb '22) UI/UX things, as well.

## 04-Feb-2022, Friday, 09:52

From Rob Weychert, [Inside ProPublica's Article Layout Framework](https://www.propublica.org/article/inside-propublicas-article-layout-framework). 

The repetition of multiple viewports as the layout options and desires are describe is useful here; there will always be surprises, but seeing breakpoints in your head as you write code is a skill worth honing.

**Category:** UI, frameworks

## 13-Jan-2022, Thursday, 11:01

In pursuit of exorcising rogue `em` units in our code base, I started just looking for `em;` (in VS Code) which meant having to sort through all the `rem;` results. It's fine, but I went on over to https://regexr.com and built this!

```
([0-9])em+
```

And hit the "Use Regular Expression" option in VS Code. Voilà! 🎉

**Category:** regex

## 05-Aug-2021, Thursday, 15:37

What files are in this `stash`? 

I make _heavy_ use of `git stash save "[message]"` and today while spinning a few plates, I was mixed up about what was in one stash vs. another. But I couldn't remember how to see which files were in a stash, nor what changes I'd made _in_ that stash. So. (

```
to see which files are in the stash:
$ git stash show --name-only stash@{1}

to see the changes in the stash:
$ git stash show -p stash@{4}
```
**Category:** git, stash

## 23-Feb-2021, Tuesday, 09:15

Securely signing git commits!

All my commits for work are signed with my work email address, but when I wanted to update another work-repo with that I didn't copy over the `signingkey` key. 🤦🏽‍♀️ As a result, when I ran `git commit -m "message"` it failed! My first thought was, "oh, copy over the `signingkey`, silly." But then trouble! I second-guessed myself and thought I only needed to restart the machine (b/c I have the authentication set to expire upon restarts). 

Well, that didn't work, of course. Copied over the `signingkey` and… it worked exactly as expected. 

Now, I know!

**Category:** git, gpg

## 11-Sep-2019, Wednesday, 08:25

From Chris:
> I knew about `rake -T` to show the desc string on a task if it exists. I knew about `rake -W` to show the line of code where all tasks are defined (including undocumented ones).
> 
> TIL: `rake -D` will show the entire desc string, even past the first period. So you can do multiline descriptions:

```bash 
$ bin/rake -D cloudinary:delete_doc_batches
Running via Spring preloader in process 49864
rake cloudinary:delete_doc_batches[batch_count,batch_size]
    Delete batches of old fetched Google Docs.
     Optional arguments:
    - batch_count. Number of batches to do. 100 is the default.
    - batch_size. Size of each batch. Default and max is 100. 
                                                             
    To do one batch of the default batch_size:
      rake cloudinary:delete_doc_batches[1]
        To do one batch of 5 documents:
      rake cloudinary:delete_doc_batches[1,5]
        To use the default (100):
      rake cloudinary:delete_doc_batches
```

**Category:** terminal, rake, searching, learning

## 08-Aug-2019, Thursday, 16:10

**Reminder** Finding all the available `rake` tasks in a project:
`bundle exec rake --tasks` (or `-T`)

You can also use a pattern with that flag to find tasks w/ that pattern in them:
`bundle exec rake -T db` for all the db-related ones, for example. 

**Category:** terminal, rake, searching

## 07-Aug-2019, Wednesday, 16:30

A normal `ctrl+c` returned "Gracefully shutting down workers…" except 10 minutes later the sequence hadn't completed. Usually another `ctrl+c` really does it but again: nothing. 

Searched a little and found `ctrl+\` in an answer at StackOverflow: [How to graceful shut down coroutines with Ctrl+C?](https://stackoverflow.com/a/45479734)

That did it! (Got a little dark, though: `[14203] ! Detected parent died, dying`)

**Category:** terminal, local environment

## 10-Jan-2019, Thursday, 10:56

GitHub's web UI doesn't show a commit count, or indeed individual commits over 250 anymore. So, how to find the real count?

```console
$ git rev-list master...HEAD --count
```

Without `master...HEAD`, you'll get back the number of commits from the repo _and_ the branch you're on: useful, but not what I was after in this case. Initially, I was just going to do the math and get the difference between the two, but then @cflipse pointed out the `...` version. 🎉

**Category:** git, github, terminal

## 20-Nov-2018, Tuesday, 15:51

I couldn't remember how to run a single test in an RSPEC file. I found [a StackOverflow answer for adding a RegEx to the command](https://stackoverflow.com/a/6116715) and since the example uses a full spec name, I thought you had to use the full name. But you _don't_! You can add a goofy string to the test name and put _that_ in the command, instead. 

(I am _sure_ I used to be able to use `-n "goofystring"` but that's not working now.)

```rails
bundle exec rspec path/to/file.rb -e "goofystring"
```

**Category:** rspec, tests, rails, console

## 14-Nov-2018, Wednesday, 11:21

Pairing with a coworker and they `git diff`'d against a different _branch_ after committing changes to the working branch. 🤯 I'm forever undoing commits so I can see the `diff`, but now I can try it this way!

```console
# working branch: in-progress
# base branch: master
# make a commit on in-progress
$ git diff master
```

**Category:** console, git

## 07-Nov-2018, Wednesday, 09:57

**Reminder:** to install updated packages, run:

```
# in /app/frontend/
$ yarn install 
# or
$ bundle exec rake frontend:install
```

**Source**: `prettier` got an update but when I grabbed the branch and tried changes locally, nothing happened. I tried running `yarn install` but again: nothing happened. It took a little pulling, but I finally got the critical missing point: that you need to be in `/app/frontend` for `yarn install` to do the thing. (Or "just" run the `rake` command.)

**Category:** package.json, angular

## May 2018

Zebra-striping tables, lists, etc.

```css
.zebrastripe
  > *:nth-child(odd)
    background: $color-row-odd

  > *:nth-child(even)
    background: $color-row-even
 ```
 
**Category:** css

## 12-Apr-2018, Thursday

Give me the last `#` lines of a file (i.e. a log)

```
tail -n 100 log/development.log
```
**Category:** terminal, console, log, searching

## November 2017

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


### 27 November-02 December

* Nope! I was pretty wrong last week with my conclusions about how the `NodeList` was being used and that business about `item`. It hadn't clicked--until this week, watching the _rest_ of the exercises video where Wes walks through the solutions--that the way the chained methods are working is they're taking what all the arrow functions automatically return as their input and declaring variable names for them as they go. 


   I mean, it seems pretty obvious when I say it like that. I understand how chained methods work, but I _wasn't_ thinking of this that way on my first trip through. Oof. 
   
   Well, I learned some stuff then and now. So. 
   
## 26-Jul-2017, Wednesday

Interrogating tests! 

Rails environment, using rspec: spit out objects and things to the console with `puts`:

```ruby
it 'checking a thing' do
puts activity # where activity is the name of an object
puts activity.class
# etc
end
```

**Category:** tests, ruby, rspec, console

## 21-Apr-2017, Friday

git-things

```
git log --name-only --pretty=format: commit1..commit2
```

**Category:** git, log

## 16-Mar-2017, Thursday

Searching for code: 

```
git log -S 'managed_overview_counts' -p
```

`-p` gives you the diff in Terminal (for easier copy/pasting if you need it)

Update: 24-Mar-2017   
**Ack!** I can't believe I forgot about [`ack`](https://beyondgrep.com/install/).

**Category:** git, console, terminal, searching

## 03-Feb-2017, Friday

Can't forget the `bundle exec` when opening a Rails console under `rbenv`: 

```
bundle exec rails c
```

**Category:** rbenv, rails, console

## 2015

Open the branch you're working on in a browser (e.g. for follow-up pull requests, etc.). Got this one from Tom C. during a pairing session. It is awesome. 

```
function open_branch { open http://[github url]/username/`basename \`pwd\``/tree/
$(git symbolic-ref head| sed -e 's/.*\///g'); }
```

(This lives in my `~/.bash_profile`)

**Category:** git, github, terminal, console, tomc

