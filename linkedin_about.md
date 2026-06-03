
> *"The same engineer who writes the bypass also writes the C++ that detects it."*

---

I'm an AppSec Engineer operating at the intersection of **attacker tradecraft and builder discipline** — I break mobile apps for a living, then build the systems that stop others from doing the same.

---

**⚔️ Offensive**
7+ mobile VAPT engagements on Android & Flutter apps.

Notable findings:
- 🔴 **CVSS 9.8** — IDOR leading to mass PII scraping + full admin takeover
- 💳 Live payment key exposure (Razorpay, EasyBuzz) with working PoC
- 🔓 DexProtector decryption via custom Frida oracle (Blowfish P_ARRAY extraction → offline Python decrypt)
- 📱 Flutter RE — Dart VM symbol recovery, SSL pinning bypass, permanent APK patching
- 🎬 Widevine CDM weaknesses + DRM/HLS content bypass
- 💥 RCE vectors, BOLA, API disclosure

Every engagement ends with a **working exploit chain** — not just a report.

---

**🛡️ Defensive — Project BlackOuT**
Independently designed and shipped a **100+ layer Android RASP SDK** — distributed as a native C++/NDK AAR.

Covers:
`Frida (4-vector)` · `LSPosed` · `Zygisk` · `APatch KPM` · `SusFS` · `TrickyStore` · `KernelSU` · `LKM audit` · `ARM64 prologue integrity` · `text-segment SHA-256 sweep` · `inline hook detection` · `15+ more`

Crypto stack: **AES-256-GCM · ECDH P-256 · HKDF-SHA256 · BoringSSL**

---

**🔬 Research**
Published deep reverse engineering of **DexShell v26 + v29** — a commercial Android packer.
Bypassed all 11 anti-tamper layers. Disassembled 1,448 ARM64 VMP methods. Found AOSP platform signing keys bundled in the APK.
→ github.com/BlackOuTv2/DexShell-Research

---

**🛠️ Tools I live in**
`Frida` · `Blutter` · `IDA Pro` · `Radare2` · `Ghidra` · `JADX` · `Android NDK` · `BoringSSL` · `Python`

---
