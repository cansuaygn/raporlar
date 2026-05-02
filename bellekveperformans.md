### 11) Bellek ve Performans Derinliği

**Stack vs Heap Farkı**

Program çalışırken veriler iki farklı yerde tutuluyor: Stack ve Heap.

- **Stack** → Daha hızlı çalışır. Küçük ve geçici veriler burada tutulur. (örneğin fonksiyon içindeki değişkenler)
- **Heap** → Daha büyük ve uzun ömürlü veriler burada tutulur. (örneğin nesneler)

Stack otomatik yönetilir, yanİ müdahale etmeyiz. 

Benim anladığım:
Stack hızlı ama sınırlı, heap esnek ama kontrol edilmesi gerekiyor.

---

Garbage Collection (GC) Nasıl Çalışır?

Garbage Collection, kullanılmayan verileri bellekten temizleyen sistemdir.

Örneğin:
Bir değişken oluşturduk ama artık hiçbir yerde kullanılmıyor → GC bunu fark eder ve siler.

Ama burada kritik nokta şu:
GC sürekli çalışmaz. Belirli zamanlarda devreye girer.

Bu da şuna sebep olabilir:
-Anlık performans düşüşleri (çünkü temizlik yapıyor)
-Gereksiz veri birikimi (GC çalışana kadar)

Yani aslında GC hayat kurtarıyor ama doğru kullanmazsan performansı etkileyebiliyor.

---

Memory Leak Nedir? Nasıl Oluşur?

Memory leak, kullanılmayan verilerin bellekten temizlenmemesi durumudur.

Yani:
Program o veriyi artık kullanmıyor ama bellek hâlâ dolu.

Bu genelde şu durumlarda olur:
-Gereksiz referanslar tutulursa
-Nesneler serbest bırakılmazsa
-Sonsuz döngü içinde veri birikirse

Sonuç:
-Program zamanla yavaşlar
-Bellek şişer
-Hatta çökme bile olabilir

Benim çıkarımım:
Bellek yönetimini doğru yapmazsan, kodun çalışsa bile sağlıklı çalışmaz.
