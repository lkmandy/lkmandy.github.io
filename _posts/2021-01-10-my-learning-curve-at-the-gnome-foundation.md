---
title: My Learning Curve at the GNOME Foundation
tags: [Outreachy]
style: fill
color: info
comments: true
description: A summary of how I evolved skill-wise while working on GNOME's Translation Editor
---

![](https://image.freepik.com/free-psd/crumpled-paper-form-light-bulb-more-you-learn-more-you-earn-quote_23-2148347760.jpg)


It's been six weeks since I started this exciting journey as an Outreachy intern at the GNOME Foundation.
Every week, I have a set of tasks to work on and a project review session every start of the week with my mentor.  
During these sessions I present the work I've done, challenges I faced and then get feedback. I've had to learn most things on the go and every task comes with it's own unique flavour of difficulty and discovery.
*Let's take a quick look at the project I'm working on...*

My project is based on completing the integration between Gtranslator and Damned Lies(DL), so as to permit translators to upload files and reserve for translation directly from Gtranslator.(This is already possible from the DL website).
I also need to extend the API(Application Programming Interface) endpoints DL provides so as to suite my use case.

#### Gtranslator

Gtranslator is an enhanced gettext po file editor for the GNOME desktop environment. It handles all forms of gettext po files and includes very useful features like find/replace, translation memory, different translator profiles, messages table, easy navigation and editing of translation messages and comments of the translation where accurate.

A .po file is simply a list of strings from the original program. They contain the actual translations. Each language has its own .po file; for example, for French there would be a fr.po file, for German there would be a de.po, for American English there might be en-US.po.

> Gtranslator is now officially called the GNOME Translation Editor [source](https://wiki.gnome.org/Apps/Gtranslator)


#### Damned Lies

Damned Lies is a web application that was built using Django to manage GNOME's translation work-flow and produce 
statistics to monitor the translation progress.
You might be wondering why the name, right? so here you go - "Lies, damned lies, and statistics" is a phrase describing the persuasive power of numbers, particularly the use of statistics to bolster weak arguments.

> Let's now find out how I have progressed in my learning so far...


### Difficulty Levels

First off keep an eye on this "letter map", I'll use the letters defined below to depict the difficulty level of a particular week.

- **E:** Easy
- **N:** Normal
- **H:** Hard
- **V:** Very Hard


### Week One

It was an **E**!
- I setup my blog (lkmandy.github.io), added it to gnome planet and wrote a blogpost on [Tips on Getting Selected for the Outreachy Program](https://lkmandy.github.io/lkmandy.github.io/blog/2020/tips-on-getting-selected-for-the-outreachy-program/)

- Setup the Damned Lies project
- Covered some concepts in Django, REST APIs and the HTTP verbs


### Week Two

I'll give it an **N**!
- Did some intensive research on Django API authentication(auth) methods and eventually settled on the Django REST API framework. Django has soo many auth packages to choose from, so this was quite a task.
- Added some endpoints for user authentication and yes this means I built a REST API!! Yay!! My very first!!

### Week Three

Returned to an **E**!
- Submitted a Work In Progress Merge Request for the REST API I built
- Did some research on the JSON-Glib and Libsoup libraries.
- Added a "Reserve for Translation button" on the Gtranslator user interface (just in a bid to setup for the main work)
- Wrote a blogpost on [How Translation works in GNOME](https://lkmandy.github.io/lkmandy.github.io/blog/2020/how-translation-works-in-gnome/)


### Week Four

Somewhat **H**!  
*Mainly because I had to research and troubleshoot a lot before seeing the green light*
- Added the module state to the Load from DL interface and submitted a Merge Request
- Enabled the "Reserve for translation button" to work for the appropriate states as on the vertimus workflow (a diagram that describes the various states and actions available during the translation process of a module) and I equally submitted a Merge Request.
- Added an icon for the upload to DL feature (just did this locally on a separate branch)


### Week Five

And I'll give it an **E**!
- Designed two mockups for the "upload file dialog"
- Coded one part of the upload file dialog(the choose file dialog)
- Tried adding the token auth information to Gtranslator, but didn't succeed.


### Week Six

I can't lie oh, it's a **V**
*I'm currently on this week and it finishes in one days as of the time I am writing this blogpost*
- Stored the DL information on every translation file downloaded from DL
- Added custom headers to a file with the DL information if it's downloaded from DL
- Create the "upload file" dialog (WIP)

*A few things I've helped me scale through, let's check them out...*


#### Tricks

- After my project review session, I go through the discussion my mentor and I (and maybe some other community members) just had, pick out all the key point mentioned and summarize them in my evernote sheet.
*My mentor usually does a recap of the goals I need to achieve for the week, which is also very very helpful*
- I read through my summary several times to make sure i don't miss out on any detail
- When a task gets hard, I never give up. I just take breaks and push hard until I succeed.
- I do extensive research and go through documentation before implementing stuff
- I submit Merge Requests as early as possible so I can get quick feedback (kudos to my mentor for this)

> It's been an interesting journey and I'm very happy with all the new things I get to learn everyday.  
The end!!
See you on the next one!!

Thanks!!
