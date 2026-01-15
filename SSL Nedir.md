# 🔒 SSL NEDİR?

**SSL** (Secure Socket Layer - Güvenli Giriş Katmanı), bilgisayar ağı üzerinden güvenli haberleşmeyi sağlamak için tasarlanmış kriptolama protokolleridir. SSL kişisel gizlilik ve güvenilirlik sağlayan, ağ üzerindeki bilgi transferi sırasında bilginin bütünlüğü ve gizliliği için sunucu (server) ile client (istemci) arasındaki iletişimin şifrelenmiş şekilde yapılabilmesine imkan verir. 

SSL, standart bir algoritmadır. **Public key (açık anahtar)** ve **private key (özel anahtar)** adı verilen anahtarların kullanımına dayalı bir kodlama yöntemine dayalıdır.

SSL (Secure Socket Layer - Güvenli Giriş Katmanı) protokolü bütün yaygın web server'ları (sunucuları) ve browser'ları (tarayıcıları) tarafından desteklenen bir protokoldür. Milyonlarca web sitesinde güvenli veri iletişimi için kullanılmaktadır. Genellikle alışveriş sitelerinde oldukça sık rastlanmaktadır.

---

## 📋 İçindekiler

- [🔍 SSL Nasıl Çalışır?](#-ssl-nasıl-çalışır)
- [🏗️ SSL/TLS Versiyonları](#️-ssltls-versiyonları)
- [📜 SSL Sertifika Türleri](#-ssl-sertifika-türleri)
- [🔐 SSL Sertifika Doğrulama Seviyeleri](#-ssl-sertifika-doğrulama-seviyeleri)
- [🌐 SSL Sertifika Sağlayıcıları](#-ssl-sertifika-sağlayıcıları)
- [✅ SSL Kurulumu](#-ssl-kurulumu)
- [🛡️ SSL Güvenliği](#️-ssl-güvenliği)
- [📊 SSL ve SEO](#-ssl-ve-seo)

---

## 🔍 SSL Nasıl Çalışır?

### 🌐 Temel Çalışma Prensibi

1. **Tarayıcı** web sitesine HTTPS ile bağlanır
2. **Sunucu** SSL sertifikasını gönderir
3. **Tarayıcı** sertifikayı doğrular
4. **Şifreli Bağlantı** kurulur
5. **Güvenli Veri Transferi** başlar

### 🔄 SSL Handshake (El Sıkışma) Süreci

```
İstemci (Client)                    Sunucu (Server)
     ↓                                    ↓
  HTTPS İsteği ────────────────────────→
     ←──────────────────────────────── SSL Sertifikası
  Sertifika Doğrulama
  Şifreleme Anahtarı ──────────────────→
     ←──────────────────────────────── Şifreli Bağlantı
  Güvenli Veri Transferi ←────────────→
```

### 🔍 Güvenli Site Göstergeleri

**Güvenli bir sitede olduğumuzu anlamak için iki şeye dikkat etmemiz gerekmektedir:**

1. **Browser'ımızın (tarayıcımızın) altında çıkacak olan bir anahtar ya da kilit simgesi**
2. **Browser'ımızın (tarayıcımızın) adres çubuğunda bulunan sayfa adresinin başındaki `http://`'nin, `https://`'ye dönen halidir**

Bunlar, güvenli bir alanda olduğumuzun göstergesidir.

### 🔐 Şifreleme Türleri

| Şifreleme Türü | Açıklama | Güvenlik |
|:---------------|:---------|:---------|
| **Simetrik Şifreleme** | Aynı anahtar | ⭐⭐⭐⭐ |
| **Asimetrik Şifreleme** | Farklı anahtarlar | ⭐⭐⭐⭐⭐ |
| **Hash Fonksiyonları** | Veri bütünlüğü | ⭐⭐⭐⭐⭐ |

### 🔑 SSL Anahtar Sistemi

**SSL (Secure Socket Layer - Güvenli Giriş Katmanı) kodlama için iki adet anahtar bulunmaktadır.** Bu anahtarlar, dijital ortamda kodlanmış yazılımlardır. Bir anahtarın kilitlemiş olduğu veriyi, sadece diğer anahtar açabilir. 

Anahtarlar oluşturulduktan sonra:
- **Private key (özel anahtar)** (birinci anahtar) server'da (sunucuda) kalır
- **Public key (açık anahtar)** (ikinci anahtar) ise, bağlantı kurmak isteyen client'e (istemciye) gönderilir

SSL (Secure Socket Layer - Güvenli Giriş Katmanı), tüm bu işlemleri otomatik olarak yapar. Dışarıdan server'la (sunucuyla) iletişime geçmek isteyen client (istemci), public key'i (açık anahtarı) kullanarak veriyi güvenli bir şekilde server'a (sunucuya) gönderir. Veri, server'a (sunucuya) ulaşmadan, transfer sırasında veriye ulaşılsa bile, şifrenin çözülmesi için server'da (sunucuda) bulunan private key (özel anahtar) gerekecektir.

### 🔒 SSL Şifreleme Seviyeleri

**SSL (Secure Socket Layer - Güvenli Giriş Katmanı) türüne göre 128 bit veya 256 bit şifreleme kullanılmaktadır.** 

Kısaca SSL (Secure Socket Layer - Güvenli Giriş Katmanı) veri alışverişi yapan bilgisayarların, herhangi bir kişinin veriye müdahale etmesini önleyerek, sadece veri alışverişi yapan bilgisayar arasında, güvenli bir şekilde verinin aktarılmasını sağlar. 

**128 bit şifrelemede 2^128 değişik anahtar vardır ve bu şifrenin çözülebilmesi çok büyük bir maliyet ve zaman gerektirir.** Kötü niyetli kişi veya kişilerin, 128 bit'lik şifreyi çözebilmesi için 1-2 milyon dolarlık çok büyük bir yatırım yaptıktan sonra 67 yıl gibi bir zaman harcaması gerekir. Kısaca anlaşıldığı gibi SSL (Secure Socket Layer - Güvenli Giriş Katmanı) güvenlik sistemi tam ve kesin bir koruma sağlar.

---

## 🏗️ SSL/TLS Versiyonları

### 📜 SSL/TLS Versiyon Geçmişi

| Versiyon | Yıl | Durum | Güvenlik |
|:--------|:---|:-----|:---------|
| **SSL 1.0** | 1994 | ❌ Kullanılmıyor | ⭐ |
| **SSL 2.0** | 1995 | ❌ Kullanılmıyor | ⭐ |
| **SSL 3.0** | 1996 | ❌ Kullanılmıyor | ⭐⭐ |
| **TLS 1.0** | 1999 | ⚠️ Eski | ⭐⭐⭐ |
| **TLS 1.1** | 2006 | ⚠️ Eski | ⭐⭐⭐ |
| **TLS 1.2** | 2008 | ✅ Yaygın | ⭐⭐⭐⭐ |
| **TLS 1.3** | 2018 | ✅ Modern | ⭐⭐⭐⭐⭐ |

### ✅ Önerilen Versiyonlar

- **TLS 1.2**: Minimum desteklenen versiyon
- **TLS 1.3**: En güvenli ve hızlı versiyon

---

## 📜 SSL Sertifika Türleri

### 🎯 Sertifika Kategorileri

| Sertifika Türü | Açıklama | Kullanım | Fiyat |
|:---------------|:---------|:---------|:------|
| **Domain Validated (DV)** | Domain doğrulamalı | Kişisel siteler | Ücretsiz/Düşük |
| **Organization Validated (OV)** | Organizasyon doğrulamalı | İşletmeler | Orta |
| **Extended Validation (EV)** | Genişletilmiş doğrulama | Kurumsal | Yüksek |
| **Wildcard SSL** | Alt domain'ler için | Çoklu subdomain | Orta-Yüksek |
| **Multi-Domain (SAN)** | Çoklu domain | Birden fazla domain | Yüksek |

### 📊 Sertifika Türleri Detayı

#### 🌐 Domain Validated (DV) SSL

**Özellikler:**
- ✅ Hızlı doğrulama (dakikalar)
- ✅ Ücretsiz seçenekler mevcut
- ✅ Temel şifreleme
- ❌ Organizasyon bilgisi yok

**Kullanım:**
- Kişisel bloglar
- Küçük web siteleri
- Test siteleri

#### 🏢 Organization Validated (OV) SSL

**Özellikler:**
- ✅ Organizasyon doğrulaması
- ✅ Güven artırır
- ⚠️ 1-3 gün doğrulama
- ⚠️ Orta fiyat

**Kullanım:**
- İşletme web siteleri
- E-ticaret siteleri
- Kurumsal siteler

#### 🏛️ Extended Validation (EV) SSL

**Özellikler:**
- ✅ En yüksek güven seviyesi
- ✅ Tarayıcıda yeşil çubuk
- ✅ Detaylı doğrulama
- ❌ Yüksek fiyat
- ❌ 1-5 gün doğrulama

**Kullanım:**
- Büyük kurumsal siteler
- Bankalar
- Finansal kurumlar

#### 🌟 Wildcard SSL

**Özellikler:**
- ✅ Tüm subdomain'ler için
- ✅ `*.example.com` formatı
- ✅ Esnek kullanım
- ⚠️ Orta-yüksek fiyat

**Kullanım:**
- Çoklu subdomain'ler
- SaaS uygulamaları
- Büyük web siteleri

---

## 🔐 SSL Sertifika Doğrulama Seviyeleri

### 📊 Doğrulama Seviyesi Karşılaştırması

| Özellik | DV | OV | EV |
|:--------|:---|:---|:---|
| **Doğrulama Süresi** | Dakikalar | 1-3 gün | 1-5 gün |
| **Domain Doğrulama** | ✅ | ✅ | ✅ |
| **Organizasyon Doğrulama** | ❌ | ✅ | ✅ |
| **Yasal Doğrulama** | ❌ | ❌ | ✅ |
| **Tarayıcı Göstergesi** | Kilit ikonu | Kilit ikonu | Yeşil çubuk |
| **Güven Seviyesi** | ⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ |
| **Fiyat** | Düşük/Ücretsiz | Orta | Yüksek |

---

## 🌐 SSL Sertifika Sağlayıcıları

### 🏢 Ücretli SSL Sağlayıcıları

| Sağlayıcı | Özellikler | Fiyat (Yıllık) | Popülerlik |
|:---------|:----------|:--------------|:----------|
| **DigiCert** | Güvenilir, EV desteği | $200-1000+ | ⭐⭐⭐⭐⭐ |
| **GlobalSign** | Kurumsal odaklı | $150-800+ | ⭐⭐⭐⭐ |
| **Comodo (Sectigo)** | Uygun fiyatlı | $50-500+ | ⭐⭐⭐⭐ |
| **GeoTrust** | Orta segment | $100-600+ | ⭐⭐⭐ |
| **RapidSSL** | Hızlı doğrulama | $50-300+ | ⭐⭐⭐ |
| **Thawte** | Güvenilir | $150-700+ | ⭐⭐⭐ |

### 🆓 Ücretsiz SSL Sağlayıcıları

| Sağlayıcı | Özellikler | Sınırlamalar | Popülerlik |
|:---------|:----------|:------------|:----------|
| **Let's Encrypt** | Tamamen ücretsiz, otomatik | 90 gün, yenileme gerekli | ⭐⭐⭐⭐⭐ |
| **Cloudflare SSL** | Ücretsiz SSL | Cloudflare kullanımı gerekli | ⭐⭐⭐⭐⭐ |
| **ZeroSSL** | Ücretsiz DV SSL | 90 gün, sınırlı | ⭐⭐⭐ |
| **SSL For Free** | Ücretsiz | Manuel yenileme | ⭐⭐ |

### 🇹🇷 Türkiye'deki SSL Sağlayıcıları

| Sağlayıcı | Özellikler | Fiyat (₺) |
|:---------|:----------|:----------|
| **Turhost** | Let's Encrypt ücretsiz | Ücretsiz |
| **Natro** | Let's Encrypt ücretsiz | Ücretsiz |
| **GetYours** | Let's Encrypt ücretsiz | Ücretsiz |
| **Hosting.com.tr** | Let's Encrypt ücretsiz | Ücretsiz |

---

## ✅ SSL Kurulumu

### 🔧 Kurulum Yöntemleri

#### 1️⃣ cPanel ile SSL Kurulumu

1. **cPanel** → **SSL/TLS** bölümüne gidin
2. **SSL Sertifikaları** seçeneğini tıklayın
3. Sertifika bilgilerini girin
4. **Otomatik HTTPS Yönlendirme** aktif edin

#### 2️⃣ Let's Encrypt ile Otomatik Kurulum

```bash
# Certbot kurulumu (Ubuntu/Debian)
sudo apt-get update
sudo apt-get install certbot python3-certbot-apache

# Apache için SSL kurulumu
sudo certbot --apache -d example.com -d www.example.com

# Nginx için SSL kurulumu
sudo certbot --nginx -d example.com -d www.example.com
```

#### 3️⃣ Manuel Kurulum

1. Sertifika dosyalarını indirin
2. Sunucuya yükleyin
3. Web server yapılandırmasını düzenleyin
4. HTTPS yönlendirmesini aktif edin

### 📝 Web Server Yapılandırması

#### 🌐 Apache (.htaccess)

```apache
# HTTP'den HTTPS'e yönlendirme
RewriteEngine On
RewriteCond %{HTTPS} off
RewriteRule ^(.*)$ https://%{HTTP_HOST}%{REQUEST_URI} [L,R=301]
```

#### 🌐 Nginx

```nginx
server {
    listen 80;
    server_name example.com;
    return 301 https://$server_name$request_uri;
}

server {
    listen 443 ssl;
    server_name example.com;
    
    ssl_certificate /path/to/certificate.crt;
    ssl_certificate_key /path/to/private.key;
}
```

---

## 🛡️ SSL Güvenliği

### 🔒 Güvenlik Önlemleri

#### ✅ Yapılması Gerekenler

- ✅ **Güncel TLS Versiyonu**: TLS 1.2 veya 1.3 kullanın
- ✅ **Güçlü Şifreleme**: Modern şifreleme algoritmaları
- ✅ **Sertifika Yenileme**: Süresi dolmadan yenileyin
- ✅ **Mixed Content Kontrolü**: HTTP içerik kullanmayın
- ✅ **HSTS**: HTTP Strict Transport Security aktif edin
- ✅ **Sertifika İzleme**: Sertifika durumunu izleyin

#### ❌ Yapılmaması Gerekenler

- ❌ Eski SSL/TLS versiyonları kullanmak
- ❌ Zayıf şifreleme algoritmaları
- ❌ Süresi dolmuş sertifikalar
- ❌ Mixed content (HTTP + HTTPS)
- ❌ Güvenlik güncellemelerini ertelemek

### 🔐 Güvenlik Kontrol Listesi

| Kontrol | Durum | Açıklama |
|:--------|:------|:---------|
| **TLS 1.2+ Aktif** | ✅ | Modern TLS versiyonu |
| **Güçlü Şifreleme** | ✅ | AES-256, RSA-2048+ |
| **Sertifika Geçerli** | ✅ | Süresi dolmamış |
| **HSTS Aktif** | ✅ | Güvenli bağlantı zorunlu |
| **Mixed Content Yok** | ✅ | Tüm içerik HTTPS |
| **Sertifika Zinciri Tam** | ✅ | Tüm sertifikalar yüklü |

---

## 📊 SSL ve SEO

### 🎯 SSL'in SEO'ya Etkisi

#### ✅ SEO Avantajları

- ✅ **Google Ranking Faktörü**: HTTPS bir sıralama faktörü
- ✅ **Güven Göstergesi**: Kullanıcı güveni artar
- ✅ **Referrer Bilgisi**: HTTPS'den HTTP'ye referrer kaybolur
- ✅ **Hız İyileştirmesi**: HTTP/2 desteği
- ✅ **AMP Uyumluluğu**: AMP sayfaları için gerekli

### 📈 SSL SEO İstatistikleri

| Metrik | HTTP | HTTPS | Fark |
|:-------|:-----|:------|:-----|
| **Google Sıralaması** | Düşük | Yüksek | +%5-10 |
| **Güven Skoru** | ⭐⭐ | ⭐⭐⭐⭐⭐ | +150% |
| **Dönüşüm Oranı** | %2.5 | %3.2 | +28% |
| **Sayfa Hızı (HTTP/2)** | Yavaş | Hızlı | +30% |

---

## 🔍 SSL Sertifika Kontrolü

### 🛠️ SSL Test Araçları

| Araç | Açıklama | URL |
|:-----|:---------|:----|
| **SSL Labs** | Detaylı SSL testi | sslabs.com/ssltest |
| **SSL Checker** | Sertifika kontrolü | sslchecker.com |
| **Why No Padlock** | Mixed content kontrolü | whynopadlock.com |
| **SSL Test** | Hızlı SSL testi | ssltest.com |

### 📋 SSL Kontrol Listesi

- [ ] Sertifika geçerli mi?
- [ ] TLS versiyonu güncel mi?
- [ ] Şifreleme güçlü mü?
- [ ] Sertifika zinciri tam mı?
- [ ] Mixed content var mı?
- [ ] HSTS aktif mi?
- [ ] Tüm sayfalar HTTPS mi?

---

## 💡 SSL İpuçları

### ✅ Başarılı SSL Kullanımı İçin

1. **Let's Encrypt Kullanın**: Ücretsiz ve otomatik
2. **Otomatik Yenileme**: Certbot ile otomatik yenileme
3. **HTTP Yönlendirme**: Tüm HTTP trafiğini HTTPS'e yönlendirin
4. **Mixed Content**: HTTP içerik kullanmayın
5. **HSTS Aktif Edin**: Güvenli bağlantıyı zorunlu kılın
6. **Sertifika İzleme**: Süresi dolmadan yenileyin

### 🔧 SSL Sorun Giderme

| Sorun | Olası Neden | Çözüm |
|:------|:-----------|:------|
| **Sertifika Hatası** | Geçersiz sertifika | Sertifikayı yenileyin |
| **Mixed Content** | HTTP içerik | Tüm içeriği HTTPS yapın |
| **Yönlendirme Döngüsü** | Yanlış yapılandırma | .htaccess'i kontrol edin |
| **Yavaş Yükleme** | Eski TLS | TLS 1.3'e geçin |

---

## 📌 Dokümantasyon Bilgileri

| Bilgi | Detay |
|:------|:------|
| 👤 **Yazar** | Bahadır B. Bekdemir |
| 📅 **Tarih** | 15.01.2026 |
| 🔢 **Versiyon** | 1.0 |

---

> 💡 **İpucu:** SSL/TLS artık web siteleri için zorunlu hale gelmiştir. Let's Encrypt gibi ücretsiz SSL sağlayıcılarını kullanarak sitenizi güvenli hale getirebilirsiniz. Ayrıca otomatik yenileme ile sertifika yönetimini kolaylaştırabilirsiniz. SSL, hem güvenlik hem de SEO açısından kritik öneme sahiptir!

