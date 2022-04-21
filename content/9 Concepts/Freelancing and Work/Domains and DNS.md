# Domains and DNS
**Domains** refers to web addresses, also called domains. e.g. ruairimcnicholas.com
**DNS** stands for Domain Name System and is how we control how different requests to a domain can be directed to different places, e.g. to host your website with one provider and your email with another involves editing DNS records.

# Introduction to the Internet
First read [[Introduction to the Internet]].

Having read that, and done some reading of your own if needed, you should now have a basic understanding of
- Domain names
- DNS records
- Nameservers



# Working with client's domains

## Getting a domain
Web design clients will either not have a domain, or will need one.
They might have one but only be using it for emails and not have a website.
If they don't have one, a new one will have to be registered.

There are many, many sellers of domains online.

Globally, popular ones are
- [Namecheap](https://www.namecheap.com/)
- [GoDaddy](https://godaddy.com)

Either of them is fine for registering a domain name.

In Ireland my go-to recommended provider is [Hosting Ireland](https://hostingireland.ie)

I advise having your client pay directly for the domain, initially and every year after for renewal, using a credit or debit card. For more on this see [[Paying for client's expenses]].

Once you have successfully registered their new domain name, I highly recommend you set it up on [[Cloudflare]] immediately. 


## Pointing a domain to hosting

If you are ready to launch a new website, you need to create an A record on the domain that points to the IP of the [[Web hosting]] account/server you are using.

Many hosting providers have a DNS area/zone that will tell you exactly what records to look up. If in doubt contact hosting support.

Double check all records as one wrong letter or number can bring down an entire website or email system! **I recommend taking and saving screenshots of all DNS records before you change them, this has saved my ass many times.**





---
**Links:** [[The Internet]] [[Web hosting]] [[Getting started with Freelance WordPress Web Design]]
**Tags:** 
**Created:** 2021-05-29  19:53