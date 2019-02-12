# Finding fun/useful/dangerous shit on the internet (OSINT)

## Contents
 1. Google-Fu (Dorking)
  - Finding creds, API keys and other sensitive info
  - Manually searching for IP cameras
  - Nobody buys books any more
 2. Shodan - How small children can find your datacenters
  - Coventry University
  - Going on a Shodan safari
  - The Shodan API
 3. Slightly evil personal investigation
  - Email addresses,stop giving them out publicly
  - People search engines
  - Social media sites are dangerous
 4. NOSINT - Anti-OSINT & privacy techniques
  - Dox yourself before your enemies do
  - Proxies, VPNs and Tor
  - Separate your aliases
 
## Google-Fu (Dorking)

Google-Fu is a fancy way of saying "advanced usage of search engines". 
Google has extremely helpful filters available for targeting specific sites, files and even people. These search techniques are known as "dorks"
or "Google dorks", people even sell these on hacking forums to people who want a fresh list of targets to hit (usually SQL injection):

![nulleddorks]

To see a list of common Google search techniques, visit here: https://support.google.com/websearch/answer/2466433?hl=en&ref_topic=3081620

### Finding creds, API keys and other sensitive info

This section will cover two main points:
 - Data breaches from hacked websites
 - Hardcoded information in open source code

### Data breaches

It is a certainty that data breaches will happen, and there's a good chance that you'll be involved in one or two if you use the same Email
address for many different websites.

![hibpexample]

Depending on the website, at least one of two things will happen with a hacked database:

 1. If it's a high-level target such as a gov or popular social media site, it'll be sold to other hackers.
 2. It'll always end up on the internet, usually after it's become saturated enough to not turn a profit when re-selling.
 
Hackers and security professionals alike have created data breach search engines, often with a subscription service that allows the client
to see hashed or cleartext passwords, below are a few examples of whitehat and (sort of) blackhat services:

**[HaveIBeenPwned?] - Created by the security researcher Troy Hunt after the Adobe hack in 2013:**

![hibp]

**[LeakedSource] - A common search engine that allows for different input formats (for example, usernames):**

![ls]

**[CITADEL] - Another search engine giving out sensitive info for cash:**

![citadel]



[nulleddorks]: https://i.imgur.com/C0ny1Hk.png "Source: Nulled.to"
[hibpexample]: https://i.imgur.com/GVx54m8.png "test@example.com's HIBP results"
[HaveIBeenPwned?]: <https://haveibeenpwned.com/>
[hibp]: https://i.imgur.com/prOHZXp.png
[LeakedSource]: <https://leakedsource.ru/>
[ls]: https://i.imgur.com/FLq72uW.png
[CITADEL]: <http://citadel.pw/>
[citadel]: https://i.imgur.com/L5HoydX.png
