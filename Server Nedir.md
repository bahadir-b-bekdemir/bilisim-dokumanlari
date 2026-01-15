# 🖥️ SERVER NEDİR?

**Server** (Sunucu), bilgisayar ağlarında, diğer ağ kullanıcıların yetkileri dahilinde erişebileceği, kullanımına veya paylaşımına açık kaynakları barındıran bilgisayarlara verilen isimdir. Bir ağda birden fazla server (sunucu) bulunabilir. Ağ topluluğuna veri dağıtım ve yönetim merkezliği yapar. 

Server'lar, ağ üzerinde diğer bilgisayarlara veya cihazlara hizmet sağlayan, sürekli çalışan ve yüksek performanslı bir bilgisayar sistemidir. Server'lar, web siteleri, e-posta, dosya paylaşımı, veritabanı ve diğer ağ servislerini sağlamak için kullanılır.

---

## 📋 İçindekiler

- [🔍 Server Nasıl Çalışır?](#-server-nasıl-çalışır)
- [🏗️ Server Türleri](#️-server-türleri)
- [💻 Server Donanımı](#-server-donanımı)
- [🌐 Server Yazılımları](#-server-yazılımları)
- [☁️ Server Modelleri](#-server-modelleri)
- [🔧 Server Yönetimi](#-server-yönetimi)
- [🛡️ Server Güvenliği](#️-server-güvenliği)

---

## 🔍 Server Nasıl Çalışır?

### 🌐 Temel Çalışma Prensibi

1. **İstemci (Client)** bir istek gönderir (örn: web sayfası isteği)
2. **Server** isteği alır ve işler
3. **Server** gerekli veriyi hazırlar (web sayfası, dosya, vb.)
4. **Server** yanıtı istemciye gönderir
5. **İstemci** yanıtı alır ve görüntüler

### 🔄 İstemci-Sunucu Modeli

```
İstemci (Client) ←→ Ağ (Network) ←→ Sunucu (Server)
     ↓                                    ↓
  İstek Gönderir                    İsteği İşler
  Yanıtı Alır                       Yanıt Gönderir
```

---

## 🏗️ Server Türleri

### 🎯 Kullanım Amacına Göre

| Server Türü | Açıklama | Kullanım Alanı |
|:-----------|:--------|:--------------|
| **Web Server** | Web sitelerini barındırır | Apache, Nginx, IIS |
| **Database Server** | Veritabanı hizmeti sağlar | MySQL, PostgreSQL, MongoDB |
| **Mail Server** | E-posta gönderimi/alımı | Postfix, Exchange, Sendmail |
| **File Server** | Dosya paylaşımı | FTP, Samba, NFS |
| **DNS Server** | Domain adlarını IP'ye çevirir | BIND, PowerDNS |
| **Application Server** | Uygulama çalıştırır | Tomcat, JBoss, Node.js |
| **Game Server** | Oyun sunucusu | Minecraft, Counter-Strike |
| **Proxy Server** | Aracı sunucu | Squid, Nginx |
| **VPN Server** | Sanal özel ağ | OpenVPN, WireGuard |
| **Media Server** | Medya akışı | Plex, Jellyfin |

### 📝 Önemli Notlar

**Server Kullanım Amacı:**
- Ayrıca server'ların (sunucuların) hangi amaçla kullanılacağı da önemlidir. Örneğin; Bir server (sunucu), **web server** (web sunucusu), **database server** (veritabanı sunucusu), **mail server** (posta sunucusu), **FTP server** (File Transfer Protocol - Dosya Transfer Protokolü sunucusu) vs. amaçlar için kullanılacak olabilir. 

**Server Kurulumu:**
- Server'ın (sunucunun) kullanım amacına göre işletim sisteminin (Windows Server, Linux vs.) ve gerekli yazılımlarının (IIS, Apache vs.) (MySQL, Oracle, MSSQL vs.) yüklenmesi gerekir. 
- Her bilgisayar gerekli olan yazılımlar yüklenmesi halinde sunucu olarak kullanılabilir. 

**Server Erişimi:**
- Server'larda (sunucularda) ana erişimin sağlanabilmesi için muhakkak bir **IP (Internet Protocol - İnternet Protokolü) adresi** ve **domain'i (alan adı)** olması gerekir.

### 💻 İşletim Sistemine Göre

| İşletim Sistemi | Açıklama | Popülerlik |
|:---------------|:---------|:----------|
| **Linux** | Açık kaynak, ücretsiz | ⭐⭐⭐⭐⭐ |
| **Windows Server** | Microsoft'un sunucu OS'u | ⭐⭐⭐⭐ |
| **Unix** | Ticari Unix sistemleri | ⭐⭐⭐ |
| **FreeBSD** | Açık kaynak BSD | ⭐⭐⭐ |

---

## 💻 Server Donanımı

### 🖥️ Temel Donanım Bileşenleri

| Bileşen | Açıklama | Önem |
|:--------|:---------|:-----|
| **CPU (İşlemci)** | İşlemleri yürütür | ⭐⭐⭐⭐⭐ |
| **RAM (Bellek)** | Geçici veri depolama | ⭐⭐⭐⭐⭐ |
| **HDD/SSD (Depolama)** | Kalıcı veri depolama | ⭐⭐⭐⭐⭐ |
| **Network Card** | Ağ bağlantısı | ⭐⭐⭐⭐⭐ |
| **Power Supply** | Güç kaynağı | ⭐⭐⭐⭐ |
| **RAID Controller** | Disk yönetimi | ⭐⭐⭐ |

### 📊 Server Özellikleri Karşılaştırması

| Server Tipi | CPU | RAM | Depolama | Kullanım |
|:-----------|:----|:----|:---------|:---------|
| **Küçük Web Server** | 2-4 çekirdek | 2-4 GB | 20-50 GB | Kişisel siteler |
| **Orta Web Server** | 4-8 çekirdek | 8-16 GB | 100-500 GB | Küçük işletmeler |
| **Büyük Web Server** | 8-16 çekirdek | 16-64 GB | 500 GB-2 TB | Büyük siteler |
| **Database Server** | 8-32 çekirdek | 32-256 GB | 1-10 TB | Veritabanı |
| **Dedicated Server** | 16+ çekirdek | 64+ GB | 2+ TB | Kurumsal |

---

## 🌐 Server Yazılımları

### 🎯 Web Server Yazılımları

| Yazılım | Açıklama | Popülerlik | Lisans |
|:--------|:---------|:----------|:-------|
| **Apache HTTP Server** | En popüler web server | ⭐⭐⭐⭐⭐ | Açık kaynak |
| **Nginx** | Yüksek performanslı | ⭐⭐⭐⭐⭐ | Açık kaynak |
| **IIS (Internet Information Services)** | Microsoft'un web server'ı | ⭐⭐⭐⭐ | Ticari |
| **LiteSpeed** | Ticari, hızlı | ⭐⭐⭐ | Ticari |
| **Caddy** | Otomatik HTTPS | ⭐⭐⭐ | Açık kaynak |

### 🗄️ Database Server Yazılımları

| Yazılım | Tür | Popülerlik | Lisans |
|:--------|:---|:----------|:-------|
| **MySQL** | İlişkisel | ⭐⭐⭐⭐⭐ | Açık kaynak |
| **PostgreSQL** | İlişkisel | ⭐⭐⭐⭐⭐ | Açık kaynak |
| **MongoDB** | NoSQL | ⭐⭐⭐⭐ | Açık kaynak |
| **MariaDB** | İlişkisel | ⭐⭐⭐⭐ | Açık kaynak |
| **Redis** | Key-Value | ⭐⭐⭐⭐ | Açık kaynak |
| **SQL Server** | İlişkisel | ⭐⭐⭐ | Ticari |

### 📧 Mail Server Yazılımları

| Yazılım | Açıklama | Popülerlik |
|:--------|:---------|:----------|
| **Postfix** | SMTP server | ⭐⭐⭐⭐⭐ |
| **Dovecot** | IMAP/POP3 server | ⭐⭐⭐⭐⭐ |
| **Microsoft Exchange** | Kurumsal e-posta | ⭐⭐⭐⭐ |
| **Sendmail** | Eski SMTP server | ⭐⭐⭐ |

---

## ☁️ Server Modelleri

### 🏢 Fiziksel vs Sanal vs Bulut

| Model | Açıklama | Avantajlar | Dezavantajlar |
|:------|:---------|:----------|:-------------|
| **Fiziksel Server** | Gerçek donanım | Tam kontrol, yüksek performans | Yüksek maliyet, bakım |
| **VPS (Virtual Private Server)** | Sanal sunucu | Esnek, uygun fiyat | Paylaşımlı kaynaklar |
| **Cloud Server** | Bulut sunucu | Ölçeklenebilir, esnek | İnternet bağımlılığı |
| **Dedicated Server** | Özel sunucu | Tam kontrol, güvenlik | Yüksek maliyet |
| **Shared Hosting** | Paylaşımlı hosting | Çok uygun fiyat | Sınırlı kontrol |

### 📊 Server Modeli Karşılaştırması

| Özellik | Fiziksel | VPS | Cloud | Shared |
|:--------|:--------|:----|:-----|:------|
| **Maliyet** | Yüksek | Orta | Değişken | Düşük |
| **Kontrol** | Tam | Yüksek | Yüksek | Düşük |
| **Performans** | Yüksek | Orta-Yüksek | Yüksek | Düşük |
| **Ölçeklenebilirlik** | Düşük | Orta | Yüksek | Düşük |
| **Bakım** | Sizin | Sağlayıcı | Sağlayıcı | Sağlayıcı |

---

## 🔧 Server Yönetimi

### 🛠️ Yönetim Araçları

#### 💻 Komut Satırı (CLI)

| Araç | Açıklama | Kullanım |
|:-----|:---------|:--------|
| **SSH** | Uzaktan bağlantı | `ssh user@server` |
| **Bash/Shell** | Komut satırı | Linux/Unix |
| **PowerShell** | Windows komut satırı | Windows Server |

#### 🖥️ Grafik Arayüz (GUI)

| Araç | Açıklama | Platform |
|:-----|:---------|:---------|
| **cPanel** | Web hosting kontrol paneli | Linux |
| **Plesk** | Hosting kontrol paneli | Linux/Windows |
| **Webmin** | Web tabanlı yönetim | Linux |
| **Remote Desktop** | Windows uzaktan masaüstü | Windows |

### 📋 Yaygın Server Görevleri

| Görev | Açıklama | Komut/İşlem |
|:------|:---------|:------------|
| **Yazılım Kurulumu** | Paket yönetimi | `apt install`, `yum install` |
| **Güvenlik Güncellemeleri** | Sistem güncellemeleri | `apt update && apt upgrade` |
| **Log İnceleme** | Log dosyalarını okuma | `tail -f /var/log/` |
| **Performans İzleme** | Kaynak kullanımı | `htop`, `top`, `df -h` |
| **Yedekleme** | Veri yedekleme | `rsync`, `tar`, `mysqldump` |
| **Firewall Yapılandırması** | Güvenlik duvarı | `ufw`, `iptables`, `firewalld` |

---

## 🛡️ Server Güvenliği

### 🔒 Temel Güvenlik Önlemleri

#### ✅ Yapılması Gerekenler

- ✅ **Güçlü Şifreler**: Karmaşık ve benzersiz şifreler kullanın
- ✅ **SSH Key Authentication**: Şifre yerine SSH anahtarları kullanın
- ✅ **Firewall**: Gereksiz portları kapatın
- ✅ **Güncellemeler**: Düzenli güvenlik güncellemeleri yapın
- ✅ **SSL/TLS**: Şifreli bağlantılar kullanın
- ✅ **Fail2Ban**: Brute force saldırılarına karşı koruma
- ✅ **Yedekleme**: Düzenli yedekleme yapın
- ✅ **Log İzleme**: Log dosyalarını düzenli kontrol edin

#### ❌ Yapılmaması Gerekenler

- ❌ Varsayılan şifreler kullanmak
- ❌ Root kullanıcı ile günlük işlemler
- ❌ Gereksiz servisleri çalıştırmak
- ❌ Güvenlik güncellemelerini ertelemek
- ❌ Güvenlik duvarını kapatmak

### 🔐 Güvenlik Araçları

| Araç | Açıklama | Kullanım |
|:-----|:---------|:---------|
| **Fail2Ban** | Otomatik IP engelleme | Brute force koruması |
| **UFW** | Basit firewall | Linux firewall yönetimi |
| **SELinux** | Güvenlik modülü | Linux güvenlik politikaları |
| **ClamAV** | Antivirus | Linux antivirus |
| **AIDE** | Dosya bütünlüğü | Dosya değişiklik tespiti |

---

## 📊 Server Performans Optimizasyonu

### ⚡ Performans İyileştirme Teknikleri

| Teknik | Açıklama | Etki |
|:-------|:---------|:-----|
| **Caching** | Önbellekleme | ⭐⭐⭐⭐⭐ |
| **CDN** | İçerik dağıtım ağı | ⭐⭐⭐⭐⭐ |
| **Load Balancing** | Yük dengeleme | ⭐⭐⭐⭐ |
| **Database Optimization** | Veritabanı optimizasyonu | ⭐⭐⭐⭐ |
| **Compression** | Sıkıştırma | ⭐⭐⭐ |
| **Minification** | Kod küçültme | ⭐⭐⭐ |

---

## 🌐 Popüler Server Sağlayıcıları

### ☁️ Bulut Server Sağlayıcıları

| Sağlayıcı | Özellikler | Popülerlik |
|:---------|:----------|:----------|
| **Amazon AWS** | En büyük bulut sağlayıcı | ⭐⭐⭐⭐⭐ |
| **Google Cloud** | Google'ın bulut servisi | ⭐⭐⭐⭐⭐ |
| **Microsoft Azure** | Microsoft'un bulut servisi | ⭐⭐⭐⭐⭐ |
| **DigitalOcean** | Geliştiriciler için | ⭐⭐⭐⭐ |
| **Linode** | Basit ve güvenilir | ⭐⭐⭐⭐ |
| **Vultr** | Yüksek performans | ⭐⭐⭐⭐ |

### 🏢 Türkiye'deki Server Sağlayıcıları

| Sağlayıcı | Özellikler | Notlar |
|:---------|:----------|:-------|
| **Turhost** | VPS, Dedicated | Türk şirketi |
| **Natro** | VPS, Cloud | Türk şirketi |
| **GetYours** | VPS, Dedicated | Türk şirketi |
| **Hosting.com.tr** | VPS, Cloud | Türk şirketi |

---

## 📌 Dokümantasyon Bilgileri

| Bilgi | Detay |
|:------|:------|
| 👤 **Yazar** | Bahadır B. Bekdemir |
| 📅 **Tarih** | 15.01.2026 |
| 🔢 **Versiyon** | 1.0 |

---

> 💡 **İpucu:** Server yönetimi için düzenli yedekleme, güvenlik güncellemeleri ve performans izleme çok önemlidir. Ayrıca gereksiz servisleri kapatarak güvenliği artırabilirsiniz.

