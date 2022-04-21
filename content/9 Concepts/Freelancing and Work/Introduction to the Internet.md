# Introduction to the Internet
You are almost certainly reading this note using a web browser connected to the internet.
But what exactly is the internet? How does it work? How do we use it to host and manage websites?


## Physical Infrastructure (Real World Stuff)
At its core, the internet is a global network of interconnected computers that can be accessed by internet-connected devices.

Many types of device exist on the internet - originally just computers, then phones and tablets, and now things like doorbells, lights, and thermostats.

For web design purposes we are interested in [[Servers]].
Servers are a particular type of computer that are designed to host files and let computers on the public internet access them. These files can be many things including
- [[HTML]] files
- Audio files
- Photo files
- Video files
- PDF files
- etc...

Many severs host some or all of these types of content. e.g.YouTube's servers mostly contain video files. A **website** is, at the minimum, [[HTML]] files, and these days usually has some photo files too.

When you type in ruairimcnicholas.com into your browser, your browser goes to a DNS service that translates the address into an [[IP address]].
Humans understand and work with website addresses, but these need to be converted into the 'address system' that the internet uses, and this is a system of IP addresses, with every public device having its own IP address.

So your browser gets told that ruairimcnicholas.com has an IP of, e.g., 187.221.43.81
This address goes to a physical server, in this case one with my hosting provider Hosting Ireland.

These servers are often providing [[Shared Hosting]] meaning multiple websites are stored on the one server.

**Your browser:**
*Hey, I see 187.221.43.81 points here; I'm looking for the website ruairimcnicholas.com*

**Server:**
Website exists, files are here.


The browser then gets sent the 'entry level' file, usually called index.php or index.html.
From here, you can navigate to other content on the website by clicking [[Hyperlinks]]. These often go to other [[HTML]] pages that may have other content.

If you click a link to a website at a different domain/website address, this process is repeated for that website.

---
**Links:** [[Domains and DNS]] [[Web hosting]]
**Tags:** 
**Created:** 2021-05-29  19:55

## The Structure of a Domain Name
At a minimum, a website address is made up of a top-level domain and a first-level domain.

A top-level domain is the very last part of the domain, e.g. .com, .co.uk, .ie
in www.example.com
com is the top-level domain.

The price of a domain depends on the TLD, ranging from €2 to €200 a year, maybe more for some.
Some are restricted by country, business type, etc.

The second-level domain name is what comes before the TLD, in our above www.example.com this is 'example', and this can go to third-level for what are called [[Sub domains]].

| second-level domain | first-level domain | top-level domain |
| ------------------- | ------------------ | ---------------- |
| knowledge.          | ruairimcnicholas.  | com              | 


## Buying a Domain Name
There are many great domain name providers out there, shop around and see who is the best.

Only one person can own a given domain name.
I own ruairimcnicholas.com so no one else can use it, and I can make more domains like
knowledge.ruairimcnicholas.com
blog.ruairimcnicholas.com
etc. 

But I have no claim over ruairimcnicholas.co.uk as an example as I don't own it. The owner can use it as they like.


Domain names are always bought for a minimum of a year and can be bought for multiple years at a time too. 

Once you buy a domain name, you can control its **DNS records** and its **nameservers**.

## Nameservers
Every domain has two to four nameservers. These are addresses on the internet that say 'This service is responsible for managing my DNS records.'
These DNS records are how you set who hosts your website, or emails, or manages your FTP client, etc.

Usually when you first buy a domain, the nameservers are set to the business from whom you bought it from, and they provide you with a servicde for managing its DNS records.
By changing the nameservers, you can manage the DNS records with a different business/provider. So you can have one company be your Registrar - the company you pay annually for the domain - and another one be the one managing DNS.

There are different reasons for wanting to do this, for my flavour of [[Freelance WordPress Web Design]] I change a domains nameservers to use [[Cloudflare]] wherever possible.

## Cloudflare
[[Cloudflare]] is a fantastic free tool that gives you many benefits for any domain name you use with it.
**I highly recommend reading my note on it and using it whenever possible.**


# Web Hosting
See [[Web hosting]]