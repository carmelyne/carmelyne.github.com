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

    <amp-img src="/assets/images/Dev-3.png" alt="Accept agreement" height="619" width="1256"></amp-img>

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

      <amp-img src="/assets/images/dev-7.png" alt="Create a new profile" height="626" width="689"></amp-img>

      *New Theme*
12. Name it whatever you want. I chose Idle Fingers because I used the colors from the Idle Fingers Theme.

      <amp-img src="/assets/images/dev-8.png" alt="Create a new profile" height="611" width="681"></amp-img>

      *New Theme*
13. Set Colors

  1. Background / Colors and Effects: #323232
  2. Text / Text: #EBDFBB
  3. Text / Bold Text: #4278B2
  4. Text / Selection: #B8332D


      <amp-img src="/assets/images/dev-9.png" alt="Set colors" height="615" width="685"></amp-img>

      *Set colors*

14. Set Idle Fingers Profile to default

      <amp-img src="/assets/images/dev-10.png" alt="new default theme" height="628" width="700"></amp-img>

      *New default theme*

15. Go back to Terminal

16. We need to show hidden files; type “defaults write com.apple.Finder AppleShowAllFiles YES”

      <amp-img src="/assets/images/dev-24.png" alt="Show hidden files" height="588" width="845"></amp-img>

      *Show hidden files*

17. Relaunch Finder

      <amp-img src="/assets/images/dev-16.png" alt="Relaunch Finder" height="331" width="356"></amp-img>

      *Relaunch Finder*

18. Go back to Terminal, Type ls -lah to check if .bash_profile exists

      <amp-img src="/assets/images/dev-11.png" alt="Back to Terminal" height="466" width="684"></amp-img>

      *ls -lah*

      <amp-img src="/assets/images/dev-12.png" alt="check if .bash_profile exists" height="464" width="686"></amp-img>

      *check if .bash_profile exists*

19. Type “touch .bash_profile”

      <amp-img src="/assets/images/dev-13.png" alt="touch .bash_profile" height="467" width="683"></amp-img>

      *touch .bash_profile*

20. Type “open .”

      <amp-img src="/assets/images/dev-14.png" alt="touch .bash_profile" height="461" width="691"></amp-img>

      *open .*

21. Find the .bash_profile and right click

      <amp-img src="/assets/images/dev-18.png" alt=".bash_profile" height="658" width="822"></amp-img>

      *.bash_profile*

22. Open with Textedit. (Alternatively you can edit it in Terminal with nano or vim but I’m a bad typer that I’d rather copy and paste selectively from my previous bash_profile file; or you can git clone one from github but I wanted to start fresh.)

      <amp-img src="/assets/images/dev-19.png" alt=".bash_profile" height="463" width="651"></amp-img>

      *open .bash_profile with TextEdit*

23. Add the script to change colors, alias and some more scripts to make life easier.

      [Github gist for the script](https://gist.github.com/carmelyne/28d58433bbb0ff9b2676)

      <amp-img src="/assets/images/dev-20.png" alt=".bash_profile" height="458" width="636"></amp-img>

      *Bash Script*
24. Save it.
25. Go back to Terminal
26. Type “source .bash_profile”

      <amp-img src="/assets/images/dev-21.png" alt=".bash_profile" height="472" width="693"></amp-img>

      *source .bash_profile*
27. Test one of the alias by typing one of the aliases like small letter L “l” for “ls -lah”

      <amp-img src="/assets/images/dev-22.png" alt=".bash_profile" height="458" width="680"></amp-img>

      *type l*
28. At this point, The Command Line Tools was successfully installed. (Forgot the screenshot)
29. Go to Terminal and type "git"

      <amp-img src="/assets/images/dev-22.png" alt=".bash_profile" height="458" width="680"></amp-img>

      *Git installed via the Command Line Developer Tools Installation*
30. Relax. Part 1 is done. Yay!
