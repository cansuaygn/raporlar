İşletim Sistemi Temelleri (Operating System Basics)

İşletim sistemi, bilgisayar donanımı ile kullanıcı veya uygulamalar arasında çalışan temel yazılımdır. Bilgisayardaki işlemci, bellek, disk gibi kaynakları yönetir ve programların bu kaynakları düzgün şekilde kullanmasını sağlar.

Bir işletim sistemi sayesinde aynı anda birden fazla program çalıştırabilir, dosyalarımızı yönetebilir ve donanımlarla iletişim kurabiliriz.

Kernel Nedir?

Kernel, işletim sisteminin en önemli ve merkezi kısmıdır. Donanım ile yazılımlar arasındaki iletişimi sağlar.

Bilgisayarda çalışan uygulamalar donanıma doğrudan erişemez. Bunun yerine kernel üzerinden işlem yaparlar.

Kernel'in başlıca görevleri:

işlemci yönetimi

bellek yönetimi

dosya sistemi yönetimi

cihaz sürücülerinin kontrolü

Örneğin bir program dosya okumak istediğinde, bu isteği kernel'e gönderir. Kernel de diske erişerek veriyi programa iletir.

Process (Süreç) Nedir?

Process, çalışmakta olan bir programdır.

Bir program çalıştırıldığında işletim sistemi o program için bir süreç oluşturur. Bu süreç, programın çalışması için gerekli olan kaynakları içerir.

Bir process içinde şu bilgiler bulunur:

program kodu

kullanılan bellek

işlemci durumu

açık dosyalar

Örneğin aynı programdan iki tane açarsak iki farklı süreç oluşur.

Thread (İş Parçacığı) Nedir?

Thread, bir süreç içinde çalışan daha küçük çalışma birimidir.

Bir process birden fazla thread içerebilir. Thread'ler aynı bellek alanını paylaşır ve aynı program içinde farklı görevleri yerine getirebilir.

Örneğin bir web tarayıcısında:

bir thread sayfayı yükleyebilir

başka bir thread video oynatabilir

başka bir thread kullanıcı etkileşimlerini yönetebilir

Bu sayede programlar daha hızlı ve verimli çalışabilir.

Process ve Thread Arasındaki Fark

Process ve thread kavramları birbirine benzer fakat farklıdır.

Process:

bağımsız çalışır

kendi bellek alanına sahiptir

daha fazla sistem kaynağı kullanır

Thread:

aynı process içinde çalışır

bellek alanını paylaşır

daha hafiftir ve daha hızlı oluşturulur

Modern uygulamalar genellikle performans için çoklu thread kullanır.

Bellek Yönetimi (Memory Management)

Bellek yönetimi, işletim sisteminin RAM kullanımını kontrol etmesidir.

Bir bilgisayarda aynı anda birden fazla program çalışabilir. Bu programların her biri RAM'de belirli bir alan kullanır.

İşletim sistemi şu görevleri yerine getirir:

her programa gerekli bellek alanını ayırmak

kullanılmayan belleği geri almak

programların birbirinin belleğine erişmesini engellemek

Bazı durumlarda RAM yetersiz kalabilir. Bu durumda işletim sistemi disk üzerinde geçici bellek alanı kullanabilir. Buna virtual memory (sanal bellek) denir.

CPU Zamanlayıcıları (CPU Scheduling)

Bilgisayarda aynı anda birden fazla program çalışıyor gibi görünse de işlemci aslında her seferinde sadece bir işlem çalıştırabilir.

İşletim sistemi, işlemciyi farklı süreçler arasında paylaştırır. Buna CPU scheduling denir.

CPU zamanlayıcısının amacı:

işlemciyi verimli kullanmak

programların adil şekilde çalışmasını sağlamak

sistem performansını artırmak

Bazı temel zamanlama yöntemleri şunlardır:

First Come First Served (FCFS)
En önce gelen işlem önce çalıştırılır.

Round Robin
Her sürece kısa bir işlem süresi verilir ve sırayla çalıştırılır.

Priority Scheduling
Önceliği yüksek olan süreçler önce çalıştırılır.