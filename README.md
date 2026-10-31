# NeuroMail — private email, no identity needed
Web app for NeuroMail, the email service of the Neuronus ecosystem.
# NeuroMail — private email, no identity needed

**Web app for NeuroMail, the email service of the Neuronus ecosystem.**

`React` · `Web app` · [mail.neuronus.net](https://mail.neuronus.net) · `License: Apache 2.0`

> [!IMPORTANT]
> **This repository contains the web interface only.** The mail server, its settings and all keys are not part of it.

---

## What NeuroMail is

NeuroMail is email you can open without telling anyone who you are.

To sign up, you don't give a name, a phone number or another email address. Your device creates 16 random words. These words are your account. You use them to sign in, and nobody else has them, not even us.

The same 16 words open every Neuronus tool: NeuroDrive, Resonance, NeuroBrowser and more. One account, one sign-in.

## Features

- **No identity to sign up.** No name, no phone number, no other email address. Just 16 words created on your device.
- **Pick your address.** Get an address on `neuronus.net`, `neuronus.cloud` or `neuronus.ai`.
- **More than one address.** Use a different address for work, shopping and sign-ups. If one leaks, the others stay clean. <!-- TODO: confirm aliases / extra addresses work in this build -->
- **Encrypted mail between NeuroMail users.** Your message is encrypted in your browser before it is sent. Only the person you write to can open it. <!-- TODO: confirm in code before publishing -->
- **PGP for everyone else.** Write to people outside Neuronus with PGP, the long-standing standard for encrypted email.
- **Works with any email.** Send to and receive from Gmail, Outlook and any other provider.

## What encryption hides, and what it does not

We want to be clear about this.

| | Stays private | The mail system can see |
|---|---|---|
| Mail between NeuroMail users | The text and attachments | Who wrote to whom, and when |
| Mail sent with PGP | The text and attachments | Who wrote to whom, and when |
| Normal mail to Gmail, Outlook and others | Nothing after it arrives | Everything. The other provider can read it, like any normal email. |

Every email system needs the sender, the receiver and the time to deliver a message. This is how email works, at every provider. Don't put private details in the subject line. <!-- TODO: confirm whether subject lines are encrypted between NeuroMail users -->

## How it fits into Neuronus

Neuronus is the Encrypted Workspace: email, files, chat, documents and more, under one account. NeuroMail is the email part.

- **NeuroDrive** — encrypted file storage
- **Resonance** — messenger with a built-in wallet
- **NeuroBrowser** — private browser

## What's in this repository

**Included:** the web interface. Sign up and sign in, inbox, sent, spam, writing messages, managing your addresses, settings.

**Not included:** the mail server, server settings, DNS records, API keys, user data.

## Getting started

Requirements: Node.js 18 or newer. <!-- TODO: confirm Node version and package manager (npm / pnpm / yarn) -->

```bash
npm install
npm run dev     # start for development
npm run build   # build for production
```

Settings: copy `.env.example` to `.env` and add the address of your backend. <!-- TODO: confirm file and variable names. Never commit a real .env. -->

Without a backend, the app opens and you can click through every screen, but it cannot send or receive mail.

## Reporting a security problem

Please don't open a public issue. Write to <!-- TODO: security contact address --> and tell us what you found and how to repeat it.

## Related

- [NeuroDrive](https://github.com/<!-- TODO org -->/neurodrive) — encrypted file storage
- [Resonance](https://github.com/<!-- TODO org -->/resonance) — messenger with a built-in wallet
- [Neuronus Computing](https://github.com/<!-- TODO org -->) — the full ecosystem

## License

Licensed under the **Apache License, Version 2.0**. See [LICENSE](LICENSE) for the full text.

Copyright © 2026 Neuronus Computing.

You may use, copy, change and share this code, including for commercial use, under the terms of the license.

**Names and logos are not included.** "Neuronus", "NeuroMail" and their logos are trademarks of Neuronus Computing. The license does not give permission to use them (section 6 of the license). If you publish a changed version, give it a different name and logo.
