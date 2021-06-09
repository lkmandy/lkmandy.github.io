---
title: Outreachy Progress Report
tags: [Outreachy]
style: border
color: warning
comments: true
description: A progress report on the work I have covered half-way into my Outreachy internship.
---

![](https://image.freepik.com/free-vector/career-progress-concept-illustration_114360-3348.jpg)


I'm halfway gone into my Outreachy internship at the GNOME Foundation. Time flies so fast right? I'm a little emotional cuz I don't want this fun adventure to end soo soon. Just roughly five weeks to go!!
Oh well, let's find out what I've been able to achieve over the past eight weeks and what my next steps are...

My internship project is to complete the integration between the GNOME Translation Editor (previously known as Gtranslator) and Damned Lies(DL). This integration involves enabling users to reserve a file for translation directly from the Translation Editor and permitting them to upload po files to DL.

Incase you don't understand any terminology or not you haven't heard about these projects before, kindly read this [blog post](https://lkmandy.github.io/lkmandy.github.io/my-learning-curve-at-the-gnome-foundation) and you'll clear all your doubts.

> Let's move forward!

So far, here are the things I've been able to accomplish:

1. Setup a button and required functions for the "reserve for translation" feature.
2. Setup a dialog and associated functions for the "upload file" feature
3. I added the module sate to the user interface which comes in very handy to enable users know what state a po file is in as on the [vertimus workflow](https://l10n.gnome.org/help/vertimus_workflow/). This will permit them know what actions can be performed.
4. In addition, users can now see custom DL headers on po files downloaded from DL or opened locally and even edit the headers as required from the edit header dialog.
5. Added some endpoints to the DL REST API to authenticate (Token Authentication) a user who wants to perform the "reserve for translation" or "upload file" operation.

> What's left?

1. The endpoints I added to the DL REST API need to be approved and merged, so that I can write real queries and complete the functions I've created for the above mentioned two features. I got some feedback on the merge request I did, which I'm currently working on.
2. Ensure that memory has been managed properly and handle security vulnerabilities.
3. Extensive testing and documentation.
4. Final evaluation and wrapping up.

*The big question is **I'm I on track??** Oh well let's find out*

I have completed 8 out of 13 weeks of my internship. according to my timeline, I'm supposed to have a version one of both features working properly. I'm about 90% close to achieving this goal.

Since my project is dependent on another project, it's a little challenging to go as fast as possible. This is because communication needs to be done with the community members managing the DL project and getting feedback or convincing them on why my changes are necessary takes quite some time.

**Next Steps:**
* I need to push hard for the DL team to merge my changes in time.
* Stay focused and complete the tasks I have left.

*I'm glad all is well and with some determination and push, I should deliver my project in time*
