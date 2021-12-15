---
layout: post
author: perry
title: Stock in the Chip Shortage
description: Where'd it all go?
summary: How to find it
tags: [imu, arduino]
date: 2021-12-14 20:41:18 -0800
---
# The Chip Shortage Is Real.

There's no doubt about it. From decades-long lead times to 
maximum-stock limits on popular chips, the effect of the
global pandemic on supply chains is being felt worldwide.

In the midst of such n serious silicon scarcity, what is the
humble hobbyist to do?

![Improvise, Adapt, Overcome](https://wompampsupport.azureedge.net/fetchimage?siteId=7575&v=2&jpgQuality=100&width=700&url=https%3A%2F%2Fi.kym-cdn.com%2Fentries%2Ficons%2Foriginal%2F000%2F023%2F987%2Fovercome.jpg)

---
<br>

# Finding Stock in a Stockless World

We've all felt it by now, the seemingly endless hours of scrolling,
searching, trying new filters, only to see the last few items of that
seemingly perfect component snatched by an unseen hand. Finding
stock is hard enough *without* a global chip shortage, so here's a
few tips for getting those parts you still need:

1. **Search every supplier you can**  
DigiKey, Mouser, Arrow, Newark, anyone you can get search terms in.  
Alternatively, search [octopart](https://octopart.com/) for many distributors at once.

2. **Don't restrict yourself to one package**  
Many components come in a range of package styles, such as a mixture of SOIC
and USON/WSON for flash chips, or QFPs & QFNs for most microcontrollers.
Apart from their footprints & dimensions, these part variants often have
the same pin assignments as their package relatives, and can be directly
swapped in (albeit, with a change of footprint) in lieu of other stock.

3. **If all else fails, find pin-compatible replacements**  
Some components just don't have alternate packages, or maybe they're out of stock
too. In that case, you might be able to find similar components using a
supplier's parametric search tool. Some suppliers, like DigiKey most recently,
even offer suggestions for replacements in clear view when searched
components have no stock. A mixture of compatible replacements and different
packages may have luck too.

<br>

## Sometimes, failure is inevitable.

No matter how far you search or how many alternatives you consider, there are
a number of specialized or otherwise hard-to-find components that are just simply
unavailable in the current state of the supply chain. Some designs can be reworked
to accomodate different solutions, but some will just have to wait, and hope, for
the shortage to end soon.
