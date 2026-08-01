**Design Pattern Nedir?**

Design Pattern, yazılım geliştirme sürecinde tekrar eden tasarım problemlerini çözmek amacıyla oluşturulmuş doğruluğu farklı projelerde kanıtlanmış genel çözüm yaklaşımlarıdır.

Burada dikkat edilmesi gereken en önemli nokta şudur:
belirli bir problemi çözen hazır bir kod parçası değildir belirli türdeki problemlerin nasıl çözülebileceğini açıklayan bir tasarım modelidir.

Buradaki tasarım;
Yazılımı oluşturan sınıfların, nesnelerin, modüllerin ve bileşenlerin birbirleriyle olan ilişkilerinin planlanmasıdır, 
Kod yazmadan önce sistemin nasıl organize edileceğine karar verme sürecidir.

**Design Pattern Türleri**
- Creational Patterns:
	Nesnelerin nasıl oluşturulacağını düzenleyen desenlerdir.
    Bu nesne nasıl oluşturulmalı?
    + Singleton: Aynı sınıftan yalnızca bir nesne oluşturulmasını sağlamak.
    + Factory : Nesne oluşturma işlemini merkezi bir yapı üzerinden yönetmek.
-Structural Patterns:
	Nesnelerin ve sınıfların nasıl bir araya ge	tirileceğini düzenleyen desenlerdir.
	Bu yapılar nasıl bağlanmalı?
    + Adapter: Birbirleriyle uyumsuz yapıların birlikte çalışmasını sağlamak
    + Decorator: Mevcut nesnenin davranışını değiştirmeden yeni özellikler eklemek.
-Behavioral Patterns:
	Nesnelerin birbirleriyle nasıl iletişim kuracağını ve nasıl davranacağını düzenleyen desenlerdir.
    Bu nesneler nasıl etkileşmeli?
    + Strategy: Aynı işi yapan farklı algoritmalar arasında çalışma anında seçim yapabilmek.
    + Observer: Bir nesnedeki değişiklikleri ilgili diğer nesnelere otomatik olarak bildirmek.

**Neden Design Pattern Kullanılır?**
1. Kodun okunabilirliğini artırmak
Standart bir yapı kullanıldığı için farklı geliştiriciler kodu daha kolay anlayabilir.

2. Kod tekrarını azaltmak
Aynı çözümün farklı yerlerde tekrar yazılması engellenir.

3. Değişiklik yapmayı kolaylaştırmak
Yeni özellik eklenirken mevcut çalışan kodun mümkün olduğunca az değiştirilmesi hedeflenir.

4. Bakım maliyetini düşürmek
Yıllar boyunca geliştirilecek projelerde hata bulma ve düzeltme süreçleri kolaylaşır.

5. Test edilebilirliği artırmak
Kod daha bağımsız parçalara ayrıldığı için birim testleri daha kolay yazılır.

6. Ortak bir dili oluşturmak
Bir ekip içinde "Factory kullanalım" veya "Observer burada daha uygun" denildiğinde herkes aynı tasarım yaklaşımını anlar. Bu, iletişimi hızlandırır ve yanlış anlaşılmaları azaltır.