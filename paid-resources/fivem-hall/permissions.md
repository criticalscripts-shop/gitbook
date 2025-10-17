---
description: Learn how to update the permissions of the resource.
---

# Permissions

The UI is accessed via the `/hall` command while inside an enabled hall location for players with Ace permission `cs-hall.control`. This check and how the UI is accessed can be changed by modifying `cs-hall/integration/client.lua` and `cs-hall/integration/server.lua` files. There is also an identifier-based check in parallel to Ace permission which can also be edited in `cs-hall/integration/server.lua` file to add any player identifiers you want.

**You may also find some ready-to-use framework-related integrations in our** [`extra-hac` GitHub](https://github.com/criticalscripts-shop/extra-hac/tree/main/cs-hall/integration)**.**
