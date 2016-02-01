---
layout: post
title:  "Dev Set up on El Capitan 10.11.2 - Part 1"
date:   2016-02-01 10:12:20
excerpt: Setting up a dev environment on a freshly installed El Capitan 10.11.2 on an iMac (2011 Edition) starting with MacOSX command line tools, customizing a theme for Terminal, and adding a .bash_profile
image:
  feature: test.jpg
  credit:
  creditlink:
technologies:
  software: El Capitan 10.11.2, MacOSX command line tools without installing Xcode, Terminal, Bash, AMP HTML
  hardware: iMac. MacBook Pro
og:
  type: TechArticle
  # examples: BlogPosting, Article, NewsArticle, TechArticle
categories: development
tags: El Capitan, bash, cli, AMP
---

Setting up a dev environment on a freshly installed El Capitan 10.11.2 on an iMac (2011 Edition) and MacBook Pro (2009 Edition) starting with MacOSX command line tools, customizing a theme for Terminal, and adding a .bash_profile

I found a few upsides on waiting to update to El Capitan. By this time, I didn't have to deal with the System Integrity Protection (SIP) when installing Homebrew, and I accidentally found out I can install MacOSX command line tools without installing Xcode. Thanks to Git for that accident.

With a fresh El Capitan install, I opened Terminal to git clone some Sketch (BTW, darn you Sketch app for forcing me to upgrade to El Capitan) plugins. This is when I was prompted to Get Xcode or install Command Line tools. Let's make this TechArticle Part 1 of the series, and these are the starting steps (1-30):

1. Open Terminal
2. Type “git clone”

    <amp-img src="/assets/images/dev-1.png" alt="Terminal with Step 2" height="377" width="603"></amp-img>

    *Terminal - Step 2*
3. A window should pop up.
4. You should see: “xcode-select: note: no developer tools were found at '/Applications/Xcode.app', requesting install. Choose an option in the dialog to download the command line developer tools.”

    <amp-img src="/assets/images/dev-2.png" alt="Opt to install Command Line Developer Tools only" height="596" width="609"></amp-img>

    *Opt to install Command Line Developer Tools only*
5. Click on "Install" instead of "Get Xcode"
6. Accept the agreement

    <amp-img src="/assets/images/dev-3.png" alt="Accept agreement" height="619" width="1256"></amp-img>

    *Accept agreement*
7. The download begins.

    <amp-img src="/assets/images/dev-4.png" alt="Downloading" height="197" width="553"></amp-img>

    *Downloading command line developer tools*
8. While that downloads, lets customize Terminal and set up a .bash_profile file in our home directory
9. Open Terminal's Preferences

    <amp-img src="/assets/images/dev-5.png" alt="Terminal Preferences" height="249" width="396"></amp-img>

    *Click on Preferences*
10. Go to the Profiles Tab

      <amp-img src="/assets/images/dev-6.png" alt="Profiles Tab" height="627" width="692"></amp-img>

      *Terminal Profiles Tab*
11. Create a New Profile Theme
