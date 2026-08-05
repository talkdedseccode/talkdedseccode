<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/banner-dark.svg">
  <img src="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/banner-light.svg" width="100%" alt="Talkdedsec Editor — a focused Windows code editor with no startup telemetry">
</picture>

<p align="center">
  <a href="https://code.talkdedsec.com"><b>Website</b></a>
  &nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://github.com/talkdedseccode/talkdedsec-editor/releases/latest"><b>Download</b></a>
  &nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://code.talkdedsec.com/en/belgeler/"><b>Documentation</b></a>
  &nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://github.com/talkdedseccode/talkdedsec-editor/discussions"><b>Discussions</b></a>
  &nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://github.com/talkdedseccode/talkdedsec-themes"><b>Themes</b></a>
  &nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://github.com/talkdedseccode/talkdedsec-editor/security"><b>Security</b></a>
</p>

<p align="center">
  <sub>Official GitHub account for <b>code.talkdedsec.com</b> and the Talkdedsec editor ecosystem.</sub>
</p>

<br>

<table>
<tr>
<td width="65%" valign="middle">

<sub>A SMALLER EDITOR. A CLEARER TRUST BOUNDARY.</sub>

# Talkdedsec Editor

A focused Windows code editor built from an open-source editor core, with telemetry, unused built-in
extensions and unnecessary startup work removed.

Talkdedsec is designed around one idea: opening a project should lead to a cursor, not a chain of
background services, reporting endpoints and product layers you never asked for.

<p>
  <kbd>Windows x64</kbd>
  <kbd>v1.130.0</kbd>
  <kbd>Per-user install</kbd>
  <kbd>No admin required</kbd>
  <kbd>Manual updates</kbd>
</p>

</td>
<td width="35%" align="center" valign="middle">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/goz-koyu.png">
  <img src="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/goz-acik.png" width="255" alt="Talkdedsec eye logo">
</picture>

<sub><b>LOOKS. LOGS NOTHING.</b></sub>

</td>
</tr>
</table>

<br>

## Why it exists

A modern editor can become a platform before it becomes useful: telemetry pipelines, update services,
account layers, bundled extensions and background work all compete with the actual job of editing code.

Talkdedsec takes the opposite direction. It keeps the familiar editor workflow, removes the parts that
are not required for that workflow and makes the remaining trust boundaries explicit.

<table>
<tr>
<td width="25%" align="center" valign="top">

### 0

startup telemetry endpoints

</td>
<td width="25%" align="center" valign="top">

### 0.41 s

measured cold start

</td>
<td width="25%" align="center" valign="top">

### 9

running processes

</td>
<td width="25%" align="center" valign="top">

### 64

built-in extensions

</td>
</tr>
</table>

<br>

## The operating principles

<table>
<tr>
<td width="50%" valign="top">

### Telemetry is removed, not muted

The base editor does not depend on an analytics pipeline or a startup reporting endpoint. Privacy is not
a switch that can be turned back on by a remote configuration.

</td>
<td width="50%" valign="top">

### Installation stays in user space

The editor installs inside the current Windows user profile, asks for no administrator privileges and
keeps its settings, extensions and session state separate from other editors.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### Updates do not run behind you

There is no background update service. A new release is installed manually over the existing version;
the user decides when the application changes.

</td>
<td width="50%" valign="top">

### The agent uses your provider account

The embedded agent connects through the account selected by the user. There is no Talkdedsec-hosted
proxy, seat fee or token resale layer between the editor and the chosen provider.

</td>
</tr>
</table>

<br>

## What the trust boundary looks like

```text
Talkdedsec Editor
├── stripped editor core
├── isolated .talkdedsec profile
├── extensions from Open VSX
└── embedded agent
    └── user-selected provider account
```

The base editor makes no startup telemetry connection. Extensions and the embedded agent may access the
network when the user installs, configures or invokes them; those requests are governed by the relevant
extension or provider.

<br>

## Measured, not estimated

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/sokuldu-dark.svg">
  <img src="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/sokuldu-light.svg" width="100%" alt="Before and after measurements for startup time, processes, built-in extensions and startup endpoints">
</picture>

<br>

| Measurement | Current build | Context |
|:--|--:|:--|
| Cold start | **0.41 s** | Production build, clean profile |
| Processes | **9** | After startup settles |
| Built-in extensions | **64** | 34 removed from the original set |
| Startup telemetry endpoints | **0** | Base editor startup |
| Idle memory | **1.40 GB** | Same measurement environment |
| Installed size | **1.12 GB** | Per-user installation |
| Installer size | **253 MB** | Windows x64 package |
| Source maps shipped | **0** | Production distribution |

<sub>
Measurement method and raw output:
<a href="https://code.talkdedsec.com/en/olcum/">code.talkdedsec.com/en/olcum</a>
</sub>

<br>

## Five complete themes, not five syntax palettes

<img src="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/themes.svg" width="100%" alt="Talkdedsec themes: Dark, Midnight, Matrix, Ember and Light">

Each built-in theme covers **183 interface colour keys** and a full **16-colour terminal palette**.
Changing a theme also changes panels, Git decorations and terminal colours instead of leaving parts of
the interface in the previous palette.

The community theme repository includes a dependency-free validator that checks submitted JSON and YAML,
required metadata, supported theme type values and colour formats before merge.

<p align="center">
  <a href="https://github.com/talkdedseccode/talkdedsec-themes"><b>Browse or contribute themes →</b></a>
</p>

<br>

## Download with a verifiable path

The Windows installer is distributed through the official
[`talkdedsec-editor` Releases page](https://github.com/talkdedseccode/talkdedsec-editor/releases/latest).
The current package is not code-signed yet, so its SHA-256 digest should be verified before execution.

<table>
<tr>
<td width="58%" valign="top">

### Verify with PowerShell

```powershell
Get-FileHash .\TalkdedsecSetup.exe -Algorithm SHA256
```

</td>
<td width="42%" valign="top">

### Current release

```text
TalkdedsecSetup.exe
v1.130.0
Windows x64
```

</td>
</tr>
</table>

Expected SHA-256:

```text
3f8a6dda74030e30a85b5f72b327099f31859d5af8b144e6b678e1327d2129a8
```

The result must match exactly. The machine-readable checksum is stored at
[`checksums/v1.130.0.sha256`](https://github.com/talkdedseccode/talkdedsec-editor/blob/main/checksums/v1.130.0.sha256).

<br>

## What is public, and what is not

<table>
<tr>
<td width="50%" valign="top">

### Public

- Product documentation and release notes
- Installer releases and checksums
- Security and contribution policies
- Third-party license notices
- Theme sources and validation tooling
- Issue and discussion history

</td>
<td width="50%" valign="top">

### Not public

- The editor's proprietary application source
- Private security advisory discussions
- User settings, extension state or agent sessions
- Provider credentials and account data
- Unpublished development builds

</td>
</tr>
</table>

The editor binary is closed source and distributed under its
[Terms of Use](https://github.com/talkdedseccode/talkdedsec-editor/blob/main/LICENSE). Open-source
components retain their original licenses, reproduced in
[`THIRD-PARTY-NOTICES.md`](https://github.com/talkdedseccode/talkdedsec-editor/blob/main/THIRD-PARTY-NOTICES.md).

<br>

## Repository map

<table>
<tr>
<td width="33%" valign="top">

### [`talkdedsec-editor`](https://github.com/talkdedseccode/talkdedsec-editor)

Official releases, documentation, issue tracking, Discussions, security policy, terms of use and
third-party notices.

**Access:** public documentation and binary releases  
**License:** editor Terms of Use

</td>
<td width="33%" valign="top">

### [`talkdedsec-themes`](https://github.com/talkdedseccode/talkdedsec-themes)

Built-in theme references, community submissions, contribution rules and automated validation tooling.

**Access:** public source  
**License:** MIT

</td>
<td width="33%" valign="top">

### [`talkdedseccode`](https://github.com/talkdedseccode/talkdedseccode)

The official GitHub profile for the project and a high-level map of the editor ecosystem.

**Access:** public profile  
**Purpose:** project overview

</td>
</tr>
</table>

<br>

## Support, contribution and security

| Need | Use |
|:--|:--|
| Download the editor | [Latest release](https://github.com/talkdedseccode/talkdedsec-editor/releases/latest) |
| Read documentation | [code.talkdedsec.com](https://code.talkdedsec.com) |
| Report a reproducible bug | [Issues](https://github.com/talkdedseccode/talkdedsec-editor/issues) |
| Ask a usage question | [Discussions](https://github.com/talkdedseccode/talkdedsec-editor/discussions) |
| Submit a theme | [talkdedsec-themes](https://github.com/talkdedseccode/talkdedsec-themes) |
| Report a vulnerability | [Private security advisory](https://github.com/talkdedseccode/talkdedsec-editor/security/advisories/new) |

Security vulnerabilities must not be posted in public Issues or Discussions. Use the private advisory
channel and include the affected version, impact and a reproducible test case when possible.

<br>

## Known boundaries

- The current Windows installer is **not code-signed**; verify its checksum before running it.
- The application binary is **closed source**, while third-party open-source notices are published.
- Extensions come from **Open VSX**; Marketplace-only extensions may be unavailable.
- There is **no automatic updater**; new versions are installed manually.
- Only the **latest published release** receives security fixes.

<br>

<details>
<summary><b>Türkçe sürüm</b></summary>

<br>

# Talkdedsec Editör

Talkdedsec; açık kaynak bir editör çekirdeğinden oluşturulan, Windows x64 için hazırlanmış, telemetriyi,
kullanılmayan yerleşik eklentileri ve gereksiz başlangıç işlerini azaltan odaklı bir kod editörüdür.

Amaç editörü daha büyük bir platforma dönüştürmek değil; proje açmak ile kod yazmaya başlamak arasındaki
yolu daha kısa, öngörülebilir ve denetlenebilir hâle getirmektir.

<p>
  <kbd>Windows x64</kbd>
  <kbd>v1.130.0</kbd>
  <kbd>Kullanıcı düzeyi kurulum</kbd>
  <kbd>Yönetici yetkisi yok</kbd>
  <kbd>Manuel güncelleme</kbd>
</p>

## Temel ilkeler

- **Telemetri kapatılmadı, kaldırıldı.** Temel editör açılışta analitik veya telemetri uç noktasına bağlanmaz.
- **Kurulum kullanıcı alanında kalır.** Yönetici yetkisi istemez ve kendi `.talkdedsec` profilini kullanır.
- **Arka planda zorunlu güncelleyici yoktur.** Yeni sürümün ne zaman kurulacağına kullanıcı karar verir.
- **Gömülü ajan kullanıcının sağlayıcı hesabını kullanır.** Arada Talkdedsec tarafından barındırılan bir proxy veya token satış katmanı yoktur.
- **Eklentiler Open VSX üzerinden gelir.** Yalnızca Marketplace'te bulunan bazı eklentiler kullanılamayabilir.

Temel editör başlangıç telemetrisi oluşturmaz. Eklentiler ve gömülü ajan, kullanıcı onları kurduğunda,
yapılandırdığında veya çalıştırdığında internete erişebilir; bu işlemler ilgili eklentinin ya da sağlayıcının
koşullarına tabidir.

## Güncel ölçümler

| Ölçüm | Güncel yapı |
|:--|--:|
| Soğuk açılış | **0,41 sn** |
| Süreç | **9** |
| Yerleşik eklenti | **64** |
| Başlangıç telemetri uç noktası | **0** |
| Boşta bellek | **1,40 GB** |
| Kurulu boyut | **1,12 GB** |
| Kurulum dosyası | **253 MB** |
| Dağıtılan source map | **0** |

Ölçüm yöntemi ve ham çıktı:
[code.talkdedsec.com/tr/olcum](https://code.talkdedsec.com/tr/olcum/)

## İndirme ve doğrulama

Kurulum dosyası yalnızca resmî
[`talkdedsec-editor` Releases](https://github.com/talkdedseccode/talkdedsec-editor/releases/latest)
sayfasından yayımlanır. Güncel paket henüz kod imzalı değildir; çalıştırmadan önce SHA-256 değerini
kontrol edin.

```powershell
Get-FileHash .\TalkdedsecSetup.exe -Algorithm SHA256
```

`v1.130.0` için beklenen değer:

```text
3f8a6dda74030e30a85b5f72b327099f31859d5af8b144e6b678e1327d2129a8
```

Sonuç birebir aynı olmalıdır.

## Şeffaflık sınırları

- Editörün uygulama binary'si kapalı kaynaktır ve kullanım şartlarıyla dağıtılır.
- Üçüncü taraf açık kaynak bileşenlerin lisansları ve bildirimleri yayımlanır.
- Mevcut kurulum dosyası kod imzalı değildir.
- Otomatik güncelleme servisi yoktur.
- Yalnızca en güncel release güvenlik düzeltmesi alır.
- Güvenlik açıkları herkese açık issue yerine
  [özel güvenlik bildirimi](https://github.com/talkdedseccode/talkdedsec-editor/security/advisories/new)
  üzerinden iletilmelidir.

## Depolar

- [`talkdedsec-editor`](https://github.com/talkdedseccode/talkdedsec-editor) — sürümler, belgeler, forum, kullanım şartları ve güvenlik politikası.
- [`talkdedsec-themes`](https://github.com/talkdedseccode/talkdedsec-themes) — tema kaynakları, topluluk katkıları ve doğrulama aracı.
- [`talkdedseccode`](https://github.com/talkdedseccode/talkdedseccode) — projenin resmî GitHub profili ve genel görünümü.

</details>

<br>

---

<p align="center">
  <sub>
    Built for a quieter editor, a smaller trust surface and a development environment that changes only when you decide it should.
  </sub>
</p>
