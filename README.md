# pw-index-mockup
Quick and dirty front page revamp (in HTML, will need to be converted to PHP?)

## Making Planworld Mobile-Friendly (with Media Queries)

### What are the priorities for functionality on mobile?

* reading plans
  * individually, by typing a name into the finger box
  * individually, by clicking on a username in one's Planwatch
  * in bulk, by clicking on Planwatch Look
* updating your own plan
* sending and reading private messages

### Points to consider

* When updating or reading an individual plan on mobile, hide extraneous navigation, but make it accessible. Phone screens are just too small to have a two-column layout.
  * like, tuck away the header navigation. tuck away Planwatch. tuck away the footer nav. (Are all of those links absolutely necessary to access on mobile?
  * is there a better accessible way to do this aside from hamburger menus?
* Long Planwatches are going to be a royal pain to scroll through - can we default to only showing usernames with updated plans on mobile? (Assign classes of "new" and "read" based on how we determine displaying the "new" flag now, apply visibility:hidden to "read" if viewport width does not exceed X?)
* Long Planwatch Look is also going to be annoying to scroll through, especially when individual users have long plans. Would like to hear from people who do use Planwatch Look whether there's anything we can do to improve that experience. Curious about the viewing stats for look.php compared to those of individual plans
  * (this is why I don't find Planwatch Look useful for my reading style; plenty of people on my planwatch have long plans, some of which include things like reminders or reading lists. But are there people who do? Does it still work for them in the mobile use case?)
  * jlodom00's 2012 mobile client contains a plan reading page, a plan writing page, and a page for Planwatch. Add a send page, figure out the UI for accessing it, and we have a wireframe - just need to rewrite in modern HTML and then enclose in a ... client?

