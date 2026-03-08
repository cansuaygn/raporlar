Linux Temelleri

Linux birçok sunucu sisteminde ve yazılım altyapısında kullanılan açık kaynaklı bir işletim sistemidir. Yazılımcıların büyük bir kısmı Linux tabanlı sistemlerle çalışır. Bu nedenle terminal kullanımı, paket yönetimi, dosya izinleri ve servis yönetimi gibi konuları bilmek önemlidir.

Terminal Nedir?

Linux sistemlerinde birçok işlem terminal üzerinden yapılır. Terminal, işletim sistemi ile doğrudan komut yazarak iletişim kurmamızı sağlar.

Terminal sayesinde dosya ve klasörleri görüntüleyebilir, klasör değiştirebilir, yeni klasör oluşturabilir, dosyalar içinde arama yapabilir ve sistemde çalışan işlemleri inceleyebiliriz.

Temel Terminal Komutları

ls

ls komutu bulunduğumuz klasördeki dosyaları ve klasörleri listelemek için kullanılır.

Örnek kullanım:

ls

Daha detaylı liste görmek için:

ls -l

cd

cd komutu klasör değiştirmek için kullanılır.

Örnek:

cd Documents

Bir üst klasöre çıkmak için:

cd ..

mkdir

Yeni klasör oluşturmak için kullanılır.

Örnek:

mkdir proje

Bu komut "proje" adlı bir klasör oluşturur.

grep

grep komutu dosyalar içinde belirli bir kelimeyi aramak için kullanılır.

Örnek:

grep hata log.txt

Bu komut log.txt dosyasında "hata" kelimesini arar.

chmod

chmod komutu dosya izinlerini değiştirmek için kullanılır.

Örnek:

chmod 755 script.sh

Bu komut dosyanın çalıştırılabilir olmasını sağlar.

top

top komutu sistemde çalışan işlemleri ve CPU kullanımını gösterir.

top

Bu komut sayesinde işlemci kullanımı, RAM kullanımı ve çalışan programlar görülebilir.

Paket Yönetimi

Linux sistemlerinde programlar paket yöneticileri aracılığıyla kurulurlar. Farklı Linux dağıtımları farklı paket yöneticileri kullanır.

Ubuntu ve Debian tabanlı sistemlerde apt kullanılır.

Program kurmak için:

sudo apt install program_adi

Paket listesini güncellemek için:

sudo apt update

Arch Linux sistemlerinde pacman kullanılır.

sudo pacman -S program_adi

Fedora ve bazı RedHat tabanlı sistemlerde dnf kullanılır.

sudo dnf install program_adi

Dosya İzinleri

Linux sistemlerinde her dosyanın belirli erişim izinleri vardır.

Bu izinler üç farklı kullanıcı türü için belirlenir:

owner (dosya sahibi)
group (grup)
others (diğer kullanıcılar)

Her kullanıcı için üç izin türü vardır:

read (okuma)
write (yazma)
execute (çalıştırma)

Linux'ta izinler şu şekilde gösterilebilir:

rwxr-xr-x

Bu ifade dosyanın kimler tarafından okunabileceğini, yazılabileceğini veya çalıştırılabileceğini gösterir.

İzinleri değiştirmek için chmod komutu kullanılır.

Servisler (systemctl)

Linux sistemlerinde bazı programlar arka planda sürekli çalışan servislerdir. Örneğin web sunucuları, veritabanı servisleri veya ağ servisleri.

Servisleri yönetmek için systemctl komutu kullanılır.

Bir servisi başlatmak:

sudo systemctl start servis_adi

Bir servisi durdurmak:

sudo systemctl stop servis_adi

Servisin durumunu görmek:

sudo systemctl status servis_adi