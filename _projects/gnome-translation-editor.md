---
name: GNOME's Translation Editor
tools: [C, Python, GTK, REST API, Libsoup]
image: https://bit.ly/3z9PImB 
description: New features added to GNOME's Translation Editor
# external_url: https://gitlab.gnome.org/users/lkmandy/activity 
---

## GNOME's Translation Editor

I added two features to this project - the [Translation Editor](https://wiki.gnome.org/Apps/Gtranslator), to enable users to:
1. Upload translation files and 
2. Reserve translation modules directly from the Translation Editor (TE). 

I achieved this by integrating TE with [Damned Lies](https://l10n.gnome.org/), following GNOME’s Human Interface Guidelines (HIG). 

Also, I collaborated with senior developers within the GNOME community to design and build a REST API using Python/Django which was used for the integration. I used the GTK library for the user interface and C to implement the overall logic. I used other libraries like libhandy, libsoup and glib. Lastly, I wrote a help guide, two blog posts and published them on [GNOME planet](https://planet.gnome.org/). Here are my [Contributions](https://gitlab.gnome.org/users/lkmandy/activity)


> Upload a Translation module

![](https://bit.ly/3ghnqhv)


> Reserve For Translation

![](https://bit.ly/3criVzU)
