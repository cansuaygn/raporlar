 Concurrency & Parallel Programming

Bu bölümde yazılımlarda aynı anda birden fazla işlemin nasıl çalıştığını öğrenmeye başladım. Concurrency ve parallelism kavramlarının benzer görünse de farklı şeyler olduğunu gördüm. Concurrency’nin birden fazla işi yönetmekle ilgili olduğunu, parallelism’in ise işlemleri gerçekten aynı anda çalıştırdığını öğrendim.

Thread mantığını ve işlemlerin arka planda nasıl yürüdüğünü araştırdım. Özellikle çok çekirdekli işlemcilerde performans artışının nasıl sağlandığını anlamaya çalıştım.

Aynı anda çalışan işlemlerin ortak verilere erişirken sorun oluşturabildiğini öğrendim ve bu noktada race condition kavramını inceledim. Bu tarz problemleri önlemek için kullanılan mutex, semaphore ve lock yapılarının temel çalışma mantığını öğrendim.

Bu süreçte thread-safe kod yazımının neden önemli olduğunu, eşzamanlı çalışan sistemlerde hata ayıklamanın neden zorlaştığını ve performans ile güvenlik arasında nasıl denge kurulduğunu daha iyi anlamaya başladım.

Bu bölüm sayesinde çok çekirdekli sistemlerde çalışan daha güvenli, daha stabil ve daha performanslı yazılımlar geliştirme konusunda temel seviye bilgi kazandım.
git commit -m "add concurrency report"