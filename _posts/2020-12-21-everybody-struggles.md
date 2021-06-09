---
title: Everybody Struggles
tags: [Outreachy]
style: fill
color: danger
description: A list of things I struggled with during my Outreachy internship and key lessons I learnt.
---

![](https://image.freepik.com/free-photo/upset-tired-woman-keeps-both-hands-temples-frowns-face-feels-overworked-after-working-long-time_273609-33989.jpg)


During week two (December 8 to 14) of my internship at the GNOME foundation, my main task was to research on the Django "API" authentication methods and implement a mode of Authentication, that will provide a secret random string, instead of the usual user-password mode to authenticate users, who had to gain access to the write APIs I was going to develop. My mentor recommended I go the Api key way, so I went on to do my work.

> The first issue was picking the right Django app/package to use from the bunch of packages I found:


### Django Packages

- Django rest framework
- Django Tastypie
- GRAPHENE-DJANGO
- Piston

*Just to name a few*...

Luckily I stumbled on the [Django packages grid](https://djangopackages.org/grids/g/api/) which clearly outlined the features of each package. It became crystal clear that the Django rest framework was the real deal.

The next challenge was the Auth section of the [Django Rest Framework](https://www.django-rest-framework.org/api-guide/authentication/#tokenauthentication) documentation didn't speak the Api Key language, but rather the Token-based Auth language. As a beginner, this was quite confusing and I kept wondering what the difference between these two was.

> I did some extensive research and here's what I found...


### API Keys

* Using API keys is a way to authenticate an application accessing the API, without referencing an actual user. The app adds the key to each API request, and the API can use the key to identify the application and authorize the request. The key can then be used to perform things like rate limiting, statistics, and similar actions.
[source - Nordic APIs](https://nordicapis.com/the-difference-between-http-auth-api-keys-and-oauth/)

* An application programming interface key (API key) is a unique code that is passed in to an API to identify the calling application or user. API keys are used to track and control how the API is being used, for example to prevent malicious use or abuse of the API. The API key often acts as both a unique identifier and a secret token for authentication, and is assigned a set of access that is specific to the identity that is associated with it.  
[source - IBM Cloud](https://cloud.ibm.com/docs/account?topic=account-manapikey)

* The only django package that provided an option for apikeys added to this to their README file *Please note that this package is NOT meant for authentication. You should NOT use this package to identify individual users, either directly or indirectly.* [source](https://florimondmanca.github.io/djangorestframework-api-key/)


### Token-based Authentication

* Token-based authentication is a protocol which allows users to verify their identity, and in return receive a unique access token. During the life of the token, users then access the website or app that the token has been issued for, rather than having to re-enter credentials each time they go back to the same webpage, app, or any resource protected with that same token. [source - Okta](https://www.okta.com/identity-101/what-is-token-based-authentication/#:~:text=Token%2Dbased%20authentication%20is%20a,receive%20a%20unique%20access%20token.&text=Auth%20tokens%20work%20like%20a,app%2C%20the%20token%20is%20invalidated.)

> Reading these conflicting write-ups confused me further and I wasn't exactly sure which one was right for my use case. What I was sure about was that I needed to authenticate users before they could gain access to the write APIs

I reached out to a few people and got some very good clarifications. It became clear that Token-based Authentication was the way to go because it met my requirements and was better supported by the Django rest framework.


### Lessons Learnt

* Always ask for help from a more experienced person when you're stuck, it will save you a lot of time.
* Read articles keenly, some maybe outdated or provide details which may not be totally correct or could just be suited for some particular use cases.

*Let me know what you think about the Api Key Vs Token Auth Struggle...*
