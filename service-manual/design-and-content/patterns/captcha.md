---
layout: detailed-guidance-2
title: CAPTCHA
category: design-and-development-resources
type: resource
audience:
    primary: designers, developers
    secondary:
status: draft
phases:
  - alpha
  - beta
  - live
page_class: buttons
breadcrumbs:
  -
    title: Home
    url: /service-manual/index.html
  -
    title: Design and content
    url: /service-manual/design-and-content/index.html
  -
    title: Design patterns
    url: /service-manual/design-and-content/patterns/index.html
---

{:.intro}
Avoid using this technique if at all possible.

## What is it?

[CAPTCHA](http://en.wikipedia.org/wiki/CAPTCHA) stands for Completely Automated Public Turing test to tell Computers and Humans Apart. These are usually images of jumbled up text that a user needs to decipher and enter before submitting a form. 

<div class="example">  
    <img src="/service-manual/assets/images/design-patterns/captcha.jpg" alt="Example of a CAPTCHA">
</div> 

CAPTCHAS are typically used to prevent automated software (bots) from completing a form or accessing a system.

---

## Why shouldn't I use one?

CAPTCHAs introduce significant problems to online services:

* **usability** - they put the burden of detecting bots on the user rather than the system. As CAPTCHAs are designed to be hard to read and understand, this makes the service much more difficult to use.

* **accessibility** - they are inaccessible by design. This effectively makes the service unusable by people with certain disabilities. Even CAPTCHAs that provide audio versions do not completely resolve this issue.

Additionally, if a 3rd party CAPTCHA service is used, there are further problems to consider:

* **privacy** - 3rd party CAPTCHA services set cookies, collect analytics and can track users across multiple sites. This introduces significant privacy concerns.
* **performance** - use of a 3rd party CAPTCHA service ties your performance to theirs. If their service goes offline, so does access to your service.
* **security** - the security of your service is tied to that of the 3rd party. If they are compromised, so is your service and its users.

---

## Alternatives to CAPTCHA

Many of the risks that CAPTCHAs are aimed to mitigate can be addressed in other ways:

* rate and connection limiting
* use of honey pots
* protective monitoring

It's important to note that even with a CAPTCHA in place bots will still get through due to advances in computer imaging and the use of CAPTCHA farms. A combination of different approaches generally gives the best results.

---

## Further reading

* [In search of the perfect CAPTCHA](http://coding.smashingmagazine.com/2011/03/04/in-search-of-the-perfect-captcha/)
* [CAPTCHA and the BBC](http://www.bbc.co.uk/blogs/bbcinternet/2010/10/captcha_and_bbc_id.html)
* [Ticketmaster ditches CAPTCHA for something simpler](http://thenextweb.com/insider/2013/01/30/good-news-music-fans-ticketmaster-is-ditching-its-captcha-conundrums-for-something-simpler/)