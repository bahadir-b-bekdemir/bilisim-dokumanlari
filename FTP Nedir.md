# 📤 FTP NEDİR?

**FTP** (File Transfer Protocol - Dosya Transfer Protokolü), internet üzerinde veya yerel bir ağda yer alan bir bilgisayara kullanıcıların yetkileri dahilinde erişebileceği dosya transfer etmeye yarayan ağ protokolüdür. Bir bilgisayardan bir başka bilgisayara bağlantı kurma ve dosya paylaşım işlevi görür. 

**Bu protokol TCP (Transmission Control Protocol - İletim Kontrol Protokolü) üzerinden çalışır.** Bir FTP (File Transfer Protocol - Dosya Transfer Protokolü) istemcisi, kullanıcının yetkisi dahilinde erişebileceği FTP (File Transfer Protocol - Dosya Transfer Protokolü) server'ına (sunucusuna) bağlanarak dosya transfer edebilir, silebilir veya değiştirebilir. 

**Her web sitenin bir FTP (File Transfer Protocol - Dosya Transfer Protokolü) adresi vardır.** Günümüzde her işletim sistemi üzerinde çalışan FTP (File Transfer Protocol - Dosya Transfer Protokolü) istemcisi yazılımlar bulunmaktadır. **CuteFTP ve FileZilla en çok tercih edilen FTP (File Transfer Protocol - Dosya Transfer Protokolü) yazılımlarıdır.**

---

## 📋 İçindekiler

- [🔍 FTP Nasıl Çalışır?](#-ftp-nasıl-çalışır)
- [🏗️ FTP Türleri](#️-ftp-türleri)
- [💻 FTP İstemcileri](#-ftp-istemcileri)
- [🔧 FTP Komutları](#-ftp-komutları)
- [🔐 FTP Güvenliği](#-ftp-güvenliği)
- [🌐 FTP vs Diğer Protokoller](#-ftp-vs-diğer-protokoller)
- [✅ FTP Kullanım İpuçları](#-ftp-kullanım-ipuçları)

---

## 🔍 FTP Nasıl Çalışır?

### 🌐 Temel Çalışma Prensibi

1. **FTP İstemcisi** (Client) FTP sunucusuna bağlanır
2. **Kimlik Doğrulama** yapılır (kullanıcı adı ve şifre)
3. **Bağlantı Kurulur** ve dosya transferi başlar
4. **Dosyalar Transfer Edilir** (yükleme/indirme)
5. **Bağlantı Kapatılır**

### 🔄 FTP Bağlantı Süreci

```
FTP İstemcisi ←→ Ağ (Network) ←→ FTP Sunucusu
     (Client)                        (Server)
     ↓                                    ↓
  Bağlantı İsteği                  Kimlik Doğrulama
  Dosya Transferi                  Dosya Transferi
  Bağlantı Kapatma                 Bağlantı Kapatma
```

### 🔌 FTP Portları

| Port | Açıklama | Kullanım |
|:----:|:---------|:---------|
| **21** | Kontrol Portu | Komutlar için |
| **20** | Veri Portu (Aktif Mod) | Veri transferi |
| **Dinamik** | Veri Portu (Pasif Mod) | Veri transferi |

### 📝 Önemli Notlar

**FTP Yazılım Türleri:**
- FTP yazılımları **client (istemci)** ve **server (sunucu)** taraflı olmak üzere ikiye ayrılır. 
- Server (sunucu) tarafındaki yazılım FTP (File Transfer Protocol - Dosya Transfer Protokolü) portunu dinleyerek erişim izni olan client'lerden (istemcilerden) transferi kabul eder. 

**Browser (Tarayıcı) ile FTP Erişimi:**
- Günümüzde hemen hemen tüm browser'lar (tarayıcılar) FTP (File Transfer Protocol - Dosya Transfer Protokolü) server'ına (sunucusuna) client (istemci) olarak bağlanabilmektedirler. 
- Browser'ın (tarayıcının) adres çubuğuna `ftp://` ile başlayan bir FTP (File Transfer Protocol - Dosya Transfer Protokolü) adresi girdiğinizde bu adresteki server'a (sunucuya) erişim hakkınız varsa bağlanabilirsiniz. 

**FTP Port:**
- **FTP (File Transfer Protocol - Dosya Transfer Protokolü) dosya transferi için varsayılan port 21'dir.**

---

## 🏗️ FTP Türleri

### 🎯 FTP Çeşitleri

| FTP Türü | Açıklama | Güvenlik | Kullanım |
|:---------|:---------|:---------|:---------|
| **FTP** | Standart FTP | ❌ Şifrelenmemiş | Eski sistemler |
| **FTPS** | FTP over SSL/TLS | ✅ Şifreli | Güvenli transfer |
| **SFTP** | SSH File Transfer Protocol | ✅ Şifreli | En güvenli |
| **FTPES** | FTP Explicit SSL/TLS | ✅ Şifreli | FTPS alternatifi |

### 📊 FTP Türleri Karşılaştırması

| Özellik | FTP | FTPS | SFTP | FTPES |
|:--------|:---|:-----|:-----|:------|
| **Güvenlik** | ❌ Yok | ✅ SSL/TLS | ✅ SSH | ✅ SSL/TLS |
| **Port** | 21 | 21, 990 | 22 | 21 |
| **Şifreleme** | ❌ | ✅ | ✅ | ✅ |
| **Hız** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐⭐ |
| **Uyumluluk** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐ |

### 🔐 Güvenli FTP Türleri Detayı

#### 🔒 FTPS (FTP over SSL/TLS)

**Özellikler:**
- ✅ SSL/TLS şifreleme
- ✅ İki mod: Implicit (990) ve Explicit (21)
- ✅ Güvenli veri transferi
- ⚠️ Firewall sorunları olabilir

**Kullanım:**
- Web hosting yönetimi
- Güvenli dosya transferi
- Kurumsal dosya paylaşımı

#### 🔒 SFTP (SSH File Transfer Protocol)

**Özellikler:**
- ✅ SSH üzerinden çalışır
- ✅ Tek port (22)
- ✅ En güvenli yöntem
- ✅ Firewall dostu

**Kullanım:**
- Linux sunucular
- Güvenli dosya yönetimi
- Otomatik yedekleme

---

## 💻 FTP İstemcileri

### 🖥️ Masaüstü FTP İstemcileri

| İstemci | Platform | Özellikler | Fiyat | Popülerlik |
|:--------|:--------|:----------|:------|:----------|
| **FileZilla** | Windows, macOS, Linux | Ücretsiz, güçlü | Ücretsiz | ⭐⭐⭐⭐⭐ |
| **WinSCP** | Windows | SFTP odaklı | Ücretsiz | ⭐⭐⭐⭐⭐ |
| **Cyberduck** | Windows, macOS | Basit arayüz | Ücretsiz | ⭐⭐⭐⭐ |
| **CuteFTP** | Windows, macOS | Profesyonel | Ücretli | ⭐⭐⭐ |
| **Transmit** | macOS | Hızlı ve güvenilir | Ücretli | ⭐⭐⭐⭐ |
| **ForkLift** | macOS | Dosya yöneticisi | Ücretli | ⭐⭐⭐ |
| **FireFTP** | Firefox Eklentisi | Tarayıcı içi | Ücretsiz | ⭐⭐⭐ |

### 🌐 Web Tabanlı FTP İstemcileri

| İstemci | Açıklama | Özellikler |
|:--------|:---------|:----------|
| **cPanel File Manager** | Hosting kontrol paneli | Tarayıcı içi dosya yönetimi |
| **Plesk File Manager** | Hosting kontrol paneli | Web tabanlı FTP |
| **Monsta FTP** | Web FTP istemcisi | Tarayıcı tabanlı |

### 📱 Mobil FTP İstemcileri

| İstemci | Platform | Özellikler |
|:--------|:---------|:----------|
| **FTP Manager** | iOS, Android | Mobil FTP erişimi |
| **AndFTP** | Android | Güçlü özellikler |
| **FTP Client** | iOS | Basit ve etkili |

---

## 🔧 FTP Komutları

### 💻 Temel FTP Komutları

| Komut | Açıklama | Örnek |
|:------|:---------|:------|
| `open` | FTP sunucusuna bağlan | `open ftp.example.com` |
| `user` | Kullanıcı adı girişi | `user myusername` |
| `pass` | Şifre girişi | `pass mypassword` |
| `ls` / `dir` | Dosya listesi | `ls` |
| `cd` | Dizin değiştir | `cd public_html` |
| `pwd` | Mevcut dizin | `pwd` |
| `mkdir` | Dizin oluştur | `mkdir newfolder` |
| `rmdir` | Dizin sil | `rmdir oldfolder` |
| `get` | Dosya indir | `get file.txt` |
| `put` | Dosya yükle | `put file.txt` |
| `delete` | Dosya sil | `delete file.txt` |
| `rename` | Dosya yeniden adlandır | `rename old.txt new.txt` |
| `binary` | İkili mod | `binary` |
| `ascii` | Metin modu | `ascii` |
| `passive` | Pasif mod | `passive` |
| `active` | Aktif mod | `active` |
| `quit` / `bye` | Bağlantıyı kapat | `quit` |

### 📝 FTP Komut Örnekleri

#### 🔌 Bağlantı Kurma

```bash
ftp ftp.example.com
# Kullanıcı adı ve şifre istenir
```

#### 📂 Dizin İşlemleri

```bash
pwd                    # Mevcut dizini göster
cd public_html         # Dizine geç
ls                     # Dosyaları listele
mkdir newfolder        # Yeni klasör oluştur
```

#### 📤 Dosya Transferi

```bash
binary                 # İkili mod (resim, video için)
put localfile.txt      # Dosya yükle
get remotefile.txt     # Dosya indir
```

---

## 🔐 FTP Güvenliği

### 🛡️ Güvenlik Önlemleri

#### ✅ Yapılması Gerekenler

- ✅ **SFTP veya FTPS Kullanın**: Şifrelenmemiş FTP kullanmayın
- ✅ **Güçlü Şifreler**: Karmaşık şifreler kullanın
- ✅ **SSH Key Authentication**: Şifre yerine anahtar kullanın
- ✅ **IP Kısıtlaması**: Belirli IP'lerden erişim
- ✅ **Firewall**: Gereksiz portları kapatın
- ✅ **Düzenli Güncelleme**: FTP yazılımlarını güncel tutun

#### ❌ Yapılmaması Gerekenler

- ❌ Şifrelenmemiş FTP kullanmak
- ❌ Zayıf şifreler kullanmak
- ❌ FTP şifrelerini paylaşmak
- ❌ Gereksiz FTP erişimleri vermek
- ❌ Güvenlik güncellemelerini ertelemek

### 🔒 Güvenlik Karşılaştırması

| Özellik | FTP | FTPS | SFTP |
|:--------|:---|:-----|:-----|
| **Şifreleme** | ❌ | ✅ | ✅ |
| **Kimlik Doğrulama** | Şifre | Şifre/SSL | Şifre/Key |
| **Veri Bütünlüğü** | ❌ | ✅ | ✅ |
| **Güvenlik Seviyesi** | ⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ |

---

## 🌐 FTP vs Diğer Protokoller

### 📊 Protokol Karşılaştırması

| Protokol | Açıklama | Kullanım | Güvenlik | Hız |
|:---------|:---------|:---------|:---------|:-----|
| **FTP** | Dosya transferi | Genel dosya transferi | ⭐ | ⭐⭐⭐⭐⭐ |
| **SFTP** | SSH üzerinden FTP | Güvenli dosya transferi | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ |
| **FTPS** | SSL/TLS üzerinden FTP | Güvenli dosya transferi | ⭐⭐⭐⭐ | ⭐⭐⭐⭐ |
| **HTTP** | Web protokolü | Web sayfaları | ⭐⭐ | ⭐⭐⭐⭐ |
| **HTTPS** | Güvenli HTTP | Güvenli web | ⭐⭐⭐⭐ | ⭐⭐⭐ |
| **SCP** | Secure Copy | Güvenli kopyalama | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ |
| **Rsync** | Senkronizasyon | Dosya senkronizasyonu | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ |

---

## ✅ FTP Kullanım İpuçları

### 💡 Etkili FTP Kullanımı

#### 🎯 Dosya Yükleme İpuçları

1. **Doğru Dizine Yükleyin**: `public_html` veya `www` klasörüne
2. **Dosya İzinlerini Kontrol Edin**: 644 (dosya), 755 (klasör)
3. **Büyük Dosyalar İçin**: Kesintisiz bağlantı kullanın
4. **Yedekleme**: Yüklemeden önce yedek alın
5. **Test Edin**: Yükleme sonrası siteyi test edin

#### 📁 Dosya Yönetimi İpuçları

- **Organize Edin**: Dosyaları klasörlere ayırın
- **İsimlendirme**: Açıklayıcı dosya isimleri kullanın
- **Temizlik**: Kullanılmayan dosyaları silin
- **Yedekleme**: Düzenli yedekleme yapın

### 🔧 FTP Ayarları

#### ⚙️ Önerilen Ayarlar

| Ayar | Değer | Açıklama |
|:-----|:------|:---------|
| **Transfer Modu** | Pasif (Passive) | Firewall uyumlu |
| **Timeout** | 60 saniye | Bağlantı zaman aşımı |
| **Retry** | 3 | Yeniden deneme |
| **Encoding** | UTF-8 | Türkçe karakter desteği |

---

## 🌐 FTP Sunucu Yazılımları

### 🖥️ Popüler FTP Sunucuları

| Yazılım | Platform | Özellikler | Lisans |
|:--------|:---------|:----------|:-------|
| **FileZilla Server** | Windows | Ücretsiz, kolay | Ücretsiz |
| **vsftpd** | Linux | Güvenli, hızlı | Açık kaynak |
| **ProFTPD** | Linux | Esnek yapılandırma | Açık kaynak |
| **Pure-FTPd** | Linux | Basit ve güvenli | Açık kaynak |
| **IIS FTP** | Windows Server | Microsoft'un FTP'si | Ticari |
| **Serv-U** | Windows | Profesyonel | Ticari |

---

## 📊 FTP Kullanım Senaryoları

### 🎯 Yaygın Kullanım Alanları

| Senaryo | Açıklama | Önerilen Yöntem |
|:--------|:---------|:----------------|
| **Web Sitesi Yükleme** | Web sitesi dosyalarını yükleme | SFTP/FTPS |
| **Yedekleme** | Sunucu yedekleme | SFTP/SCP |
| **Dosya Paylaşımı** | Dosya paylaşımı | FTPS |
| **Otomatik Yedekleme** | Zamanlanmış yedekleme | SFTP/SCP |
| **İçerik Yönetimi** | CMS dosya yönetimi | SFTP |

---

## 🔧 FTP Bağlantı Sorunları ve Çözümleri

### ⚠️ Yaygın Sorunlar

| Sorun | Olası Neden | Çözüm |
|:------|:-----------|:------|
| **Bağlantı Hatası** | Yanlış sunucu/port | Sunucu ve portu kontrol edin |
| **Kimlik Doğrulama Hatası** | Yanlış şifre | Şifreyi kontrol edin |
| **Pasif Mod Hatası** | Firewall | Aktif mod deneyin |
| **Yavaş Transfer** | Ağ sorunu | Bağlantıyı kontrol edin |
| **Dosya İzni Hatası** | CHMOD ayarları | Dosya izinlerini düzenleyin |

---

## 📌 Dokümantasyon Bilgileri

| Bilgi | Detay |
|:------|:------|
| 👤 **Yazar** | Bahadır B. Bekdemir |
| 📅 **Tarih** | 15.01.2026 |
| 🔢 **Versiyon** | 1.0 |

---

> 💡 **İpucu:** Güvenlik için mutlaka SFTP veya FTPS kullanın. Şifrelenmemiş FTP kullanmak, şifrelerinizin ve verilerinizin ele geçirilmesine neden olabilir. Ayrıca büyük dosyalar için kesintisiz bağlantı kullanmayı unutmayın!

