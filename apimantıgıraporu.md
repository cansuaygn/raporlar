# API Mantığı (REST & JSON Temelleri)

Bu çalışmada backend geliştirmenin temel konularından biri olan **API mantığını** anlamaya çalıştım. Modern web uygulamalarında frontend ile backend arasındaki iletişim API üzerinden sağlanır. Bu yüzden API kavramını öğrenmek backend geliştirmeye giriş için önemli bir adımdır.

Bu araştırmada şu konular incelenmiştir:

- API nedir?
- API neden kullanılır?
- REST mimarisi
- HTTP metodları (GET, POST, PUT, DELETE)
- JSON veri yapısı
- Basit bir API endpoint tasarımı

---

# API Nedir?

**API (Application Programming Interface)** iki farklı yazılımın birbiriyle iletişim kurmasını sağlayan bir arayüzdür.

Bir uygulama başka bir uygulamadan veri almak istediğinde API kullanır. Örneğin bir hava durumu uygulaması yaptığımızı düşünelim. Telefon uygulaması doğrudan meteoroloji veritabanına bağlanmaz. Bunun yerine bir API isteği gönderir.

Örnek bir API isteği şu şekilde olabilir:

```http
GET /weather?city=istanbul

Sunucu bu isteği aldıktan sonra veriyi işler ve sonucu genellikle JSON formatında geri gönderir.

{
  "city": "Istanbul",
  "temperature": 21,
  "status": "Cloudy"
}

Bu sayede farklı uygulamalar aynı servisi kullanabilir.

API Neden Kullanılır?

API kullanımı modern yazılım mimarisinde çok önemlidir.

Sistemlerin bağımsız çalışmasını sağlar

Frontend ve backend ayrı geliştirilir. Örneğin bir sistemde:

Web sitesi

Mobil uygulama

Masaüstü uygulaması

hepsi aynı API üzerinden veri alabilir.

Veri paylaşımını kolaylaştırır

Bazı servisler API üzerinden veri sağlar.

Örnekler:

Google Maps API

OpenWeather API

Stripe ödeme API

Yazılım mimarisini daha düzenli hale getirir

Backend tarafı:

veriyi işler

veritabanını yönetir

güvenliği sağlar

Frontend ise sadece API üzerinden veri alır ve kullanıcıya gösterir.

REST API Nedir?

REST (Representational State Transfer) web API'leri tasarlamak için kullanılan bir mimari yaklaşımdır.

REST mimarisinde sistemdeki her veri bir resource (kaynak) olarak düşünülür.

Örneğin bir uygulamada şu kaynaklar olabilir:

/users
/products
/orders

Her kaynak üzerinde belirli işlemler yapılabilir. Bu işlemler HTTP metodları ile belirlenir.

HTTP Metodları

REST API'lerde en sık kullanılan dört temel HTTP metodu vardır.

GET

GET metodu sunucudan veri almak için kullanılır.

Örnek bir istek:

GET /users

Sunucu tüm kullanıcıları döndürür.

[
  {"id": 1, "name": "Ali"},
  {"id": 2, "name": "Ayşe"}
]
POST

POST metodu yeni veri oluşturmak için kullanılır.

POST /users

İstek ile birlikte gönderilen veri:

{
  "name": "Cansu",
  "age": 19
}

Sunucu bu veriyi alarak yeni bir kullanıcı oluşturur.

PUT

PUT metodu mevcut veriyi güncellemek için kullanılır.

PUT /users/1

Gönderilen veri:

{
  "name": "Ali Yılmaz"
}

Bu işlem kullanıcı bilgilerini günceller.

DELETE

DELETE metodu veriyi silmek için kullanılır.

DELETE /users/1

Bu istek kullanıcıyı sistemden kaldırır.

JSON Veri Yapısı

API'lerde veri alışverişi genellikle JSON (JavaScript Object Notation) formatı ile yapılır.

JSON:

hafif bir veri formatıdır

insanlar tarafından kolay okunur

makineler tarafından hızlı işlenir

Örnek bir JSON veri yapısı:

{
  "name": "Cansu",
  "age": 19,
  "skills": ["Python", "SQL", "API"]
}

JSON yapısında veriler anahtar-değer (key-value) şeklinde tutulur.

Nesneler { }

Diziler [ ]

ile gösterilir.

Basit Bir API Endpoint Tasarımı

Bir REST API tasarlanırken endpointler genellikle kaynak mantığı ile oluşturulur.

Örnek olarak bir stok yönetim sistemi düşünelim.

Tüm ürünleri listelemek için:

GET /products

Tek bir ürünü getirmek için:

GET /products/1

Yeni ürün eklemek için:

POST /products

Gönderilen veri şu şekilde olabilir:

{
  "name": "Laptop",
  "price": 25000
}

Ürün güncellemek için:

PUT /products/1

Ürün silmek için:

DELETE /products/1

Bu yapı REST API tasarımında oldukça yaygın olarak kullanılır.

Backend Açısından API'nin Önemi

Backend geliştirmenin büyük bir kısmı API tasarlamak ve yönetmek üzerine kuruludur.

Backend tarafında geliştiriciler genellikle:

endpoint oluşturur

veritabanı ile bağlantı kurar

gelen istekleri işler

güvenlik kontrolleri yapar

veri formatlarını yönetir

Modern yazılım sistemlerinin çoğu API tabanlı mimari kullanır.

Örneğin:

mobil uygulamalar

web uygulamaları

mikroservis sistemleri

Bu nedenle API mantığını anlamak backend geliştirmeye giriş için önemli bir adımdır.