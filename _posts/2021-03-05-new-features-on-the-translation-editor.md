---
title: New Features on the Translation Editor
tags: [GNOME, Open-source]
style: fill
color: primary
comments: true
description: Translators can now  "reserve" and "upload" a translation module, directly from the GNOME Translation Editor. Learn more about these new features!!
---

![](https://image.freepik.com/free-vector/new-functions-concept-illustration_114360-6156.jpg)


> New feature alert!!

I just wrapped up with my Outreachy internship at the GNOME foundation and I'm very excited to say it's now possible to "reserve" and "upload" a translation module, directly from the GNOME Translation Editor. However, these changes are yet to be added to the master branch; definitely after the string freeze. There are still a number of UI/UX improvements that need to be done but it's functional.
As with every new version, there's always room for improvement so don't hesitate to provide feedback.

## I. Reserve for translation

You can reserve a translation module (aka po file) to let other team members know you are currently working on a particular po file, so that multiple people don't work on one file at a given moment.

To reserve a translation module:
* Click on the Load from DL button (if you are on the main window) or Open from Damned Lies icon (if a po file is open) in the header bar. You can also use the Ctrl+D keyboard shortcut.
* Select your desired po file; specifying the particular team, module, branch and domain.
* The state of the po file is displayed.
* Select the "Reserve for translation" checkbox to reserve your chosen po file.
* A message dialog will display the status of the operation.
* If the message dialog displays a success message, you have successfully reserved the po file for translation.
* If the "Reserve for translation" checkbox is deactivated, it means the po file cannot be reserved. This is because it is not in the appropriate state. See the [Vertimus workflow](https://l10n.gnome.org/help/vertimus_workflow/) for more details.


## II. Upload a new translation

After translating a po file, you can upload it to Damned Lies(DL) to make the new version available to everyone and to make DL show the new statistics for that file. Note that the po file that is uploaded is that which is currently open at a given time; as it is not yet possible to manually select a file to upload.

To upload a po file:
* Click on the Upload file icon in the header bar or use the Ctrl+B keyboard shortcut.
* A message dialog will display the status of the operation.
* If the message dialog displays a success message, you have successfully uploaded the po file to Damned Lies.
* Again, if the Upload file icon is deactivated, it means the po file cannot be uploaded. This is because it is not in the appropriate state. Again, see the [vertimus workflow](https://l10n.gnome.org/help/vertimus_workflow/") for more details.

> Note that a po file must be reserved (in the state; Translating) before it can be uploaded to Damned Lies

It's been a very interesting learning experience and I'm very glad with this milestone.

**Many thanks to my mentor Daniel Garcia Moreno (@danigm) for his superb mentorship and support through out my internship**

Thanks!!
