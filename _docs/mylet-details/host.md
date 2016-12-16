---
title: Mylet host
category: Mylet details
order: 32
---

Developers must specify mylet host fields to integrate MYLE back-end with their apps. See more low level details in [API reference](https://getmyle.github.io/api/#mylet).

The secret must be kept private and is used for security purposes in communication between mylet and MYLE: [https://getmyle.github.io/api/#authorization-header](https://getmyle.github.io/api/#authorization-header)

Note: there two environments when a mylet is run:
1. sandbox when testing a mylet
2. production when a mylet is live

Both of them can be distinguished by presence of `sandbox` query parameter in hook or UI URLs. More about that here: [https://getmyle.github.io/api/#api-hosts](https://getmyle.github.io/api/#api-hosts)