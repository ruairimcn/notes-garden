# Email hosting
If you are setting up a company's first website, they may also be looking to have email account set up - web and mail often come hand-in-hand.

You can choose to pass on this work (and ideally be able to recommend someone in your network who is reliable at this work, but this won't always be possible at the start of your career),
or to learn how to do it, and offer it as a service.

I highly recommend using [[Google Workspace]] (formerly GSuite) or Microsoft 365, they are both very solid email solutions.
However they cost around €5 a month per user.

Many [[Shared Hosting]] plans come with a generous amount of email accounts included. 
However these tend to be less reliable than the likes of Google Workspace in the long-run, e.g. less outbound emails going to spam. 

So I recommend that you recommend [[Google Workspace]] to your clients - it will cause you less headaches in the long run!


## Shared Hosting Emails with cPanel
If you do end up hosting emails on a [[Shared Hosting]] account, I can give you the following advice for setting it up properly on cPanel - if you use something else like Plex, good luck :) ([[Google is your friend]])

### 1. Double check the settings for each account
- Check the storage quota per account, make sure it doesn't default to something small like 250MB
- Double-check the spelling of each account


### 2. Turn off Grey Listing (or at least be aware of it)
Some cPanel accounts have an option called Grey Listing under the 'Email' section. It is a spam filter but I have found it to be far too aggressive, marking important mail as spam. If you have this problem and it is turned on, turn it off.

### Set up Email Deliverability - DKIM and SPF 
Under 'Email Deliverability' is a check that cPanel will run to determine if two TXT records are set up correctly, DKIM and SPF.
I don't know exactly how these two things work, but I do know they help to reduce the number of your outbound emails that go to spam, and that setting these up and having cPanel verify them as correct **is a crucial step with this kind of email setup.**

Follow the instructions in cPanel to set up and verify these two records.






---
**Links:** [[Web hosting]] [[Freelance WordPress Web Design]] [[Getting started with Freelance WordPress Web Design]]
**Tags:** 
**Created:** 2021-05-30  11:54