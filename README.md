# dedsploit
Framework for attacking network protocols and network exploitation.

__Official Website:__ http://dedsploit.tech

![Logo](logo.png)


### I. Introduction

 This entire project brought upon a lot of the ideals from the Watch Dogs franchise, and even actual hacking culture, to life. This framework aims to exploit and attack some common every-day vulnerabilities, whether it is a misconfiguration of a SSH server, or even the utilization of `apache2` as a web server, which could be subjected to malicious __Slowloris__ DoS attacks.

The framework comprises of several modules, and within each module will be attack vectors.

    main
    |
    +--SSH
    |    +--
    |       |- bruteforce - bruteforce vulnerable SSH server
    |
    +--SMTP
    |     +--
    |        | - bruteforce - bruteforce SMTP address (aka email)
    |        |
    |        | - smsbomb - utilizes smtp-to-email gateway to spam SMS messages
    |
    +--HTTP
    |      +--
    |         | - slowloris - Layer-7 DoS attack using slow headers and malformed GET requests to a vulnerable web server
    |         
    |         
    |
    +--Recon
    |       +--
    |          | - pscan - port scan with Nmap
    |          |
    |          | - hosts - scan for active hosts
    |
    +--Miscellanous
    |             +--
    |                | - arpspoof - MITM where user fakes ARP messages on LAN, intercepting packets from host
    |
    |
    +------

### II. Installation & Usage

In order to install this program, it is best that you are on a __Linux-based__ distro, preferably __Kali-Linux__. You may also be on macOS, but this rollout is tentative and may be buggy.

## Quick n' Dirty One-liner

    $ curl https://raw.githubusercontent.com/ex0dus-0x/dedsploit/master/installer | sudo /bin/bash 

## Building from Source

First, `git clone`.

    $ git clone https://github.com/ex0dus-0x/dedsploit

Change directory, and then run the installer script (Must be root or have superuser permissions):

    $ cd /path/to/dedsploit
    $ ./installer

The `installer` script will install of the necessary dependencies for you.


Once finished, execute with:

    $ dedsploit

If you decide to build from source, do keep in mind that you may remove the repository you clone after installation, since dedsploit has been reinstalled elsewhere and is now part of your `$PATH`.

---

Example of the __ssh__ bruteforce module in use (obsolete, replace video!):

[![asciicast](https://asciinema.org/a/atqn7b3j8j24qzgtfhz3flqho.png)](https://asciinema.org/a/atqn7b3j8j24qzgtfhz3flqho)

### III. TODO

* Misc. module - may include embedded and IOT attack vectors

### IV. Issues?

If you ever have any issues regarding the source code of this framework, as well as any errors you have encountered, please do not hesitate to open a new issue!
