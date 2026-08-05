<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/banner-dark.svg">
  <img src="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/banner-light.svg" width="100%" alt="Talkdedsec Editor — no telemetry, no unnecessary background services">
</picture>

<p align="center">
  <a href="https://code.talkdedsec.com"><b>Website</b></a>
  &nbsp;·&nbsp;
  <a href="https://github.com/talkdedseccode/talkdedsec-editor/releases/latest"><b>Download</b></a>
  &nbsp;·&nbsp;
  <a href="https://code.talkdedsec.com/en/belgeler/"><b>Documentation</b></a>
  &nbsp;·&nbsp;
  <a href="https://github.com/talkdedseccode/talkdedsec-editor/discussions"><b>Discussions</b></a>
  &nbsp;·&nbsp;
  <a href="https://github.com/talkdedseccode/talkdedsec-themes"><b>Themes</b></a>
  &nbsp;·&nbsp;
  <a href="https://github.com/talkdedseccode/talkdedsec-editor/security"><b>Security</b></a>
</p>

<p align="center">
  <sub>Official GitHub account for <b>code.talkdedsec.com</b> and the Talkdedsec editor ecosystem.</sub>
</p>

<br>

<table>
<tr>
<td width="64%" valign="top">

<sub>THE PROJECT</sub>

# Talkdedsec Editor

A focused Windows code editor built from an open-source editor core, with telemetry, unused built-in
extensions and unnecessary startup work removed.

The goal is not to turn an editor into a platform. It is to keep the path between opening a project and
writing code as short, predictable and private as possible.

**Current release:** `v1.130.0`  
**Platform:** Windows x64  
**Installation:** Per-user, no administrator rights required

</td>
<td width="36%" align="center" valign="middle">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/goz-koyu.png">
  <img src="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/goz-acik.png" width="250" alt="Talkdedsec eye logo">
</picture>

<sub><b>LOOKS. LOGS NOTHING.</b></sub>

</td>
</tr>
</table>

<br>

## Built around four rules

<table>
<tr>
<td width="50%" valign="top">

### No telemetry

Telemetry is removed rather than hidden behind a setting. The editor does not depend on an analytics
pipeline or a startup reporting endpoint.

</td>
<td width="50%" valign="top">

### No privileged install

The application installs inside the current user profile and does not require administrator access.
It keeps its own settings and extension state.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### No forced updater

There is no background update service. New versions are installed manually over the existing one, while
user settings remain intact.

</td>
<td width="50%" valign="top">

### Your provider, your account

The embedded agent connects through the account selected by the user. There is no separate seat fee,
token resale layer or Talkdedsec-hosted proxy in the middle.

</td>
</tr>
</table>

<br>

## Measured, not estimated

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/sokuldu-dark.svg">
  <img src="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/sokuldu-light.svg" width="100%" alt="Before and after measurements for startup time, processes, extensions and startup endpoints">
</picture>

<br>

| Measurement | Current build |
|:--|--:|
| Cold start | **0.41 s** |
| Processes | **9** |
| Built-in extensions | **64** |
| Startup telemetry endpoints | **0** |
| Idle memory | **1.40 GB** |
| Installed size | **1.12 GB** |
| Installer size | **253 MB** |
| Source maps shipped | **0** |

<sub>
Measured on the same machine with a production build and a clean profile. Method and raw output:
<a href="https://code.talkdedsec.com/en/olcum/">code.talkdedsec.com/en/olcum</a>
</sub>

<br>

## Themes without unfinished edges

<img src="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/themes.svg" width="100%" alt="Talkdedsec themes: Dark, Midnight, Matrix, Ember and Light">

Five themes ship with the editor. Each covers **183 interface colour keys** and a complete
**16-colour terminal palette**, so changing a theme also changes panels, Git decorations and terminal
colours instead of leaving parts of the interface behind.

Community themes live in [`talkdedsec-themes`](https://github.com/talkdedseccode/talkdedsec-themes).
Contributions are checked automatically before merge.

<br>

## Download and verify

The current Windows installer is published only through the
[`talkdedsec-editor` Releases page](https://github.com/talkdedseccode/talkdedsec-editor/releases/latest).

The current installer is not code-signed yet. Verify its SHA-256 digest before running it:

```powershell
Get-FileHash .\TalkdedsecSetup.exe -Algorithm SHA256
```

Expected digest for `v1.130.0`:

```text
3f8a6dda74030e30a85b5f72b327099f31859d5af8b144e6b678e1327d2129a8
```

Machine-readable checksum:
[`checksums/v1.130.0.sha256`](https://github.com/talkdedseccode/talkdedsec-editor/blob/main/checksums/v1.130.0.sha256)

<br>

## Repository map

| Repository | Purpose | License / access |
|:--|:--|:--|
| [`talkdedsec-editor`](https://github.com/talkdedseccode/talkdedsec-editor) | Releases, documentation, issue tracking, security policy and third-party notices | Editor binary under Terms of Use |
| [`talkdedsec-themes`](https://github.com/talkdedseccode/talkdedsec-themes) | Built-in theme references, community themes and validation tooling | MIT |
| [`talkdedseccode`](https://github.com/talkdedseccode/talkdedseccode) | Official GitHub profile and project overview | Profile content |

<br>

## Trust and disclosure

- Security vulnerabilities should be reported through
  [GitHub Security Advisories](https://github.com/talkdedseccode/talkdedsec-editor/security/advisories/new),
  not through a public issue.
- Third-party licenses and notices are published in
  [`THIRD-PARTY-NOTICES.md`](https://github.com/talkdedseccode/talkdedsec-editor/blob/main/THIRD-PARTY-NOTICES.md).
- The editor binary is closed source and distributed under
  [Terms of Use](https://github.com/talkdedseccode/talkdedsec-editor/blob/main/LICENSE).
- Community themes and their validation tooling are maintained separately under the MIT license.
- Open VSX is used as the extension source; Marketplace-only extensions may not be available.

<br>

<details>
<summary><b>Türkçe özet</b></summary>

<br>

# Talkdedsec Editör

Talkdedsec; açık kaynak bir editör çekirdeği üzerine kurulan, Windows x64 için hazırlanmış, gereksiz
başlangıç işlerini ve kullanılmayan yerleşik bileşenleri azaltmayı hedefleyen bir kod editörüdür.

Temel yaklaşımı nettir:

- Telemetri ayarla kapatılmak yerine kaynaktan kaldırılır.
- Kurulum kullanıcı hesabına yapılır; yönetici yetkisi istenmez.
- Arka planda zorunlu güncelleme servisi çalışmaz.
- Gömülü ajan, kullanıcının seçtiği sağlayıcı hesabı üzerinden bağlanır.
- Eklentiler Open VSX üzerinden gelir.
- Editörün ayarları ve oturum verileri kendine ait `.talkdedsec` alanında tutulur.

### Güncel sürüm

| | |
|:--|--:|
| Sürüm | **v1.130.0** |
| Soğuk açılış | **0,41 sn** |
| Süreç | **9** |
| Yerleşik eklenti | **64** |
| Başlangıç telemetri uç noktası | **0** |
| Boşta bellek | **1,40 GB** |
| Kurulu boyut | **1,12 GB** |
| Kurulum dosyası | **253 MB** |

Ölçüm yöntemi ve ham sonuçlar:
[code.talkdedsec.com/tr/olcum](https://code.talkdedsec.com/tr/olcum/)

### İndirme güvenliği

Kurulum dosyası yalnızca
[`talkdedsec-editor` Releases](https://github.com/talkdedseccode/talkdedsec-editor/releases/latest)
sayfasından yayımlanır. Mevcut paket henüz kod imzalı olmadığı için çalıştırmadan önce SHA-256 değeri
kontrol edilmelidir.

```powershell
Get-FileHash .\TalkdedsecSetup.exe -Algorithm SHA256
```

Beklenen değer:

```text
3f8a6dda74030e30a85b5f72b327099f31859d5af8b144e6b678e1327d2129a8
```

Güvenlik açıklarını herkese açık issue olarak yazmak yerine
[özel güvenlik bildirimi](https://github.com/talkdedseccode/talkdedsec-editor/security/advisories/new)
üzerinden gönderin.

</details>

<br>

---

<p align="center">
  <sub>
    Built for a quieter editor, a smaller trust surface and a more predictable development environment.
  </sub>
</p>
