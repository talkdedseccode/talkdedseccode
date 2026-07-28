<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/banner-dark.svg">
  <img src="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/banner-light.svg" width="100%" alt="Talkdedsec — kod editörü. Telemetri yok.">
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
ayarla gizlenmedi, kaldırıldı. Açılışta bağlanılan sunucu yok. Güncelleme sunucusu yok. Yerleşik eklenti
sayısı 98'den 64'e indi. Geriye kalan editörün kendisi: dosya, düzenleyici, terminal, git, ve editörün
çekirdeğinde çalışan bir ajan.

Ölçümler tek bir makinede, üretim sürümü üzerinde, soğuk profille alındı. Yuvarlanmadı.

<sub><b>Windows x64 · sürüm 1.130.0 · kullanıcı düzeyi kurulum, yönetici hakkı istemez</b></sub>

</td></tr>
</table>

<br>

<table>
<tr>
<td width="66%" valign="top">

### Ölçümler

| | |
|:---|---:|
| Açılış, soğuk profil | **0,41 sn** |
| Süreç sayısı | **9** |
| Boşta bellek | **1,40 GB** |
| Kurulu boyut | **1,12 GB** |
| Kurulum dosyası | **253 MB** |
| Yerleşik eklenti | **64** <sub>← 98</sub> |
| Açılışta bağlanılan uç nokta | **0** |
| Pakette kalan source map | **0** |

<sub>Yöntem ve ham çıktılar: <a href="https://code.talkdedsec.com/tr/olcum/">code.talkdedsec.com/tr/olcum</a></sub>

</td>
<td width="34%" align="center" valign="top">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/goz-koyu.png">
  <img src="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/goz-acik.png" width="240" alt="Talkdedsec logosu — noktalardan oluşan bir göz">
</picture>

<sub><b>BAKAR, KAYDETMEZ</b></sub>

</td>
</tr>
</table>

<br>

### Temalar

<img src="https://raw.githubusercontent.com/talkdedseccode/talkdedseccode/main/assets/themes.svg" width="100%" alt="Beş tema: Dark, Midnight, Matrix, Ember, Light">

Kurulumla birlikte beş tema geliyor; her biri 183 renk anahtarı ve 16 renklik terminal paleti taşıyor.
Tema değişince editör kromu, paneller, git işaretleri ve terminal çıktısı birlikte dönüyor —
yalnız kod alanı değil.

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
server. Built-in extensions went from 98 down to 64. What remains is the editor itself: files, editor,
terminal, git, and an agent running in the editor core.

Measurements were taken on a single machine, on the production build, with a cold profile. Nothing rounded.

| | |
|:---|---:|
| Cold start, clean profile | **0.41 s** |
| Process count | **9** |
| Idle memory | **1.40 GB** |
| Installed size | **1.12 GB** |
| Installer | **253 MB** |
| Built-in extensions | **64** <sub>← 98</sub> |
| Endpoints contacted at startup | **0** |
| Source maps left in the package | **0** |

<sub>Method and raw output: <a href="https://code.talkdedsec.com/en/olcum/">code.talkdedsec.com/en/olcum</a></sub>

Five themes ship with the editor, each carrying 183 color keys and a 16-color terminal palette. Switching
a theme turns the editor chrome, panels, git decorations and terminal output together — not just the code area.

- **[talkdedsec-editor](https://github.com/talkdedseccode/talkdedsec-editor)** — docs, releases, terms of use and third-party notices
- **[talkdedsec-themes](https://github.com/talkdedseccode/talkdedsec-themes)** — community themes, via pull request, no account needed

</details>

<br>

---

<sub>
Editör açık kaynak bir editör çekirdeği üzerine kuruldu; lisans ve üçüncü taraf bildirimleri editör
deposunda. Editörün kendisi kapalı kaynaktır ve kullanım şartlarıyla dağıtılır. Temalar MIT.
</sub>


