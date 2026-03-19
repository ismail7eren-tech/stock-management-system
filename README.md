Stok ve Sipariş Yönetim Sistemi
Bu proje; işletmelerin ürün envanterlerini dijital ortamda takip etmeleri, dinamik stok güncellemeleri yapmaları ve satış/sipariş süreçlerini yönetmeleri için geliştirilmiş Flask tabanlı bir otomasyon sistemidir.

Sistem, sadece veri kaydetmekle kalmayıp, stok yetersizliği gibi durumlarda kullanıcıyı uyaran bir iş mantığına (Business Logic) sahiptir.

🚀 Öne Çıkan Özellikler
📊 Dinamik Envanter Takibi
Sistemdeki tüm ürünler, mevcut stok miktarlarıyla birlikte listelenir. Stok miktarı 5 adetin altına düşen ürünler için sistem otomatik olarak "Kritik Stok" uyarısı vererek tedarik sürecini hatırlatır.

🛡️ Akıllı Sipariş ve Stok Kontrolü
Yetersiz Stok Engelleme: Bir kullanıcı, mevcut stoktan daha fazla sipariş girmeye çalıştığında sistem işlemi reddeder.

Flash Mesaj Desteği: Hatalı işlemlerde (yetersiz stok vb.) kırmızı uyarı, başarılı işlemlerde ise yeşil onay kutuları ile kullanıcı anlık olarak bilgilendirilir.

Otomatik Senkronizasyon: Sipariş onaylandığı anda ilgili ürünün stoğu otomatik olarak düşürülür ve sipariş geçmişine kaydedilir.

📜 İşlem Geçmişi
Verilen tüm siparişler; ürün adı, miktar ve işlem tarihi bilgileriyle birlikte kronolojik olarak listelenir.

🛠️ Teknik Altyapı
Bu proje, ölçeklenebilir ve hafif bir mimari üzerine inşa edilmiştir:

Backend: Python ve Flask framework'ü kullanılarak tüm rota ve veritabanı kontrolleri sağlanmıştır.

Veritabanı: İlişkisel veri yapısı için SQLite3 kullanılmıştır. urunler ve siparisler tabloları birbirine bağlı mantıkla çalışır.

Frontend: Kullanıcı arayüzü modern HTML5 ve CSS3 ile tasarlanmış, veriler Jinja2 şablon motoru ile dinamik olarak işlenmiştir.

Çalıştırma Komutu
py app.py
