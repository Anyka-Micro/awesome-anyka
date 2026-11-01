# Awesome Anyka

A curated list of open-source SDKs, tools and applications for the **Anyka SoC family** (AK3918 and others), maintained by [Anyka](https://github.com/Anyka-Micro).

Each entry is marked **Official** (maintained by Anyka) or **Community** (maintained by its author, credited and linked). Every project keeps its own license.

> [!IMPORTANT]
> - **Community projects aren't supported by Anyka.** Report issues to their authors.
> - **Check the license.** `No license — link only` means you may not redistribute or re-host the project.
> - **Flashing is at your own risk.** Custom firmware can permanently damage a device and may void its warranty. Back up the original flash first.

## Contents

- [How to read the tables](#how-to-read-the-tables)
- [SDKs & low-level tooling](#-sdks--low-level-tooling)
- [Applications](#-applications)
- [Contributing](#contributing)

## How to read the tables

| Column | What it tells you |
|---|---|
| **Maintainer** | **Official**: maintained by Anyka. **Community**: maintained by the named author, who is the right contact for issues. |
| **Status** | 🟢 **Active**: code pushed in the last 12 months. ⚪ **Inactive**: no pushes for over 12 months; it may still work, but expect no fixes. 📦 **Archived**: read-only, kept for reference. |
| **License** | As stated in the project's own repository. `No license — link only` means you may not redistribute it. `Unclear — see repo` means read the repository's terms yourself. `⚠️ Bundles Anyka binaries` means the repo includes Anyka's prebuilt libraries or kernel modules: the project's license doesn't cover them, and Anyka hasn't licensed their redistribution. |
| **Checked** | When we last verified the license and status. Things change, so always confirm in the repository. |

---

## 🧰 SDKs & low-level tooling

Toolchains, BSPs, kernel and U-Boot trees, flashing and recovery tools.

| Project | Maintainer | What it is | Chips | Status | License | Checked |
|---|---|---|---|---|---|---|
| [OpenIPC/firmware](https://github.com/OpenIPC/firmware) | Community · [@OpenIPC](https://github.com/OpenIPC) | Buildroot-based replacement firmware for IP cameras from many SoC vendors; its Anyka layer has board configs for the AK3916EV300 and AK3918EV300. | AK3916EV300, AK3918EV300 | 🟢 Active | MIT · ⚠️ Bundles Anyka binaries | 2026-11-01 |
| [Nemobi/arm-anykav200-crosstool-docker](https://github.com/Nemobi/arm-anykav200-crosstool-docker) | Community · [@Nemobi](https://github.com/Nemobi) | A Dockerfile that packages the anykav200 cross toolchain into a container image. | AK3918 (anykav200 toolchain) | ⚪ Inactive (May 2022) | No license — link only | 2026-11-01 |
| [MXDMY/ak37e_lvgl8](https://github.com/MXDMY/ak37e_lvgl8) | Community · [@MXDMY](https://github.com/MXDMY) | A port of the LVGL 8.2 graphics library to the AK37E platform, meant as a starting template for GUI apps. | AK37E | 📦 Archived | Apache-2.0 · ⚠️ Bundles Anyka binaries | 2026-11-01 |

## 📷 Applications

Firmware, camera and streaming apps, and integrations built on the SDKs above.

| Project | Maintainer | What it is | Chips | Status | License | Checked |
|---|---|---|---|---|---|---|
| [MuhammedKalkan/Anyka-Camera-Firmware](https://github.com/MuhammedKalkan/Anyka-Camera-Firmware) | Community · [@MuhammedKalkan](https://github.com/MuhammedKalkan) | SD-card based custom firmware and apps (RTSP, web UI, PTZ) for AK3918 cameras. Many later projects build on it. | AK3918 (tested on AK3918v200EN080) | ⚪ Inactive (Feb 2025) | MIT · ⚠️ Bundles Anyka binaries | 2026-11-01 |
| [kkrzysztofik/Anyka_ak3918_hacking_journey](https://github.com/kkrzysztofik/Anyka_ak3918_hacking_journey) | Community · [@kkrzysztofik](https://github.com/kkrzysztofik) | An actively maintained continuation of Gerge's AK3918 hacking project (originally on Gitea), adding fixes and a Rust rewrite of the ONVIF services. | AK3918 | 🟢 Active | GPL-3.0 · ⚠️ Bundles Anyka binaries | 2026-11-01 |
| [ThatUsernameAlreadyExist/anyka-v4l2rtspserver](https://github.com/ThatUsernameAlreadyExist/anyka-v4l2rtspserver) | Community · [@ThatUsernameAlreadyExist](https://github.com/ThatUsernameAlreadyExist) | An AK3918 port of mpromonet's v4l2rtspserver RTSP server. | AK3918 | ⚪ Inactive (Apr 2025) | Unlicense · ⚠️ Bundles Anyka binaries | 2026-11-01 |
| [dangerousplay/kamoder](https://github.com/dangerousplay/kamoder) | Community · [@dangerousplay](https://github.com/dangerousplay) | Replacement camera firmware written in Rust that boots from the SD card, with RTSP, ONVIF, PTZ and a web UI. | AK3918 (EV200, AV100) | 🟢 Active | GPL-3.0 · ⚠️ Bundles Anyka binaries | 2026-11-01 |
| [michelostojski/akost-firmware](https://github.com/michelostojski/akost-firmware) | Community · [@michelostojski](https://github.com/michelostojski) | A Buildroot external tree that builds open firmware for AK39EV330 cameras such as the GNCC GK2, with RTSP and ONVIF. | AK39EV330 | 🟢 Active | MIT | 2026-11-01 |
| [jphein/anyka3918-gc1084-camera](https://github.com/jphein/anyka3918-gc1084-camera) | Community · [@jphein](https://github.com/jphein) | Local RTSP, PTZ and Home Assistant support for AK3918 cameras with a GC1084 sensor, such as the Teruhal TC20. | AK3918 | 🟢 Active | GPL-3.0 · ⚠️ Bundles Anyka binaries | 2026-11-01 |
| [SotosSW/anykav380-ak3918-hacking](https://github.com/SotosSW/anykav380-ak3918-hacking) | Community · [@SotosSW](https://github.com/SotosSW) | Takes V380-style AK3918 cameras off the cloud with RTSP, ONVIF and an improved PTZ daemon. Builds on work by MuhammedKalkan and kuhnchris. | AK3918 | 🟢 Active | GPL-3.0 · ⚠️ Bundles Anyka binaries | 2026-11-01 |

<!--
  ROW TEMPLATE. Every column is required (see https://github.com/Anyka-Micro/.github/blob/main/CONTRIBUTING.md).
  Status: 🟢 Active (pushed in last 12 months) / ⚪ Inactive (Mon YYYY of last push) / 📦 Archived
  Official:  | [Anyka-Micro/REPO](https://github.com/Anyka-Micro/REPO) | **Official** · Anyka | One sentence. | AK3918EV300 | 🟢 Active | SPDX-ID | YYYY-MM-DD |
  Community: | [OWNER/REPO](https://github.com/OWNER/REPO) | Community · [@OWNER](https://github.com/OWNER) [, fork of [x/y](…)] | One sentence, your own words. | AK3918EV300 | 🟢 Active | SPDX-ID / No license — link only / Unclear — see repo [· ⚠️ Bundles Anyka binaries] | YYYY-MM-DD |
-->

## Contributing

Suggest, correct or remove an entry through [the issue forms](https://github.com/Anyka-Micro/awesome-anyka/issues/new/choose), or open a pull request that follows the [contribution & attribution policy](https://github.com/Anyka-Micro/.github/blob/main/CONTRIBUTING.md). Community authors who ask to be unlisted are removed within 7 days, no questions asked.

## License

This list is licensed under [CC BY 4.0](LICENSE). Listed projects are under their own licenses. The Anyka name and logo are trademarks of Anyka and are not covered by this license.

---

<sub>Projects marked **Community** are the work of their respective authors and are listed for convenience. Anyka does not maintain, support or warrant them, and listing a project doesn't mean its author is affiliated with Anyka.</sub>
