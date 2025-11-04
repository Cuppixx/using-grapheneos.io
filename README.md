# Using [GrapheneOS](https://grapheneos.org)

<p align="center">
  <a href="https://grapheneos.org"><img src="https://img.shields.io/badge/GrapheneOS-blue" /></a>
  <a href="https://github.com/GrapheneOS"><img src="https://img.shields.io/badge/Source-blue" /></a>
  <a href="https://grapheneos.org/releases#2025102800"><img src="https://img.shields.io/badge/On%20GOS%20Build-2025102800-blue" /></a>
  <img src="https://img.shields.io/github/last-commit/Cuppixx/Using-GrapheneOS?label=Using%20GrapheneOS%20last%20edited&color=blue" />
</p>

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
| **Obsidian**        | Markdown-based note-taking; syncs across devices via Syncthing-Fork |
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
| **Banking**                 |  My local banking app — not listed by name for obvious reasons |
| **Crunchyroll**             |  |
| **Discord**                 | Used for social reasons (contacts, gaming and dev communities) |
| **Joyn**                    | TV/streaming app for live content |
| **Loxone**                  | Smart home / security control app; work requirement |
| **Malwarebytes**            | On-demand malware scanning for peace of mind |
| **Mobile Games**            | A few games for when I'm traveling (Gwent, KARDS, Fallout Shelter, etc. ...) |
| **Netflix**                 |  |
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

I did however install **OpenScan** to complement the default **Camera** app, since GrapheneOS doesn't include document scanning out of the box. Beyond that, the camera app works fine for my needs. That said, I'm not a photography enthusiast or heavy picture-taker — so if you have a favorite camera app with better image quality or features that meet your requirements, don't hesitate to replace the default. GrapheneOS's camera is solid for basic use, but it's not trying to compete with flagship camera apps.

Special mention goes to **Vanadium**, the hardened default browser. It strikes a great balance between usability and security. I haven’t felt the need to replace it with something like Brave — which offer more features, sure, but also comes with more settings bloat. Vanadium just works, securely and comfortably.

Among the third-party FOSS apps, there’s a core group I consider essential for a security-hardened setup:

- **Aegis** – for managing 2FA codes securely
- **Bitwarden** – for password management
- **Malwarebytes** – for on-demand scanning (not always active)
- **Orbot** – for routing traffic through Tor when needed

These four cover a lot of bases when it comes to digital hygiene and peace of mind.

GrapheneOS doesn’t ship with voice input out of the box, and most keyboards either require network access or lack features. That’s why I use **FUTO Keyboard** — it offers offline speech-to-text, solid typing feel, and a fully local privacy model. It’s one of the few keyboards that hits the sweet spot of usability and privacy.

**Obsidian + Syncthing-Fork** deserves a special mention as one of the best privacy-respecting productivity setups I've found. Instead of paying for Obsidian's premium sync service, I use Syncthing-Fork to handle vault synchronization across all my devices — completely free, peer-to-peer, and with no cloud middleman. You get full control: sync your entire vault, cherry-pick specific folders, or set up multiple sync configurations. It's fast, reliable, and keeps everything local-first. Add plugins like Excalidraw for visual thinking and Kanban boards for task management, and you've got a surprisingly powerful low-overhead system for planning, mapping ideas, and staying organized — all without recurring subscriptions or third-party servers touching your data.

**Tailscale**, **KDE Connect**, and **Syncthing-Fork** form a powerful, privacy-respecting trinity for seamless device interaction, file sharing, and remote access. Tailscale creates a secure mesh VPN across all your devices — phone, laptop, desktop, or server — allowing direct, encrypted communication over the internet or local network, without requiring port forwarding or exposing devices publicly. KDE Connect bridges Android and Linux devices over the same network (or via Tailscale), enabling clipboard sync, file transfers, notifications, and even remote input, making day-to-day phone-to-desktop integration smooth and convenient. Syncthing-Fork handles continuous, peer-to-peer file synchronization over local networks or Tailscale, keeping folders in sync between devices in a fully encrypted, self-hosted way, ideal for backups, project sharing, or media libraries. Together, these three apps replace many proprietary cloud services, providing a fully local, encrypted, and self-controlled ecosystem for file sharing, device connectivity, and remote access.

**Thunderbird** is still relatively new on mobile as of writing this. It merged with **K-9 Mail**, though both remain available as separate apps. While Thunderbird is coming along nicely, if you feel dissatisfied or just want to explore your options, K-9 Mail is still actively maintained and worth considering — in fact, some users may find it even more polished for mobile use at this stage.

A few other FOSS apps that really impressed me:

- **NewPipe** is an excellent YouTube frontend — works great overall, though it can get a bit clunky when routing through a VPN.
- **OpenReads** was a pleasant surprise; I'd never used a book-tracking app before, but if you read regularly, it's absolutely worth trying.
- **Organic Maps** — as someone who relied exclusively on Google Maps for years, I was genuinely surprised by how well it performed.

All three are solid enough that I'd recommend them for daily use, even if you're not running GrapheneOS.

Among the proprietary apps, many are essential — online banking, contactless payments, and communication tools are hard to avoid. Others, like streaming services or mobile games, are entirely optional depending on your lifestyle. Then there are apps that fall somewhere in between, where your needs may vary: Proton Calendar and Tailscale are good examples, though both are among the most privacy-respecting proprietary options available.
But the one app I haven't found a satisfactory replacement for is **Spotify**. If you have Spotify Premium, it's hands down the best music streaming experience on mobile — nothing else comes close in terms of library size, discovery features, and overall usability. Without Premium, though, the mobile app is nearly unusable. If you're already paying for it, there's no better option out there.
