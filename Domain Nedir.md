# 🌐 DOMAIN NEDİR?

**Domain** (Alan Adı), bir web sitesinin internetteki adı ve adresidir. Domain, **DNS** (Domain Name System - Alan Adı İsimlendirme Sistemi) ve **IP** (Internet Protocol - İnternet Protokolü) adresi denilen, bilgisayarların ve server'ların (sunucuların) birbirini tanımasını sağlayan isimlendirme ve numara sisteminin daha basitleştirilmiş ve akılda kalması için kelimelerle ifade edilmiş halidir. 

Örneğin; Extra Eğitim'in domain'leri (alan adları) `extraegitim.com` ve `extraacademy.com`'dur. `extraegitim.com` veya `extraacademy.com` domain'i (alan adı) browser'ın (tarayıcının) adres çubuğuna yazıldığında browser (tarayıcı) bu domain'i (alan adını) önce DNS (Domain Name System - Alan Adı İsimlendirme Sistemi) üzerinden IP (Internet Protocol - İnternet Protokolü) adresine çevirir, daha sonra kullanıcıyı bu IP (Internet Protocol - İnternet Protokolü) adresine sahip bilgisayara yönlendirir.

Domain'ler, karmaşık IP adreslerini (örneğin: `192.168.1.1`) hatırlanabilir isimlere (örneğin: `example.com`) dönüştürür.

---

## 📋 İçindekiler

- [🔍 Domain Nasıl Çalışır?](#-domain-nasıl-çalışır)
- [🏗️ Domain Yapısı](#️-domain-yapısı)
- [📝 Domain Türleri](#-domain-türleri)
- [🌍 En Popüler Domain Uzantıları](#-en-popüler-domain-uzantıları)
- [💰 Domain Fiyatlandırması](#-domain-fiyatlandırması)
- [🔧 DNS ve Domain İlişkisi](#-dns-ve-domain-ilişkisi)
- [✅ Domain Seçimi İpuçları](#-domain-seçimi-ipuçları)

---

## 🔍 Domain Nasıl Çalışır?

### 🌐 Temel Çalışma Prensibi

1. **Kullanıcı** tarayıcıya bir domain adı yazar (örn: `www.example.com`)
2. **DNS (Domain Name System)** bu domain'i IP adresine çevirir
3. **Tarayıcı** IP adresine bağlanır ve web sitesini gösterir

### 🔄 DNS Çözümleme Süreci

```
Kullanıcı → Tarayıcı → DNS Sunucusu → IP Adresi → Web Sunucusu → Web Sitesi
```

### 📡 IP (Internet Protocol) Adresi Nedir?

**IP (Internet Protocol - İnternet Protokolü) adresi**, interneti ya da **TCP/IP** (Transmission Control Protocol / Internet Protocol - İletim Kontrol Protokolü / İnternet Protokolü) kullanan diğer paket anahtarlamalı ağlara bağlı cihazların, ağ üzerinden birbirleri ile veri alışverişi yapmak için kullandıkları adrestir. İnternete bağlanan her bilgisayara, internet servis sağlayıcısı tarafından bir IP adresi atanır ve internetteki diğer bilgisayarlar bu bilgisayara verilen bu IP adresi üzerinden ulaşırlar.

IP adresine sahip iki farklı cihaz aynı ağda olmasa dahi, yönlendiriciler vasıtası ile birbirleri ile iletişim kurabilirler. IP adresleri şu anda yaygın kullanımda olan **IPv4** (Internet Protocol Version 4 - İnternet Protokolü Versiyon 4) için 32 bit boyunda olup, noktalarla ayrılmış 4 adet 8 bitlik sayıyla gösterilir. Örneğin: `216.239.38.10` vs.

### 🔗 TCP/IP (Transmission Control Protocol / Internet Protocol) Nedir?

**TCP/IP** (Transmission Control Protocol / Internet Protocol - İletim Kontrol Protokolü / İnternet Protokolü), bilgisayarlar ile veri iletme / alma birimleri arasında organizasyonu sağlayan, böylece bir yerden diğerine veri iletişimini olanaklı kılan pek çok veri iletişim protokolüne verilen genel addır. Bir başka değişle, TCP/IP bilgisayarlar arası veri iletişiminin kurallarını koyar. 

- **TCP (Transmission Control Protocol - İletim Kontrol Protokolü)**: Verinin iletimden önce paketlere ayrılmasını ve karşı tarafta bu paketlerin yeniden düzgün bir şekilde birleştirilmesini sağlar.
- **IP (Internet Protocol - İnternet Protokolü)**: İletilen paketlerin istenilen ağ adresine yönlendirilmesini kontrol eder.

---

## 🏗️ Domain Yapısı

### 📐 Domain Bileşenleri

Bir domain adı şu bölümlerden oluşur:

```
www.example.com
│  │       │
│  │       └─ TLD (Top-Level Domain)
│  └───────── SLD (Second-Level Domain)
└──────────── Subdomain (Alt Domain)
```

| Bileşen | Açıklama | Örnek |
|:--------|:---------|:------|
| **Subdomain** | Ana domain'in alt alan adı | `www`, `mail`, `blog` |
| **SLD** | İkinci seviye domain (ana isim) | `example` |
| **TLD** | Üst seviye domain (uzantı) | `.com`, `.org`, `.net` |

### 📊 Örnek Domain Yapıları

| Domain | Subdomain | SLD | TLD | Açıklama |
|:-------|:---------|:----|:----|:---------|
| `www.example.com` | `www` | `example` | `.com` | Standart web sitesi |
| `mail.example.com` | `mail` | `example` | `.com` | E-posta sunucusu |
| `blog.example.com` | `blog` | `example` | `.com` | Blog alt domain'i |
| `example.com` | - | `example` | `.com` | Kök domain (subdomain yok) |

---

## 📝 Domain Türleri

### 🎯 TLD (Top-Level Domain) Kategorileri

#### 🌍 gTLD (Generic Top-Level Domain)

Genel amaçlı domain uzantıları:

| Uzantı | Açıklama | Kullanım |
|:------|:---------|:---------|
| `.com` | Commercial (Ticari) | En popüler, ticari siteler |
| `.org` | Organization (Organizasyon) | Kar amacı gütmeyen kuruluşlar |
| `.net` | Network (Ağ) | Ağ ve teknoloji şirketleri |
| `.info` | Information (Bilgi) | Bilgilendirme siteleri |
| `.biz` | Business (İş) | İşletmeler |
| `.xyz` | Genel | Modern, genel kullanım |
| `.online` | Online | Online hizmetler |
| `.site` | Site | Web siteleri |
| `.store` | Store (Mağaza) | E-ticaret siteleri |
| `.tech` | Technology (Teknoloji) | Teknoloji şirketleri |

#### 🏛️ ccTLD (Country Code Top-Level Domain)

Ülke kodlu domain uzantıları:

| Uzantı | Ülke/Bölge | Açıklama |
|:------|:-----------|:---------|
| `.tr` | Türkiye | Türkiye için resmi domain |
| `.us` | Amerika Birleşik Devletleri | ABD için domain |
| `.uk` | Birleşik Krallık | İngiltere için domain |
| `.de` | Almanya | Almanya için domain |
| `.fr` | Fransa | Fransa için domain |
| `.jp` | Japonya | Japonya için domain |
| `.cn` | Çin | Çin için domain |
| `.ru` | Rusya | Rusya için domain |
| `.au` | Avustralya | Avustralya için domain |
| `.ca` | Kanada | Kanada için domain |

#### 🏢 sTLD (Sponsored Top-Level Domain)

Sponsorlu domain uzantıları:

| Uzantı | Açıklama | Kullanım |
|:------|:---------|:---------|
| `.edu` | Education (Eğitim) | Eğitim kurumları (ABD) |
| `.gov` | Government (Hükümet) | Devlet kurumları (ABD) |
| `.mil` | Military (Askeri) | Askeri kurumlar (ABD) |
| `.int` | International (Uluslararası) | Uluslararası organizasyonlar |
| `.aero` | Aviation (Havacılık) | Havacılık sektörü |
| `.museum` | Museum (Müze) | Müzeler |
| `.coop` | Cooperative (Kooperatif) | Kooperatifler |

---

## 🌍 En Popüler Domain Uzantıları

### 📊 Dünya Çapında Kullanım İstatistikleri

| Sıra | Uzantı | Kullanım Oranı | Açıklama |
|:----:|:------|:--------------|:---------|
| 1 | `.com` | ~48% | En popüler ve güvenilir |
| 2 | `.org` | ~4% | Organizasyonlar için |
| 3 | `.net` | ~3% | Ağ ve teknoloji |
| 4 | `.info` | ~2% | Bilgilendirme |
| 5 | `.co` | ~1% | Kolombiya/Şirket alternatifi |
| 6 | `.io` | ~1% | Teknoloji startupları |
| 7 | `.xyz` | ~1% | Modern, genel kullanım |

---

## 💰 Domain Fiyatlandırması

### 💵 Ortalama Domain Fiyatları (Yıllık)

| Uzantı | Ortalama Fiyat (USD) | Ortalama Fiyat (TL) | Notlar |
|:------|:-------------------|:-------------------|:-------|
| `.com` | $10-15 | ₺300-450 | En popüler |
| `.org` | $12-18 | ₺360-540 | Organizasyonlar |
| `.net` | $12-18 | ₺360-540 | Ağ servisleri |
| `.info` | $2-15 | ₺60-450 | Bilgilendirme |
| `.biz` | $3-20 | ₺90-600 | İşletmeler |
| `.tr` | ₺50-150 | ₺50-150 | Türkiye domain'i |
| `.io` | $30-50 | ₺900-1500 | Teknoloji |
| `.xyz` | $1-15 | ₺30-450 | Genel kullanım |

### 💡 Maliyet Faktörleri

- **Uzantı Türü**: Bazı uzantılar daha pahalıdır
- **Domain Kayıt Şirketi**: Farklı fiyatlandırmalar
- **Özel Domain'ler**: Premium domain'ler çok daha pahalı
- **Yenileme Ücreti**: İlk yıl indirimli olabilir

### 📝 Önemli Notlar

**Domain Kiralama Sistemi:**
- Domain'ler, internet servis sağlayıcılarından veya register (kayıt) firmalarından satın alınarak, kaydetmesi istenebilir. 
- **Aslında domain (alan adı), satın aldığınız değil kiraladığınız bir hizmettir.**
- Minimum bir yıl maksimum on yıl kayıt ettirilebilir. 
- Kayıt ettirilen her domain (alan adı) zaman içerisinde yenilenebilir veya başka bir firmaya transfer edilebilir.

**Türkiye Domain Uzantıları (.tr):**
- Türkiye'nin ülke domain uzantısı (alan adı) olan `.tr` uzantılı domain'ler (`.com.tr`, `.net.tr` vs.), **ODTÜ** (Orta Doğu Teknik Üniversitesi) (http://www.nic.tr) tarafından yönetilmekte ve tahsis edilmektedir. 
- Bu domain'ler (alan adları) ise, minimum bir yıl maksimum beş yıl kayıt ettirilebilir. 
- Kayıt ettirilen her domain (alan adı) zaman içerisinde yenilenebilir fakat ODTÜ (Orta Doğu Teknik Üniversitesi) tarafından başka bir firmaya transfer edilemezler.

---

## 🔧 DNS ve Domain İlişkisi

### 🌐 DNS (Domain Name System) Nedir?

**DNS (Domain Name System - Alan Adı İsimlendirme Sistemi)**, web space'ı (web alanını) bölümlemeye, bölümleri adlandırmaya ve bölümler arası iletişimi organize etmeye yarayan, bilgisayar, servis, internet veya özel bir ağa bağlı herhangi bir kaynak için hiyerarşik dağıtılmış bir adlandırma sistemidir. 

Kısaca DNS, domain (alan adı) ile IP (Internet Protocol - İnternet Protokolü) adresleri arasındaki bağlantıyı kurmak amacıyla geliştirilmiş bir sistemdir. DNS sayesinde IP adresinin hangi bilgisayara bağlı olduğu bulunur. Dolayısıyla istenilen sitenin yeri belirlenmiş olur. Ayrıca farklı bir işlem yapılmak isteniyor ise istediğiniz yere de ulaşmanızı sağlar.

DNS, domain adlarını IP adreslerine çeviren bir sistemdir.

### 🔄 DNS Kayıt Türleri

| Kayıt Türü | Kısaltma | Açıklama | Örnek |
|:-----------|:--------|:---------|:------|
| **A Record** | A | IPv4 adresini gösterir | `192.168.1.1` |
| **AAAA Record** | AAAA | IPv6 adresini gösterir | `2001:0db8::1` |
| **CNAME** | CNAME | Başka bir domain'e yönlendirir | `www` → `example.com` |
| **MX Record** | MX | E-posta sunucusu adresi | `mail.example.com` |
| **TXT Record** | TXT | Metin bilgisi (SPF, DKIM vb.) | `v=spf1 include:_spf.google.com` |
| **NS Record** | NS | Name Server (İsim sunucusu) | `ns1.example.com` |
| **SOA Record** | SOA | Start of Authority (Yetki başlangıcı) | Domain yönetim bilgileri |

---

## ✅ Domain Seçimi İpuçları

### 🎯 İyi Bir Domain Seçmek İçin

#### ✅ Yapılması Gerekenler

- ✅ **Kısa ve Hatırlanabilir**: Kolay yazılabilir ve hatırlanabilir olmalı. **Domain seçerken kolay ve hatırlanabilir olması, ulaşılabilirlik açısından oldukça önem taşımaktadır.**
- ✅ **Açıklayıcı**: İşinizi veya içeriğinizi yansıtmalı
- ✅ **Anahtar Kelime İçermeli**: SEO için önemli
- ✅ **Hiphen (-) Kullanmayın**: Mümkünse kullanmayın
- ✅ **Sayı Kullanmayın**: Karışıklığa neden olabilir
- ✅ **Telif Hakkı Kontrolü**: Başka bir markayla çakışmamalı
- ✅ **Sosyal Medya Uyumluluğu**: Sosyal medya hesaplarıyla uyumlu olmalı

#### ❌ Yapılmaması Gerekenler

- ❌ Çok uzun domain'ler
- ❌ Karmaşık yazımlar
- ❌ Telif hakkı ihlali riski
- ❌ Çok fazla sayı ve özel karakter
- ❌ Belirsiz veya anlamsız isimler

### 📝 Domain Seçim Örnekleri

| ✅ İyi Örnekler | ❌ Kötü Örnekler | Açıklama |
|:---------------|:----------------|:---------|
| `techstore.com` | `tech-store-2024-online-shop.com` | Çok uzun |
| `myblog.com` | `my-blog-123.com` | Sayı ve tire kullanımı |
| `designstudio.com` | `dsgnstudi0.com` | Karmaşık yazım |
| `coffeeshop.com` | `coffee-shop-istanbul-turkey.com` | Gereksiz detaylar |

---

## 🔐 Domain Güvenliği

### 🛡️ Önemli Güvenlik Önlemleri

1. **Domain Kilitleme**: Yetkisiz transferleri önler
2. **WHOIS Gizliliği**: Kişisel bilgileri korur
3. **İki Faktörlü Doğrulama**: Hesap güvenliğini artırır
4. **Otomatik Yenileme**: Domain'in süresi dolmasını önler
5. **Güvenli Şifre**: Güçlü ve benzersiz şifre kullanın

---

## 📅 Domain Yaşam Döngüsü

### 🔄 Domain Kayıt Süreci

1. **Kullanılabilirlik Kontrolü**: Domain'in müsait olup olmadığını kontrol edin
2. **Kayıt**: Domain kayıt şirketinden satın alın
3. **DNS Yapılandırması**: DNS kayıtlarını yapılandırın
4. **Yenileme**: Her yıl yenileme yapın
5. **Süre Dolması**: Süre dolduğunda yenileme yapılmazsa domain serbest kalır

### ⏰ Domain Süresi Dolma Süreci

- **0-30 gün**: Normal kullanım
- **30-60 gün**: Grace Period (İtiraz süresi) - Ek ücretle yenilenebilir
- **60-75 gün**: Redemption Period (Kurtarma süresi) - Yüksek ücretle kurtarılabilir
- **75+ gün**: Domain serbest kalır, herkes satın alabilir

---

## 🌐 Domain Kayıt Şirketleri

### 🏢 Popüler Domain Kayıt Şirketleri

| Şirket | Özellikler | Fiyat Aralığı |
|:-------|:----------|:-------------|
| **GoDaddy** | En büyük kayıt şirketi | $2-20/yıl |
| **Namecheap** | Uygun fiyatlı, güvenilir | $1-15/yıl |
| **Google Domains** | Google'ın domain servisi | $12/yıl |
| **Cloudflare** | Ücretsiz WHOIS gizliliği | Maliyet fiyatı |
| **Name.com** | Kullanıcı dostu arayüz | $3-20/yıl |
| **Türkiye'de**: | | |
| **Turhost** | Türk kayıt şirketi | ₺50-200/yıl |
| **Natro** | Türk kayıt şirketi | ₺40-180/yıl |
| **GetYours** | Türk kayıt şirketi | ₺45-190/yıl |

---

## 📌 Dokümantasyon Bilgileri

| Bilgi | Detay |
|:------|:------|
| 👤 **Yazar** | Bahadır B. Bekdemir |
| 📅 **Tarih** | 15.01.2026 |
| 🔢 **Versiyon** | 1.0 |

---

> 💡 **İpucu:** Domain seçerken, markanızı yansıtan, SEO dostu ve kolay hatırlanabilir bir isim seçmek önemlidir. Ayrıca domain'inizi zamanında yenilemeyi unutmayın!

