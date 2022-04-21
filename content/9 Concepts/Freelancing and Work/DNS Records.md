# DNS Records
DNS Records are records attached to a domain name that routes different requests to different IP addresses.
In plain English, this allows you to host, say, your website with one hosting provider, and your email with a compeltely different provider, typically [[GSuite]] or [[Microsoft Outlook]].

Boy did I used to hate these things, because I didn't fully understand them. I kind of just blundered my way through them, occassionally looking something up on Google, until I pieced together an understanding much slower than I should have.
**Don't do this 🙃** DNS is important, get a grip on it :)

## The Two Golden Rules of DNS Records

^cbd316

Following these two DNS_related rules will save you a lot of headaches and hassle in your freelance web design career: 
1. **ALWAYS** take a screenshot of the existing DNS records and save this somewhere safe, in case you need to change anything back.
2. **ALWAYS** double check what you are entering and deleting; you don't want to crash the emails for a whole office... 🤓


## Types of DNS Record
There are several types of record that a DNS record can be, depending on what it is used for. These are the most common:

| Record Type  | Purpose                                                                                                                                                        |
| ------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| A Record     | 'A' stands for 'address' and is the most basic record. It indicates the IP address for a domain. Used to set what server your domain will load its website from. |
| CNAME Record | CNAME records point directly to a domain name, not an IP, allowing them to be 'bulk updated', e.g. you can have 4 CNAME records point to an A record, and if you change the A record's IP, it's changed straight away for all four CNAME records.                                                                                                                                           |
| MX Record    | Used for directing email services. Stands for 'Mail Exchanger record'. e.g. setting up [[GSuite]] (Gmail for business) involves setting up 4 MX records (multiple ones are often used for load balancing and redundancy).                                                                                                                                                               |
| TXT Record   | Allows the entering of text, often quite a lot of it, for things like email authentication (DKIM and SPF), Google Search Console Verification, etc.                                                                                                                                                               |


Don't worry; whenever you need to go near DNS records, the service requiring the change will usually provide a comprehensive guide on how to change them. But don't forget to follow [[DNS Records#^cbd316|The Two Golden Rules of DNS Records]]!!

## An example
![[rmcn.com DNS records.png]]

Here is a screenshot of the DNS records for my personal domain, ruairimcnicholas.com.
Note for security I wouldn't go posting DNS records online if I were you, but I've hidden the most important thing which is my origin IP address. And I don't think I'm interesting enough yet to have hackers reading my [[Second brain]]!


**A record:** This has an IP hidden in red that is the address of my WordPress hosting, so when you put ruairimcnicholas.com into your web browser, you are directed to this server by this DNS record, and the server serves you up my website! The **orange cloud** means this record is being proxied through Cloudflare; the IP is disguised/hidden, and their various security and speed services are being provided.

**CNAME records:** The first one I put there as it is part of the instructions to set up Obsidian Publish, which is what you are probably reading this note on. Note it says 'knowledge', this is how I have two different websites available depending on what you type in:

| Address                        | Goes to                                     |
| ------------------------------ | ------------------------------------------- |
| ruairimcnicholas.com           | WordPress website (inactive)                |
| knowledge.ruairimcnicholas.com | Obsidian Publish [[Second brain]] (active!) |
| linkedin.ruairimcnicholas.com  | A redirect to my LinkedIn profile                                            |

**MX Records:** I use [[ProtonMail]] for my email and it had me enter these MX mail exchange records to get it working.

**TXT records:** All of these are for ProtonMail and are for helping less of my mail go into people's spam, and help stop people from impersonating my email address.


If you need to change DNS records for a client and are not comfortable doing so:
Stay calm, follow the provided instuctions while following [[DNS Records#^cbd316|The Two Golden Rules of DNS Records]]!!

## Cloudflare
[[Cloudflare]] lets you make almost instant (seconds) changes to DNS records and have them propagate globally in seconds. This is a huge step up from the 24 hour window that is given for standard DNS updates. 
**Use Cloudflare for all of your domains where possible!**



---
**Links:** [[Domains and DNS]] [[Introduction to the Internet]]
**Tags:** 
**Created:** 2021-05-30  10:35