---
title: pastevents
displaytext: Past Events
layout:  null
tab: true
order: 1
tags: owasp-slc wasatch-appsec
---

# Past Events

See all [recent events in MeetUp](https://www.meetup.com/owasp-slc/events/past/).

## August 25, 2022 - Tokens
* Talked about all the various kinds of tokens in use in web applications; used to primarily be session cookies, but now there are refresh, access, JWT, bearer, self-contained tokens and more.
* Talked about maintaining the controls of immediately logging out users and logging out any other sessions of a particular account when their password is changed. This is trickier in a microservices architecture that relies on self-contained and non-revokable access tokens to be performant. Solutions include managing expectations by telling partners and penetration testers that your access tokens will stay alive up to 5-10 minutes (or whatever you set their expiration to be) even after the session is destroyed. Also talked about setting up a revoked list that would have to be disseminated to all microservices in some way (list should be short if it is only users who click the log out button or other user sessions when a user changes their password and the list can be purged once the tokens expire naturally anyway).

## February 22, 2022 - Mobile App Pen testing
* It's getting harder (to jailbreak and analyze)
* [Pentesting iOS without a jailbreak](https://medium.com/securing/pentesting-ios-apps-without-jailbreak-91809d23f64e)
* Many vulnerabilities are actually with the APIs mobile apps utilize
* [Proxyman.io](https://proxyman.io/)

## Thursday, January 12
* Developer Training
* Round Table Discussion

## November 22nd and talked about:
* OWASP's new [Top 10](https://owasp.org/Top10/) 2021
* OWASP Top 10 is almost entirely categories now with SSRF the last Top 10 that sounds like a single vulnerability; most are collections of dozens of CWEs
* XSS is now part of the broad injection category, but in some ways, a lot of these could be linked into even broader categories in the same way; there's a lot of overlap as illustrated by a [venn diagram](https://www.owasptopten.org/thedata) that was shared, but it was for the 2017 Top 10
* Lots of company's use OWASP Top 10 for training
* Top 10 can also be used for threat modeling/checklists or as a way to check tool/process coverage (e.g., does tool X find OWASP Top 10 A??)

## September 29, 2021
* Career progression in AppSec (from entry level up to technical tracks and management),
* How participating in conferences and events (e.g., CTF) can help entry level candidates,
* Impostor syndrom is common in this industry and we all often have to look things up or refresh our memory or learn something new,
* How technical leaders provide value by "scaling their services" (helping others be more effective).
