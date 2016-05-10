---
layout: default
title: "Privacy and Security"
---
<div class="row"><div class="col-sm-12" markdown="1">

This page describes the way our Telegram bot works with data and permissions, which
become available to it, while serving the end user.

### Messages

The bot is based upon Telegram, so all your messages are secured by its protocol. See [Telegram security][telegram-security] and [privacy policy][telegram-privacy] for more information.

The bot (in its application code) has access to all messages, that are sent to it. This is, obviously, required for bot to function properly. These messages are never stored on our servers, they only determine bot's next reply once. These messages are not processed in any other kind of way.

### Infrastructure

The bot consists of three major components: telegram bot, uber api client and web site (different from current one). 

All components are hosted in a secure Microsoft's Azure cloud, see more on [Azure security][azure-security]. All external communication (telegram, uber, site visitors) is secured by HTTPS. 

Local communication is secured by the Azure cloud itself.

### Uber

The bot uses official Uber API to communicate with Uber. **The bot does not and will never ask to type your passwords for any third party apps, sites, etc** (including Uber and Telegram). 

When authorizing, the password is typed on the Uber official site. The bot will never request rides or do any other communication with Uber API, unless expicitly requested by the end user.

To see details, check [Uber docs][uber-docs],
which we used as a primary guide.

[telegram-security]: https://telegram.org/faq#security
[telegram-privacy]: https://telegram.org/privacy
[azure-security]: https://www.microsoft.com/en-us/TrustCenter/Security/AzureSecurity
[uber-docs]: https://developer.uber.com

</div></div>