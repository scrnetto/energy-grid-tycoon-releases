<p align="center">
  <img src="immagini/logo.png" alt="Voltvale: Energy Grid Tycoon logo" width="700">
</p>

🇬🇧 English · 🇮🇹 [Italiano](README.it.md)

# ⚡ Voltvale: Energy Grid Tycoon

[![Latest version](https://img.shields.io/github/v/release/scrnetto/energy-grid-tycoon-releases?include_prereleases&label=version&color=f2c230)](https://github.com/scrnetto/energy-grid-tycoon-releases/releases)
[![Status](https://img.shields.io/badge/status-alpha-orange)](#versions)
[![Play in the browser](https://img.shields.io/badge/play-in%20the%20browser-3fae5a)](https://scrnetto.github.io/energy-grid-tycoon-releases/)
[![Platforms](https://img.shields.io/badge/platforms-Windows%20%7C%20macOS%20%7C%20Linux%20%7C%20Web-3f8fc9)](#download-the-game)
[![Last update](https://img.shields.io/github/release-date-pre/scrnetto/energy-grid-tycoon-releases?label=last%20update&color=3f8fc9)](https://github.com/scrnetto/energy-grid-tycoon-releases/releases)
[![Downloads](https://img.shields.io/github/downloads/scrnetto/energy-grid-tycoon-releases/total?label=downloads&color=3f8fc9)](https://github.com/scrnetto/energy-grid-tycoon-releases/releases)
[![Licence](https://img.shields.io/badge/licence-free%2C%20all%20rights%20reserved-lightgrey)](LICENSE.md)
[![Languages](https://img.shields.io/badge/languages-it%20%7C%20en%20%7C%20de%20%7C%20fr%20%7C%20es-009246)](#languages)
[![Made with Unity](https://img.shields.io/badge/made%20with-Unity%206-1d2330?logo=unity)](https://unity.com/)

**You run the power grid of a growing town.** Every hour the town needs energy: a little at night, a lot in the
evening. Build power plants, solar farms, wind farms and batteries, connect everything with power lines, find
people to work in them, feed everyone, and grow the town to **400 residents within two game years**, without constant
blackouts, without debt and without choking it with pollution.

An original game by **Marco Scarlino**. Free to play.

![A game on day six: solar farms, wind farms and a battery around the town hall](immagini/schermata-partita.png)

> **Status: in development (alpha).** You can play from start to finish, but a lot is still missing and some
> things may not work. Every report helps: see [Reporting a problem or an idea](#reporting-a-problem-or-an-idea).

## Play now in your browser

**[▶ Play Voltvale in your browser](https://scrnetto.github.io/energy-grid-tycoon-releases/)**: nothing to
install. You need a recent browser (Chrome, Firefox, Edge, Safari) on a computer with a mouse and keyboard, or a
tablet: **tap = click, long press = right-click**. Click on the game before using the keyboard. Your saves stay in
the browser you use.

## Download the game

Every version is on the **[Releases](../../releases)** page. Download the file for your system from the latest
version:

| System | File | How to start it |
|---|---|---|
| **Windows** 10/11 (64-bit) | `Voltvale-<version>-windows.zip` | Extract the zip and open `Voltvale.exe` |
| **macOS** 12 or later | `Voltvale-<version>-macos.zip` | Extract the zip and open `Voltvale.app` |
| **Linux** (64-bit) | `Voltvale-<version>-linux.zip` | Extract the zip and run `Voltvale` |

### First launch

The game isn't signed with a paid certificate, so your system may warn you that it comes from an unknown
developer. This is normal for independent games.

- **Windows**: if you see «Windows protected your PC», click **More info**, then **Run anyway**.
- **macOS**: if you see «cannot be opened because the developer cannot be verified», **right-click the app →
  Open**, then confirm with **Open**. You only need to do this once. If your Mac says the app «is damaged», open
  Terminal in the folder of the zip and type `xattr -cr Voltvale.app`.
- **Linux**: if it doesn't start, make the file executable with `chmod +x Voltvale`.

**Checking the download (optional).** Each version has a `SHA256SUMS.txt` file with the fingerprint of every zip.
On Linux run `sha256sum -c SHA256SUMS.txt`, on macOS `shasum -a 256 -c SHA256SUMS.txt`.

### Requirements

- A screen of at least 1280×800.
- Mouse and keyboard (a tablet is fine for the web version).
- About 200 MB of free space.
- Any graphics card from the last 10 years: built-in ones are fine too.

## How to play

The game opens with the **start menu**: **New game**, or **Continue** to pick up your last save. The game starts on
**18 October 2020** and begins **paused**: press **Space** to start the clock. At 1× speed one game hour lasts one
second, and you can speed up to 2× and 4×. The seasons follow the calendar: you start in autumn, and in winter the
days are shorter and the sky is cloudier.

- **Goal**: reach **400 residents** with pollution **below the limit** within **2 years**.
- **Defeat**: if your money stays in the red for **30 days in a row**, or if the 2 years run out.
- **The grid**: every building must be connected to the **town hall**. **Power lines** start from the town hall
  and extend it, diagonals included. A building is connected if it touches the town hall, a line or another
  connected building: a group of buildings side by side is connected if one of them touches the grid.
- **Demand and energy**: the town uses little energy at night and a lot in the evening, around 7 pm. If there
  isn't enough, there's a **blackout**: residents get angry and some leave.
- **Energy sources**:
  - the **sun** only produces by day, and little in winter or under clouds;
  - the **wind** changes from hour to hour;
  - **coal** always produces, but it pollutes and burns the coal dug up by the **mines**.
- **Batteries** store the extra energy and give it back when needed, for example in the evening.
- **Surplus energy** is sold to the outside grid, but the more you offer, the less it's worth.
- **Pollution**: coal power plants pollute and the air clears slowly. One power plant is fine, too many are not.
  Above the limit people are unhappy and the town stops growing.
- **Growth**: the town grows if residents are happy, there's room in the **districts** and there's enough
  **food** in store.

### Work and staff

Buildings need people to run them.

- About **56 %** of the residents work. The bar at the top shows filled jobs out of the available workforce.
- **Coal power plants**, **solar farms**, **wind farms**, **coal mines** and the **food** buildings need staff. The **Tile** panel shows
  how many they have, for example **Staff: 8/10**.
- With too few staff a building produces less; **with no staff at all it stops** and shows the **«no staff»**
  signal.
- Workers go **to energy first**, then **to food**, then **to the mines**, then **to district services** (shops, local schools).
  Districts keep working even when their services are short of staff.
- **Unemployment** means less tax income, and if it's high, slightly less happy residents.

### Food

Residents eat every hour. The food stock is in the top bar, next to the ear of wheat, and turns red when it's
running low.

- **Farm** (plains): produces with the seasons, a lot in summer and **nothing in winter**.
- **Fishing boat** (coast): fishes all year round, but stops when the wind is too strong.
- **Greenhouse** (plains or hills): produces all year round, but **uses a lot of power**.
- **Cold store** (plains): raises how much food the town can keep.
- **Food runs on the grid**: food buildings use power. During a **blackout** they don't produce, and cold stores
  lose part of the extra food.
- **If the stock runs out**, food is imported automatically, but it's expensive. Imported food keeps the town from
  starving, but it **doesn't grow**: growth needs at least one day of its own stock.
- **If the money runs out too**, famine hits and residents leave.
- The **Tile** panel shows how much each building produces (for example **Food: 2.0/h**), how much room a cold
  store adds, and how much power it uses.

### Controls

Hover over any icon or button: a tooltip explains what it is. Hover over a building on the map to see its status
and how much energy it produces or uses.

| Control | What it does |
|---|---|
| Keys **1–9** and **0** | Pick what to build: Power line, Coal mine, Coal power plant, Solar farm, Wind farm, Battery, District, Farm, Fishing boat, Greenhouse. Pick the Cold store from the list on the left |
| **Left click** | Places the chosen building. With nothing chosen, selects a tile and shows its details |
| **Right click** (on a tablet: long press) | With a building chosen, cancels the choice. With nothing chosen, asks to confirm demolition (half the cost refunded) |
| **Esc** | Cancels the choice; if there's nothing to cancel, opens the **pause menu** (Resume, Save and quit to menu, New game, Language) |
| **F11** | Full screen / window |
| **Space** or the ▶/❚❚ button | Pause / resume |
| **F** or the arrow buttons | Speed 1×, 2×, 4× |
| **V** | Advance by a single hour |
| **WASD** or **arrow keys**, middle mouse button | Move the view |
| **Mouse wheel** | Zoom |
| **Save** / **Load** (at the top) | Saves or resumes the game. The game also saves by itself every day |

### Languages

The game is in **Italian, English, German, French and Spanish**. Pick **Language** in the start menu or the pause
menu to switch at any time, without restarting; your choice is remembered. On first launch the game uses your
system language if it's one of these five, and English otherwise. In the web version you can open a language
straight away by adding `?lingua=en` (or `it`, `de`, `fr`, `es`) to the address.

### Signals on buildings

- **Unplugged plug** (white and red circle): the building isn't connected to the grid.
- **Crossed-out lightning bolt** (yellow circle): it's connected but gets no power (blackout), or a coal power
  plant has stopped because the coal has run out. A greenhouse or cold store with no power doesn't work.
- **Crossed-out hard hat** (light-blue circle): **no staff**, so the building has stopped. Build more districts or
  free up workers.
- **Lights at night**: after dark, districts and the town hall switch their lights on. A building with no power
  stays dark, so a dark district at night is a warning.

### Tips for your first game

1. Pause and look at the map: **hills** are good for wind farms, and the dark **coal deposits** are where mines go.
2. Run a **power line** from the town hall towards where you want to build.
3. Start with some **solar and wind** and a **battery** for the evening.
4. Don't build too many power plants at once: each one needs **staff**, and the town is still small.
5. Build **districts** as long as production keeps up with demand.
6. Put down a **farm** early and plan for winter: farms stop in winter, so you need a stock, a fishing boat or a
   greenhouse.
7. Keep an eye on the **chart at the bottom**: if the red line (demand) goes above the green one (production), a
   blackout is coming.

## Where saves are stored

Saves stay on your computer, or in your browser for the web version, and the game sends nothing over the
internet.

- **Windows**: `%USERPROFILE%\AppData\LocalLow\Marco Scarlino\Voltvale\salvataggi`
- **macOS**: `~/Library/Application Support/Marco Scarlino/Voltvale/salvataggi`
- **Linux**: `~/.config/unity3d/Marco Scarlino/Voltvale/salvataggi`

**Coming from an earlier version?** The first time you start version 0.3.0, the game **copies** your saves from
the old «Energy Grid Tycoon» folder (same path, with «Energy Grid Tycoon» instead of «Voltvale»). The old folder
stays where it is. You'll need to choose your **language** again once.

**From 0.4.0** saves use a new format. Saves from earlier versions still load: the town restarts with the
starting food stock. A 0.4.0 save doesn't open in earlier versions.

Saves from one alpha version might not work with the next one: the [changelog](CHANGELOG.md) says so when it
happens.

## Versions

Versions follow [semantic versioning](https://semver.org/) in three stages:

| Stage | Example | What it means |
|---|---|---|
| **Alpha** | `0.3.0-alpha.1` | The game changes a lot between versions; parts are missing; there may be bugs and saves that don't carry over |
| **Beta** | `0.9.0-beta.1` | All the main parts are there; bugs and game balance are being polished |
| **Stable** | `1.0.0` | The first complete version. Then `1.0.1` for fixes and `1.1.0` for new features |

Alpha and beta versions are marked on GitHub as **pre-releases**. What changes in each version is in the
**[CHANGELOG](CHANGELOG.md)** and on each release page.

## Reporting a problem or an idea

Open a report on the **[Issues](../../issues/new/choose)** page and choose:
- **Problema** (problem): something doesn't work. Say what you were doing, what you expected and which version of the game
  you have.
- **Idea**: a suggestion to improve the game.

You need a GitHub account, which is free. If you don't have one, feel free to write to Marco directly.

## Licence

Voltvale is **free**: you can download it and play as much as you like. You may **not** redistribute, sell or
modify it: to let someone else play, send them the link to this page. The details are in [LICENSE.md](LICENSE.md)
(in Italian, with a summary in English).

## Credits

Designed and made by **Marco Scarlino**, with Unity and with the help of AI tools for code, graphics and
translations.
