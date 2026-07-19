# Güvenlik Temelleri (Security Basics)

 Uygulamanın kullanıcı bilgilerini koruyabilmesi ve kötü niyetli kişilere karşı güvenli olması da gerekir.
  Bu nedenle güvenlik, yazılım geliştirmenin en önemli parçalarından biridir. 

Authentication ve Authorization kavramları birbirine çok benzese farklı amaçlara hizmet eder. 
Authentication, sisteme giriş yapan kişinin gerçekten o kişi olup olmadığını doğrulama işlemidir. 
    Kullanıcının e-posta ve şifresini girerek sisteme giriş yapması buna örnek verilebilir. 
Authorization ise sisteme giriş yapan kullanıcının hangi işlemleri yapabileceğini belirler. 
    Örneğin bir yönetici kullanıcı yeni kullanıcı ekleyebilirken normal bir kullanıcı sadece kendi bilgilerini görüntüleyebilir. 
Yani Authentication "Kimsin?" sorusuna cevap verirken Authorization "Ne yapabilirsin?" sorusuna cevap verir.

Günümüzde birçok web uygulamasında JWT yani JSON Web Token kullanılmaktadır.
Kullanıcı giriş yaptıktan sonra sunucu tarafından bir token oluşturulur ve kullanıcı sonraki isteklerinde bu tokenı gönderir. 
Böylece her istekte tekrar kullanıcı adı ve şifre kontrolü yapılmasına gerek kalmaz. 
JWT üç bölümden oluşur: Header, Payload ve Signature. 
    Payload kısmında kullanıcıyla ilgili bazı bilgiler bulunabilir ancak bu bölüm şifrelenmediği için parola gibi hassas bilgilerin burada tutulmaması gerekir.

OAuth ise farklı uygulamalara mevcut hesaplarımızla giriş yapmamızı sağlayan bir yetkilendirme mekanizmasıdır. 
    Örneğin bir uygulamaya "Google ile Giriş Yap" seçeneğiyle giriş yaptığımızda uygulama Google hesabımızın şifresini öğrenmez bunun yerine Google gerekli doğrulamayı yapar ve uygulamaya belirli izinler verir bu yöntem hem kullanıcıya  kolaylık sağlar hem de güvenliği artırır.

Yazılım geliştirme sırasında karşılaşılabilecek en yaygın saldırılardan biri SQL Injection'dır Eğer kullanıcıdan alınan veriler doğrudan SQL sorgusunun içine eklenirse saldırgan sorguyu değiştirebilir ve veritabanındaki bilgilere erişebilir. 
Bu nedenle parametreli sorgular kullanılması, kullanıcı girişlerinin doğrulanması ve mümkün olduğunda ORM araçlarından yararlanılması önemlidir. 

Bir diğer yaygın saldırı türü ise XSS yani Cross Site Scripting saldırılarıdır bu saldırılarda amaç web sayfasına zararlı JavaScript kodları ekleyerek bu kodların başka kullanıcıların tarayıcılarında çalışmasını sağlamaktır. Böyle bir durumda kullanıcı oturum bilgileri ele geçirilebilir veya sahte içerikler gösterilebilir.
     XSS saldırılarından korunmak için kullanıcıdan gelen verilerin filtrelenmesi, HTML karakterlerinin güvenli hale getirilmesi ve gerekli durumlarda Content Security Policy gibi güvenlik önlemlerinin uygulanması gerekir.

Bu konuları araştırırken güvenli yazılım geliştirmenin sadece kod yazmaktan ibaret olmadığını fark ettim.  Özellikle Authentication ile Authorization arasındaki farkı ve JWT ile OAuth'un hangi amaçlarla kullanıldığını daha iyi anladım. Ayrıca SQL Injection ve XSS gibi saldırıların, kullanıcıdan alınan verilerin kontrol edilmemesi durumunda ne kadar ciddi sonuçlar doğurabileceğini öğrendm.

