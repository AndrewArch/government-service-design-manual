---
layout: detailed-guidance
title: Addresses
subtitle: 
category: design-and-development-resources
type: resource
audience:
  primary: content-designers, designers
type: guide
status: draft
breadcrumbs:
  -
    title: Home
    url: /service-manual
  -
    title: User centered design
    url: /service-manual/user-centered-design
---

How you choose to capture addresses depends on what you want to do with them and which geographical regions you need to support. We'll discuss three approaches here:

1. **[Free text box](#free-text-box)**
2. **[Multiple fields](#multiple-fields)**
3. **[Address finder](#address-finder)**

<h2 class="heading-36" id="free-text-box">1. Free text box</h2>

A single, multi-line text box where users write out the address in full.

<h3 class="heading-24">Pros</h3>

* It can handle any possible address format
* People can copy and paste addresses from the clipboard
* People don't have to work out which part of the address goes in which field

<h3 class="heading-24">Cons</h3>

* Parsing addresses for sub-parts (region, street etc.) is hard, and impossible to do with 100% accuracy
* Many legacy back-end systems expect multi-field addresses

<h3 class="heading-24">Guidance</h3>

Use when you're expecting a very broad range of address formats and you don't need to use specific sub-parts of the address.


<h2 class="heading-36" id="multiple-fields">2. Multiple fields</h2>

The address is broken down into multiple fields. Here's an example that works for simple UK addresses:


<h3 class="heading-24">Pros</h3>

* You can easily extract the parts of an address and do things with them
* You can give help for or validate each part of the address separately
* Works well with browsers that have auto-complete enabled


<h3 class="heading-24">Cons</h3>

* Hard to find a single format that works for a broad range of regions
* No guarantee that people will use the fields as you intended
* Can't easily paste addresses from the clipboard

<h3 class="heading-24">Guidance</h3>

Only use multiple address fields when you know which regions the addresses will come from and can find a format that supports them all.

<h4 class="heading-19">UK addresses</h4>

* 'postcode' is one word
* let people enter postcodes with or without spaces
* avoid making individual fields mandatory (but warn users if they don't fill in any fields)
* Royal Mail do not need a county as long as the town and postcode are included
* include a county field though - it lets people who don't know their postcode give a valid address
* make the field lengths appropriate - it helps people understand the form


<h2 class="heading-36" id="address-finder">3. Address finder</h2>

Sometimes referred to as 'postcode lookup'. An address finder lets users specify a UK address by inputing their postcode (and optionally street name or number) and selecting the address from a list.

Here's how this pattern was implemented on the [Lasting Power of Attorney](https://lastingpowerofattorney.service.gov.uk/) service.

<h3 class="heading-24">Pros</h3>

* People entering UK addresses don't have to enter as much information
* Reduces the chance of mis-typed UK addresses

<h3 class="heading-24">Cons</h3>

* Requires greater effort to implement

<h3 class="heading-24">Guidance</h3>

* Make it clear that the address finder only works for UK addresses
* Provide a manual option for people with international adresses or addresses that are missing or badly formed in the Royal Mail database


---

[Discuss this page on Hackpad](https://designpatterns.hackpad.com/Addresses-CgrMSGRAhRc)
