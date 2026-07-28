<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/banner-dark.svg">
  <img src="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/banner-light.svg" width="100%" alt="Talkdedsec — kod editörü. Telemetri yok. 0,41 sn açılış, 9 süreç, 64 eklenti, 0 telemetri ucu.">
</picture>

<p align="center">
  <a href="https://code.talkdedsec.com"><b>code.talkdedsec.com</b></a>
  &nbsp;·&nbsp;
  <a href="https://github.com/talkdedseccode/talkdedsec-editor"><b>editör</b></a>
  &nbsp;·&nbsp;
  <a href="https://github.com/talkdedseccode/talkdedsec-themes"><b>temalar</b></a>
  &nbsp;·&nbsp;
  <a href="https://github.com/talkdedseccode/talkdedsec-editor/discussions"><b>forum</b></a>
</p>

<br>

<table>
<tr><td valign="top">

<sub>ŞU AN ÜZERİNDE ÇALIŞTIĞIM</sub>

## [Talkdedsec](https://code.talkdedsec.com)

**Açtığın anda hazır olan bir kod editörü.**

Modern editörler her açılışta bir sürü şeyi birlikte getiriyor: kullanmadığın dil paketleri, arka planda
konuşan telemetri katmanları, güncelleme kontrolleri, kurulum sırasında sormadan eklenen servisler.
Bunların hiçbiri sana bir şey kazandırmıyor ama açılış süresini, bellek kullanımını ve süreç sayısını
belirleyen şey tam olarak bunlar.

Talkdedsec bu katmanların sökülmesiyle ortaya çıktı. Telemetri kaynaktan kaldırıldı — kapatılmadı,
ayarla gizlenmedi, kaldırıldı. Açılışta bağlanılan sunucu yok. Güncelleme sunucusu yok. Geriye kalan
editörün kendisi: dosya, düzenleyici, terminal, git, ve editörün çekirdeğinde çalışan bir ajan.

<sub><b>Windows x64 · sürüm 1.130.0 · kullanıcı düzeyi kurulum, yönetici hakkı istemez</b></sub>

</td></tr>
</table>

<br>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/sokuldu-dark.svg">
  <img src="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/sokuldu-light.svg" width="100%" alt="Sökülmeden önce ve sonra: açılış 2-4 sn'den 0,41 sn'ye, süreç 12-14'ten 9'a, yerleşik eklenti 98'den 64'e, açılışta bağlanılan uç nokta sıfıra indi.">
</picture>

<br>

<table>
<tr>
<td width="62%" valign="top">

### Geri kalan ölçümler

| | |
|:---|---:|
| Boşta bellek | **1,40 GB** |
| Kurulu boyut | **1,12 GB** |
| Kurulum dosyası | **253 MB** |
| Pakette kalan source map | **0** |
| Tema | **5** <sub>× 183 renk anahtarı</sub> |
| Eklenti kaynağı | **Open VSX** |

<sub>Yöntem ve ham çıktılar: <a href="https://code.talkdedsec.com/tr/olcum/">code.talkdedsec.com/tr/olcum</a></sub>

</td>
<td width="38%" align="center" valign="middle">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/goz-koyu.png">
  <img src="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/goz-acik.png" width="300" alt="Talkdedsec logosu — noktalardan oluşan bir göz">
</picture>

<sub><b>BAKAR, KAYDETMEZ</b></sub>

</td>
</tr>
</table>

<br>

### Temalar

<img src="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/themes.svg" width="100%" alt="Beş tema: Dark, Midnight, Matrix, Ember, Light">

Her tema 183 renk anahtarı ve 16 renklik terminal paleti taşıyor. Tema değişince editör kromu, paneller,
git işaretleri ve terminal çıktısı birlikte dönüyor — yalnız kod alanı değil.

<br>

### Depolar

- **[talkdedsec-editor](https://github.com/talkdedseccode/talkdedsec-editor)** — editörün belgeleri, sürümleri, kullanım şartları ve üçüncü taraf bildirimleri
- **[talkdedsec-themes](https://github.com/talkdedseccode/talkdedsec-themes)** — topluluk temaları; hesap açmadan, pull request ile

<br>

<details>
<summary><b>English</b></summary>

<br>

**A code editor that is ready the moment you open it.**

Modern editors bring a lot along on every launch: language packs you never use, telemetry layers talking
in the background, update checks, services added during install without asking. None of it does anything
for you, yet it is exactly what determines startup time, memory use and process count.

Talkdedsec is what was left after those layers were stripped out. Telemetry was removed at the source —
not disabled, not hidden behind a setting, removed. No server is contacted at startup. There is no update
server. What remains is the editor itself: files, editor, terminal, git, and an agent running in the editor core.

**Before and after the strip** — cold start 2–4 s → **0.41 s** · processes 12–14 → **9** ·
built-in extensions 98 → **64** · endpoints contacted at startup → **0**

| | |
|:---|---:|
| Idle memory | **1.40 GB** |
| Installed size | **1.12 GB** |
| Installer | **253 MB** |
| Source maps left in the package | **0** |
| Themes | **5** <sub>× 183 color keys</sub> |
| Extension source | **Open VSX** |

<sub>Measured on a single machine, on the production build, with a cold profile. Nothing rounded.
Method and raw output: <a href="https://code.talkdedsec.com/en/olcum/">code.talkdedsec.com/en/olcum</a></sub>

Each theme carries 183 color keys and a 16-color terminal palette. Switching a theme turns the editor
chrome, panels, git decorations and terminal output together — not just the code area.

- **[talkdedsec-editor](https://github.com/talkdedseccode/talkdedsec-editor)** — docs, releases, terms of use and third-party notices
- **[talkdedsec-themes](https://github.com/talkdedseccode/talkdedsec-themes)** — community themes, via pull request, no account needed

</details>

<br>

---

<sub>
Editör açık kaynak bir editör çekirdeği üzerine kuruldu; lisans ve üçüncü taraf bildirimleri editör
deposunda. Editörün kendisi kapalı kaynaktır ve kullanım şartlarıyla dağıtılır. Temalar MIT.
</sub>
