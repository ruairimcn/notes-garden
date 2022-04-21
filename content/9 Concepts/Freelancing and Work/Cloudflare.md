# Cloudflare
Cloudflare is a service for managing and securing domain names, offering free and paid plans.

At the time of writing, 30th May 2021, [[Propeller Digital]] has 114 domains on Cloudflare.

Almost every client I work with I add to Cloudflare where possible.
**I recommend adding all domains that you work with to Cloudflare unless there's some reason not to (there usually isn't)**

# Benefits

## 1. Free SSL Certificate
[[SSL Certificates]] are still a large market on the internet, even though there are ways to set them up for free using services like [[Let's Encrypt]] and Cloudflare. They can range from €10 to €100 a year for 'normal' ones and over this for more advanced ones which I haven't used.

Cloudflare provides SSL certs for free, saving you or your client cash - always a good think!


## 2. Free security tools
I discuss the importance of [[Digital Security]] on my note [[Getting started with Freelance WordPress Web Design]]. Cloudflare helps with this by
- Presenting malicious traffic or suspected bot traffic with a [[Captcha Challenge]] to help prevent spam and hack attempts
- Helps to prevent against [[DDoS Attacks]]
- Allows you to set firewall rules, e.g. block all traffic from a specific country
- Hiding your web hosting server/origin server's IP address to help hide it from malicious hackers and bots.


## 3. Free speed tools
Cloudflare has a number of tools for speeding up your websites:
- Websites are cached across a global [[CDN|Content Delivery Network]]; if your website is hosted with a provider in the UK, people in the USA will have cached content served from Minifythe nearest Cloudflare server in the USA. They have servers in 200+ cities across 100+ countries.
- They [[Minify]] the website's [[HTML]], [[CSS]], and [[Javascript]], that is they made the code smaller so that it downloads quicker.
- They have other tools you can turn on like Brotli Compression and Rocket Loader to speed up your website's loading time. More features are available if you upgrade to a paid plan (which I haven't, ever, with any of the 114 domains we have on it. Hasn't been needed!)

## 4. Instant DNS Record Propagation
This one won't seem as impressive to some new web designers intitially, but in time you might come to see this as your favourite thing about Cloudflare.

When you make a hange to [[DNS Records]], the change usually takes anywhere from 4 to 24 hours to 'propagate' around the globe, meaning there are different DNS servers around the world that need to get this new information in order to direct people to the right place. They cannot check for new records every few minutes as this would put too much of a strain on the server, so it's done every few hours.

Cloudflare, with methods I haven't looked into, allow your DNS changes to propage in seconds (sometimes a few minutes) around the globel. This is handy for just getting websites and email providers working faster, but also is a saviour if you ever make a mistake with a DNS records as the fix can take hours to propagate! 



## 5. Other handy bits
Page rules for forwarding, basic analytics, and scrape shields are handy too.



---
**Links:**  [[Domains and DNS]] [[Web hosting]] [[Getting started with Freelance WordPress Web Design]]
**Tags:** 
**Created:** 2021-05-30  10:02