---
title: Vulns 1001 Notes
date: 2020-09-15T11:30:03+00:00
tags:
  - kfs
author: mugurel
showToc: true
TocOpen: false
draft: false
hidemeta: false
comments: false
description: Desc Text.
canonicalURL: https://canonical.url/to/page
disableHLJS: false
disableShare: false
hideSummary: false
searchHidden: true
ShowReadingTime: true
ShowBreadCrumbs: true
ShowPostNavLinks: true
ShowWordCount: true
ShowRssButtonInSectionTermList: true
UseHugoToc: true
cover:
  image: <image path/url>
  alt: <alt text>
  caption: <text>
  relative: false
  hidden: true
editPost:
  URL: https://github.com/ft-mugurel/blog/content/
  Text: Suggest Changes
  appendFilePath: true
---
# 01
# Vulnerability Types
- Heap out of bounds
- Use after free
- Taype confusion
- uninitialized use 

# Terms
## ACID (Atacker Controlled Input Data)
- ACID is a term used to describe the input data that an attacker can control.
## Shellcode 
- Shellcode means a piece of code that an attacker wants user to execute.
## Exploit Primitives
- Exploit primitives are the basic building blocks of an exploit. They are the fundamental techniques that an attacker can use to gain control of a system or application.
### Example 
- Overite of return adress
- Overite of other local varibales
- Overite of heap data
## Exploit Chain
- This means that an attacker can use multiple exploit primitives together to create a more complex exploit.
## Zero Day
- A zero-day vulnerability is a security flaw that is unknown to the vendor and has not been patched. Attackers can exploit these vulnerabilities before the vendor releases a fix, making them particularly dangerous.
## N-day
- An N-day vulnerability is a security flaw that has been publicly disclosed and for which a patch is available. Attackers can exploit these vulnerabilities if users do not apply the patch in a timely manner.

