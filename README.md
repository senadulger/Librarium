# Librarium – Kütüphane Yönetim Sistemi

## 1. Proje Hakkında
Bu proje, "Java Programlama ve Veritabanı Yönetim Sistemleri" dersleri için final ödevi olarak geliştirilmiştir. Temel amaç; veritabanı yönetimi, kimlik doğrulama, yetkilendirme ve tam kapsamlı (full-stack) web geliştirme becerilerini **Java Spring Boot** ve modern web teknolojileri kullanarak pekiştirmektir.

## 2. Özellikler
*   **Kimlik Doğrulama & Yetkilendirme:** Güvenli giriş ve kayıt sistemi.
*   **Kullanıcı Rolleri:**
    *   **Standart Üye (User):** Kitap arayabilir, ödünç alabilir, geçmiş işlemlerini görüntüleyebilir ve profilini düzenleyebilir.
    *   **Yönetici (Admin):** Tüm kitapları, üyeleri, şubeleri ve ödünç işlemlerini yönetebilir. Gecikmiş kitapları takip edebilir.
*   **Katalog Yönetimi:** Kitap ekleme, güncelleme, silme ve kategori/yazar bazlı filtreleme.
*   **Stok Takibi:** Şube bazlı stok ve envanter yönetimi.
*   **Ödünç Sistemi:** Ödünç alma, iade etme ve otomatik ceza hesaplama.
*   **Dashboard:** Sistem istatistiklerinin görsel olarak sunulduğu yönetim paneli.

## 3. Teknoloji Yığını

| Kategori | Teknoloji | Açıklama |
| :--- | :--- | :--- |
| **Frontend** | HTML5 / CSS3 | Kullanıcı arayüzü yapısı ve stilizasyonu |
| | Vanilla JavaScript | Dinamik arayüz etkileşimleri ve API iletişimi |
| **Backend** | Java 17 | Ana programlama dili |
| | Spring Boot 3 | Backend framework ve bağımlılık yönetimi |
| | Spring Data JPA | Veritabanı erişimi ve ORM |
| **Veritabanı** | PostgreSQL | İlişkisel veritabanı yönetim sistemi |
| **Araçlar** | Maven | Proje ve bağımlılık yönetimi |
| | Lombok | Boilerplate kod azaltımı (Getter/Setter vb.) |

## 4. Proje Yapısı ve Mantığı
*   **MVC Mimarisi:** Backend tarafı Model-View-Controller desenine uygun olarak (Model, Repository, Service, Controller katmanları) tasarlanmıştır.
*   **Servis Katmanı:** İş mantığı (Business Logic) servis sınıflarında toplanarak modülerlik sağlanmıştır.
*   **RESTful API:** Frontend ve Backend haberleşmesi REST API prensiplerine uygun uç noktalar (endpoints) üzerinden sağlanır.

## 5. Proje Nasıl Çalıştırılır?

### Ön Gereksinimler
*   Java JDK 17 kurulu olmalı
*   PostgreSQL kurulu ve çalışıyor olmalı
*   Maven kurulu olmalı

### Kurulum

1.  **Depoyu Klonlayın:**
    ```bash
    git clone https://github.com/Irmakyil/library-management-system.git
    cd library-management-system
    ```

2.  **Veritabanı Ayarları:**
    `src/main/resources/application.properties` dosyasını kendi veritabanı bilgilerinizle güncelleyin:
    ```properties
    spring.datasource.url=jdbc:postgresql://localhost:5432/library_db
    spring.datasource.username=postgres
    spring.datasource.password=sifreniz
    ```

3.  **Uygulamayı Çalıştırın:**
    ```bash
    mvn spring-boot:run
    ```
    Uygulama varsayılan olarak `http://localhost:8080` adresinde çalışacaktır.

## 6. Proje Demo Videosu
Uygulamanın temel özelliklerini ve genel işleyişini görmek için aşağıdaki demo videosunu izleyebilirsiniz:

https://github.com/user-attachments/assets/29b9e86a-5ff0-4c78-8a89-daa0df11fa11

## 7. Proje Raporu
Teknik detaylar, diyagramlar (ER, Class vb.) ve ekran görüntülerini içeren detaylı inceleme için depodaki **Rapor.pdf** dosyasına göz atabilirsiniz.

## 8. Yazarlar

| Üye | LinkedIn |
| :--- | :--- |
| [Irmak Yılmaz](https://github.com/Irmakyil) | <a href="https://www.linkedin.com/in/yilmazirmak/" target="_blank">LinkedIn</a> |
| [Sena Nur Dülger](https://github.com/senadulger) | <a href="https://www.linkedin.com/in/senadulger/" target="_blank">LinkedIn</a> |
| [Zehra Gül Özdemir](https://github.com/zehrose) | <a href="https://www.linkedin.com/in/zehra-gul-ozdemir/" target="_blank">LinkedIn</a> |
