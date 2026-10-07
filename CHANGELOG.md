# Changelog

What changed in each Humbar release. [Русская версия](CHANGELOG.ru.md) · [Download](https://github.com/ItsDarkEzz/humbar/releases/latest)

## 1.0.2 — 2026-10-07

### Added
- **Island size.** Settings → Island → Size: the width of the player, and the width and height of the open island. A taller island is used, not padded — its tiles and lists grow with it.
- **Pets on either side.** Settings → Pets → Position: right or left of the island.
- **Agents stay quiet while you are in them.** While the terminal, editor or Claude app running a session is in front, its questions, permission requests and “done” stay off the island; a request still unanswered comes up when you switch away. One switch in Settings → AI Agents.
- **A request answered in the agent leaves the island at once** instead of waiting out its timeout.

### Fixed
- **The volume and brightness indicator was empty when nothing was playing.** The island opened its wings but showed no icon, bar or percent until a player had a track. It now shows them every time, and agent and timer chips step aside instead of sitting over the level bar.

## 1.0.1 — 2026-10-07

### Added
- **Pets for your AI agents.** Claude Code, Codex, Droid and OpenCode can each have a pet that stands beside the island while that agent has sessions and acts out what it is doing: working, waiting for you, done. When an agent finishes, its pet celebrates for a moment and leaves. Humbar comes with its own pet, Hum.
- **Any pet in the open Codex pet format.** Pets you already have in `~/.codex/pets` appear in Humbar by themselves. Settings → Pets also has a community list from codex-pets.net (Popular and New) with one-click install — the list is requested only when you press Browse.
- **Pet size** from 40 to 120 pt, and for every pet a choice of **which of its animations plays in each state** — authors draw them differently, so you pick by sight.
- **A message notification leaves as soon as you have seen the message.** Opening the messenger folds its notification away at any moment, not only once it has become a chip. For Telegram, reading the chat — on the Mac or on your phone — does the same.

### Fixed
- The island did not open when the pointer was pushed against the very top edge of the screen; it took two or three tries. It opens at once now.
- System notices (charging, Caps Lock, drives, downloads, Bluetooth) could vanish when several arrived while another notification was on screen. They now wait their turn.
- Telegram: muted private chats were announced, with “Muted” or “Premium” shown as the sender. Chats with a comma in their name also lost their muted mark. Private chats without badges, which the chat list used to miss, are now announced.
- Charging and battery notices no longer wait for an open menu or a drag to finish.

### Changed
- Privacy: the optional pet list is the only new network request, and only on your click. Pets from the community list are third-party work and are saved on your Mac only.

### Website
- You can now pay with USDT on [humbar.app/buy](https://humbar.app/buy/) and get your licence key on the same page.

## 1.0.0 — 2026-10-05

The first paid release: free for 7 days, then $3.99 once.

- Synced lyrics for any player, word by word, from Yandex Music, LRCLIB, NetEase and Kugou.
- Claude Code, Codex, OpenCode and Droid ask for permissions, questions and plan approval right by the camera; Claude plan limits at a glance.
- Messenger notifications with quick reply, a hub of everyday tools, small islands for charging, Focus, AirPods and more.
- Offline licence keys, English and Russian.

Versions up to 0.9.0 were published under the GNU GPL v3; from 1.0 Humbar is under its own [licence](LICENSE).
