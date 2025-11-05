# Using [GrapheneOS](https://grapheneos.org)

<p align="center">
  <a href="https://grapheneos.org"><img src="https://img.shields.io/badge/GrapheneOS-blue" /></a>
  <a href="https://github.com/GrapheneOS"><img src="https://img.shields.io/badge/Source-blue" /></a>
  <a href="https://grapheneos.org/releases#2025102800"><img src="https://img.shields.io/badge/On%20GOS%20Build-2025102800-blue" /></a>
  <img src="https://img.shields.io/github/last-commit/Cuppixx/Using-GrapheneOS?label=Using%20GrapheneOS%20last%20edited&color=blue" />
</p>

<div align="justify">
Welcome to <b>Using GrapheneOS</b>, a personal collection of notes, apps, configs, and insights from my experience using GrapheneOS as a daily driver.
<br><br>
While the web is full of reviews, this repo aims to cut through some of the noise and give yet another, user-level perspective.
I'll cover the open-source apps I rely on, the commercial software I haven't found good <a href="https://en.wikipedia.org/wiki/Free_and_open-source_software">FOSS</a> or open-source replacements for, the settings and tweaks I personally like, and even the small annoyances that come up along the way.
<br><br>
Whether you're considering switching to GrapheneOS, already jumped ship, or just curious about using a <i>privacy-focused, de-googled Android fork</i> — this hopefully helps to get some insights.
</div>

## 🧭 What You'll Find Here

- A curated list of all the apps I use and what I use them for
- My personal GrapheneOS setup: settings, features, and configuration
- Some notes on what works well and what doesn't
- Some tips, workarounds, and mini-guides based on experience

### ⚠️ Heads-Up

<div align="justify">
Before getting into the first major topic, I want to clear up a common misconception about GrapheneOS. While it's well-known as a <i>privacy-focused Android fork</i>, <b>you don't need to be a hardcore privacy enthusiast to benefit from using it</b>.
<br><br>
Yes, GrapheneOS is built with strong security and privacy principles at its core — but that doesn't mean you <i>must</i> give up Google services or only use open-source apps to enjoy it. In fact, <b>you can absolutely use GrapheneOS while still relying on Google apps and other proprietary software</b>, and it works just fine.
<br><br>
I personally use GrapheneOS in a pretty casual way. I do appreciate the built-in privacy and security features, but I'm also perfectly fine with using the Google Play Store — thanks to GrapheneOS's <i>sandboxed Google Play compatibility layer</i> — for a good chunk of my apps.
<br><br>
But the <b>number one reason</b> I stick with GrapheneOS — tho this applies to most custom Android OSes — is how <b>clean</b> it is. No bloat, no preinstalled junk I didn't ask for and can't remove (looking at you Facebook), and no forced usage of certain apps. Just a fast, minimalist system that stays out of my way. And best of all, no more mysterious background processes eating up resources with no explanation. <b>My phone runs what I tell it to run — nothing more, nothing less</b>.
</div>

## 📦 Apps I Use – Overview

Here's a quick breakdown of all the apps I currently use on my GrapheneOS device, what category they fall into, and what I use them for.

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

*_You can find additional information on GOS and its <a href="https://grapheneos.org/features">features</a> on their webpage._

### 🟩 OpenSource Apps

Chosen to replace proprietary tools and Add, Expand or Replace functionality on GrapheneOS.

| App                 | Description |
|---------------------|-------------|
| **Aegis**           | 2FA code manager; secure, open-source alternative to Google Authenticator |
| **AvesLibre**       | Lightweight and privacy-friendly gallery |
| **Bitwarden**       | Password manager; secure cloud sync with open-source backend |
| **Breezy Weather**  | Weather app |
| **FUTO Keyboard**   | Privacy-respecting keyboard; offline speech-to-text and a local privacy model |
| **KDE Connect**     | Cross-device sync and file sharing between Android and Linux desktops |
| **Mastodon**        | Decentralized social media client |
| **NewPipe**         | YouTube frontend; ad-free, background playback and downloads |
| **Obtainium**       | Install and update FOSS and open-source apps directly from GitHub and co. |
| **OpenReads**       | Book-/read-tracker |
| **OpenScan**        | Lightweight PDF scanner |
| **OpenTracks**      | GPS tracking for workouts and trips |
| **Orbot**           | Tor routing for apps; useful for privacy or circumventing censorship |
| **Organic Maps**    | Offline maps and navigation |
| **Syncthing-Fork**  | Peer-to-peer file sync; local-first, no cloud needed |
| **Termux**          | Terminal emulator and Linux environment; powerful automation and admin tasks |
| **Thunderbird**     | Full-featured, cross-platform email client |
| **Twire**           | Alternate, open-source Twitch client |

### 🧠 OpenSource and Native GrapheneOS Apps - Thoughts

<div align="justify">
The default <b>GrapheneOS App Store</b> isn't really an "app store" in the traditional sense. Its main purpose is to update GrapheneOS system apps and optionally install sandboxed Google Play Services. Yes, you <i>can</i> install <a href="https://accrescent.app/">Accrescent</a> through it — another FOSS app store — but personally, I've never been fully satisfied with either F-Droid or Accrescent.
<br><br>
That's why I use <b>Obtainium</b>. Tho it's not technically an "app store" either and functions more like a lightweight package manager that pulls APKs directly from trusted upstream sources like GitHub or GitLab. It gives me full control over updates and sources, without relying on the middlemen.
<br><br>
As for some of the other native apps:
<br><br>
<ul>
<li>I've never had much use for the <b>Auditor</b> or <b>Info</b> apps, tho they're nice to have.</li>
<li>The default <b>Gallery</b> app is a rough experience — basic and clunky. Thus <b>AvesLibre</b> (or just Aves) has become my go-to media viewer. It feels more like a desktop app, which is a vibe I also appreciate in the <b>Files</b> app.</li>
<li>One of the things I really like about GrapheneOS is that it doesn't try to hide the file system. With the default <b>Files</b> app, you can easily browse the contents of your device without artificial limitations. That's rare these days.</li>
</ul>
The rest of the built-in apps generally do their job well enough that I haven't felt the need to replace them.
<br><br>
I did however install <b>OpenScan</b> to complement the default <b>Camera</b> app, since GrapheneOS doesn't include document scanning out of the box. Beyond that, the camera app works fine for my needs. That said, I'm not a photography enthusiast or heavy picture-taker — so if you have a favorite camera app with better image quality or features that meet your requirements, don't hesitate to replace the default. GrapheneOS's camera is solid for basic use, but it's not trying to compete with flagship camera apps.
<br><br>
Special props go to <b>Vanadium</b>, the hardened default browser. It strikes a great balance between usability and security. I haven't felt the need to replace it with something like Brave — which offer more features, sure, but also comes with more settings bloat. Vanadium just works, securely and comfortably.
<br><br>
Among the third-party open-source apps, there's a core group I consider essential for a security-hardened setup:
<br><br>
<ul>
<li><b>Aegis</b> – for managing 2FA codes securely</li>
<li><b>Bitwarden</b> – for password management, 2FA codes and secure storage</li>
<li><b>Orbot</b> – for routing traffic through Tor when needed</li>
</ul>
These three cover a lot of bases when it comes to digital hygiene and peace of mind.<br>
Orbot is an app you can probably skip if you don't need secure routing, and Aegis isn't necessary unless you use 2FA codes — but Bitwarden should really be a staple in every setup. I personally use Aegis alongside Bitwarden so that if something ever happened to my Bitwarden account, my passwords and 2FA codes wouldn't both be lost at the same time. Plus, I just really like Aegis's design — it feels clean and straightforward. In the end, it mostly comes down to personal preference.
<br><br>
GrapheneOS doesn't ship with voice input out of the box, and most keyboards either require network access or lack features. That's why I use <b>FUTO Keyboard</b> — it offers offline speech-to-text, solid typing feel, and a fully local privacy model. It's one of the few keyboards that hits the sweet spot of usability and privacy.
<br><br>
<b>Thunderbird</b> is still relatively new on mobile as of writing this. It merged with <b>K-9 Mail</b>, though both remain available as separate apps. While Thunderbird is coming along nicely, if you feel dissatisfied or just want to explore your options, K-9 Mail is still actively maintained and worth considering — in fact, some users may find it even more polished for mobile at this stage.
<br><br>
<b>Termux</b> adds a full-fledged Linux terminal environment into your phone, capable of running real command-line tools, programming languages, and even lightweight servers — all without root access. With its built-in package manager, you can install familiar utilities like <code>ssh</code>, <code>python</code>, or <code>git</code>, effectively turning your device into a pocket-sized Linux workstation. It's an incredibly flexible tool for anyone who enjoys tinkering, scripting, or automating things — and it shines when it comes to smart home setups. Through simple shell or Python scripts, Termux can monitor or control IoT devices, interact with APIs like <b>Home Assistant</b>, or perform scheduled automation tasks completely offline and securely. If you want to take things further, <b>Tasker</b> can trigger Termux scripts based on conditions like time, location, or system state, making complex automations both local and private. Pairing Termux with <b>Syncthing-Fork</b> allows you to keep scripts, configs, or logs in sync across all your devices without relying on cloud storage. Add <b>Tailscale</b> to the mix, and you can securely access your Termux environment or smart home network remotely, no port forwarding or public exposure needed.
<br><br>
Other open-source apps that really impressed me:
<br><br>
<ul>
<li><b>NewPipe</b> is an excellent YouTube frontend — works great overall, though it can get a bit clunky when routing through a VPN.</li>
<li><b>OpenReads</b> was a pleasant surprise; I'd never used a book-tracking app before, but if you read regularly, it's absolutely worth trying.</li>
<li><b>Organic Maps</b> — as someone who relied exclusively on Google Maps for years, I was genuinely surprised by how well it performed.</li>
</ul>
These three (but really, just all of the above mentioned apps) are solid enough that I'd recommend them for daily use, even if you're not running GrapheneOS.
<br><br>
<p align="center">
<a href="https://github.com/beemdevelopment/Aegis"><img src="https://img.shields.io/badge/Aegis-blue" /></a>
<a href="https://github.com/deckerst/aves"><img src="https://img.shields.io/badge/AvesLibre-blue" /></a>
<a href="https://github.com/bitwarden"><img src="https://img.shields.io/badge/Bitwarden-blue" /></a>
<a href="https://github.com/futo-org/android-keyboard"><img src="https://img.shields.io/badge/FUTO Keyboard-blue" /></a>
<a href="https://github.com/KDE/kdeconnect-kde"><img src="https://img.shields.io/badge/KDE%20Connect-blue" /></a>
<a href="https://github.com/TeamNewPipe/NewPipe"><img src="https://img.shields.io/badge/NewPipe-blue" /></a>
<a href="https://github.com/ImranR98/Obtainium"><img src="https://img.shields.io/badge/Obtainium-blue" /></a>
<a href="https://github.com/mateusz-bak/openreads"><img src="https://img.shields.io/badge/OpenReads-blue" /></a>
<a href="https://github.com/ethereal-developers/OpenScan"><img src="https://img.shields.io/badge/OpenScan-blue" /></a>
<a href="https://github.com/guardianproject/orbot-android"><img src="https://img.shields.io/badge/Orbot-blue" /></a>
<a href="https://github.com/organicmaps/organicmaps"><img src="https://img.shields.io/badge/Organic Maps-blue" /></a>
<a href="https://github.com/Catfriend1/syncthing-android"><img src="https://img.shields.io/badge/SyncthingFork-blue" /></a>
<a href="https://github.com/termux/termux-app"><img src="https://img.shields.io/badge/Termux-blue" /></a>
<a href="https://www.thunderbird.net/"><img src="https://img.shields.io/badge/Thunderbird-blue" /></a>
<a href="https://github.com/thunderbird/thunderbird-android"><img src="https://img.shields.io/badge/K9 Mail-blue" /></a>
</p>
</div>

### 🔒 Proprietary / Closed Source Apps

Used when no equivalent FOSS or open-source app meets functionality needs — trade-offs acknowledged.

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
| **Obsidian**                | Markdown-based note-taking; syncs across devices via Syncthing-Fork |
| **Paypal**                  |  |
| **Play Games / Play Store** | Sandboxed via GOS |
| **Proton Calendar**         | Encrypted calendar; privacy-first, seamlessly syncs across devices |
| **Spotify**                 |  |
| **Tailscale**               | Mesh VPN; used for remote access and secure networking |
| **Teams**                   | Work requirement |
| **WhatsApp**                | Used for social reasons (contacts, family) |

### 🧠 (Proprietary) Apps - Thoughts

<div align="justify">
<b>Obsidian + Syncthing-Fork</b> deserves a special mention as one of the best privacy-respecting productivity setups I've found. Instead of paying for Obsidian's premium sync service, I use Syncthing-Fork to handle vault synchronization across all my devices — completely free, peer-to-peer, and with no cloud middleman. You get full control: sync your entire vault, cherry-pick specific folders, or set up multiple sync configurations. It's fast, reliable, and keeps everything local-first. Add plugins like Excalidraw for visual thinking and Kanban boards for task management, and you've got a surprisingly powerful low-overhead system for planning, mapping ideas, and staying organized — all without recurring subscriptions or third-party servers touching your data.
<br><br>
<b>Tailscale</b>, <b>KDE Connect</b>, and <b>Syncthing-Fork</b> form a powerful, privacy-respecting trinity for seamless device interaction, file sharing, and remote access. Tailscale creates a secure mesh VPN across all your devices — phone, laptop, desktop, or server — allowing direct, encrypted communication over the internet or local network, without requiring port forwarding or exposing devices publicly. KDE Connect bridges Android and Linux devices over the same network (or via Tailscale), enabling clipboard sync, file transfers, notifications, and even remote input, making day-to-day phone-to-desktop integration smooth and convenient. Syncthing-Fork handles continuous, peer-to-peer file synchronization over local networks or Tailscale, keeping folders in sync between devices in a fully encrypted, self-hosted way, ideal for backups, project sharing, or media libraries. Together, these three apps replace many proprietary cloud services, providing a fully local, encrypted, and self-controlled ecosystem for file sharing, device connectivity, and remote access.
<br><br>
I use <b>Proton Calendar</b> because I wanted a privacy‑focused alternative to Google Calendar. It's fully encrypted, easy to use, and works seamlessly across devices. While it doesn't have all the bells and whistles of some mainstream calendars, it covers the essentials — scheduling, reminders, and recurring events — without sending your data to third‑party trackers. Even though it's not a FOSS app, Proton is a well‑respected company in the privacy community, and their services are widely trusted and secure. Worth noting: use of the app currently depends on an internet connection for full editing and syncing — offline creation or edits are not yet reliably supported.
<br><br>
I include <b>Malwarebytes</b> as a lightweight on-demand malware scanner. While GrapheneOS is very secure by default, I like having the peace of mind of occasionally scanning for malicious APKs, suspicious files, or potentially harmful apps I might sideload. The free version is more than sufficient for this on-demand scanning, but if you want real-time protection — either for an extra layer of security on Android or when using a less secure OS — the paid subscription is, in my opinion, worth it. Malwarebytes can also be used on Windows, where it remains one of the most reliable malware scanners I've personally used. I don't run it constantly on my phone, so it doesn't affect performance, but it's a helpful safety net when testing new software or sharing files.
<br><br>
Among the proprietary apps, many are essential — online banking, contactless payments, and communication tools are hard to avoid. Others, like streaming services or mobile games, are entirely optional depending on your lifestyle. Then there are apps that fall somewhere in between, where your needs may vary: Obsidian and Proton Calendar are good examples, though both are among the most privacy-respecting proprietary options available.
But the one app I haven't found a satisfactory replacement for is <b>Spotify</b>. If you have Spotify Premium, it's hands down the best music streaming experience on mobile — nothing else comes close in terms of library size, features, and overall usability. Without Premium, though, the mobile app is nearly unusable. If you're already paying for it, there's no better option out there.
<br><br>
<p align="center">
<a href="https://www.malwarebytes.com/"><img src="https://img.shields.io/badge/Malwarebytes-blue" /></a>
<a href="https://obsidian.md/"><img src="https://img.shields.io/badge/Obsidian-blue" /></a>
<a href="https://proton.me/calendar"><img src="https://img.shields.io/badge/Proton%20Calendar-blue" /></a>
<a href="https://tailscale.com/"><img src="https://img.shields.io/badge/Tailscale-blue" /></a>
</p>
</div>
