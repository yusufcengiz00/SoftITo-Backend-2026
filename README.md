# 🚀 Softito Backend Developer Eğitimi — Proje Portföyü

Bu depo, **Softito Backend Developer Eğitimi** kapsamında geliştirdiğim 9 projeyi bir araya getirir. Her proje **.NET & ASP.NET Core** ekosisteminde farklı mimari yaklaşımlar (N-Katmanlı, Monolitik, Client-Server), farklı veritabanı stratejileri (Code First / DB First) ve farklı veri erişim teknolojileri (EF Core, Dapper, ADO.NET) denenerek hazırlanmıştır.

---

## 🧰 Teknoloji Yelpazesi

`.NET 8 / 10` · `ASP.NET Core MVC` · `Razor Pages` · `Web API` · `Entity Framework Core` · `Dapper` · `ADO.NET` · `SQL Server` · `ASP.NET Core Identity` · `EPPlus` · `QuestPDF` · `Serilog` · `Bootstrap 5` · `jQuery / AJAX` · `Chart.js`

---

## 📂 Projeler

### 1️⃣ 🏋️ Fitness Management System
**Spor salonu üye, antrenör, şube ve supplement yönetim sistemi.**
🔗 [github.com/yusufcengiz00/FitnessManagement-MVC-CodeFirst](https://github.com/yusufcengiz00/FitnessManagement-MVC-CodeFirst)

- 🏗️ Mimari: ASP.NET Core MVC (Monolitik)
- 🗄️ Veritabanı: Code First · EF Core
- 📊 Raporlama: QuestPDF & EPPlus
- 🌙 Premium koyu tema (dark mode) tasarım

---

### 2️⃣ 🚗 Araç Kiralama ve Takip Sistemi
**Araç, müşteri, sözleşme ve ödeme takibi yapan kiralama otomasyonu.**
🔗 [github.com/yusufcengiz00/AracKiralama-MVC-DBFirst](https://github.com/yusufcengiz00/AracKiralama-MVC-DBFirst)

- 🏗️ Mimari: ASP.NET Core MVC (Monolitik)
- 🗄️ Veritabanı: Database First · EF Core
- 📈 Chart.js ile canlı ödeme grafikleri
- 📊 Raporlama: QuestPDF & EPPlus

---

### 3️⃣ 🎓 CourseManager
**Kurs, öğrenci ve sertifika yönetimi için eğitim otomasyonu.**
🔗 [github.com/yusufcengiz00/CourseManager-RazorPages](https://github.com/yusufcengiz00/CourseManager-RazorPages)

- 🏗️ Mimari: ASP.NET Core Razor Pages
- 🗄️ Veritabanı: Database First · **Saf ADO.NET** (ORM'siz)
- ⚡ Maksimum sorgu performansı odaklı
- 📊 Raporlama: QuestPDF & EPPlus

---

### 4️⃣ 🎬 Movie Manager System
**Film, kategori ve kullanıcı yorumu/puan yönetim sistemi.**
🔗 [github.com/yusufcengiz00/MovieManagerSystem_MVC_NTier_](https://github.com/yusufcengiz00/MovieManagerSystem_MVC_NTier_)

- 🏗️ Mimari: N-Katmanlı (N-Tier)
- 🗄️ Veritabanı: Code First · EF Core (async)
- ⭐ Kategori puan ortalamaları ve istatistik raporları
- 🎨 Mor-indigo gradyanlı glassmorphism tasarım

---

### 5️⃣ 📦 StockFlow
**Depo, tedarikçi ve stok hareketi takip sistemi.**
🔗 [github.com/yusufcengiz00/StockFlow_WithJquery-MVC](https://github.com/yusufcengiz00/StockFlow_WithJquery-MVC)

- 🏗️ Mimari: ASP.NET Core MVC (Monolitik)
- 🗄️ Veritabanı: Code First · EF Core
- ⚙️ jQuery + AJAX ile anlık, sayfa yenilemesiz işlemler
- 🔄 Otomatik stok adedi güncelleme algoritması

---

### 6️⃣ 🍔 FoodOrder — Yemek Sipariş Yönetim Sistemi
**Restoran sipariş, ürün ve kullanıcı süreçleri yönetimi.**
🔗 [github.com/yusufcengiz00/FoodOrderManagementSystem](https://github.com/yusufcengiz00/FoodOrderManagementSystem)

- 🏗️ Mimari: ASP.NET Core MVC (Monolitik)
- 🗄️ Veritabanı: Database First · **Dapper** + Stored Procedure
- 🔐 Session tabanlı kimlik doğrulama (BaseController koruması)
- 🧾 Türkçe karakter uyumlu CSV/Excel & istemci taraflı PDF (html2pdf.js)

---

### 7️⃣ 💻 CodeVault System
**Rol tabanlı geliştirici & yönetici iş takip portalı.**
🔗 [github.com/yusufcengiz00/CodeVaultSystem](https://github.com/yusufcengiz00/CodeVaultSystem)

- 🏗️ Mimari: Client-Server (ayrı Web API + MVC, HttpClient ile REST haberleşme)
- 🗄️ Veritabanı: Code First · EF Core (çift veritabanı)
- 🔐 ASP.NET Core Identity ile rol tabanlı yetkilendirme
- 📊 Raporlama: QuestPDF & EPPlus (çoklu sekme Excel)

---

### 8️⃣ 🛒 ShopZone
**Admin paneli ve müşteri mağazasını ayıran e-ticaret platformu.**
🔗 [github.com/yusufcengiz00/ShopZone](https://github.com/yusufcengiz00/ShopZone)

- 🏗️ Mimari: Hibrit — Web API (backend) + MVC (frontend)
- 🗄️ Veritabanı: Database First · **Dapper** + EF Core hibrit kullanım
- 🛡️ Stored Procedure tabanlı, SQL enjeksiyonuna karşı korumalı veri erişimi
- 🛒 Session tabanlı sepet yönetimi

---

### 9️⃣ 🌱 EcoSphere
**Kurumsal karbon ayak izi, kaynak tüketimi ve sürdürülebilirlik yönetim portalı.**
🔗 [github.com/yusufcengiz00/EcoSphere](https://github.com/yusufcengiz00/EcoSphere)

- 🏗️ Mimari: N-Katmanlı + Areas (rol bazlı fiziki ayrım)
- 🗄️ Veritabanı: Code First · EF Core
- 🧩 Repository + **Unit of Work** tasarım deseni
- 🍪 Çerezsiz oturum yönetimi (static session + localStorage)
- 📝 Serilog ile yapılandırılmış loglama
- 📊 Raporlama: QuestPDF & EPPlus

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
