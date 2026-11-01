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
| **License** | As stated in the project's own repository. `No license — link only` means you may not redistribute it. `Unclear — see repo` means read the repository's terms yourself. |
| **Checked** | When we last verified the license and status. Things change, so always confirm in the repository. |

---

## 🧰 SDKs & low-level tooling

Toolchains, BSPs, kernel and U-Boot trees, flashing and recovery tools.

| Project | Maintainer | What it is | Chips | Status | License | Checked |
|---|---|---|---|---|---|---|
| [Nemobi/arm-anykav200-crosstool-docker](https://github.com/Nemobi/arm-anykav200-crosstool-docker) | Community · [@Nemobi](https://github.com/Nemobi) | A Dockerfile that packages the anykav200 cross toolchain into a container image. | AK3918 (anykav200 toolchain) | ⚪ Inactive (May 2022) | No license — link only | 2026-11-01 |

## 📷 Applications

Firmware, camera and streaming apps, and integrations built on the SDKs above.

| Project | Maintainer | What it is | Chips | Status | License | Checked |
|---|---|---|---|---|---|---|
| [michelostojski/akost-firmware](https://github.com/michelostojski/akost-firmware) | Community · [@michelostojski](https://github.com/michelostojski) | A Buildroot external tree that builds open firmware for AK39EV330 cameras such as the GNCC GK2, with RTSP and ONVIF. | AK39EV330 | 🟢 Active | MIT | 2026-11-01 |

<!--
  ROW TEMPLATE. Every column is required (see https://github.com/Anyka-Micro/.github/blob/main/CONTRIBUTING.md).
  Status: 🟢 Active (pushed in last 12 months) / ⚪ Inactive (Mon YYYY of last push) / 📦 Archived
  Official:  | [Anyka-Micro/REPO](https://github.com/Anyka-Micro/REPO) | **Official** · Anyka | One sentence. | AK3918EV300 | 🟢 Active | SPDX-ID | YYYY-MM-DD |
  Community: | [OWNER/REPO](https://github.com/OWNER/REPO) | Community · [@OWNER](https://github.com/OWNER) [, fork of [x/y](…)] | One sentence, your own words. | AK3918EV300 | 🟢 Active | SPDX-ID / No license — link only / Unclear — see repo | YYYY-MM-DD |
-->

## Contributing

Suggest, correct or remove an entry through [the issue forms](https://github.com/Anyka-Micro/awesome-anyka/issues/new/choose), or open a pull request that follows the [contribution & attribution policy](https://github.com/Anyka-Micro/.github/blob/main/CONTRIBUTING.md). Community authors who ask to be unlisted are removed within 7 days, no questions asked.

## License

This list is licensed under [CC BY 4.0](LICENSE). Listed projects are under their own licenses. The Anyka name and logo are trademarks of Anyka and are not covered by this license.

---

<sub>Projects marked **Community** are the work of their respective authors and are listed for convenience. Anyka does not maintain, support or warrant them, and listing a project doesn't mean its author is affiliated with Anyka.</sub>
