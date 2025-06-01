# 📚 Kitap Bilgi Sistemi - Linked Data Uygulaması

## Proje Açıklaması
Bu proje, **Semantik Bilgi Yönetimi** dersi kapsamında geliştirilmiş bir linked data uygulamasıdır. Google Books API kullanarak kitap verilerini JSON-LD formatında sunan bir web uygulaması.

## 🎯 Proje Hedefleri
- Postman API Platform kullanımı
- Linked Data (JSON-LD) formatında veri sunumu
- Real-time API entegrasyonu
- Semantic web standartlarına uygun knowledge graph oluşturma

## 🛠️ Kullanılan Teknolojiler
- **Postman API Platform** - API test ve dokümantasyon
- **Google Books API** - Kitap verisi kaynağı
- **JSON-LD** - Linked data formatı
- **HTML/CSS/JavaScript** - Frontend
- **Schema.org** - Semantic markup

## 📁 Dosya Yapısı
```
├── index.html                              # Ana web uygulaması
├── Kitap-Bilgi-Sistemi.postman_collection.json  # Postman collection
└── README.md                               # Bu dosya
```

## 🚀 Kurulum ve Kullanım

### 1. Web Uygulaması
- `index.html` dosyasını tarayıcıda açın
- Kitap adı veya yazar adı girin
- "Ara" butonuna tıklayın
- Sonuçlarda JSON-LD formatını görmek için "Linked Data" kısmını açın

### 2. Postman Collection
- `Kitap-Bilgi-Sistemi.postman_collection.json` dosyasını Postman'a import edin
- Collection içindeki istekleri çalıştırın
- Tests sekmesinde linked data dönüşümü kodunu inceleyin

## 📊 Linked Data Formatı

Uygulama, kitap verilerini şu JSON-LD yapısında sunar:

```json
{
  "@context": "https://schema.org/",
  "@type": "Book",
  "@id": "book:kitap-adi",
  "name": "Kitap Adı",
  "author": [
    {
      "@type": "Person",
      "name": "Yazar Adı"
    }
  ],
  "datePublished": "2023",
  "description": "Kitap açıklaması...",
  "genre": ["Kategori"],
  "publisher": "Yayınevi",
  "url": "Detay linki"
}
```

## 🔍 API Endpoints

### Google Books API
- **Base URL**: `https://www.googleapis.com/books/v1/volumes`
- **Arama**: `?q=python` (kitap adı)
- **Yazar Arama**: `?q=inauthor:martin`
- **Kategori Arama**: `?q=subject:programming`

## 📈 Özellikler

### ✅ Tamamlanan
- [x] Google Books API entegrasyonu
- [x] JSON-LD formatında veri dönüşümü
- [x] Web arayüzü
- [x] Real-time arama
- [x] Postman collection
- [x] Knowledge graph yapısı

### 🔄 Geliştirilebilir
- [ ] Birden fazla API entegrasyonu
- [ ] Görsel knowledge graph
- [ ] Veri filtreleme seçenekleri
- [ ] Favoriler sistemi

## 📚 Semantic Web Standartları

Bu uygulama şu standartları kullanır:
- **JSON-LD**: W3C linked data formatı
- **Schema.org**: Semantic markup vocabulary
- **RDF**: Resource Description Framework prensipleri

## 🎓 Eğitim Değeri

Bu proje şu konuları kapsar:
- API entegrasyonu ve test
- Linked data kavramları
- Semantic web teknolojileri
- JSON-LD formatı
- Knowledge graph yapıları

## 👨‍🎓 Geliştirici
- **Öğrenci**: Bilge Hari Kayalak
- **Ders**: Semantik Bilgi Yönetimi
- **Program**: Bilgi ve Belge Yönetimi
- **Tarih**: Haziran 2025

## 📄 Lisans
Bu proje eğitim amaçlı geliştirilmiştir.

---
**Not**: Bu uygulama Postman API Platform kullanılarak geliştirilmiş linked data uygulamasıdır.
