# Finding fun/useful/dangerous shit on the internet (OSINT)

## Contents
 1. Google-Fu (Dorking)
  - Finding creds, API keys and other sensitive info
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

![cit]

Plenty more examples exist, but you get the point.

You don't always have to pay for these things however, because paste sites exist.

Sites such as Pastebin, Ghostbin, DOXbin, Zerobin, Hastebin etc store a hilarious amount of breach data. This is often because hackers like to share their data using anonymous accounts (as is the default on Pastebin), Doxes are also submitted on these sites for the same reason.

Later on I'll be covering Shodan safaris (finding interesting devices using Shodan),  the same can be done for Pastebin. A "service" known as [PSBDMP] collects Pastebin Dumps that it thinks contain sensitive info:

It's fun to come across kids running each other over Habbo Hotel, introducing Sankru of 'Hatter Gang':

![hatter1]

He's even included his own Twitter account, for the clout obviously.

**If it can be done to passwords, it can be done to API keys:**

![apikey]

For the sake of time, I won't go into finding SSH keys and backups, but those are out there too.

### Getting free books to level up your hackerman skills

Anybody who's been on the Discord knows about the eBooks that appear out of nowhere, it doesn't even require the effort of "piracy".

`"{BOOK TITLE}" filetype:pdf`
That's it...

You'll get a lot of spam link with that dork, but you'll generally find what you want in the first page or so.

(Ran out of time because I'm great with preparation, so we wing it from here on out)

SHODAN REPORT: https://www.shodan.io/report/mugjgkwX


[nulleddorks]: https://i.imgur.com/C0ny1Hk.png "Source: Nulled.to"
[hibpexample]: https://i.imgur.com/GVx54m8.png "test@example.com's HIBP results"
[HaveIBeenPwned?]: <https://haveibeenpwned.com/>
[hibp]: https://i.imgur.com/prOHZXp.png
[LeakedSource]: <https://leakedsource.ru/>
[ls]: https://i.imgur.com/FLq72uW.png
[CITADEL]: <http://citadel.pw/>
[cit]: https://i.imgur.com/iI2TOcu.png
[netflixacc]: https://i.imgur.com/OitsWVW.png
[PSBDMP]: <https://psbdmp.ws/>
[hatter1]: https://i.imgur.com/umZlg8d.png
[apikey]: https://i.imgur.com/5qp1jlC.png
