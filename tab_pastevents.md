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

## September 21st, 2023
* In person at Weave in Lehi
* Seth Law presented on Modern vs Old 5k00l AppSec
* Some key points were
  * Ware report from 1970 and how many of the same issues (usually with different names) still exist today
  * AppSec is not a "point solution" in that you can't just implement a SAST/DAST tool and think it is solved

## August 30th, 2023
* Virtual
* Testing with Nuclei - Justin
* Risk assessments and threat modeling - Mark
  
## May 25th, 2023
* in person (park)
* Book Club: Discuss Project Zero Trust ([goodreads link](https://www.goodreads.com/book/show/60659055-project-zero-trust))
  
## April 27th, 2023 - virtual
* Mike McCabe spoke to us about Terraform and Infrastructure as Code security

## March 30th, 2023 - In person at Salt Lake County building
* How to Measure Anything in CyberSecurity
* How do you calculate the likelihood of an incident occuring?
* Use the Monte Carlo method to understand annual loss expectancy
* https://docs.google.com/spreadsheets/d/1if1MTESnwY31_Qm4MfPnUZrl4GtP0toRG8xS2OZIXfQ/edit?usp=sharing
* You need to cater your presentation to your audience; some folks like critical/high/medium/low classifications, some might want $ amounts like annual loss expectancy

## February 23rd, 2023 - virtual
* Talked mainly about metrics
  * How do you show value to your leadership (finding bugs earlier in SDLC and fixing them quicker; show value in $ of saved engineer time, customer happiness)
  * Mentioned Doug Hubbard's (the author) book on How to Measure Anything in Cybersecurity
  * Success stories

## January 24th, 2023 - In person at HealthEquity
* HealthEquity hosted an onsite meet-up in Draper.
* We discussed third party scripts and how to secure them:
  * Discussed use of SRI for versioned scripts and how a CSP offers partial protection for dynamic scripts that can't be protected via SRI (primarily by preventing an attacker from including scripts from domains not allowed on the CSP).
  * Some script vendors are so big (e.g., Google) that if they were compromised, your company probably wouldn't be in the news even from the downstream impact, but if your script vendor is smaller and your data is sensitive, you could be the headline.
  * Limiting these types of risky scripts to less-used pages or only loading them when the user wants to use the functionality could help limit impact.
  * Other potential solutions include scanning the scripts (before as a preventive solution or even after as a detective solution [Seth had a solution along these lines]), using iframes, and/or using a tool like feroot.

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
