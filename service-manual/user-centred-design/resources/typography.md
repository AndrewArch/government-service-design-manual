---
layout: detailed-guidance
title: Typography
subtitle: Creating clear, easy to read type for the web
category: design-and-development-resources
type: resource
phases:
  - alpha
  - beta
  - live
audience:
  primary: designers
status: draft
breadcrumbs:
  -
    title: Home
    url: /service-manual
  -
    title: User centred design
    url: /service-manual/user-centred-design
---

Services should use clear, easy to read type, with consistent styles and a clear hierarchy of information.

## The GOV.UK typeface

GOV.UK uses the typeface New Transport, created especially for government use. This typeface is embedded in the GOV.UK CSS and is served to browsers via a WOFF file (or an EOT file for Internet Explorer 8). The font is hinted to display well on all browsers. Older browsers do not receive the typeface.

We currently use two weights of New Transport: Light and Bold. Italics should not be used. The number of different type sizes on a page should be kept to the minimum, and only one typeface/font should be used on each website.

## Using New Transport

New Transport is not licensed for use outside of the GOV.UK domain. When your service goes live you'll be given access to the typeface.

If the service uses numbers in columns or tables, you should change these to use the tabular numbers version of New Transport. This replaces the standard numbers with new versions that have a fixed width. The main noticeable difference is a base on the character 1. GDS has used this on the [Performance Platform](/performance) and [Trade Tariff](/trade-tariff).


## Colour contrast

Text must have enough contrast against the background colour to be readable. This should be tested to conform with our [accessibility requirements](/service-manual/user-centred-design/accessibility). Generally we use type in #0B0C0C against a white or light grey background. Links should be blue and underlined, as mentioned in our guidance on [colour palettes](/service-manual/user-centred-design/resources/colour-palettes).

## Type size

Type should be large enough to be easily read. This is generally larger than many current websites: 36px for headlines, 19px for body text. This can be included using default styles in Sass from the [GOV.UK Frontend Toolkit](/service-manual/user-centred-design/resources/sass-repositories). These include line height spacing that works across browsers.


##Further reading

* [A blog post from Ben Terrett on why we chose New Transport](https://gds.blog.gov.uk/2012/07/05/a-few-notes-on-typography/)
* [Shared asset libraries](/service-manual/user-centred-design/resources/shared-asset-libraries)
