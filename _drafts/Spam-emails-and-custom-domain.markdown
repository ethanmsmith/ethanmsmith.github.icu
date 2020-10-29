---
layout: post
title:  "Spam Email and Custom Domain"
date:   2020-11-1
categories: email forwarding custom domain
permalink: :slug
---
I was getting way too many spam emails (both at work and personal email) that I got fed up. Inspired by the age old method of using a companies name as your middle name when signing up for mailing lists, coupons, new accounts, etc. and wanting to [de-google][deGoogle] as much as possible (I still use Android), I decided to use a custom domain and email forwarding to track which companies sell my email and to whom.

One of the first uses I had for this was when I started looking into graduate schools and I signed up for information from Syracuse. A few months later and I received an email to `syracuse@ethansmith.io` from UC Berkley. Right away I could see my idea paying off. Since then, I have been slowly combing through the list of sites I have accounts with and have changed the email on the accounts to `websitename@ethansmith.io`. 

## I see this as having multiple benefits:
1. __My email accounts on sites are now unique__  
If there is a data breach on Netflix, for example, my email is still safe from a brute force attack on Hulu. Coupled with a password manager like bitwarden, my accounts are all unique and have long, secure pass phrases.
2. __I don't have to use a "spam email" and remember which site uses which email address__  
Prior to using this method, I would use my old email address from middle school for sites that I did not care about or that I did not want to have my primary email. This led to me not remembering which email I was using for a specific site and caused me to have to go through password recovery processes.
3. __My online accounts are now email provider agnostic__  
If I want to stop using gmail and switch over to a more privacy focused email provider such as Protonmail, I do not have to update my email information on multiple accounts or create a forwading rule in Gmail to my new email (thus defeating the purpose of switching away from Gmail altogether).
4. __I can use a deny or allow list on incoming emails to block any offending emails__  
If one site starts selling my data to everyone and their cousins, I can simply block that email. Alternatively, if a bad actor decides to sign me up for multiple different spam sites using a few different alias, I can simply create an allow list of my known aliases in my email client or set up individual aliases for each website (up to 100 for free on Name Cheap and Google Domains)

## Steps to replicate with Google Domains (Ironic, I know)
I use google domains, but the steps are similar for other domain hosts
1. Navigate to your domain settings and select email from the left hand navigation
![Google Domains Email][googleDomainsNavigation]
2. Click add alias
3. For the alias, put in an asterisk and for forwarding address, put in the email you want to forward to.
![Add email alias][genericEmailAlias]

## NameCheap is even easier
1. Choose manage next to the domain name you want to set up forwarding on.
2. Scroll down to "Redirect Email" and choose "Add Catch-All"
![Add Catch-All Email Forward][catchAllEmail]

[deGoogle]: https://www.reddit.com/r/degoogle
[catchAllEmail]: /assets/NameCheap - Email.png
[genericEmailAlias]: /assets/Add email alias.png
[googleDomainsNavigation]: /assets/Google Domains - Email.png