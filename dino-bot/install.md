---
title: Setting up DinoBot
permalink: /dino-bot/install
---

# Setting up DinoBot (test version)

DinoBot is in a small private test. If you have been invited, you will receive your own
**step-by-step setup guide** and the install command privately, together with your invitations.
This page gives an overview so you know what to expect.

## What you need

- **A Mac** with macOS 13.5 or newer. Macs with an Apple chip are tested.
- **An iPhone** with the **TestFlight** app (free, from the App Store).
- **Your invitations**, sent to you privately:
  1. a TestFlight email: "You're invited to test DinoBot";
  2. a personal **download key**. It only lets your Mac download DinoBot (it can read, never
     change anything) and stops working after 30 days. Treat it like a password.
- **A Tailscale account** (free, from [tailscale.com](https://tailscale.com)). You can sign in with Google, Apple or Microsoft.
- **An account with an AI service** for your bots, for example Claude (Pro or Max).

Keep the Mac switched on and logged in while you use DinoBot: when it is asleep or off, the bots
can't answer. In the first hour DinoBot also downloads about 1 GB of voice models, so use a good
connection.

## How setup works

The first setup takes about 15 minutes.

1. **Get the app.** Accept the TestFlight invitation on your iPhone and install DinoBot.
2. **Set up Tailscale** on the Mac and the iPhone, logged in with the same account on both.
3. **Install DinoBot on the Mac.** Open Terminal and paste the lines from your setup guide. The
   installer checks that the download is genuine and installs nothing if the check fails. It
   then shows a QR code.
4. **Connect the iPhone.** Open DinoBot and scan the QR code. The app then helps you sign in to
   your AI service and pick models.
5. **Say hello.** Your first bot should answer within a minute.

## If something goes wrong

Run `~/.dinobot/bin/dinobot doctor` in Terminal and send everything it prints to the person who
invited you, with a screenshot of where it stopped.

Never send anyone the QR code, your download key, or the files in `~/.dinobot/secrets/`,
`~/.dinobot/daemon.env` and `~/.dinobot/pi/auth.json`: they contain your passwords and keys.

## Removing DinoBot

Run `~/.dinobot/bin/dinobot uninstall --purge` in Terminal, then delete the app from the iPhone.

See also the [privacy policy](privacy).
