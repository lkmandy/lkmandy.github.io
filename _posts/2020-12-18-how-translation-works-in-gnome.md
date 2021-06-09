---
title: How Translation Works in GNOME
tags: [GNOME]
style: fill
color: success
comments: true
description: A brief description of the Translation workflow in GNOME
---


## Overview

GNOME uses a web application called Damned Lies (DL) to manage their translation work-flow and produce 
statistics to monitor the translation progress. DL is specifically intended to be used within GNOME. 
There used to be a separate tool called Vertimus but it has been merged  into DL.
Participants in the translation of GNOME belong to translation teams, one for each language to which 
GNOME is translated, and they can have one of three roles: translator, reviewer and committer

> Let's dig deeper into what these roles entails...


## Translation Roles


### 1. Translators

Translators contains persons helping with GNOME translations into a specific language, who added themselves to the translation team.Translators could add comment to a specific PO file translation, 
could reserve it for translations and could suggest new translations by up471 load a new PO file. 
The suggested translations will be reviewed by other team members


### 2. Reviewer

Reviewers are GNOME translators which were assigned by the team coordinator to review newly suggested translations(by translators,reviews or committers). They have access to all actions available to a translators with the addition of some reviewing task (ex reserve a translation file for proofreading, mark a translation as being ready to be included in GNOME).


### 3. Committer

Committers are people with rights to make changes to the GNOME translations that will be release.
Unless a translations is not commit481 ted by a committer, it will only remain visible in the web interface, as an attached PO file. Committers have access to all actions of a reviewer with the addition of marking a PO file as committed and archiving a discussion for new suggestions.


## The Translation Workflow

The workflow used for managing translations is called the [Vertimus Workflow](https://l10n.gnome.org/help/vertimus_workflow/). It describes the various states and actions available during the translation process of a module.
My focus will be on the orange section of the workflow, which is peculiar to translators (as illustrated here [workflow image](https://l10n.gnome.org/help/vertimus_workflow/)
  
- The base state of a module is None, which shows as “Inactive” in Damned lies.
- A translator can then decide to work on a module, so they will **Reserve for Translation** which changes the state from **None -> Translating**. 
- Another pathway that enables one to perform a **Reserve for Translation** is moving from the **To review -> Translating** state. This happens when a module was not properly translated.
- When a translator is done translating, they can then **Upload the new translation**, which changes the state from **Translating** -> **Translated**
- Again, if a module needs to be improved after being translated, it moves from **Translated -> Tranlating**
- Bear in mind that translators can add comments at any point in order to give more context to their work.

> This post is in a bit to evaluate my understanding. I'll appreciate any feedback so I can improve and or correct any misconceptions.

Thanks!!


### References/More Reads
- [APERTIS - Internationalization](https://www.apertis.org/designs/internationalization/internationalization.pdf)
- [GNOME Wiki](https://wiki.gnome.org/TranslationProject/ContributeTranslations)
- [Social Source Commons](https://socialsourcecommons.org/tool/show/2642/)
