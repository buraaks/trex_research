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

* __Frontend Nedir?__

   Frontend, kullanıcının doğrudan etkileşimde bulunduğu web sitesinin görsel ve işlevsel yüzüdür.

   * __Kapsadığı Teknolojiler__:

     -HTML – Sayfa iskeleti

     -CSS – Stil ve düzen

     -JavaScript – Dinamik etkileşimler


* __Backend Nedir?__

Backend, sistemin sunucu tarafında çalışan, kullanıcının görmediği ama tüm işlevselliği sağlayan kısmıdır.

   * __Kapsadığı Teknolojiler__:

     -Programlama dilleri: Python, PHP, Ruby, Java, C#

     -Veritabanları: MySQL, PostgreSQL, MongoDB
 
     -Frameworkler: Laravel, Django, Spring, ASP.NET


</details>

<details><summary>-	Web sunucusu nedir? API nedir? API türleri</summary>

* __Web Sunucusu Nedir?__
 Web sunucusu, HTTP isteklerini alıp yanıtlayan bir yazılım veya donanım sistemidir. Temel görevi, istemciden (genellikle bir tarayıcıdan) gelen isteğe karşılık olarak web sayfası, veri veya dosya sunmaktır.

 * __Örnek Web Sunucuları__:

    -Apache

    -Nginx

    -Microsoft IIS

* __Görevleri__:

   -İstemciden gelen HTTP/HTTPS isteklerini dinlemek

   -İlgili dosyaları (HTML, CSS, JS) sunmak

   -Dinamik içerik için backend uygulamalarla iletişim kurmak

* __API Nedir?__

 API (Application Programming Interface), iki yazılımın birbiriyle standartlaştırılmış bir şekilde iletişim kurmasını sağlayan arayüzdür. Bir nevi yazılımlar arası “protokol” gibi düşünebilirsin.

 Gerçek Hayat Analojisi: Bir restoranda garson (API), senin siparişini mutfağa (sunucu) iletir ve yemeği sana getirir.

  * __Kullanım Alanları__:

       -Mobil uygulamaların sunucudan veri çekmesi

       -Web sitelerinin harici servislerle (ödeme, harita, hava durumu) entegrasyonu

       -Mikroservis mimarilerinde servisler arası iletişim

Video: [API nedir? ](https://www.youtube.com/watch?v=nXFI5Cd8FZE&list=PLeZr8VTNC1oZpyWb0azboUg01D5_Wr5I_)

</details>

<details><summary>-	HTTP nedir? HTTP metodları: GET, POST, PUT, DELETE</summary>

* __HTTP Nedir?__

HTTP (Hypertext Transfer Protocol), web tarayıcıları ile sunucular arasında veri alışverişini sağlayan bir iletişim protokolüdür. İnternet üzerindeki sayfaların yüklenmesi, veri gönderimi ve alınması gibi işlemler HTTP üzerinden gerçekleşir.

- İstemci (Client): Genellikle bir web tarayıcısıdır.

- Sunucu (Server): İstemciden gelen isteklere yanıt veren sistemdir.

HTTP, metin tabanlı bir protokoldür ve genellikle TCP/IP üzerinden çalışır.

* __HTTP Metodları__

  -HTTP protokolü, istemcinin sunucuya ne tür bir işlem yapmak istediğini   belirtmek için çeşitli metodlar kullanır. En yaygın kullanılan HTTP   metodları şunlardır:

  `GET` : Sunucudan veri almak için kullanılır. Örneğin bir web sayfasını görüntülemek.

  `POST`: Sunucuya veri göndermek için kullanılır. Örneğin bir formu doldurup göndermek.

  `PUT`: Sunucudaki mevcut veriyi güncellemek için kullanılır.

  `DELETE`: Sunucudaki veriyi silmek için kullanılır.

</details>

<details><summary>-	RESTful servislerin çalışma mantığı</summary>

REST (Representational State Transfer), web servislerinin daha basit, ölçeklenebilir ve standartlara uygun şekilde tasarlanmasını sağlayan bir mimari yaklaşımdır. RESTful servisler, HTTP metodlarını kullanarak kaynaklara erişim sağlar.

Kaynak (Resource): Her veri öğesi bir kaynak olarak temsil edilir ve genellikle bir URL ile tanımlanır.

*  __HTTP Metodları ile İşlem__:

   `GET /users` : Tüm kullanıcıları getirir.

   `POST /users` : Yeni bir kullanıcı oluşturur.

   `PUT /users/1` : ID’si 1 olan kullanıcıyı günceller.

   `DELETE /users/1` : ID’si 1 olan kullanıcıyı siler.

* __Stateless (Durumsuzluk)__: Her istekte gerekli tüm bilgiler yer alır; sunucu önceki istekleri hatırlamaz.

* __JSON Formatı__: Veri alışverişi genellikle JSON formatında yapılır.

</details>

<details><summary>-	JSON veri formatı ve kullanım amacı</summary>
JSON Veri Formatı ve Kullanım Amacı

JSON (JavaScript Object Notation), veri yapılarının kolayca okunabilir ve yazılabilir şekilde temsil edilmesini sağlayan hafif bir veri formatıdır. Özellikle web uygulamalarında istemci ile sunucu arasında veri alışverişi için yaygın olarak kullanılır.

Okunabilirlik: İnsanlar tarafından kolayca okunabilir ve anlaşılabilir.

Hafiflik: XML gibi diğer formatlara göre daha az yer kaplar.

Dil Bağımsızlığı: JSON, birçok programlama dili tarafından desteklenir.

Veri Yapısı: Anahtar-değer (key-value) çiftleri ve dizi (array) yapıları içerir.

* __Örnek JSON verisi__:

```
{
  "id": 1,
  "name": "Ali",
  "email": "ali@example..com"
}
```

Bu format sayesinde RESTful servisler, veri alışverişini hızlı ve etkili bir şekilde gerçekleştirebilir.

</details>

<details><summary>-	SOAP ve GraphQL nedir, REST’ten farkları</summary>

* __SOAP (Simple Object Access Protocol)__:

   -XML tabanlı bir protokoldür.

   -Katı kurallara ve standartlara sahiptir.

   -Güvenlik, hata yönetimi ve işlem bütünlüğü gibi konularda daha kapsamlıdır.

   -HTTP dışında SMTP gibi farklı protokoller üzerinden de çalışabilir.

   -Genellikle kurumsal sistemlerde tercih edilir.

* __GraphQL__:

    -Facebook tarafından geliştirilmiş bir sorgulama dilidir.

    -İstemci, tam olarak ihtiyaç duyduğu veriyi tanımlar ve sadece o veri döner.

    -Tek endpoint üzerinden çalışır.

    -JSON formatında veri döner.

    -REST’e göre daha esnek ve verimli veri çekimi sağlar.

* __REST ile Farkları__:

    -SOAP, REST’e göre daha karmaşık ve ağırdır; GraphQL ise daha esnek ve hafiftir.

    -REST çoklu endpoint yapısına sahiptir; GraphQL tek endpoint ile çalışır.

    -REST’te sunucu ne döneceğine karar verir; GraphQL’de istemci belirler.

Her yaklaşımın avantajları ve kullanım alanları farklıdır. REST genellikle basit ve hızlı çözümler için tercih edilirken, SOAP daha güvenli ve kurumsal sistemlerde; GraphQL ise veri esnekliği ve performans gerektiren modern uygulamalarda kullanılır.

</details>

<details><summary>-	HTTP metodlarını örneklerle açıklama</summary>

| Metod   | Amaç | Özellikler | Örnek Kullanım |
|---------|------|------------|----------------|
| **GET** | Sunucudan veri almak | - URL üzerinden parametre gönderilir<br>- Önbelleğe alınabilir<br>- Tarayıcı geçmişinde saklanır | `GET /products?id=15` |
| **POST** | Sunucuya veri göndermek (yeni kaynak oluşturmak) | - Veri gövde (body) içinde gönderilir<br>- Önbelleğe alınmaz<br>- Form gönderimlerinde yaygın | `POST /users` + `{ "name": "Burak" }` |
| **PUT** | Var olan kaynağı tamamen güncellemek veya yoksa oluşturmak | - İdempotent<br>- Tüm veriyi günceller | `PUT /users/5` + `{ "name": "Burak", "age": 30 }` |
| **PATCH** | Kaynağın belirli alanlarını güncellemek | - Kısmi güncelleme<br>- Daha az veri transferi | `PATCH /users/5` + `{ "age": 31 }` |
| **DELETE** | Kaynağı silmek | - Geri dönüşsüz olabilir<br>- Yetkilendirme gerektirir | `DELETE /users/5` |
| **HEAD** | Sadece başlık bilgilerini almak | - Gövde yok<br>- Dosya boyutu, tip gibi bilgileri öğrenmek için | `HEAD /file.zip` |
| **OPTIONS** | Sunucunun desteklediği metodları öğrenmek | - CORS ön kontrol isteklerinde kullanılır | `OPTIONS /users` → `Allow: GET, POST, PUT, DELETE` |


</details>

<details><summary>-	REST vs SOAP vs GraphQL temel karşılaştırması</summary>

| Özellik / Mimari | REST | SOAP | GraphQL |
|------------------|------|------|---------|
| **Tanım** | HTTP üzerinde çalışan, kaynak odaklı mimari stil | XML tabanlı, katı kurallara sahip mesajlaşma protokolü | İstemcinin ihtiyaç duyduğu veriyi tanımlayabildiği sorgu dili |
| **Veri Formatı** | Genellikle JSON (XML, HTML de olabilir) | Sadece XML | JSON (genellikle), tip sistemi ile |
| **Uç Nokta (Endpoint)** | Her kaynak için ayrı endpoint | Tek endpoint olabilir ama işlem bazlı SOAP action’lar | Tek endpoint üzerinden tüm sorgular |
| **Performans** | Basit ve hızlı, ancak fazla veri dönebilir (over-fetching) | XML ve ek protokoller nedeniyle daha yavaş | Gereksiz veri dönmez (over-fetching/under-fetching çözülür) |
| **Güvenlik** | HTTPS + OAuth/JWT gibi standart yöntemler | WS-Security ile mesaj seviyesinde güvenlik | REST’teki yöntemler + sorgu bazlı yetkilendirme |
| **Standartlaşma** | Esnek, resmi standart yok (HTTP kuralları dışında) | Katı standartlar (WSDL, XML Schema) | Şema (schema) ile tip güvenliği, resmi sorgu yapısı |
| **Kullanım Alanı** | Web servisleri, mobil API’ler, mikroservisler | Kurumsal entegrasyonlar, bankacılık, yüksek güvenlik gerektiren sistemler | Modern web ve mobil uygulamalar, veri yoğun istemciler |
| **Avantajlar** | Basit, yaygın, öğrenmesi kolay, esnek | Güvenli, standart, protokol bağımsız | Esnek veri sorgusu, tek endpoint, az veri transferi |
| **Dezavantajlar** | Over-fetching/under-fetching olabilir | Karmaşık, ağır, XML zorunluluğu | Öğrenme eğrisi, caching ve rate limit yönetimi daha karmaşık |


</details>

<details><summary>-	JSON veri örneği açıklaması</summary>

```
{
  "isim": "Burak",
  "yas": 29,
  "ogrenciMi": true,
  "beceriler": ["JavaScript", "Python", "Markdown"],
  "adres": {
    "sehir": "Bursa",
    "ilce": "Nilüfer",
    "postaKodu": 16140
  }
}
```

</details>

***
## 4. ASP.NET

<details><summary>-	ASP.NET ve ASP.NET Core nedir? Avantajları, farkları</summary>

* __ASP.NET Nedir?__

   -Microsoft tarafından geliştirilen, .NET Framework üzerinde çalışan bir web uygulama geliştirme platformudur.

   -Genellikle Windows tabanlı sunucularda çalışır.

   -ASP.NET Web Forms, MVC ve Web API gibi farklı mimari yaklaşımları destekler.

   -Daha eski ve olgun bir teknolojidir; kurumsal projelerde hâlâ yaygın olarak kullanılır.

   * ASP.NET Avantajları:

     -Kurumsal projelerde denenmiş ve test edilmiş.

     -Geniş dokümantasyon ve destek.

     -Windows Server ile tam uyum.

* __ASP.NET Core Nedir?__

   -ASP.NET’in modern, yeniden tasarlanmış versiyonudur.

   -Platform bağımsızdır: Windows, macOS ve Linux üzerinde çalışabilir2.

   -.NET Core veya .NET 5+ ile birlikte gelir; açık kaynaklı ve topluluk desteklidir.

   -Modüler, hafif ve yüksek performanslıdır.

   -Bulut ve mikro hizmet mimarileri için optimize edilmiştir.

     * __ASP.NET Core Avantajları__:

       -Yüksek performans ve düşük kaynak tüketimi.

       -Platformlar arası geliştirme imkânı.

       -Modern mimariler (MVC, Razor Pages, Blazor, gRPC) ile uyumlu.
 
       -CI/CD ve container ortamlarıyla kolay entegrasyon.

       -Açık kaynak olduğu için sürekli güncelleniyor.

* [ASPN.NET e başlamak için tıkla](https://dotnet.microsoft.com/en-us/apps/aspnet)

</details>

<details><summary>-	MVC nedir, ne için kullanılır?  </summary>

* __MVC (Model–View–Controller)__, yazılım geliştirmede kullanılan bir mimari desen olup, uygulamayı üç temel bileşene ayırarak daha düzenli, test edilebilir ve sürdürülebilir hale getirir. Senin gibi sistematik düşünen biri için bu yapı, kodun mantıksal bölümlere ayrılması açısından oldukça verimlidir.

|Bileşen|Görevi|
|-------|------|
|Model|Verileri temsil eder. Veritabanı işlemleri, iş mantığı ve veri yönetimi burada yapılır|
|View|Verileri temsil eder. Veritabanı işlemleri, iş mantığı ve veri yönetimi burada yapılır.|
|Controller|Kullanıcıdan gelen istekleri alır, uygun Model’i çağırır ve sonucu View’a iletir.|

- Ne için kullanılır: MVC, web uygulamalarında kodun mantıksal katmanlara ayrılmasını sağlayarak daha düzenli ve test edilebilir bir yapı sunar.

- Nerelerde kullanılır: ASP.NET, Django, Laravel gibi framework’lerde web, mobil ve masaüstü uygulama geliştirmede yaygın olarak kullanılır.
</details>

<details><summary>-	Middleware nedir, nasıl çalışır?</summary>

* __Middleware Nedir?__
   -Middleware, bir uygulamanın istek–yanıt döngüsünde araya girerek işlemler yapmasını sağlar.

   -Örneğin: kimlik doğrulama, hata yönetimi, loglama, yönlendirme, önbellekleme gibi görevleri üstlenebilir.

   -Her middleware bileşeni, bir pipeline içinde sırayla çalışır ve isteği bir sonraki bileşene iletir veya durdurabilir.

* __Nasıl Çalışır?__
   -İstek gelir → Middleware bileşeni isteği alır.

   -İşlem yapar → İsteği okur, düzenler veya kontrol eder.

   -Sonraki bileşene iletir → next() fonksiyonu ile zincirdeki bir sonraki middleware’e geçilir.

   -Yanıt döner → Middleware, yanıt üzerinde işlem yapabilir veya doğrudan döndürebilir.

* __Örnek Senaryo:__
```
app.Use(async (context, next) =>
{
    Console.WriteLine("İstek alındı: " + context.Request.Path);
    await next.Invoke(); // Sonraki middleware'e geç
    Console.WriteLine("Yanıt gönderiliyor.");
});
```
   -Bu örnekte, gelen isteği loglayan bir middleware tanımlanmış. next.Invoke() çağrısı ile zincirdeki bir sonraki middleware çalıştırılıyor, ardından yanıt sürecinde işlem yapılabiliyor.
</details>

<details><summary>-	Dependency Injection (DI) nedir, neden önemlidir?</summary>

* __DI Nedir?__

   -Dependency Injection (DI), yazılım geliştirmede bir sınıfın ihtiyaç duyduğu nesneleri kendisi oluşturmak yerine dışarıdan almasını sağlayan bir tasarım desenidir. Bu yaklaşım, kodun daha modüler, test edilebilir ve bakımı kolay olmasını sağlar.

   -Bir sınıfın bağımlı olduğu diğer sınıfları doğrudan oluşturmak yerine, bu bağımlılıkların enjekte edilmesi prensibine dayanır.

   -Örneğin bir OrderService sınıfı, EmailSender gibi bir servise ihtiyaç duyuyorsa, onu new ile oluşturmak yerine dışarıdan alır.

```
public class OrderService
{
    private readonly IEmailSender _emailSender;

    public OrderService(IEmailSender emailSender)
    {
        _emailSender = emailSender;
    }
}
```
   -Bu örnekte OrderService, IEmailSender bağımlılığını dışarıdan alır—yani bağımlılık enjekte edilir.

   * __Neden Önemlidir?__
     -Gevşek bağlılık (Loose Coupling): Sınıflar birbirine sıkı sıkıya bağlı olmaz, böylece bir bileşen değiştiğinde diğerleri etkilenmez.

     -Test kolaylığı: Mock veya sahte nesnelerle birim testler kolayca yazılabilir.

     -Yeniden kullanılabilirlik: Aynı sınıf farklı bağımlılıklarla tekrar kullanılabilir.

     -Bakım kolaylığı: Bağımlılıklar merkezi olarak yönetildiği için sistemin bakımı daha kolay ve güvenlidir.

</details>

<details><summary>-	Katmanlı Mimari (Layered Architecture)</summary>

Katmanlı mimari, yazılım projelerinde sistemsel karmaşıklığı azaltmak, sürdürülebilirliği artırmak ve geliştirme sürecini modülerleştirmek için kullanılan bir yapılandırma yaklaşımıdır. Senin gibi optimizasyon ve sistem tasarımına meraklı biri için bu mimari, hem mantıksal ayrım hem de test edilebilirlik açısından oldukça güçlü bir temel sunar.

* __Katmanlar__: Presentation – Business – Data Access

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


