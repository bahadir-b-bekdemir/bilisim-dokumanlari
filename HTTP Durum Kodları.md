# 🌐 HTTP DURUM KODLARI

Sitenizdeki bir sayfayla ilgili olarak server'ınıza (sunucunuza) istekte bulunulduğunda, server'ınız (sunucunuz) isteğe yanıt olarak bir **HTTP** (Hyper Text Transfer Protocol - Hiper Metin Transferi Protokolü) durum kodu döndürür. Bu durum kodu isteğin durumuyla ilgili bilgiler sağlar.

Örneğin; Kullanıcı bir browser'dan (tarayıcıdan) sayfanıza eriştiğinde. Önemli olan kısmı ise **Google Bot** (Google robotu) ve benzeri diğer bot'lar (robotlar) web sitelerini ziyaret ettiğinde aldıkları bu durum kodlarını anlamlandırır ve arama sonuçlarından çıkartacakları sayfaları, değişen sayfa adreslerini bu şekilde anlayıp arama sonucuna yansıtır.

Durum kodlarının **5 kategorisi** vardır ve bu kategoriler **1, 2, 3, 4 ve 5** ile başlar. Sitelerinin sayfa sayıları gerek az gerekse de çok fazla olduğundan site sahiplerinin bu kodları kontrol etmeleri ve yanlışlık olmadığından emin olmaları gerekmektedir. **SEO** (Search Engine Optimization - Arama Motoru Optimizasyonu) açısından da son derece önemlidir.

---

## 📋 İçindekiler

- [ℹ️ 1xx - Bilgilendirme (Informational)](#️-1xx---bilgilendirme-informational)
- [✅ 2xx - Başarılı (Success)](#-2xx---başarılı-success)
- [🔄 3xx - Yönlendirme (Redirection)](#-3xx---yönlendirme-redirection)
- [❌ 4xx - İstemci Hatası (Client Error)](#-4xx---istemci-hatası-client-error)
- [⚠️ 5xx - Sunucu Hatası (Server Error)](#️-5xx---sunucu-hatası-server-error)
- [📝 .htaccess Örnekleri](#-htaccess-örnekleri)

---

## ℹ️ 1xx - Bilgilendirme (Informational)

Bu kodlar, isteğin alındığını ve işlemin devam ettiğini gösterir.

| Kod | İsim | Açıklama |
|:---:|:----|:---------|
| **100** | **Continue** | İstek alındı ve işlem devam ediyor. İstemci isteğin geri kalanını göndermeye devam edebilir. |
| **101** | **Switching Protocols** | Sunucu, istemcinin isteğine göre protokolü değiştiriyor. |
| **102** | **Processing** | İşlem devam ediyor. Uzun süren işlemler için kullanılır. |
| **103** | **Early Hints** | İlk ipuçları. Sunucu, yanıt hazırlanırken bazı ipuçları gönderebilir. |

---

## ✅ 2xx - Başarılı (Success)

Bu kodlar, isteğin başarıyla alındığını, anlaşıldığını ve işlendiğini gösterir.

| Kod | İsim | Açıklama |
|:---:|:----|:---------|
| **200** | **OK** | ✅ İstek başarıyla işlendi. Server (sunucu), isteği başarıyla işlemiştir ve genellikle bu, server'ın (sunucunun) istenen sayfayı sağladığı anlamına gelir. 200 kodu sitenin aktif / çalışır durumda olduğunu Google Bot'una (Google robotuna) ve benzeri diğer bot'lara (robotlara) bildirir, Google Bot (Google robotu) ve benzeri diğer bot'larda (robotlarda) bu şekilde sitenin aktif / çalışır durumda olduğunu anlayıp index'leme (indeksleme) işlemine devam eder. |
| **201** | **Created** | İstek başarılı ve yeni bir kaynak oluşturuldu. |
| **202** | **Accepted** | İstek kabul edildi ancak henüz işlenmedi. |
| **203** | **Non-Authoritative Information** | Döndürülen bilgi, kaynak sunucudan gelen bilgi değil, başka bir kaynaktan geliyor. |
| **204** | **No Content** | İstek başarılı ancak yanıt içeriği yok. |
| **205** | **Reset Content** | İstek başarılı, görünümü sıfırlamak için kullanılır. |
| **206** | **Partial Content** | Sunucu, kaynağın yalnızca bir kısmını döndürüyor. |
| **207** | **Multi-Status** | Çoklu durum yanıtı. Birden fazla kaynak için durum bilgisi. |
| **208** | **Already Reported** | DAV binding'lerinde kullanılır. Zaten bildirilmiş. |
| **226** | **IM Used** | Sunucu, isteği yerine getirmek için IM (Instance Manipulation) gerçekleştirdi. |

---

## 🔄 3xx - Yönlendirme (Redirection)

Bu kodlar, isteğin tamamlanması için ek işlem yapılması gerektiğini gösterir.

| Kod | İsim | Açıklama |
|:---:|:----|:---------|
| **300** | **Multiple Choices** | İstek için birden fazla seçenek var. İstemci birini seçmelidir. |
| **301** | **Moved Permanently** | 🔴 **EN ÖNEMLİ YÖNLENDİRME KODU!** İstenen sayfa **kalıcı olarak** yeni bir konuma taşındı anlamını ifade etmektedir. Server (sunucu) bir GET veya HEAD isteğine yanıt olarak bu yanıtı verdiğinde, istekte bulunanı otomatik olarak yeni konuma yönlendirir. Bir sayfanın veya sitenin kalıcı olarak yeni bir konuma taşındığını Google Bot'una (Google robotuna) ve benzeri diğer bot'lara (robotlara) bildirmek için bu kodu kullanmalısınız. Sitenizi bir kaç sene önce açtınız, daha sonra yapı değişikliğine veya domain (alan adı) değiştirme yoluna gittiniz. İşte bu durumda 301 kodu sitenizin hayatını kurtaran bir kod olarak karşınıza çıkar. Çünkü yıllardır emek verdiğiniz site veya sayfaların sayfa adresleri de bu değişiklik ile değişecektir. Google ve benzeri arama motorlarının index'leme (indeksleme) mekanizmasını sayfa adresleri üzerine kurduğundan yaptığınız değişikliği Google Bot'larına (Google robotlarına) ve benzeri diğer bot'lara (robotlara) 301 ile bildirmediğiniz sürece eski sayfa adresleriniz ve yeni sayfa adresleriniz olmak üzere Google'da ve benzeri diğer arama motorlarında index'li (indeksli) sayfalarınız oluşur. Bu durum kopya içerik sorununa neden olacak ve kısa zaman içerisinde Google'dan ve benzeri diğer arama motorlarından gelen trafiğiniz dörtte biri veya daha fazla oranda düşecek, eski sıralamalarınız gidecektir. Fakat 301 kodunu doğru kullanırsanız eski sıralamalarınızın yeni sayfa adreslerine geçmesini sağlayabilir, trafik kaybını engelleyebilirsiniz. Burada da en önemli nokta 301 yaparken eski sayfa adreslerinizi birebir yeni adreslerinize yönlendirmeniz gerektiğidir. Yani eskisiteadi.com/setler sayfasının yeni adı yenisiteadi.com/eğitim-setleri ise ilk sayfa adresini ikinci adrese 301 ile yönlendirmeniz gerekmektedir. Bütün site için bu yapıyı kurmanız gerekmektedir. 301 yönlendirmesi server (sunucu) üzerinde yapılması gerekir. |
| **302** | **Found** | ⚠️ **Geçici yönlendirme** çeşidi olarak bilinir. Eğer bir sayfa adresini arama motorunda göstermek isteyip kullanıcının eriştiği yerde başka adres kullanmak istiyorsanız bu yöntemi kullanabilirsiniz. Server (sunucu) şu anda isteğe farklı bir konumda bulunan bir sayfayla yanıt veriyor, ancak istekte bulunanın gelecek istekler için özgün konumu kullanmaya devam etmesi gerekiyor. Bu kod, bir GET veya HEAD isteği için istekte bulunanı otomatik olarak farklı bir konuma yönlendirmesi bakımından 301 koduna benzer. Ancak Google Bot (Google robotu) ve benzeri diğer bot'lar (robotlar) özgün konumu taramaya ve dizine eklemeye devam edeceğinden bir sayfanın veya sitenin taşındığını Google Bot'a (Google robotuna) ve benzeri diğer bot'lara (robotlara) bildirmek için bu kodu kullanmamalısınız. 302 yönlendirme şekli verimsiz bir yönlendirme şeklidir aslında, arama sonuçlarında hiçbir şeyi değiştirmez. Genelde yapılan hata 301 yerine 302 yapılmasıdır. 302 geçici yönlendirme olduğundan yönlendirilen URL (Uniform Resource Locator - Nizami Kaynak Bulucu) arama sonuçlarında çıkmaya devam eder. |
| **303** | **See Other** | Yanıt, başka bir konumda bulunuyor ve GET metodu kullanılarak alınmalı. |
| **304** | **Not Modified** | Kaynak değiştirilmemiş. Önbellekten kullanılabilir. |
| **305** | **Use Proxy** | İstenen kaynağa erişmek için bir proxy kullanılmalı. (Artık kullanılmıyor) |
| **306** | **Switch Proxy** | Artık kullanılmıyor. Eski proxy kodları için kullanılırdı. |
| **307** | **Temporary Redirect** | Geçici yönlendirme. İstek aynı metotla tekrar yapılmalı. |
| **308** | **Permanent Redirect** | Kalıcı yönlendirme. İstek aynı metotla tekrar yapılmalı. (301'den farkı, metot değişmez) |

---

## ❌ 4xx - İstemci Hatası (Client Error)

Bu kodlar, isteğin hatalı olduğunu veya sunucunun isteği yerine getiremediğini gösterir.

| Kod | İsim | Açıklama |
|:---:|:----|:---------|
| **400** | **Bad Request** | İstek hatalı. Sunucu, isteği anlayamadı veya işleyemedi. |
| **401** | **Unauthorized** | Yetkisiz erişim. Kimlik doğrulama gerekiyor. |
| **402** | **Payment Required** | Ödeme gerekli. (Şu anda kullanılmıyor, gelecekte kullanılabilir) |
| **403** | **Forbidden** | Yasak. Sunucu isteği anladı ancak yetkilendirme reddedildi. |
| **404** | **Not Found** | 🔴 **EN SIK GÖRÜLEN HATA!** Server (sunucu) istenen sayfayı bulamıyor. Örneğin; İstek, server'da (sunucuda) bulunmayan bir sayfa için yapılmışsa, server (sunucu) genellikle bu kodu döndürür. 404 kodu da Google Bot'larına (Google robotlarına) ve benzeri diğer bot'lara (robotlara) sayfanın artık var olmadığını bildirir. Böylece Google Bot'ları (Google robotları) ve benzeri diğer bot'lar (robotlar) ilgili sayfayı index'lerinden (indekslerinden) siler bir daha arama sonuçlarında getirmemeye çalışırlar. |
| **405** | **Method Not Allowed** | İstek metodu bu kaynak için izin verilmiyor. |
| **406** | **Not Acceptable** | İstenen kaynak, kabul edilebilir içerik özelliklerine sahip değil. |
| **407** | **Proxy Authentication Required** | Proxy kimlik doğrulaması gerekiyor. |
| **408** | **Request Timeout** | İstek zaman aşımına uğradı. Sunucu, isteği beklerken zaman aşımına uğradı. |
| **409** | **Conflict** | İstek, mevcut kaynak durumuyla çakışıyor. |
| **410** | **Gone** | Kaynak artık mevcut değil ve bir daha olmayacak. 404'ten farkı, kaynağın kalıcı olarak kaldırıldığını belirtir. |
| **411** | **Length Required** | İstek, Content-Length başlığı gerektiriyor. |
| **412** | **Precondition Failed** | Ön koşul başarısız. Sunucu, istekte belirtilen ön koşullardan birini karşılamıyor. |
| **413** | **Payload Too Large** | İstek varlığı çok büyük. Sunucu, işlemek için çok büyük. |
| **414** | **URI Too Long** | İstek URI'si çok uzun. Sunucu, işlemek için çok uzun. |
| **415** | **Unsupported Media Type** | Desteklenmeyen medya türü. İstek varlığı, desteklenmeyen bir format. |
| **416** | **Range Not Satisfiable** | İstenen aralık karşılanamıyor. |
| **417** | **Expectation Failed** | Beklenti başarısız. Sunucu, Expect başlık alanındaki gereksinimi karşılayamıyor. |
| **418** | **I'm a teapot** | "Ben bir çaydanlığım" - RFC 2324'ten esprili bir kod. (Gerçek kullanımda nadiren görülür) |
| **421** | **Misdirected Request** | Yanlış yönlendirilmiş istek. İstek, yanıt üretemeyen bir sunucuya gönderildi. |
| **422** | **Unprocessable Entity** | İşlenemeyen varlık. İstek doğru formatta ancak semantik hatalar var. |
| **423** | **Locked** | Kilitli. Kaynak kilitli. |
| **424** | **Failed Dependency** | Başarısız bağımlılık. Önceki istek başarısız olduğu için bu istek başarısız. |
| **425** | **Too Early** | Çok erken. Sunucu, tekrarlanan isteklere karşı korumalı bir isteği işlemek istemiyor. |
| **426** | **Upgrade Required** | Yükseltme gerekli. Sunucu, farklı bir protokol kullanılmasını gerektiriyor. |
| **428** | **Precondition Required** | Ön koşul gerekli. Sunucu, isteğin koşullu olmasını gerektiriyor. |
| **429** | **Too Many Requests** | Çok fazla istek. Kullanıcı belirli bir süre içinde çok fazla istek gönderdi. |
| **431** | **Request Header Fields Too Large** | İstek başlık alanları çok büyük. Sunucu, başlıkları işlemek istemiyor. |
| **451** | **Unavailable For Legal Reasons** | Yasal nedenlerle kullanılamıyor. Kaynak, yasal nedenlerle erişilemez. |

---

## ⚠️ 5xx - Sunucu Hatası (Server Error)

Bu kodlar, sunucunun geçerli bir isteği yerine getiremediğini gösterir.

| Kod | İsim | Açıklama |
|:---:|:----|:---------|
| **500** | **Internal Server Error** | 🔴 **SUNUCU HATASI!** Server (sunucu) hatayla karşılaştı ve isteği gerçekleştiremiyor. Ziyaret edilmeye çalışılan web sitesinde, web sayfasının görüntülenmesini engelleyen bir server (sunucu) sorunu var anlamına gelir. Web sitesi bakımından veya komut dosyası kullanan etkileşimli web sitelerindeki bir programlama hatasından kaynaklanır. |
| **501** | **Not Implemented** | Uygulanmadı. Sunucu, isteği yerine getirmek için gerekli işlevselliğe sahip değil. |
| **502** | **Bad Gateway** | 🔴 **AĞ GEÇİDİ HATASI!** Server (sunucu) hatayla karşılaştı ve bad gateway (geçersiz ağ geçidi) sorunu. Ziyaret edilmeye çalışılan web sitesinde, web sayfasının görüntülenmesini engelleyen bir server'da (sunucuda) bad gateway (geçersiz ağ geçidi) sorunu var anlamına gelir. Server (sunucu) bakımından veya gateway (ağ geçidi) ayarlamaları hatasından kaynaklanır. |
| **503** | **Service Unavailable** | 🔴 **HİZMET KULLANILAMAZ!** Server (sunucu) şu anda kullanılamıyor anlamına gelir. Bu çoğu zaman genellikle geçici bir durumdur. Genellikle server'ın (sunucunun) aşırı yüklü olduğu durumlarda server (sunucu) bu kodu döndürür. |
| **504** | **Gateway Timeout** | Ağ geçidi zaman aşımı. Sunucu, bir ağ geçidi veya proxy olarak çalışırken zaman aşımına uğradı. |
| **505** | **HTTP Version Not Supported** | HTTP sürümü desteklenmiyor. Sunucu, istekte kullanılan HTTP protokol sürümünü desteklemiyor. |
| **506** | **Variant Also Negotiates** | Varyant ayrıca müzakere ediyor. Sunucu, iç içe geçmiş seçim yapıyor. |
| **507** | **Insufficient Storage** | Yetersiz depolama. Sunucu, isteği tamamlamak için yeterli depolama alanına sahip değil. |
| **508** | **Loop Detected** | Döngü tespit edildi. Sunucu, isteği işlerken sonsuz döngü tespit etti. |
| **510** | **Not Extended** | Genişletilmedi. Sunucu, isteği yerine getirmek için daha fazla uzantı gerektiriyor. |
| **511** | **Network Authentication Required** | Ağ kimlik doğrulaması gerekli. İstemci, ağa erişmek için kimlik doğrulaması yapmalı. |

---

## 📝 .htaccess Örnekleri

### 🔄 301 Yönlendirme (Kalıcı Yönlendirme)

#### Tek Sayfa Yönlendirme

```apache
Redirect /eskiadres.html http://www.yenisiteadi.com/yeniadres.html [R=301,L]
```

#### Komple Site Yönlendirme

```apache
RewriteCond %{HTTP_HOST} ^([^.:]+\.)*eskisiteadi\.com\.?(:[0-9]*)?$ [NC]
RewriteRule ^/(.*)$ http://www.yenisiteadi.com/$1 [R=301,L]
```

#### www Olmadan www'ye Yönlendirme

```apache
RewriteCond %{HTTP_HOST} ^yenisiteadi\.com$ [NC]
RewriteRule ^(.*)$ http://www.yenisiteadi.com/$1 [R=301,L]
```

#### www'den www Olmadan Yönlendirme

```apache
RewriteCond %{HTTP_HOST} ^www\.yenisiteadi\.com$ [NC]
RewriteRule ^(.*)$ http://yenisiteadi.com/$1 [R=301,L]
```

### 🔄 302 Yönlendirme (Geçici Yönlendirme)

```apache
Redirect /eskiadres.html http://www.yenisiteadi.com/yeniadres.html [R=302,L]
```

### ❌ 404 Hata Sayfası Özelleştirme

```apache
ErrorDocument 404 /404.html
```

veya

```apache
ErrorDocument 404 /404.php
```

### 🔒 403 Yasak Erişim Özelleştirme

```apache
ErrorDocument 403 /403.html
```

### ⚠️ 500 Sunucu Hatası Özelleştirme

```apache
ErrorDocument 500 /500.html
```

---

## 📌 Dokümantasyon Bilgileri

| Bilgi | Detay |
|:------|:------|
| 👤 **Yazar** | Bahadır B. Bekdemir |
| 📅 **Tarih** | 15.01.2026 |
| 🔢 **Versiyon** | 2.0 |

---

## 💡 SEO İpuçları

- ✅ **200 OK**: Sayfalarınızın çoğu bu kodu döndürmelidir.
- 🔴 **301 Moved Permanently**: Domain değişikliği veya sayfa taşıma işlemlerinde mutlaka kullanın.
- ⚠️ **302 Found**: SEO için önerilmez, geçici yönlendirmeler için kullanın.
- ❌ **404 Not Found**: Eksik sayfaları düzenli olarak kontrol edin ve gerekirse 301 ile yönlendirin.
- ⚠️ **500/502/503**: Bu hataları hızlıca çözün, arama motorları sitenizi taramayı durdurabilir.

---

> 📚 **Referanslar:** RFC 7231, RFC 7232, RFC 7233, RFC 7234, RFC 7235, RFC 7236, RFC 7237, RFC 7238, RFC 7239, RFC 7240
