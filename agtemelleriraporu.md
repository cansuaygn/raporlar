Networking Basics
Introduction
Networking, bilgisayarların ve cihazların birbirleriyle veri alışverişi yapmasını sağlayan sistemdir. İnternet üzerinden çalışan çoğu yazılım aslında ağ iletişimi kullanır. Web siteleri, mobil uygulamalar ve oyunlar veri gönderip almak için ağ protokollerinden yararlanır.

Bu raporda ağ temelleri olan IP, Port, DNS, TCP, UDP, paket yapısı ve bazı ağ araçları açıklanmaktadır.

IP Address
IP adresi, ağ üzerindeki her cihazın benzersiz kimliğidir. Cihazlar birbirleriyle iletişim kurarken IP adreslerini kullanır.

Örnek IP adresleri:

192.168.1.1
8.8.8.8
142.250.190.78
IP adresleri sayesinde veri paketleri doğru hedef cihaza gönderilir.

IP adresleri ikiye ayrılır:

Public IP: İnternet üzerinde erişilebilir IP adresi
Private IP: Yerel ağlarda kullanılan IP adresi
Port
Port, bir bilgisayarda çalışan farklı servisleri ayırmak için kullanılan numaradır. Aynı IP adresinde birden fazla servis çalışabilir ve port numarası hangi servise bağlanılacağını belirler.

Yaygın port örnekleri:

80 → HTTP
443 → HTTPS
22 → SSH
21 → FTP
3306 → MySQL
Örnek bağlantı:

example.com:8080

Buradaki 8080 port numarasını temsil eder.

DNS (Domain Name System)
DNS sistemi domain isimlerini IP adreslerine çevirir. İnsanlar IP adresleri yerine site isimlerini kullanır.

Örnek:

google.com → 142.250.190.78

Bir kullanıcı web sitesi açtığında şu adımlar gerçekleşir:

Tarayıcı domain adresini DNS sunucusuna sorar
DNS sunucusu domainin IP adresini bulur
Tarayıcı bu IP adresine bağlanır
Bu sayede kullanıcılar karmaşık IP adreslerini ezberlemek zorunda kalmaz.

TCP (Transmission Control Protocol)
TCP güvenilir veri iletimi sağlayan bir protokoldür. Verilerin kaybolmadan ve doğru sırayla iletilmesini sağlar.

TCP bağlantısı kurulurken üç aşamalı bir süreç gerçekleşir:

Client → SYN
Server → SYN-ACK
Client → ACK

Bu işlem tamamlandıktan sonra veri iletimi başlar.

TCP genellikle şu alanlarda kullanılır:

Web siteleri
Dosya transferi
E-posta sistemleri
SSH bağlantıları
UDP (User Datagram Protocol)
UDP TCP'ye göre daha hızlı fakat daha az güvenilir bir protokoldür. Bağlantı kurmadan veri gönderir ve paketlerin ulaşıp ulaşmadığını kontrol etmez.

UDP genellikle şu sistemlerde kullanılır:

Online oyunlar
Video streaming
Sesli iletişim uygulamaları
Bu sistemlerde hız güvenilirlikten daha önemlidir.

Packet Structure
İnternet üzerinden gönderilen veriler paketlere bölünür. Bu paketler ağ üzerinden gönderilir ve hedefte tekrar birleştirilir.

Bir veri paketi genellikle şu bölümlerden oluşur:

Header
Payload
Header kısmında ağ bilgileri bulunur (IP adresi, port vb.). Payload kısmı ise gönderilen asıl veridir.

Network Tools
Ping
Ping komutu bir sunucuya erişim olup olmadığını kontrol etmek için kullanılır.

Örnek:

ping google.com

Traceroute
Traceroute veri paketinin hedefe ulaşana kadar geçtiği ağ cihazlarını gösterir.

Örnek:

traceroute google.com

Nslookup
Nslookup bir domain adresinin IP adresini öğrenmek için kullanılır.

Örnek:

nslookup google.com

Conclusion
Networking temelleri internet üzerinden çalışan yazılımları anlamak için önemlidir. IP adresleri cihazların kimliğini belirler, portlar farklı servisleri ayırır ve DNS sistemi domain isimlerini IP adreslerine çevirir. TCP ve UDP protokolleri veri iletimini sağlar. Ping, traceroute ve nslookup gibi araçlar ise ağ bağlantılarını analiz etmek için kullanılır.