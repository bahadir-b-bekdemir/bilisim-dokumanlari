# 🌐 TARAYICILAR VE TARAYICI GÖRÜNTÜLEME MOTORLARI

Hazırlanmış olan bir web sayfası içeriğini görüntülemeye yarayan programlara **browser** (tarayıcı) adı verilir. **HTML** (Hyper Text Markup Language - Zengin Metin İşaretleme Dili), **XML** (Extensible Markup Language - Genişletilebilir İşaretleme Dili), **Javascript**, **CSS** (Cascading Style Sheets - Basamaklı Stil Şablonları veya Basamaklı Biçim Sayfaları), **XSL** (Extensible Style Language - Genişletilebilir Stil Dili) vs. gibi bir browser'ın (tarayıcının) bel kemiği olan özellikleri render'layan (sunan) gömülü kit veya programlara da **browser visualization engine** (tarayıcı görüntüleme motoru) denir.

Günümüzde, **Google Chrome**, **Internet Explorer**, **Microsoft Edge**, **Mozilla Firefox**, **Opera**, **Safari**, **Yandex Browser** vs. browser'lar (tarayıcılar) sıklıkla kullanılmaktadır.

Browser'lar (tarayıcılar), web sayfamızın içeriğini **browser visualization engine** (tarayıcı görüntüleme motoru) denilen sistemleri sayesinde kullanıcılara görüntülerler. Yazılım veya tasarım alanında yenilikler oldukça browser visualization engine'ları da (tarayıcı görüntüleme motorları da) sürekli olarak geliştirici firma tarafından isteklere cevap verebilmesi için güncellenirler.

İlgili browser (tarayıcı) sürümü güncellendiği zaman aslında bu browser'ın (tarayıcının) visualization engine'ı da (görüntüleme motoru da) güncellenir. Bazen browser'ın (tarayıcının) görselliğinin de iyileştirme işlemlerinde kullanılır. Browser (tarayıcı) geliştiren firmalar daima visualization engine'larına (görüntüleme motorlarına) uyarlı uygulamalar yaparlar.

---

## 📋 İçindekiler

- [🔍 Görüntüleme Motorları Hakkında](#-görüntüleme-motorları-hakkında)
- [📊 Tarayıcı ve Görüntüleme Motoru Tablosu](#-tarayıcı-ve-görüntüleme-motoru-tablosu)
- [📈 Pazar Payı Bilgileri](#-pazar-payı-bilgileri)

---

## 🔍 Görüntüleme Motorları Hakkında

### 🎯 Ana Görüntüleme Motorları

| Motor | Geliştirici | Açıklama |
|:------|:-----------|:---------|
| **Blink** | Google, Opera | Chromium projesinin bir parçası. WebKit'ten fork edilmiştir. |
| **WebKit** | Apple | Açık kaynaklı görüntüleme motoru. Safari ve eski Chrome'da kullanıldı. |
| **Gecko** | Mozilla | Firefox ve Thunderbird'de kullanılan açık kaynaklı motor. |
| **Trident** | Microsoft | Internet Explorer ve eski Edge'de kullanılan motor. (Artık geliştirilmiyor) |
| **EdgeHTML** | Microsoft | Microsoft Edge'in eski sürümlerinde kullanılan motor. (Artık kullanılmıyor) |
| **Presto** | Opera Software | Opera'nın eski sürümlerinde kullanılan motor. (Artık kullanılmıyor) |

### ⚙️ JavaScript Motorları

| Motor | Tarayıcı | Açıklama |
|:------|:---------|:---------|
| **V8** | Chrome, Edge, Opera, Vivaldi | Google tarafından geliştirilen yüksek performanslı JavaScript motoru. |
| **SpiderMonkey** | Firefox | Mozilla tarafından geliştirilen JavaScript motoru. |
| **JavaScriptCore (Nitro)** | Safari | Apple tarafından geliştirilen JavaScript motoru. |
| **Chakra** | Internet Explorer, Eski Edge | Microsoft tarafından geliştirilen JavaScript motoru. (Artık kullanılmıyor) |

---

## 📊 Tarayıcı ve Görüntüleme Motoru Tablosu

| 🖥️ Tarayıcı | 🏢 Geliştirici | 🎨 Görüntüleme Motoru | ⚡ JavaScript Motoru | 📱 Platform | 📅 Durum | 🔖 User-Agent Öneki |
|:-----------|:--------------|:---------------------|:-------------------|:----------|:--------|:------------------|
| **Google Chrome** | Google | Blink | V8 | Windows, macOS, Linux, Android, iOS | ✅ Aktif | `Chrome` |
| **Microsoft Edge** (Yeni) | Microsoft | Blink | V8 | Windows, macOS, Linux, Android, iOS | ✅ Aktif | `Edg` |
| **Microsoft Edge** (Eski) | Microsoft | EdgeHTML | Chakra | Windows 10 | ❌ Durduruldu | `Edge` |
| **Internet Explorer** | Microsoft | Trident | Chakra | Windows | ❌ Durduruldu | `MSIE` / `Trident` |
| **Mozilla Firefox** | Mozilla Foundation | Gecko | SpiderMonkey | Windows, macOS, Linux, Android, iOS | ✅ Aktif | `Firefox` |
| **Safari** | Apple | WebKit | JavaScriptCore (Nitro) | macOS, iOS | ✅ Aktif | `Safari` |
| **Opera** (Yeni) | Opera Software | Blink | V8 | Windows, macOS, Linux, Android, iOS | ✅ Aktif | `OPR` |
| **Opera** (Eski) | Opera Software | Presto | Carakan | Windows, macOS, Linux | ❌ Durduruldu | `Opera` |
| **Yandex Browser** | Yandex | Blink | V8 | Windows, macOS, Linux, Android, iOS | ✅ Aktif | `YaBrowser` |
| **Brave** | Brave Software | Blink | V8 | Windows, macOS, Linux, Android, iOS | ✅ Aktif | `Brave` |
| **Vivaldi** | Vivaldi Technologies | Blink | V8 | Windows, macOS, Linux, Android | ✅ Aktif | `Vivaldi` |
| **Tor Browser** | The Tor Project | Gecko | SpiderMonkey | Windows, macOS, Linux, Android | ✅ Aktif | `Firefox` |
| **Samsung Internet** | Samsung | Blink | V8 | Android | ✅ Aktif | `SamsungBrowser` |
| **UC Browser** | UCWeb | Blink (Yeni) / U2 (Eski) | V8 | Windows, Android, iOS | ✅ Aktif | `UCBrowser` |
| **Baidu Browser** | Baidu | Blink | V8 | Windows, Android, iOS | ✅ Aktif | `Baidu` |
| **QQ Browser** | Tencent | Blink | V8 | Windows, Android, iOS | ✅ Aktif | `QQBrowser` |
| **360 Secure Browser** | Qihoo 360 | Blink | V8 | Windows, Android | ✅ Aktif | `360SE` / `360EE` |
| **Maxthon** | Maxthon International | Blink (Yeni) / Trident (Eski) | V8 | Windows, macOS, Android, iOS | ✅ Aktif | `Maxthon` |
| **Pale Moon** | Moonchild Productions | Goanna (Gecko fork) | SpiderMonkey | Windows, Linux | ✅ Aktif | `PaleMoon` |
| **Waterfox** | System1 | Gecko | SpiderMonkey | Windows, macOS, Linux | ✅ Aktif | `Waterfox` |
| **Basilisk** | Moonchild Productions | Goanna (Gecko fork) | SpiderMonkey | Windows, Linux | ✅ Aktif | `Basilisk` |
| **Falkon** | KDE | QtWebEngine (Blink) | V8 | Linux, Windows | ✅ Aktif | `Falkon` |
| **Konqueror** | KDE | KHTML (Eski) / WebKit (Yeni) | JavaScriptCore | Linux | ✅ Aktif | `Konqueror` |
| **Midori** | Christian Dywan | WebKit | JavaScriptCore | Linux, Windows | ✅ Aktif | `Midori` |
| **Epiphany (GNOME Web)** | GNOME | WebKit | JavaScriptCore | Linux | ✅ Aktif | `Epiphany` |
| **Lunascape** | Lunascape Corporation | Trident / Gecko / WebKit | Chakra / SpiderMonkey / JavaScriptCore | Windows | ⚠️ Sınırlı | `Lunascape` |
| **Avant Browser** | Avant Force | Trident / Gecko | Chakra / SpiderMonkey | Windows | ⚠️ Sınırlı | `Avant` |
| **Sleipnir** | Fenrir Inc. | Blink | V8 | Windows, macOS, Android, iOS | ✅ Aktif | `Sleipnir` |
| **Coc Coc** | Coc Coc Inc. | Blink | V8 | Windows, Android | ✅ Aktif | `CocCoc` |
| **Naver Whale** | Naver Corporation | Blink | V8 | Windows, macOS, Android | ✅ Aktif | `Whale` |
| **SRWare Iron** | SRWare | Blink | V8 | Windows, macOS, Linux | ✅ Aktif | `Iron` |
| **Comodo Dragon** | Comodo Group | Blink | V8 | Windows | ✅ Aktif | `Comodo` |
| **Chromium** | Chromium Project | Blink | V8 | Windows, macOS, Linux | ✅ Aktif | `Chromium` |
| **Ungoogled Chromium** | Eloston | Blink | V8 | Windows, macOS, Linux | ✅ Aktif | `Chromium` |
| **Microsoft Edge Legacy** | Microsoft | EdgeHTML | Chakra | Windows 10 | ❌ Durduruldu | `Edge` |
| **Internet Explorer Mobile** | Microsoft | Trident | Chakra | Windows Phone | ❌ Durduruldu | `IEMobile` |
| **Opera Mini** | Opera Software | Presto (Sunucu tarafı) | - | Android, iOS | ✅ Aktif | `Opera Mini` |
| **Opera Touch** | Opera Software | Blink | V8 | Android, iOS | ✅ Aktif | `OPR` |
| **Firefox Focus** | Mozilla Foundation | Gecko | SpiderMonkey | Android, iOS | ✅ Aktif | `Focus` |
| **Firefox Klar** | Mozilla Foundation | Gecko | SpiderMonkey | Android | ✅ Aktif | `Klar` |
| **DuckDuckGo Browser** | DuckDuckGo | Blink (Android) / WebKit (iOS) | V8 / JavaScriptCore | Android, iOS | ✅ Aktif | `DuckDuckGo` |

---

## 📈 Pazar Payı Bilgileri

### 🌍 Dünya Çapında Pazar Payı (2024)

| Tarayıcı | Pazar Payı | Notlar |
|:---------|:----------|:-------|
| **Google Chrome** | ~65% | En popüler tarayıcı |
| **Safari** | ~19% | Özellikle macOS ve iOS'ta güçlü |
| **Microsoft Edge** | ~5% | Windows 10/11 ile birlikte gelir |
| **Mozilla Firefox** | ~3% | Açık kaynak topluluğu tarafından desteklenir |
| **Opera** | ~2% | Özellikle mobilde popüler |
| **Samsung Internet** | ~2% | Android cihazlarda yaygın |
| **Diğerleri** | ~4% | Yandex, Brave, Vivaldi vb. |

### 📱 Mobil Pazar Payı

| Tarayıcı | Pazar Payı | Notlar |
|:---------|:----------|:-------|
| **Chrome Mobile** | ~65% | Android ve iOS'ta yaygın |
| **Safari Mobile** | ~25% | iOS cihazlarda varsayılan |
| **Samsung Internet** | ~5% | Samsung cihazlarda varsayılan |
| **Opera Mobile/Mini** | ~2% | Veri tasarrufu özellikleri |
| **Diğerleri** | ~3% | Firefox, UC Browser vb. |

---

## 🔧 Görüntüleme Motoru Karşılaştırması

| Özellik | Blink | WebKit | Gecko | Trident | EdgeHTML |
|:--------|:-----|:-------|:------|:--------|:---------|
| **Geliştirici** | Google, Opera | Apple | Mozilla | Microsoft | Microsoft |
| **Açık Kaynak** | ✅ Evet | ✅ Evet | ✅ Evet | ❌ Hayır | ❌ Hayır |
| **Durum** | ✅ Aktif | ✅ Aktif | ✅ Aktif | ❌ Durduruldu | ❌ Durduruldu |
| **Kullanıldığı Yerler** | Chrome, Edge, Opera | Safari | Firefox | IE (Eski) | Edge (Eski) |
| **Standart Desteği** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐⭐ |
| **Performans** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐ | ⭐⭐⭐ |

---

## 💡 Önemli Notlar

### 🔴 Durdurulan Tarayıcılar

- **Internet Explorer**: Microsoft tarafından 15 Haziran 2022'de resmi olarak durduruldu.
- **Microsoft Edge Legacy (EdgeHTML)**: Chromium tabanlı yeni Edge'e geçiş yapıldı.
- **Opera (Presto)**: 2013'te Blink motoruna geçiş yapıldı.

### ✅ Aktif Geliştirme

- **Blink**: Google ve Opera tarafından aktif olarak geliştirilmektedir.
- **Gecko**: Mozilla tarafından aktif olarak geliştirilmektedir.
- **WebKit**: Apple tarafından aktif olarak geliştirilmektedir.

### 🎯 Web Geliştirme İçin Öneriler

1. **Chrome/Edge (Blink)**: Modern web standartları için en iyi destek
2. **Firefox (Gecko)**: Açık kaynak ve gizlilik odaklı
3. **Safari (WebKit)**: macOS ve iOS kullanıcıları için önemli
4. **Cross-browser Testing**: Tüm ana tarayıcılarda test yapın

---

## 📌 Dokümantasyon Bilgileri

| Bilgi | Detay |
|:------|:------|
| 👤 **Yazar** | Bahadır B. Bekdemir |
| 📅 **Tarih** | 15.01.2026 |
| 🔢 **Versiyon** | 2.0 |

---

> 💡 **İpucu:** Web geliştirme yaparken, farklı görüntüleme motorlarını test etmek önemlidir. Her motor, web standartlarını farklı şekillerde yorumlayabilir.
