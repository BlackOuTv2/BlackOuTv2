<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=28&duration=3000&pause=1000&color=58A6FF&center=true&vCenter=true&width=800&lines=AppSec+Engineer+%7C+Android+RASP+Architect;I+build+the+defenses+%E2%80%94+and+break+them;Mobile+RE+%C3%97+AI+%7C+Frida+%C2%B7+Flutter+%C2%B7+NDK;CVSS+9.8+%7C+DexProtector+%7C+Widevine+CDM;Project+BlackOuT+%E2%80%94+100%2B+Layer+RASP+SDK" alt="Typing SVG" />

<br/>

[![Telegram](https://img.shields.io/badge/Telegram-@BlackOuTv1-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/BlackOuTv1)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-black0ut-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/black0ut/)
[![Instagram](https://img.shields.io/badge/Instagram-@cyberxblackout-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/cyberxblackout/)
[![Research](https://img.shields.io/badge/DexShell_Research-58a6ff?style=for-the-badge&logo=github&logoColor=white)](https://blackoutv2.github.io/DexShell-Research)

</div>

---

## 👤 Who I Am

> *I'm an AppSec Engineer who builds the defenses — and breaks them.*

```python
profile = {
    "role"      : "AppSec Engineer | Android RASP Architect | Mobile RE × AI",
    "offensive" : "7+ Mobile VAPT engagements | CVSS 9.8 Critical | RCE | BOLA | DRM bypass",
    "defensive" : "Project BlackOuT — 100+ layer Android RASP (C++/NDK AAR SDK)",
    "re_focus"  : ["DexProtector", "DexShell VMP", "Widevine CDM", "Flutter Dart VM"],
    "tools"     : ["Frida", "Blutter", "IDA Pro", "Radare2", "Ghidra", "JADX", "BoringSSL"],
    "crypto"    : ["AES-256-GCM", "ECDH P-256 + HKDF-SHA256", "Blowfish ECB/CBC"],
    "principle" : "Same engineer who writes the bypass also writes the C++ that detects it",
}
```

---

## ⚔️ Offensive — Mobile VAPT

<table>
<tr>
<td>

**7+ VAPT Engagements** on native Android & Flutter apps

| Finding | Severity |
|---------|----------|
| IDOR — mass PII scraping + admin takeover | 🔴 **CVSS 9.8 Critical** |
| DRM/HLS content bypass | 🔴 Critical |
| Live payment key exposure (Razorpay, EasyBuzz) | 🔴 Critical |
| RCE vector | 🔴 Critical |
| DexProtector asset decryption (Frida oracle) | 🟠 High |
| Widevine CDM architecture weakness | 🟠 High |
| BOLA / API disclosure | 🟠 High |

*Every finding ships with a working exploit chain — not just a report.*

</td>
<td>

**Techniques**

```
→ DexProtector Frida oracle technique
  Blowfish ECB/CBC P_ARRAY extraction
  ECB/CBC mode detection
  Offline Python decryption playbook

→ Flutter RE
  Blutter-based Dart VM symbol recovery
  SSL pinning bypass
  Dart integrity bypass
  Geofence/GPS bypass
  Permanent APK patching (3+ targets)

→ Widevine CDM
  Architecture weakness analysis
  Level downgrade techniques
```

</td>
</tr>
</table>

---

## 🛡️ Defensive — Project BlackOuT

> **Independently architected and shipped** — a 100+ layer Android Runtime Application Self-Protection platform, distributed as a native **C++/NDK AAR SDK**.

<table>
<tr>
<td width="50%">

**Detection Vectors**

```cpp
// Anti-Frida (4 vectors)
✅ Frida server port detection
✅ /proc/maps named-region scan
✅ D-Bus interface enumeration
✅ RegisterNatives pattern match

// Anti-Root Frameworks
✅ LSPosed module detection
✅ Zygisk process inspection
✅ APatch KPM fingerprint
✅ SusFS filesystem anomaly
✅ TrickyStore prop spoofing detect
✅ KernelSU + LKM audit

// Code Integrity
✅ ARM64 prologue integrity check
✅ Text-segment SHA-256 sweep
✅ Inline hook detection
✅ GOT/PLT tamper detection
✅ 15+ additional threat vectors
```

</td>
<td width="50%">

**Crypto Stack**

```
AES-256-GCM          ← asset encryption
ECDH P-256           ← ephemeral key exchange
HKDF-SHA256          ← key derivation
BoringSSL            ← crypto backend
```

**Architecture**
```
Native C++/NDK
  └─ AAR SDK (drop-in integration)
  └─ Zero Java surface (harder to hook)
  └─ Anti-debug hardened
  └─ Obfuscated symbol table
  └─ Self-attestation chain
```

</td>
</tr>
</table>

---

## 🔬 Published Research

### [DexShell Android Packer — Deep Reverse Engineering](https://github.com/BlackOuTv2/DexShell-Research)

Complete RE of **DexShell / DexProtectX** commercial packer across v26 and v29.

| | v26 | v29 |
|-|-----|-----|
| VMP | Threaded bytecode interpreter (256-opcode ISA) | **Native AOT compiler** |
| Protection | ASCII JNI names | **Runic Unicode obfuscation** |
| New | — | InstrumentationHijacker, DexHeaderRestore, delayed_detection |
| Methods | 14,375 | **1,448 ARM64 compiled functions** |

**Key findings:**
- `platform.pk8` (AOSP signing key) bundled in APK — system-level signing capability
- Plaintext credentials in SharedPreferences
- 514 DexShell classes hidden in encrypted runtime DEX
- All 11 anti-tamper layers documented and bypassed

[![View Research](https://img.shields.io/badge/Full_Research-58a6ff?style=for-the-badge&logo=github)](https://github.com/BlackOuTv2/DexShell-Research)
[![Visual Diagrams](https://img.shields.io/badge/Flowcharts_%26_Diagrams-3fb950?style=for-the-badge&logo=github)](https://blackoutv2.github.io/DexShell-Research)

---

## 🛠️ Tools & Stack

<div align="center">

![Frida](https://img.shields.io/badge/Frida-ff6b35?style=for-the-badge&logoColor=white)
![IDA Pro](https://img.shields.io/badge/IDA_Pro-4A90D9?style=for-the-badge&logoColor=white)
![Radare2](https://img.shields.io/badge/radare2-58a6ff?style=for-the-badge&logoColor=white)
![Ghidra](https://img.shields.io/badge/Ghidra-ff0000?style=for-the-badge&logoColor=white)
![JADX](https://img.shields.io/badge/JADX-3fb950?style=for-the-badge&logoColor=white)
![Blutter](https://img.shields.io/badge/Blutter-bc8cff?style=for-the-badge&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++_NDK-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![BoringSSL](https://img.shields.io/badge/BoringSSL-d29922?style=for-the-badge&logoColor=white)

</div>

---

## 📊 GitHub Stats

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=BlackOuTv2&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&icon_color=3fb950&text_color=e6edf3&count_private=true" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=BlackOuTv2&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=e6edf3&langs_count=6" />

<img src="https://github-readme-streak-stats.herokuapp.com/?user=BlackOuTv2&theme=github-dark-blue&hide_border=true&background=0d1117&stroke=30363d&ring=58a6ff&fire=f85149&currStreakLabel=58a6ff" />

</div>

---

## 📫 Contact

<div align="center">

| 💬 Telegram | 💼 LinkedIn | 📸 Instagram |
|------------|------------|-------------|
| [@BlackOuTv1](https://t.me/BlackOuTv1) | [black0ut](https://www.linkedin.com/in/black0ut/) | [@cyberxblackout](https://www.instagram.com/cyberxblackout/) |

</div>

---

<div align="center">

![Profile Views](https://komarev.com/ghpvc/?username=BlackOuTv2&color=58a6ff&style=flat-square&label=Profile+Views)

*"The same engineer who writes the bypass also writes the C++ code that detects it."*

</div>
