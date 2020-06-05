---
layout: post
title: Track USCIS Case with Python
---

Recently I am waiting for my OPT application to get approved by USCIS.
I need a CLI program, which can track USCIS case status and email me once the status changes.
So I created a small [Python project](https://github.com/zhangyaqi1989/USCIS-Case-Tracker).


Basic usage is listed as follows.

## 1. Check a range of receipt numbers

```bash
python uscis.py -s YSC2090175300 -n 10 -v -r
```

The above code checks status of receipt numbers from
YSC2090175300 to YSC2090175309.

-n is used to set number of receipt numbers tracked.

-v is used to print status of each receipt number to CLI.

-r is used to print pass ratio to CLI.

## 2. Watch one or more receipt numbers and email a message when status changes

```bash
python watch.py
```

You need to put receipt numbers to src/receipts.data (one number per line) and an email address to src/email.data.
