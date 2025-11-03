# Using GrapheneOS

Welcome to **Using GrapheneOS**, a personal collection of notes, apps, configs, and insights from my experience using GrapheneOS as a daily driver.

While the web is full of reviews, this repo aims to cut through some of the noise and give yet another, user-level perspective.
I’ll cover the open-source apps I rely on, the commercial software I haven’t found good open-source replacements for, the settings and tweaks I personally like, and even the small annoyances that come up along the way.

Whether you're considering switching to GrapheneOS, already jumped ship, or just curious about using a _privacy-focused, de-googled Android fork_ — this hopefully helps to get some insights.

## 🧭 What You’ll Find Here

- A curated list of all the apps I use and what I use them for
- My personal GrapheneOS setup: settings, features, and configuration
- Some notes on what works well and what doesn’t
- Some tips, workarounds, and mini-guides based on experience

### ⚠️ Heads-Up

Before getting into the first major topic, I want to clear up a common misconception about GrapheneOS. While it’s well-known as a _privacy-focused Android fork_, **you don't need to be a hardcore privacy enthusiast to benefit from using it**.

Yes, GrapheneOS is built with strong security and privacy principles at its core — but that doesn’t mean you _must_ give up Google services or only use open-source apps to enjoy it. In fact, **you can absolutely use GrapheneOS while still relying on Google apps and other proprietary software**, and it works just fine.

I personally use GrapheneOS in a pretty casual way. I do appreciate the built-in privacy and security features, but I'm also perfectly fine with using the Google Play Store — thanks to GrapheneOS’s _sandboxed Google Play compatibility layer_ — for a good chunk of my apps.

But the **number one reason** I stick with GrapheneOS — tho this applies to most custom Android OSes — is how **clean** it is. No bloat, no preinstalled junk I didn’t ask for (and can't remove - looking at you, Facebook) and no forced usage of certain apps. Just a fast, minimalist system that stays out of my way. And best of all, no more mysterious background processes eating up resources with no explanation. **My phone runs what I tell it to run — nothing more, nothing less**.

## 📦 Apps I Use – Overview

Here’s a quick breakdown of all the apps I currently use on my GrapheneOS device, what category they fall into, and what I use them for.

### 🟩 Native GrapheneOS Apps

These are the system apps that come pre-installed with GrapheneOS. They're sandboxed, secure, and cover most basic functions.

| App            | Description |
|----------------|-------------|
| **App Store**  | Install trusted - core - apps (including sandboxed Play Services). Very limited otherwise |
| **Auditor**    | Verifies device integrity and security |
| **Calculator** |  |
| **Camera**     | Secure default camera app; lacking some features like document scanning |
| **Clock**      | Alarm, timer, stopwatch, and world clock |
| **Contacts**   |  |
| **Files**      | Basic file manager with storage access framework |
| **Gallery**    | Very bare bones, lacking most features |
| **Info**       |  |
| **Messaging**  |  |
| **PDF Reader** |  |
| **Settings**   |  |
| **Telephone**  |  |
| **Vanadium**   | Hardened browser based on Chromium; optimized for privacy |

### 🟩 OpenSource Apps

Chosen to replace proprietary tools and Add, Expand or Replace functionality on GrapheneOS.

| App                 | Description |
|---------------------|-------------|
| **Aegis**           | 2FA code manager; secure, open source alternative to Google Authenticator |
| **AvesLibre**       | Lightweight and privacy-friendly gallery |
| **Bitwarden**       | Password manager; secure cloud sync with open source backend |
| **Breezy Weather**  | Reliable weather app |
| **FUTO Keyboard**   | Privacy-respecting keyboard; no network access and local speech to text AI |
| **KDE Connect**     | Cross-device sync and file sharing between Android and Linux desktops |
| **Mastodon**        | Decentralized social media client |
| **NewPipe**         | YouTube frontend; ad-free, background playback and downloads |
| **Obtainium**       | Install and update FOSS apps directly from GitHub |
| **OpenReads**       | Lightweight book-/read-tracker |
| **OpenScan**        | Scan documents to PDF |
| **OpenTracks**      | GPS tracking for workouts and trips |
| **Orbot**           | Tor routing for apps; useful for privacy or circumventing censorship |
| **Organic Maps**    | Offline maps and navigation |
| **Syncthing-Fork**  | Peer-to-peer file sync; local-first, no cloud needed |
| **Termux**          | Terminal emulator and Linux environment; powerful automation and admin tasks |
| **Thunderbird**     | Full-featured, cross-platform email client |
| **Twire**           | Open source Twitch client |

### 🔒 Proprietary / Closed Source Apps

Used when no equivalent FOSS app meets functionality needs — trade-offs acknowledged.

| App                         | Description |
|-----------------------------|-------------|
| **Banking**                 |  My local banking app - not listed by name for obvious reasons |
| **Crunchyroll**             |  |
| **Discord**                 | Used for social reasons (contacts, gaming and dev communities) |
| **Joyn**                    | TV/streaming app for live content |
| **Loxone**                  | Smart home / security control app; work requirement |
| **Malwarebytes**            | On-demand malware scanning for peace of mind |
| **Mobile Games**            | A few games for when I'm traveling (Gwent, KARDS, Fallout Shelter, etc. ...) |
| **Netflix**                 |  |
| **Obsidian**                | Markdown-based note-taking; syncs across devices via Syncthing-Fork |
| **Paypal**                  |  |
| **Play Games / Play Store** | Sandboxed via GOS |
| **Proton Calendar**         | Encrypted calendar; privacy-first, seamlessly syncs across devices |
| **Spotify**                 |  |
| **Tailscale**               | Mesh VPN; used for remote access and secure networking |
| **Teams**                   | Work requirement |
| **WhatsApp**                | Used for social reasons (contacts, family) |

## 🧠 Apps I Use - Thoughts

Let’s get a few things out of the way.

The default **GrapheneOS App Store** isn't really an "app store" in the traditional sense. Its main purpose is to update GrapheneOS system apps and optionally install sandboxed Google Play Services. Yes, you *can* install [Accrescent](https://accrescent.app/) through it — another FOSS app store — but personally, I’ve never been fully satisfied with either F-Droid or Accrescent.

That’s why I use **Obtainium**. While it's not technically a "store," it's more like a lightweight package manager that pulls APKs directly from trusted upstream sources like GitHub or GitLab. It gives me full control over updates and sources, without relying on middlemen.

As for some of the native apps:

- I’ve never had much use for the **Auditor** or **Info** apps.
- The default **Gallery** app is a rough experience — basic and clunky.
- In contrast, **Aves Libre** has become my go-to media viewer. It feels more like a desktop app, which is a vibe I also appreciate in the **Files** app.

Speaking of Files: one of the things I really like about GrapheneOS is that it doesn’t try to hide the file system. With the default **Files** app, you can easily browse the contents of your device without artificial limitations. That’s rare these days.

The rest of the built-in apps generally do their job well enough that I haven't felt the need to replace them.

Special mention goes to **Vanadium**, the hardened default browser. It strikes a great balance between usability and security. I haven’t felt the need to replace it with something like Brave — which offer more features, sure, but also comes with more settings bloat. Vanadium just works, securely and comfortably.

Among the third-party FOSS apps, there’s a core group I consider essential for a security-hardened setup:

- **Aegis** – for managing 2FA codes securely
- **Bitwarden** – for password management
- **Malwarebytes** – for on-demand scanning (not always active)
- **Orbot** – for routing traffic through Tor when needed

These four cover a lot of bases when it comes to digital hygiene and peace of mind.

GrapheneOS doesn’t ship with voice input out of the box, and most keyboards either require network access or lack features. That’s why I use **FUTO Keyboard** — it offers offline speech-to-text, solid typing feel, and a fully local privacy model. It’s one of the few keyboards that hits the sweet spot of usability and privacy.



