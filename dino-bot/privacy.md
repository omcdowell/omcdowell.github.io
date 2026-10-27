---
title: DinoBot privacy policy
permalink: /dino-bot/privacy
---

# DinoBot privacy policy

Last updated: 27 October 2026

DinoBot is an iPhone app that lets you chat with AI bots that run on **your own computer**. This policy explains what the app does with your information. It covers the DinoBot iPhone app and the DinoBot software you install on your computer.

**In short:** your chats, files and settings stay on your phone and your own computer. We (the publisher, omcdowell) do not run a server that receives them. There are no accounts to create, and the app has no advertising, analytics, tracking or crash-reporting code. We receive nothing about you from the app.

## How DinoBot works

1. You install the DinoBot software on your own Mac or Linux computer.
2. You connect your iPhone to that computer over **Tailscale**, a private network you set up with your own Tailscale account. DinoBot only connects through Tailscale. It does not use a relay server run by us.
3. Your bots run on your computer, using the AI service you choose (see "Your AI provider" below).

Tailscale encrypts the connection between your phone and your computer. Tailscale's own privacy policy covers your use of Tailscale.

## What we collect

Nothing. We do not collect, receive or store your name, email address, contacts, location, chat messages, files, voice recordings, usage statistics, advertising identifiers or device identifiers. There is nothing to sign up for.

## What stays on your phone

The app keeps the following in its own private storage on your iPhone:

- **Your paired computers:** the name you gave each one, its Tailscale address, and the connection password that was in the pairing code.
- **A copy of recent chats**, so they open quickly and can be read when you are offline.
- **Your app settings**, such as which setup steps you have finished and your display preferences.
- **Small bot pictures** for the Live Activity on the Lock Screen, kept in storage that only DinoBot and its widget can read.
- **A notification token**, if you allow notifications (see "Notifications" below).

All of this is deleted when you delete the app.

## What goes to your computer

The app sends the following **only to your own computer**, over Tailscale:

- **Messages, photos and files** you send to your bots, and any files you open or download from your computer in the app.
- **Voice recordings for dictation**, when you hold the microphone button. Audio streams to your computer and is turned into text there, by a speech model running on your computer. The app does not keep the audio.
- **Sign-ins for your AI provider.** When you sign in during setup, the sign-in happens on your computer. Your phone only shows you the code or page to approve. The sign-in is stored on your computer. Your phone never stores it.

Your bots' chats, memory and settings are stored on your computer.

## Phone permissions

- **Camera:** only to scan the pairing QR code. No pictures are kept or sent.
- **Photos:** only the photos you pick to send to a bot. iOS lets you pick them without giving the app your whole library.
- **Microphone:** only while you use dictation or voice. The app may keep recording while the screen is locked if you started dictation before locking it.
- **Notifications:** asked for after your first bot reply, not before. You can say no and still use the app.

## Notifications

If you allow notifications, the app gives your computer a notification token. When a bot sends you a message while the app is closed, **your computer** sends the notification through **Expo's push service** (expo.dev), which passes it to **Apple's Push Notification service**. To do this, Expo and Apple handle the notification token and the notification itself: the bot's name and the start of its message. Their own privacy policies apply. We do not run a notification server and do not see your notifications.

The Live Activity (busy bots on the Lock Screen) updates only while the app is open. Those updates go directly from your computer to your phone over Tailscale.

## Your AI provider

Your bots use an AI service that you choose and sign in to, for example Anthropic (Claude), OpenAI (ChatGPT or Codex), GitHub Copilot or OpenRouter. When a bot works, **your computer** sends your messages, any files the bot reads, and the bot's instructions and memory to that provider, using your own account. That provider's terms and privacy policy apply. We never see this traffic. The app on your phone never contacts an AI provider itself.

Using a Claude login in DinoBot may be billed by Anthropic as extra usage on your Claude account.

## What else the DinoBot software on your computer contacts

So that it can work, the DinoBot software on your computer also:

- downloads DinoBot updates and its speech model from public download sites (for example GitHub);
- fetches the current list of AI models from pi.dev, the model catalogue used by the pi agent that DinoBot is built on;
- may send search queries and web addresses to a web search or page-reading service (by default Exa and Jina) when a bot searches the web for you.

None of these services receive anything from us, and we receive nothing from them about you.

## Network test

The app's Network page has a **Test network** button. Only when you tap it, the app checks your internet connection by contacting Cloudflare (1.1.1.1) and Google (8.8.8.8 and google.com). Those companies see your phone's IP address, as with any website. Nothing else is sent. The app never runs these checks by itself.

## Sharing and selling

We do not sell, rent or share personal information, because we do not receive any. Information leaves your phone and your computer only to go to the services described above: your AI provider, Tailscale, and, for notifications, Expo and Apple.

## Keeping and deleting your information

You control everything:

- **On your phone:** delete the app, or remove a computer in the app's settings.
- **On your computer:** delete a bot in the app, or uninstall the DinoBot software and delete its folders.
- **With your AI provider:** that provider keeps information according to its own policy. You can manage it in your account with them.

## Children

DinoBot is not meant for children under 13, or the minimum age for digital services in your country, and we do not knowingly collect information from children.

## Changes to this policy

If this policy changes, we will update this page and the date at the top. We will mention significant changes in the app's release notes.

## Contact

For questions about this policy, or to report a security or privacy problem, use **GitHub private vulnerability reporting** on the public repository that hosts this page: [github.com/omcdowell/omcdowell.github.io/security](https://github.com/omcdowell/omcdowell.github.io/security) → "Report a vulnerability". Reports are private between you and the maintainer.
