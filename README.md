# LearnIT - Bilişim ve Yazılım Akademisi

Bu proje, **Marmara Üniversitesi Bilgisayar ve Öğretim Teknolojileri Öğretmenliği (BÖTE)** 3. sınıf **İnternet Tabanlı Programlama** dersi kapsamında geliştirilen örnek bir eğitim ve dosya paylaşım web sitesi arayüzüdür.

Arayüz tamamen **saf HTML5 ve CSS3** ile hazırlanmış olup **JavaScript içermez**. Sayfalar ve formlar, ileride eklenecek **PHP backend** ve **veritabanı** yapısına kolayca bağlanabilecek şekilde ayrıştırılmıştır.

## Dosya Yapısı

```text
LearnIT/
├── index.html        # Ana sayfa: müfredat listesi, ders içeriği, soru-cevap ve yorumlar
├── login.html        # Kullanıcı giriş sayfası (öğrenci / eğitmen seçimi)
├── files.html        # Dosya yükleme, filtreleme ve listeleme sayfası
├── lesson-add.html   # Yeni ders / müfredat ekleme sayfası
├── style.css         # Tüm sayfalar için ortak koyu tema ve duyarlı (responsive) stiller
├── README.md         # Proje dokümantasyonu
└── LICENSE           # GNU General Public License v3.0 (GPLv3)
```

## Özellikler

- **Saf HTML + CSS Mimarisi:** Harici kütüphane veya JavaScript bağımlılığı yoktur; tüm stiller tek bir `style.css` dosyasında toplanmıştır.
- **Ayrıştırılmış Sayfalar:** Giriş (`login.html`), dosya paylaşımı (`files.html`), ders ekleme (`lesson-add.html`) ve ders görüntüleme (`index.html`) ayrı HTML sayfalarındadır.
- **PHP & Veritabanına Hazır Formlar:** Tüm formlarda uygun `method`, `name` ve dosya yükleme için `enctype="multipart/form-data"` nitelikleri tanımlıdır.
- **Duyarlı Tasarım:** Masaüstü ve mobil ekranlara uyumlu koyu tema arayüzü.

## Kurulum ve Çalıştırma

Herhangi bir derleme adımı gerektirmez:

1. Projeyi yerel sunucunuzun kök dizinine (ör. `/srv/http/LearnIT` veya `htdocs/LearnIT`) yerleştirin veya `index.html` dosyasını doğrudan tarayıcıda açın.
2. PHP ve veritabanı bağlantısı eklerken HTML dosyalarındaki `action=""` (örneğin `login.html` içinde geçici `action="index.html"`) ve `href="#"` alanlarını ilgili `.php` uç noktalarınıza yönlendirebilirsiniz.

## Lisans

Bu proje **GNU General Public License v3.0 (GPLv3)** ile lisanslanmıştır. Ayrıntılar için [LICENSE](LICENSE) dosyasına bakabilirsiniz.
