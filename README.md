<p align="center">
<a href="https://trex.com.tr/en/">
<img src="https://trex.com.tr/assets/img/logo.png"
alt="Trex Logo"
width="300" height="100">
</a>

</p>
<p align="center">
Trex Dijital Akıllı Üretim Sistemleri A.Ş 
</p>

***
## ARAŞTIRMA & RAPORLAMA ÖDEVİ (.NET)
***
## İçindekiler
- 1 . [Modern Yazılım Geliştirme Pratikleri](#1-modern-yazılım-geliştirme-pratikleri)
- 2 . [.NET Ekosistemi](#2-net-ekosistemi)
- 3 . [Backend Geliştirme Temelleri](#3-backend-geliştirme-temelleri)
- 4 . [ASP.NET](#4-aspnet)
- 5 . [Veritabanı ve ORM](#5-veritabanı-ve-orm)
- 6 . [Güvenlik ve Performans](#6-güvenlik-ve-performans)
- 7 . [Logging ve Hata Yönetimi](#7-logging-ve-hata-yönetimi)
- 8 . [Yazılım Geliştirme Prensipleri](#8-yazılım-geliştirme-prensipleri)
***
<a id="1-modern-yazılım-geliştirme-pratikleri"></a>
## 1. Modern Yazılım Geliştirme Pratikleri 
<details>
<summary>- Git nedir? GitHub nedir?</summary>
     Git, yazılım projelerindeki tüm değişiklikleri kaydedip yönetmeye yarayan bir versiyon kontrol sistemi iken; GitHub, bu Git projelerini internet üzerinde depolamayı, paylaşmayı ve işbirliği yapmayı sağlayan bulut tabanlı bir platformdur.
 	</details>
<details><summary>- Temel Git komutları</summary>
ali was here
`git init` → Yeni bir Git deposu (proje) başlatır.

`git clone [url]` →  Var olan bir uzak (remote) depoyu bilgisayarına kopyalar.

`git add [dosya]` → Dosyayı bir sonraki commit için hazırlık alanına (staging area) ekler.

`git commit -m "mesaj"` → Hazırlanan değişiklikleri kalıcı olarak kaydeder.

`git push` → Yerel (local) commitleri GitHub gibi uzak depoya gönderir.

`git pull` → Uzak depodaki son değişiklikleri bilgisayarına indirip birleştirir.

`git branch [isim]` → Yeni bir dal (branch) oluşturur.

`git merge [isim]` → Belirtilen dalı (branch) aktif dal ile birleştirir.

</details>
<details><summary>-	Merge conflict nedir, nasıl çözülür?</summary>

* Merge conflict, iki branch'ın 'merge'lenirken bir dosyanın aynı yerinde farklı değişiklikler yapılmış olmasından kaynaklanan 'merge'lenememe durumudur. Git, aynı yerde birbirinden farklı iki değişikliği nasıl ele alması gerektiğini bilemez ve hata verir. Dosyada çakışan bölge(ler),
    * `<<<<<<<HEAD` ve `=======`
* arasında gösterilir. Bu kısımda hangi versiyonun kabul edileceği yazılımcı tarafından manuel şekilde belirlenir ve ancak böyle 'merge' işlemi gerçekleşebilir.

</details>


</details>
<details><summary>-	CI/CD nedir? Azure DevOps, GitHub Actions ile pipeline örnekleri</summary>     

**- CI (Continuous Integration / Sürekli Entegrasyon)**:** Geliştirilen kodun otomatik olarak test edikmesidir , hatanın daha kolay anlaşılmasını sağlar.

**- CD (Continuous Delivery / Deployment / Sürekli Teslimat / Dağıtım):** Bir kod geliştirilirken yayınlanmasını sağlar. Yeni sürümleri daha hızlı yayınlanmasını sağlar.

</details>

<details><summary>-	Software Development Life Cycle (SDLC)</summary> 

 **-Yazılım Geliştirme Yaşam Döngüsü (SDLC)**: Bir yazılım fikirden gerçeğe geçişine kadar geçen süredir.

**o	Aşamalar**
1. Planlama:	Projenin amacı, kapsamı, zaman ve maliyet tahminleri yapılır.
2. Analiz:	Gereksinimler toplanır, sistem gereksinimleri belirlenir (ne yapılacak?).
3. Geliştirme:	Yazılım tasarlanır ve kodlanır.
4. Test:	Yazılım hatalara karşı test edilir, doğruluk ve kalite kontrolü yapılır.
5. Dağıtım:	Testleri geçen ürün üretim ortamına (kullanıcılara) sunulur.
6. Bakım:	Canlı sistemde hata düzeltme, iyileştirme ve güncellemeler yapılır.

**o	Agile/Scrum/Kanban metodolojileri**

 * Agile: Yazılımı küçük parçalara bölerek , hızlı ve esnek şekilde geliştirmeyi amaçlayan yaklaşım.

 * Scrum: Agile içinde, işleri sabit süreli sprint’lere (kısa süreli çalışma periyodu) ayırarak ekip çalışmasını yöneten bir çerçeve.

 * Kanban: İşlerin görsel bir panoda sürekli akışla yönetildiği, esnek bir Agile yöntemi.

</details>

***

## 2. NET Ekosistemi

<details><summary>-	.NET nedir? Tarihçesi, amacı, neden kullanılır?</summary>
     
**- .NET** microsoft tarafından geliştirilen bir yazılım geliştirme platformudur.2002 yılında piyasaya sürülmüştür . Amacı farklı yazılım dillerini bir araya getirerek yazılım geliştirmeyi kolaylaştırmaktır.Web , masaüstü ve mobil uygulamalar gibi çeşitli alanlarda kullanlıabilir.

</details>

<details><summary>-	.NET Framework, .NET Core ve .NET 7/8+ farkları</summary>
     
|Özellik             | .NET Framework | .NET Core             | .NET                  |
|--------------------|----------------|-----------------------|-----------------------|
|Platform            |Windows         |Windows, Linux, macOS  |Windows, Linux, macOS  |
|Açık Kaynak         |Hayır           |Evet                   |Evet                   |
|Performans          |Orta            |Yüksek                 |Çok Yüksek             |
|Modülerlik          |Monolitik       |Modüler                |Modüler                |
|Güncelleme Desteği  |Sınırlı         |Aktif                  |Sürekli                |
|Microservis Desteği |Zayıf           |Güçlü                  |Güçlü                  |
|Bulut Uygulamları   |Kısıtlı         |Uygun                  |Uygun                  |
|Modern API Desteği  |Kısıtlı         |Geniş                  |Geniş                  |
</details>

<details><summary>•	Senkron ve Asenkron Programlama</summary>

**Senkron Programlama:** İşlemler sırasıyla gerçekleşir. Genllikle daha basit ve anlaşılırdır ancak uzun süren işlemlerde kullanıcı deneyimini olumsuz etkileyebilir.

**Asenkron Programlama:** İşlemler aynı anda veya birbirinden bağımsız çalışabilir.Uzun süren işlemler arka planda yürütülürken kullanıcı arayüzü yanıt vermeye devam eder.

- **Anahtar Kavramlar:**
`async` : Bir metodun asenkron olduğunu belirtir , bu metod `await` ile çağırabilir.
`await` : Asenkron bir işlemin tamamlanmasını beklerken kontrolü çağıran metoda geri verir.
`Task` : .NET'te asenkron işlemleri temsil eden bir türdür. Bir işlemin gelecekte tamamlanacağını ifade eder. Örneğin, bir dosya okuma işlemi `Task<string>` dönebilir. `Task nesnesi`, işlem tamamlandığında sonucu sağlar.

</details>
<details><summary>• arrow function (=>) ifadesinin C#’taki yeri</summary>

   C# dilinde `=>` operatörü, lambda ifadelerini tanımlamak için kullanılır. Lambda ifadeleri, isimsiz metodlar oluşturmak için kullanılır ve genellikle kısa, tek satırlık işlemler için tercih edilir.

   `=>` operatörü kullanarak girilen değerin karesini alma, örnek kod:
   
`
Console.Write("Bir sayı girin: ");
int x = Convert.ToInt32(Console.ReadLine());
Func<int, int> kareAl = x => x * x;
Console.WriteLine($"{x} sayısının karesi: {kareAl(x)}");
`

</details>

***
## 3. Backend Geliştirme Temelleri

<details><summary>-	Backend nedir? Frontend ile farkları</summary>

o Frontend Nedir?

Frontend, kullanıcının doğrudan etkileşimde bulunduğu web sitesinin görsel ve işlevsel yüzüdür.

* Kapsadığı Teknolojiler:

  -HTML – Sayfa iskeleti

  -CSS – Stil ve düzen

  -JavaScript – Dinamik etkileşimler


o Backend Nedir?

Backend, sistemin sunucu tarafında çalışan, kullanıcının görmediği ama tüm işlevselliği sağlayan kısmıdır.

* Kapsadığı Teknolojiler:

   -Programlama dilleri: Python, PHP, Ruby, Java, C#

   -Veritabanları: MySQL, PostgreSQL, MongoDB

   -Frameworkler: Laravel, Django, Spring, ASP.NET


</details>

<details><summary>-	Web sunucusu nedir? API nedir? API türleri</summary>

o Web Sunucusu Nedir?
 Web sunucusu, HTTP isteklerini alıp yanıtlayan bir yazılım veya donanım sistemidir. Temel görevi, istemciden (genellikle bir tarayıcıdan) gelen isteğe karşılık olarak web sayfası, veri veya dosya sunmaktır.

 * Örnek Web Sunucuları:

    -Apache

    -Nginx

    -Microsoft IIS

* Görevleri:

   -İstemciden gelen HTTP/HTTPS isteklerini dinlemek

   -İlgili dosyaları (HTML, CSS, JS) sunmak

   -Dinamik içerik için backend uygulamalarla iletişim kurmak

o API Nedir?

 API (Application Programming Interface), iki yazılımın birbiriyle standartlaştırılmış bir şekilde iletişim kurmasını sağlayan arayüzdür. Bir nevi yazılımlar arası “protokol” gibi düşünebilirsin.

 Gerçek Hayat Analojisi: Bir restoranda garson (API), senin siparişini mutfağa (sunucu) iletir ve yemeği sana getirir.

* Kullanım Alanları:

    -Mobil uygulamaların sunucudan veri çekmesi

    -Web sitelerinin harici servislerle (ödeme, harita, hava durumu) entegrasyonu

    -Mikroservis mimarilerinde servisler arası iletişim
</details>

<details><summary>-	HTTP nedir? HTTP metodları: GET, POST, PUT, DELETE</summary>

o HTTP Nedir?

HTTP (Hypertext Transfer Protocol), web tarayıcıları ile sunucular arasında veri alışverişini sağlayan bir iletişim protokolüdür. İnternet üzerindeki sayfaların yüklenmesi, veri gönderimi ve alınması gibi işlemler HTTP üzerinden gerçekleşir.

- İstemci (Client): Genellikle bir web tarayıcısıdır.

- Sunucu (Server): İstemciden gelen isteklere yanıt veren sistemdir.

HTTP, metin tabanlı bir protokoldür ve genellikle TCP/IP üzerinden çalışır.

* HTTP Metodları

  -HTTP protokolü, istemcinin sunucuya ne tür bir işlem yapmak istediğini   belirtmek için çeşitli metodlar kullanır. En yaygın kullanılan HTTP   metodları şunlardır:

  `GET` : Sunucudan veri almak için kullanılır. Örneğin bir web sayfasını görüntülemek.

  `POST`: Sunucuya veri göndermek için kullanılır. Örneğin bir formu doldurup göndermek.

  `PUT`: Sunucudaki mevcut veriyi güncellemek için kullanılır.

  `DELETE`: Sunucudaki veriyi silmek için kullanılır.

</details>

<details><summary>-	RESTful servislerin çalışma mantığı</summary>

</details>

<details><summary>-	JSON veri formatı ve kullanım amacı</summary>

</details>

<details><summary>-	SOAP ve GraphQL nedir, REST’ten farkları</summary>

</details>

<details><summary>-	HTTP metodlarını örneklerle açıklama</summary>

</details>

<details><summary>-	REST vs SOAP vs GraphQL temel karşılaştırması</summary>

</details>

<details><summary>-	JSON veri örneği açıklaması</summary>

</details>

***
## 4. ASP.NET

<details><summary>-	ASP.NET ve ASP.NET Core nedir? Avantajları, farkları</summary>

</details>

<details><summary>-	MVC nedir, ne için kullanılır?  </summary>

</details>

<details><summary>-	Middleware nedir, nasıl çalışır?</summary>

</details>

<details><summary>-	Dependency Injection (DI) nedir, neden önemlidir?</summary>

</details>

<details><summary>-	Katmanlı Mimari (Layered Architecture)</summary>

</details>

<details><summary>-	Clean Architecture</summary>

</details>

***
## 5. Veritabanı ve ORM

<details><summary>-	SQL nedir? </summary>

</details>

<details><summary>-	İlişkisel ve ilişkisel olmayan veri tabanları arasındaki farklar</summary>

</details>

<details><summary>-	ORM nedir? Entity Framework Core nedir?</summary>

</details>

<details><summary>-	DbContext nedir, nasıl kullanılır?</summary>

</details>

<details><summary>-	LINQ nedir? En çok kullanılan LINQ ifadeleri</summary>

</details>

<details><summary>-	Code-First ve Database-First yaklaşımı nedir?</summary>

</details>

<details><summary>-	Temel SQL sorguları: SELECT, INSERT, UPDATE, DELETE</summary>

</details>

<details><summary>-	LINQ örnekleri ve karşılık gelen SQL açıklamaları</summary>

</details>

<details><summary>- Code-First vs DB-First karşılaştırması</summary>

</details>

<details><summary>-	4 temel SQL sorgusuna örnek

</summary>

</details>

***
## 6. Güvenlik ve Performans 

<details><summary>-	Authentication vs Authorization nedir?</summary>

</details>

<details><summary>-	Authentication vs Authorization nedir?</summary>

</details>

<details><summary>-	OAuth, OAuth2.0, OpenIddict, OpenID nedir? Aralarındaki </summary>

</details>

<details><summary>-	Performans artımı için ne yapılabilir? (AsNoTracking, IAsyncEnumerable, caching, profiling, redis)</summary>

</details>

<details><summary>-	Performans artımı için ne yapılabilir? (AsNoTracking, IAsyncEnumerable, caching, profiling, redis)</summary>

</details>

<details><summary>-	JWT yapısının temel bileşenleri</summary>

</details>

<details><summary>-	Performans için önerilen en az 3 teknik ve açıklamaları</summary>

</details>

<details><summary>-	OWASP 10 listesi ve her biri için 1–2 cümlelik açıklamalar</summary>

</details>

***
## 7. Logging ve Hata Yönetimi

<details><summary>-	Neden loglama yapılır? Log seviyesi nedir?</summary>

</details>

<details><summary>-	ASP.NET Core'da logging altyapısı</summary>

</details>

<details><summary>-	Global exception handling nasıl yapılır?</summary>

</details>

<details><summary>-	UseExceptionHandler ve ILogger nasıl kullanılır?</summary>

</details>

<details><summary>-	Log seviyelerinin açıklamaları (Information, Warning, Error vs.)</summary>

</details>

<details><summary>-	Örnek hata yönetim kodu açıklaması</summary>

</details>


***
## 8. Yazılım Geliştirme Prensipleri




<details><summary>-	SOLID prensipleri: Her biri için kısa açıklama ve örnek</summary>

</details>

<details><summary>-	Design Patterns: Singleton, Repository, Factory</summary>

</details>

<details><summary>-	Clean Code nedir, neden önemlidir?</summary>

</details>

<details><summary>-	Yazılım Mimari Desenleri</summary>

</details>

<details><summary>-	Her SOLID prensibi için kısa örnek</summary>

</details>

<details><summary>-	En az 2 design pattern açıklaması</summary>

</details>

<details><summary>-	Clean Code uygulama örnekleri</summary>

</details>

<details><summary>-	Farklı yazılım mimarilerini karşılaştıran bir tablo veya kısa açıklamalar</summary>

</details>

---

<details><summary></summary>

</details>


6. özellikler

8. destek ve iletişim 

10. tşk


