<p align="center">
  <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTFu1buZizYN8-s1SiqsMyp9Sa-r8OUBSZUSmHSXLTbDtuT9A5f2pSlbvQ&s=10" alt="Banner" width="100%" height="180"/>
</p>

# 🚀 Softito Backend Developer Eğitimi — Proje Portföyü

Bu depo, **Softito Backend Developer Eğitimi** kapsamında geliştirdiğim 9 projeyi bir araya getirir. Her proje **.NET & ASP.NET Core** ekosisteminde farklı mimari yaklaşımlar (N-Katmanlı, Monolitik, Client-Server), farklı veritabanı stratejileri (Code First / DB First) ve farklı veri erişim teknolojileri (EF Core, Dapper, ADO.NET) denenerek hazırlanmıştır.

---

## 🧰 Teknoloji Yelpazesi

`.NET 8 / 10` · `ASP.NET Core MVC` · `Razor Pages` · `Web API` · `Entity Framework Core` · `Dapper` · `ADO.NET` · `SQL Server` · `ASP.NET Core Identity` · `EPPlus` · `QuestPDF` · `Serilog` · `Bootstrap 5` · `jQuery / AJAX` · `Chart.js`

---

## 📂 Projeler

### 1️⃣ 🏋️ Fitness Management System
**Spor salonlarının üye, antrenör, şube ve supplement envanter süreçlerini dijitalleştiren tam kapsamlı yönetim sistemi.**

🔗 [github.com/yusufcengiz00/FitnessManagement-MVC-CodeFirst](https://github.com/yusufcengiz00/FitnessManagement-MVC-CodeFirst)

Sistem, kullanıcıların karşılandığı modern bir tanıtım arayüzü ile veri yönetiminin yapıldığı premium koyu mod admin panelini bir araya getirir. Model katmanındaki C# sınıfları (Üye, Antrenör, Salon, Supplement) EF Core aracılığıyla ilişkisel SQL Server tablolarına dönüştürülür; Controller katmanı arama filtreleri ve CRUD isteklerini karşılayarak iş mantığını yürütür.

- 🏗️ **Mimari:** ASP.NET Core MVC (Monolitik) · Dependency Injection ile bağımlılık yönetimi
- 🗄️ **Veritabanı:** Code First — C# modelleri üzerinden migration tabanlı şema yönetimi, SQL scriptsiz taşınabilirlik
- 📊 **Raporlama:** QuestPDF ile tek tıkla PDF, EPPlus ile bellek üzerinde (in-memory) dinamik Excel üretimi
- 📈 **Analitik Panel:** Yaş ortalamaları, şube bazlı üye dağılımı, antrenör-üye eşleşme metrikleri
- 🔗 **İlişkisel Yapı:** Üye→Şube, Antrenör→Üye, Supplement→Şube arasında One-to-Many ilişkiler
- 🔍 **Sunucu Taraflı Arama:** Büyük veri kümelerinde performansı koruyan veritabanı düzeyinde filtreleme
- 🌙 **Tasarım:** Bootstrap 5.3 + CSS grid/flexbox, Inter & Bebas Neue tipografisi, glassmorphism ve mikro animasyonlu koyu tema

---

### 2️⃣ 🚗 Araç Kiralama ve Takip Sistemi
**Kiralama süreçlerinin operasyonel ve finansal takibini yapan web tabanlı yönetim sistemi.**

🔗 [github.com/yusufcengiz00/AracKiralama-MVC-DBFirst](https://github.com/yusufcengiz00/AracKiralama-MVC-DBFirst)

Araç envanteri, müşteri kayıtları, kiralama sözleşmeleri ve ödemelerin uçtan uca CRUD işlemlerini kolaylaştırır. SQL Server bağlantısı `appsettings.json` üzerinden EF Core ile sağlanır; Controller sınıfları LINQ sorgularının sonuçlarını güçlü tipli modeller ya da ViewBag aracılığıyla Razor görünümlerine taşır.

- 🏗️ **Mimari:** ASP.NET Core MVC (Monolitik) · Dependency Injection
- 🗄️ **Veritabanı:** Database First — mevcut SQL Server şeması temel alınarak EF Core model sınıfları türetilmiştir
- 📈 **Grafik Entegrasyonu:** Chart.js ile son ödeme hareketlerinin kronolojik, interaktif çizgi grafiği
- 📊 **Raporlama:** QuestPDF ile finansal tabloların şablonlu PDF çıktısı, EPPlus ile otomatik genişlik ayarlı Excel export
- 🎯 **Yönetici Paneli:** Canlı performans grafikleriyle desteklenen dinamik istatistik ekranı
- 🎨 **Tasarım:** Bootstrap 5, FontAwesome, Google Fonts (Inter & Outfit) ile responsive, koyu tema destekli premium arayüz

---

### 3️⃣ 🎓 CourseManager
**Eğitim kurumlarının kurs, öğrenci ve sertifika verilerini merkezi olarak yönettiği otomasyon uygulaması.**

🔗 [github.com/yusufcengiz00/CourseManager-RazorPages](https://github.com/yusufcengiz00/CourseManager-RazorPages)

Ziyaretçiler için `/` üzerinden akademinin vizyonu ve aktif kursların salt okunur şekilde listelendiği bir tanıtım portalı; yetkililer için `/Admin/Index` altında öğrenci, kurs ve sertifika CRUD işlemlerinin yürütüldüğü bir kontrol paneli sunar. Veritabanı işlemleri harici bir ORM kullanılmadan doğrudan `SqlConnection` / `SqlCommand` ve parametrik SQL sorgularıyla gerçekleştirilir.

- 🏗️ **Mimari:** ASP.NET Core Razor Pages — Page Model Pattern
- 🗄️ **Veritabanı:** Database First / Klasik SQL — **saf ADO.NET** (`System.Data.SqlClient`, `Microsoft.Data.SqlClient`), ORM katmanı yok
- ⚡ **Performans Odaklı:** Gereksiz katman ve paket yüklerinden kaçınan hafif (lightweight) mimari
- 📊 **Analitik Dashboard:** Toplam bütçe değeri, ortalama süreler gibi metriklerin gerçek zamanlı SQL sorgularıyla hesaplanması
- 📄 **Raporlama:** QuestPDF ile A4 düzeninde kurumsal PDF, EPPlus ile hücre biçimlendirmeli `.xlsx` çıktısı
- 🎨 **Tasarım:** Bootstrap 5 + Font Awesome 6, özel `modern.css` ile gradyan ve glassmorphism efektleri

---

### 4️⃣ 🎬 Movie Manager System
**Film kayıtlarını, kategorileri ve kullanıcı yorumu/puanlarını merkezi olarak yöneten sistem.**

🔗 [github.com/yusufcengiz00/MovieManagerSystem_MVC_NTier_](https://github.com/yusufcengiz00/MovieManagerSystem_MVC_NTier_)

Ziyaretçilerin film arayıp yorumları okuyabildiği salt okunur bir Kullanıcı Portalı ile yöneticilerin veri yönetimi ve raporlama yapabildiği bir Admin CRM Kontrol Paneli barındırır. Proje `MovieManagerSystem` (sunum), `MovieManagerSystem.Data` (veri erişim) ve `MovieManagerSystem.Model` (veri modeli) olmak üzere üç katmana ayrılmıştır; ilişkisel veriler `Include` ve `ToListAsync` gibi asenkron LINQ sorgularıyla çekilir.

- 🏗️ **Mimari:** N-Katmanlı (N-Tier) — Sunum / Veri Erişim / Veri Modeli katmanları ayrımı
- 🗄️ **Veritabanı:** Code First · EF Core `DbContext` ile asenkron erişim
- ⭐ **İstatistik Raporları:** Kategori puan ortalamaları (ilerleme çubuklu), format/teknoloji analizleri
- 📊 **Raporlama:** EPPlus ile bellek üzerinde Excel, QuestPDF ile PDF belge üretimi, HTTP yanıtı ile doğrudan indirme
- 🔎 **Kullanıcı Portalı:** Film arama, kategoriye göre filtreleme, yorum okuma
- 🎨 **Tasarım:** Mor-indigo gradyanlar, parlayan derecelendirme yıldızları, hover geçişleri, Inter/Outfit yazı tipleri, glassmorphism

---

### 5️⃣ 📦 StockFlow
**Depodaki ürün, tedarikçi ağı ve stok hareketlerini anlık izleyen depo otomasyon sistemi.**

🔗 [github.com/yusufcengiz00/StockFlow_WithJquery-MVC](https://github.com/yusufcengiz00/StockFlow_WithJquery-MVC)

Yönetici ve depo görevlileri için iki ayrı portal sunarak iş süreçlerini dijitalleştirir. Frontend'deki AJAX etkileşimlerini dinleyen ve JSON döndüren MVC Controller uçları; veritabanı işlemlerini `ApplicationDbContext` üzerinden EF Core ile yürütür. Bir stok hareketi eklendiğinde/güncellendiğinde/silindiğinde arka plan algoritmaları ilgili ürünün stok adedini otomatik günceller.

- 🏗️ **Mimari:** MVC (Monolitik)
- 🗄️ **Veritabanı:** Code First · EF Core Migration ile sürüm kontrollü şema
- ⚙️ **Asenkron CRUD & AJAX:** Sayfa yenilenmeden arka planda çalışan ürün, tedarikçi ve stok hareketi yönetimi
- 🔄 **Dinamik Stok Kontrolü:** Giriş/çıkış işlemlerine bağlı otomatik stok hesaplama ve yetersiz stok uyarıları
- 🔍 **Anlık jQuery Filtreleme:** Barkod, isim, firma adı veya şehre göre istemci taraflı arama ve sıralama
- 🎨 **Tasarım:** Slate koyu mod, yarı saydam kart bileşenleri (glassmorphic), Inter yazı tipi, akıcı hover animasyonları

---

### 6️⃣ 🍔 FoodOrder — Yemek Sipariş Yönetim Sistemi
**Restoran ve yemek servisleri için sipariş, ürün ve kullanıcı süreçlerinin merkezi yönetimi.**

🔗 [github.com/yusufcengiz00/FoodOrderManagementSystem](https://github.com/yusufcengiz00/FoodOrderManagementSystem)

Yetkili personelin sipariş oluşturup yönettiği güvenli bir admin dashboard ile son kullanıcıların güncel menüyü inceleyebildiği salt okunur bir yemek portalı sunar. Veritabanı sorguları doğrudan performans odaklı Stored Procedure'ler üzerinden Dapper mikro-ORM'i ile asenkron tetiklenir; oturum bilgileri sunucu tarafında saklanır ve `BaseController` aracılığıyla yetkisiz erişimler engellenir.

- 🏗️ **Mimari:** ASP.NET Core MVC (Monolitik) · Stored Procedure Tabanlı Veri Erişimi (Dapper Context Wrapper) · Action Filter tabanlı `BaseController` koruması
- 🗄️ **Veritabanı:** Database First — ilişkisel tablolar (Users, Products, Orders, OrderDetails) ve stored procedure'ler SQL betiğiyle önceden tasarlandı
- ⚡ **Dapper Entegrasyonu:** EF Core gibi ağır ORM'ler yerine yüksek performanslı mikro-ORM tercihi
- 🔐 **Session-Based Authentication:** Kullanıcı girişi gerektiren sayfaların ActionFilter ile korunması
- 📊 **Dinamik Dashboard:** Toplam ciro, aktif sipariş sayısı, kayıtlı kullanıcı/ürün sayısı gibi anlık metrikler
- 🧾 **Raporlama:** İstemci taraflı `html2pdf.js` ile doğrudan PDF indirme, UTF-8 BOM kodlamalı Türkçe karakter uyumlu CSV/Excel çıktısı

---

### 7️⃣ 💻 CodeVault System
**Geliştirici (Developer) ve yönetici (Admin) portallarını barındıran rol tabanlı kod ve iş yönetim portalı.**

🔗 [github.com/yusufcengiz00/CodeVaultSystem](https://github.com/yusufcengiz00/CodeVaultSystem)

Geliştiricilerin kendi görev ve yorumlarını yönetebildiği, yöneticilerin ise projeleri, teknolojileri ve geliştiricileri dinamik raporlarla takip edebildiği çift katmanlı bir sistemdir. **CodeVaultAPI** çekirdek iş mantığını ve `CodeVaultSystemDB` veritabanını yönetirken, **CodeVaultMVC** kullanıcı arayüzünü ve `CodeVaultSystem_MVC_DB` üzerinden Identity tabanlı kimlik doğrulamayı üstlenir; iki katman arasındaki haberleşme `HttpClient` ile asenkron REST istekleri üzerinden yürütülür.

- 🏗️ **Mimari:** Client-Server — bağımsız Web API + MVC katmanları, REST üzerinden haberleşme
- 🗄️ **Veritabanı:** Code First · EF Core Migrations, **çift veritabanlı** yapı (API + Identity)
- 🔐 **Role-Based Authorization:** Admin ve Developer rolleri için ayrı yetkilendirme kuralları
- 🌱 **Otomatik Seeding:** Uygulama her başladığında önceden tanımlı admin hesabının oluşturulması/parola güncellemesi
- 🔗 **Otomatik Profil Eşleşmesi:** Yeni kayıt olan geliştiricilerin API profilleriyle e-posta üzerinden otomatik eşleşmesi
- 📊 **Raporlama:** EPPlus ile çoklu sekme destekli Excel, QuestPDF ile A4 kurumsal PDF
- 🎨 **Tasarım:** Neon glow efektleri, yüksek kontrastlı form alanları, tamamen responsive koyu tema

---

### 8️⃣ 🛒 ShopZone
**Admin paneli ile müşteri mağazasını ayrı arayüzlerde sunan modern e-ticaret uygulaması.**

🔗 [github.com/yusufcengiz00/ShopZone](https://github.com/yusufcengiz00/ShopZone)

MVC ön yüz katmanı, veritabanı işlemlerini doğrudan gerçekleştirmek yerine Web API'deki REST uç noktalarına asenkron `HttpClient` servisleriyle istek gönderir. API katmanı, stored procedure'leri çalıştıran Dapper mikro-ORM'i ile SQL Server'a erişirken; dashboard'daki basit aggregate/sayım sorguları performans için doğrudan EF Core (`CountAsync`) ile MVC tarafında çekilir — bu hibrit yaklaşım hız ile geliştirme kolaylığını dengeler.

- 🏗️ **Mimari:** Hibrit çift katman — ASP.NET Core Web API (backend) + ASP.NET Core MVC (frontend)
- 🗄️ **Veritabanı:** Database First — şema ve stored procedure'ler `ShopZoneDB_Setup.sql` kurulum scripti ile oluşturuldu
- 🧩 **Repository Pattern:** API katmanında veri erişiminin soyutlanması
- 🛡️ **Stored Procedure Entegrasyonu:** SQL enjeksiyonuna karşı korumalı, veritabanı seviyesinde optimize sorgular
- 🛒 **Session Tabanlı Sepet:** Kullanıcı oturumu boyunca sepet verisinin sunucu tarafında güvenli saklanması
- 📊 **Raporlama:** QuestPDF ve EPPlus ile sipariş/ürün/kullanıcı listelerinin PDF ve Excel dışa aktarımı
- ⚖️ **Hibrit Veri Yönetimi:** Dashboard'da EF Core, CRUD operasyonlarında Dapper/SQL Server kullanımı

---

### 9️⃣ 🌱 EcoSphere
**Kurumların karbon ayak izi, kaynak tüketimi ve atıklarını izleyen; sürdürülebilirlik hedefleri belirleyip sertifika/denetim süreçlerini yöneten kurumsal portal.**

🔗 [github.com/yusufcengiz00/EcoSphere](https://github.com/yusufcengiz00/EcoSphere)

Çalışanların veri girişi yaptığı, yöneticilerin bu verileri denetleyip raporladığı bir koordinasyon sistemidir. `EcoSphere.Core`, `EcoSphere.Data` ve `EcoSphere.MVC` katmanlarına ayrılmış N-Katmanlı mimari, fiziki yetki ayrımı için Areas yapısını (Admin / User) kullanır. Yazma işlemleri generic repository yerine `IUnitOfWork` üzerinden yönetilir ve `CompleteAsync()` ile veritabanına toplu olarak yansıtılır.

- 🏗️ **Mimari:** N-Katmanlı (Core / Data / MVC) + Areas ile rol bazlı fiziki ayrım
- 🗄️ **Veritabanı:** Code First — Migrations ile seed verili, sıfırdan otomatik kurulum
- 🧩 **Tasarım Desenleri:** Generic Repository + Entity-Specific Repository + **Unit of Work** (tek transaction sınırında toplu yazma)
- 🍪 **Çerezsiz Oturum Yönetimi:** Sunucuda statik `CurrentSession` yapısı, istemcide localStorage tabanlı oturum yardımcıları
- 📁 **Dosya Saklama:** GUID ile benzersizleştirilmiş atık fişleri ve sertifikaların `wwwroot/uploads` altında saklanması, yolların veritabanına kaydı
- 🖼️ **Görsel Önizleme:** JavaScript tabanlı global modal ile dinamik görsel önizleme, yükleme ve silme
- 🔐 **Çerezsiz "Beni Hatırla" & Şifre Sıfırlama:** localStorage tabanlı hatırlama, veritabanı doğrulamalı güvenli şifre güncelleme
- 📝 **Structured Logging:** Serilog ile oturum açma, şifre sıfırlama, veri ekleme/silme gibi kritik hareketlerin konsola ve log dosyasına kaydı
- 📊 **Raporlama:** EPPlus ile Excel, QuestPDF ile şık tasarımlı kurumsal sürdürülebilirlik PDF raporları
- 🎨 **Tasarım:** Vanilla CSS + Frosted Glassmorphism efektli Razor şablonları, sol sidebar'lı admin ekranı ve üst navbar'lı responsive kullanıcı portalı

---

## 🧭 Proje Karşılaştırma Tablosu

| # | Proje | Mimari | Veritabanı Yaklaşımı | Veri Erişimi | Öne Çıkan |
|---|-------|--------|----------------------|--------------|-----------|
| 1 | Fitness Management | MVC Monolitik | Code First | EF Core | Analitik raporlama |
| 2 | Araç Kiralama | MVC Monolitik | DB First | EF Core | Chart.js grafikleri |
| 3 | CourseManager | Razor Pages | DB First | ADO.NET | ORM'siz, saf SQL |
| 4 | Movie Manager | N-Katmanlı | Code First | EF Core | Async LINQ |
| 5 | StockFlow | MVC Monolitik | Code First | EF Core | jQuery/AJAX |
| 6 | FoodOrder | MVC Monolitik | DB First | Dapper | Stored Procedure |
| 7 | CodeVault | Client-Server | Code First | EF Core | Identity + REST API |
| 8 | ShopZone | Hibrit API+MVC | DB First | Dapper + EF Core | Stored Procedure + Hibrit |
| 9 | EcoSphere | N-Katmanlı + Areas | Code First | EF Core | Unit of Work + Serilog |

---

## 👤 Geliştirici

**Yusuf Cengiz**

🔗 [github.com/yusufcengiz00](https://github.com/yusufcengiz00)
