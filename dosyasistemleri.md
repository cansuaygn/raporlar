# Dosya Sistemleri ve Depolama Mantığı

Bilgisayarda veriler disk üzerinde saklanır. Fakat bu verilerin nasıl düzenleneceğini ve nasıl okunacağını belirleyen bir yapı gerekir. Bu yapıya dosya sistemi denir.

Dosya sistemi, işletim sistemi ile depolama aygıtı arasında çalışır ve dosyaların diskte nasıl tutulacağını belirler.

---

## Dosya Sistemi Nedir?

Dosya sistemi, depolama aygıtındaki verilerin organize edilmesini sağlar.

Bilgisayarda bulunan:

- belgeler
- fotoğraflar
- videolar
- program dosyaları

hepsi dosya sistemi sayesinde düzenli şekilde saklanır.

Dosya sistemi olmadan işletim sistemi diskteki verileri anlayamaz.

---

## NTFS – ext4 – APFS

Farklı işletim sistemleri farklı dosya sistemleri kullanır.

NTFS genellikle Windows işletim sistemlerinde kullanılır. Büyük dosyaları destekler ve dosya izinleri gibi gelişmiş özellikler sunar.

ext4 Linux sistemlerinde kullanılan yaygın bir dosya sistemidir. Hızlı ve kararlı olması nedeniyle birçok Linux dağıtımında tercih edilir.

APFS ise Apple tarafından geliştirilen bir dosya sistemidir ve macOS işletim sistemlerinde kullanılır. Özellikle SSD diskler için optimize edilmiştir.

---

## Blok Yapısı Nedir?

Depolama sistemlerinde veriler küçük parçalara bölünerek saklanır. Bu parçalara blok denir.

Bir dosya diskte tek parça olarak bulunmaz. Bunun yerine birden fazla blok halinde saklanır.

Örnek olarak bir dosya şu şekilde tutulabilir:

Dosya = Blok1 + Blok2 + Blok3

Bu bloklar diskte farklı yerlerde bulunabilir. Dosya sistemi bu blokların yerini takip eder ve dosya okunurken bu blokları tekrar bir araya getirir.

---

## HDD Nasıl Çalışır?

HDD (Hard Disk Drive) mekanik bir depolama cihazıdır.

İçinde dönen manyetik diskler bulunur. Bu disklerin üzerinde veriler manyetik olarak saklanır.

Disk dönerken bir okuma yazma kafası diskin üzerine hareket eder ve verileri okur veya yazar.

Bu nedenle HDD'ler mekanik yapıya sahiptir ve SSD'lere göre daha yavaştır.

HDD'nin avantajı büyük kapasite sunması ve genellikle daha ucuz olmasıdır.

---

## SSD Nasıl Çalışır?

SSD (Solid State Drive) mekanik parça içermez.

Veriler flash bellek hücrelerinde saklanır ve elektronik olarak okunur veya yazılır.

Mekanik hareket olmadığı için SSD'ler çok daha hızlıdır.

SSD'nin avantajları:

- daha hızlı veri okuma ve yazma
- sessiz çalışma
- darbelere karşı daha dayanıklı olması

Dezavantajı ise genellikle HDD'ye göre daha pahalı olmasıdır.

---

## Sonuç

Dosya sistemleri ve depolama teknolojileri bilgisayar performansında önemli rol oynar.

NTFS, ext4 ve APFS farklı işletim sistemlerinde kullanılan dosya sistemleridir.

Veriler disk üzerinde bloklar halinde saklanır ve dosya sistemi bu blokların yerini yönetir.

HDD mekanik bir depolama cihazıdır ve daha yavaştır. SSD ise elektronik depolama kullandığı için daha hızlı veri erişimi sağlar.

Bu konuları anlamak, veri okuma ve yazma hızlarının neden farklı olduğunu anlamaya yardımcı olur.