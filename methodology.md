# The Hacking Methodology
 1. Recon / Intelligence Gathering
 2. Vulnerability Scanning
 3. Exploitation
 4. Post-Exploitation
 5. Reporting (or just flexing)

# Contents
 1. [Recon / Intel. Gathering]
	- What is it?
	- [Semi-]Passive Intelligence Gathering
	- Active Intelligence Gathering
	- Examples of Intelligence Gathering
	- Relevant Concepts & Jargon
	- Tools referenced

## Recon / Intel. Gathering
### What is it?
Recon is the first step in any engagement, the objective here is to collect as much information as possible about targets 
(this can be physical/virtual systems, people and other present technologies)within a pre-defined scope. [[1]]

Understanding your target's attack surface is crucial to a successful hack. Blindly trying to run exploits at a system will only get you
laughed at and probably caught / arrested.

Generally speaking, recon methods can be split into two categories: **Passive** and **Active**.

### [Semi-]Passive Intelligence Gathering
Passive intel gathering is just what it sounds like, *passive*. During this phase you should not perform any action that would be seen as
suspicious by your target. For example, viewing a target website's index page would not normally trigger any security countermeasures.

Whereas running an [XMAS scan] against all ports on a machine *might just* raise a flag or two on an intrusion detection system...

Passive intel gathering also generally includes Open-Source Intelligence Gathering (OSINT); OSINT can be defined as a variety of 
intel gathering methods using publicly available sources, such as (public) social media pages and search engine results. While useful 
data can be collected using OSINT, it normally requires a lot of time (depending on the size of your scope) and can yield false results.

### Active Intelligence Gathering
Active intel gathering (sometimes referred to as *footprinting* ) is the polar opposite to its passive counterpart. Utilising what you've
found from passive recon, you can now make better-informed interactions with your target. This phase of recon involves actively sending
data to a target in the hopes of provoking a response; banner grabbing and port scanning are both components of active 
intelligence gathering.

**NOTE:** This does not include fuzzing or vulnerability analysis. It is simply intended to retrieve accurate, first-hand information 
about the technologies installed on your target (e.g. version numbers, operating system types etc).

### Examples of Intelligence Gathering
 - Using Shodan to scan for internet-facing hosts owned by Coventry University.
 - Passively sniffing packets traveling over a public network using Wireshark.
 - Actively scanning for open ports on a system using a tool like Nmap.
 - Searching forums / message boards for a target individual's posts.

### Relevant Concepts & Jargon:
 - *Scope* - Boundaries set for the attacker so a penetration test remains relevant. For example, an attacker may only be allowed to
 engage with the `cuscmoodle.coventry.ac.uk` subdomain, instead of `coventry.ac.uk` as a whole. Attacking out-of-scope targets may be
 extremely dangerous and potentially illegal (e.g. attacking a 3rd party service provider without their consent).
 - *Attack surface* - Potential points of attack or exploitation (known as 'attack vectors') make up an attack surface. Targets running
 a large number of different services and applications have a better chance of having vulnerabilities, thus presenting a larger attack
 surface.
 - *Banner grabbing* - Banner grabbing is used to identify the version of applications and operating system that the target host 
 is running. This is usually performed on HTTP (port 80), FTP (port 21), and SMTP (port 25) ports using a tool like Nmap.
 - *Port scanning* - A process that sends client requests to a range of server port addresses on a host, with the goal of finding an 
 active port. Typically a port scan is not considered a malicious attempt on its own, however low-priority alerts may be triggered on
 high-security targets (for example, a government server).

### Tools referenced:
 - [Shodan]
 - [Nmap]
 - [Wireshark]

[1]: <http://www.pentest-standard.org/index.php/Intelligence_Gathering#What_it_is>
[2]: <https://en.wikipedia.org/wiki/Open-source_intelligence>
[XMAS scan]: <https://en.wikipedia.org/wiki/Christmas_tree_packet>
[Shodan]: <https://www.shodan.io/>
[Nmap]: <https://nmap.org/>
[Wireshark]: <https://www.wireshark.org/index.html#aboutWS>
[Recon / Intel. Gathering]: <https://github.com/kieran-walker-0/cuscs/blob/master/methodology.md#recon--intel-gathering>
