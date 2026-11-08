# Packet Builder

A desktop app for **Windows and Linux** for building **multi-ship helicopter
mission kneeboard packets** and exporting them as:

* an **interactive, iPad-sized PDF** with tappable navigation buttons — a cover
  "contents" grid plus Home / Prev / Next on every page, and
* a **2-up print PDF** — each card printed twice on one landscape sheet with a
  cut line down the middle, so a sheet prints and cuts into two paper kneeboard
  cards.

It replaces the PowerPoint + Excel + manual-hyperlink workflow with one tool
that includes only the sections a given mission actually needs.

---

## ⬇ Download

All downloads are on the **[latest release](../../releases/latest)** page.

### Windows

**[Download `PacketBuilderSetup.exe`](../../releases/latest/download/PacketBuilderSetup.exe)**

Run it. The installer shows the licence, creates a Start-menu entry (and an
optional desktop shortcut), associates `.pkt` packet files with the app, and
includes an uninstaller.

> **Windows SmartScreen** will warn about an unrecognized publisher, because
> the installer is not code-signed. Choose **More info → Run anyway**.

Requires 64-bit Windows.

### Linux

**[Download `PacketBuilder-linux-x86_64.tar.gz`](../../releases/latest/download/PacketBuilder-linux-x86_64.tar.gz)**

Unpack it and run the installer from a terminal:

```bash
tar xzf PacketBuilder-linux-x86_64.tar.gz
cd PacketBuilder-linux
./install.sh
```

Or download and install in one line:

```bash
curl -L https://github.com/meta-n8/packetbuilder_releases/releases/latest/download/PacketBuilder-linux-x86_64.tar.gz | tar xz && PacketBuilder-linux/install.sh
```

The installer shows the licence, then installs for your user only (no
`sudo`) under `~/.local`: an app-launcher entry, a `packetbuilder` command,
and the `.pkt` file association. Uninstall with `./install.sh --uninstall`.
To update, download the new release and run `./install.sh` again.

Requires 64-bit (x86-64) Linux with glibc 2.35 or newer — e.g. Ubuntu 22.04+,
Debian 12+, Fedora 36+, Linux Mint 21+, or Arch.

---

## Licence — free for individuals, paid for organizations

| | |
|---|---|
| **Free** | You are a person who installed your own copy on a computer you own or control — **including using it for your own job or official duties**. |
| **Paid** | Any **organizational** use: installing on organization-managed systems, handing copies out internally, an organization standardizing on or mandating it, procurement, or contractors using it on an organization's behalf. "Organization" includes companies, non-profits, schools, and **government agencies and military units** at any level. |

Organizations get a **30-day evaluation**. For an organizational licence,
contact **belay.weasel7901@eagereverest.com**.

Full terms: [`LICENSE.txt`](LICENSE.txt) · third-party components:
[`THIRD-PARTY-NOTICES.txt`](THIRD-PARTY-NOTICES.txt)

This is **proprietary software**. The source code is not public and is not
distributed with the installer.

---

## ⚠ Planning aid only

Packet Builder formats what you type. **It does not validate anything.** It is
not certified, approved or endorsed by any government, military organization or
aviation authority, and it is not a source of aeronautical information.

**Verify every value against current, official, authoritative sources before
any operational use.** Do not use it or its output as a primary source for
navigation, flight planning or the conduct of flight.

It produces no classification markings and applies no access controls — the
classification, marking, handling and safeguarding of anything you create with
it is entirely your responsibility.

---

## What's in a packet

Every section is optional and pages can be reordered — build only what the
mission needs.

* **Cover** with an auto-generated contents grid of tappable tabs, recolourable,
  with labelled section dividers
* **Commo card** — aircraft/chalk table with commo-check boxes you tick in the
  exported PDF, commo-check frequencies, crew duties, mission sets, PACE plan,
  astro/light data, airfield frequencies, performance/fuel
* **Timeline** — enter local times (`HHMM`, or `HH:MM:SS` for seconds; a zone
  letter like `0900L` is fine) and the T/O ± column is computed from the
  takeoff event ("Takeoff", "Take off", "T/O" or "TO"), updating live as you
  type
* **Concept** and **route cards** — upload imagery with a rotatable north arrow
  and a legs table
* **SP / PZ / LZ / FARP cards** — upload satellite imagery, orient a compass to
  north, drag and rotate helicopter icons, add text, arrows, Xs and boxes
* **IIMC break-up** — computed from a few parameters, with a plan-view diagram
* **Approach plate** — upload the plate as an image or PDF
* **Document page** — any image or PDF, full page
* **EXCHECK** — execution checklist with prowords

Packets save as `.pkt` files you can reopen and edit (save and export dialogs
start in your **Documents** folder). Unsaved work is **autosaved** in the
background every minute — if the app closes unexpectedly, it offers to
recover your packet the next time it starts.

---

## What's new in v1.0.8

* **Linux version** — see [Download](#-download).
* **Timeline:** the T/O ± column now shows in the editor and updates as you
  type; more takeoff spellings and zone-suffixed times are recognised.
* **Crash recovery:** background autosave with a recovery prompt on startup.
* **Clearer close prompt:** *Save / Don't Save / Cancel* replaces the old
  "Discard unsaved changes? Yes / No", which was easy to misread.
* Save, open and export dialogs start in **Documents**.
* Approach plates and images with upper-case extensions (`.PDF`, `.JPG`) now
  appear in the file picker.
* Cover, Timeline, IIMC and zone pages fit narrow windows instead of
  scrolling sideways.

---

## Support

Questions, bugs and licensing: **belay.weasel7901@eagereverest.com**

Copyright © 2026 meta-n8. All rights reserved.
