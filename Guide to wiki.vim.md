# Guide to wiki.vim

DE *wiki-intro-guide*

LAST UPDATED: 2023-03-01
The following guide is more or less an essay on how I personally use
`wiki.vim` for structuring and writing my notes. I take the liberty of writing
in the first tense, as this is clearly a subjective matter. An initial version
of this was posted as a comment in an issue thread [0] (note: the links are
listed at the bottom). I recommend anyone interested to read the entire thread
(although it is quite long!).

I've structured the following guide in two main sections. The first section
concerns how to keep a personal wiki or knowledge base. In the second,
I explain how I keep my daily journal. But first, a quote that I think
captures the most important concept in a single sentence (by @mgoral [1]):

> I think that the most important thing is to not overthink things and just
> > keep writing stuff down.
>
> Executive summary ~
> - Speed is key - make sure you have a fast workflow:
>   - Use a keyboard shortcut in your desktop/window manager to open Vim/neovim
>       with the wiki index (e.g. <alt-n>).
>         - Use something like |:WikiPages| and `ripgrep` (with e.g.
>             `ctrlsf.vim` [2]) for searching.
>             - Write short pages and use links between related pages.
>             - Don't obsess about the wiki structure.
>
>             A personal wiki ~
>             People write things down. Take notes. Why? Because people, or at
least most of
us, don't remember things for too long. From my point of view, taking notes
is a way to extend my memory. And writing the notes is itself a useful
process, because it often helps both to learn and to remember things.

I find the idea of keeping my notes linked and easily searchable in pure text
to be extremely potent. With `wiki.vim`, I can very quickly locate relevant
notes for a topic. I believe strongly that speed or efficiency is the key
aspect of a good personal-knowledge system. However, before I continue, I want
to stress that `wiki.vim` is just one such system. There are probably
countless, and I encourage everyone to find a system that works for them. Some
alternatives are listed under |wiki-intro-alternatives|.

So, some context: My personal wiki consists per 2023-03-01 of 2728 pages with
a total of 96969 lines (excluding my journal). I first started taking notes in
2007, so this is perhaps 16 years' worth of writing. I use Syncthing [3] to
keep my notes synchronized across my computers, phones, and tablets. I've
previously also used Dropbox.

Needless to say, it is important to be able to find relevant notes fast.
I have a global Vim mapping `<leader>ow` to open a page search interface.
I previously used |:WikiPages|, which works very well! Today, though, I use
Telescope [4] with a personal function to list wiki files [5]. It usually
takes no more than a couple of seconds from the moment I think of something
until I have opened the relevant note. A key here is to use simple names for
the pages. I prefer several short pages instead of one long, if possible.
I also don't worry about using spaces in my wiki file names.

Sometimes I search for things within pages. For this, I rely on `ripgrep` [6].
I use `ctrlsf.vim` [2] (which uses `ripgrep` as a backend). I map this to
`<leader>ff`. This makes it very easy and fast to search the wiki. And if my
search has too many hits, I can either narrow it down by changing the search
pattern, or I can search within the result buffer of `ctrlsf.vim`. This has
generally not failed me in finding information I'm looking for. I don't spend
a lot of time searching for things. If I know I've written about something,
I always find it with `<leader>ow` and/or `<leader>ff`, and usually in
a matter of seconds.

How do I write my notes? I make sure to write down what I feel like at the
moment. I then clean it up and rinse/repeat as something is developing. I add
links to relevant external and internal pages/resources. I often add examples,
for instance tools I discover or libraries I learn about.

With time, I've started to adopt an unstructured approach where I avoid
complicated structure and subdirectories. I try to use the proper names of
things as the name of a page. The simple structure makes it easy to convert
text to the correct links and it makes it easy to remember the relevant page
names.

I don't worry about having many pages. I don't worry about almost empty pages.
I don't worry about keeping my pages in a hierarchy. I've found it can be
useful to split information into separate pages, as it makes it easier to link
things. I sometimes find the graph features useful, e.g. |wiki-graph-in|, but
I don't use them much.

However, sometimes I write down stuff that I don't know where to put. This is
where I use my index (`index.wiki`). This file is where I put anything that
does not currently have a home. I may also use it to link to pages that need
attention. For example, if I were to notice that my wiki page about Topic X is
outdated and/or needs some work, then I add a link to it from my index. With
time, I work through the index (often slowly) and move content into more
dedicated pages. For this workflow to work well, it is crucial that my index
is extremely accessible. I therefore have a global keyboard shortcut on all my
computers to open the index in neovim in new terminal. Specifically, I map
<alt-n> to the shell command `urxvt -e nvim +WikiIndex`, where `urxvt` is
a well-known terminal. This way, it takes less than a second from the moment
I have a thought until I can start to add it to my `index.wiki` for later
processing. The speed allows me to write down a thought immediately and then
continue with the current work without being severely disrupted - this is what
makes the concept so important.

Although I do add a lot of text to my wiki, I've also realized that I should
not add all data there. For instance, I've come to use Zotero [7] for managing
my literature database. This is also why there is now some support for Zotero
within `wiki.vim` (see |wiki-link-cite|).

For some topics, I may write a wiki page about stuff where I have links to
data files in which I can append new data and to scripts I can run to
visualize the data. Thus, I don't keep everything in the wiki, instead, I may
write the "metadata" and general overview in the wiki, and then keep the real
data and relevant tools as a "third party".

Daily journal ~

I keep a daily journal. I use |:WikiJournal| to open today's page. For each
day, I tend to write a short memo on what I did that day. I've found it
convenient to format this as lists for each main topic/project/activity. This
makes it easier to write weekly and monthly summaries.

I use |WikiJournalToWeek| and |WikiJournalToMonth| commands to create the
summaries. I write them in retrospective. I use another plugin of mine,
lists.vim [8], which has a command `ListsUniq` that I use to quickly write
and combine these summaries.

I reserve my journal for work-related activities. This includes minutes of
meetings or notes from events and courses. However, I don't use my journal to
log mundane tasks or other temporal activities. Instead, I keep a log of such
things in a related wiki page. For instance, I have a wiki page for my house
where I keep a log of repairs and similar.

I usually plan my work week each Monday by manually writing and maintaining
TODOs for each day in the week. I also have an entry for the next Monday where
I put TODOs that are not for the present week.

This way, my journal serves as a task tracker where I write quick comments
about tasks when I work on them. I generally avoid adding "real" information
content to my journal. Instead, I create links to my main wiki and put
valuable content there. This way, if I work on something, then work on it
again after a long break, the content is readily available when I get back to
it. In some cases, I do link from my wiki to a specific journal entry - for
instance when I refer to meeting notes.

If I'm curious about what I did at a particular date, I use calendar.vim [9]
to find the date and open the corresponding entry (see [10, 11] for my related
Vim configuration). I'm generally never interested in any form of journal
index (|WikiJournalIndex| exists because some users find it useful, though).
The calendar.vim interface is more or less everything I need in that regard.

Similar to my personal wiki index, I use a global shortcut to open today's
journal page: <alt-j>. This is mapped to `urxvt -e nvim +WikiJournal`. I find
it very useful as it makes it very easy to quickly open my daily journal if
I want to make a note or read about something I did earlier.

Over time, the journal entries have a great value in that it is easy to go
back and see what I did at a particular point in time. The summaries make it
easy to get a larger overview. I don't use them often, but when I do, I'm glad
I have them. I also find the process of writing all of these things useful as
it makes me think about what I'm doing - both the planning part and the
retrospective part.

Closing words ~

Finally, I again stress that these are my personal experiences and opinions,
and I very much acknowledge that what works for me probably does not work for
everyone else.

References ~

[0]:  https://github.com/lervag/wiki.vim/issues/101#issuecomment-709571804
[1]:  https://github.com/lervag/wiki.vim/issues/101#issuecomment-718284921
[2]:  https://github.com/dyng/ctrlsf.vim
[3]:  https://syncthing.net/
[4]:  https://github.com/nvim-telescope/telescope.nvim
[5]:
https://github.com/lervag/dotnvim/blob/fddbc2def970cb4bd61894d60c0e7e266408f2f8/lua/lervag/util/ts.lua#L40-L71
[6]:  https://github.com/BurntSushi/ripgrep
[7]:  https://www.zotero.org/
[8]:  https://github.com/lervag/lists.vim
[9]:  https://github.com/itchyny/calendar.vim
[10]:
https://github.com/lervag/dotnvim/blob/fddbc2def970cb4bd61894d60c0e7e266408f2f8/lua/lervag/init/packages.lua#L1335-L1347
[11]: https://github.com/lervag/dotnvim/blob/main/ftplugin/calendar.lua

