# Kübra Aydın — İç Mimarlık

Kurumsal (B2B) müşterilere yönelik iç mimarlık ve proje yönetimi hizmetlerini tanıtan, çift dilli (Türkçe/İngilizce) statik web sitesi.

## Yapı

```
index.html         Tüm sayfa içeriği (tek sayfa, bölüm bazlı)
css/style.css       Tasarım sistemi
js/translations.js  TR/EN metin sözlüğü
js/main.js          Dil değişimi, mobil menü, scroll animasyonları, iletişim formu
images/             Görseller (favicon, portre fotoğrafı)
```

Derleme adımı gerekmez — düz HTML/CSS/JS. `index.html` dosyasını bir tarayıcıda açmak ya da herhangi bir statik dosya sunucusundan servis etmek yeterlidir, örn:

```
npx serve .
```

## İçerik güncelleme

- Metinler: `js/translations.js` içindeki `tr` ve `en` nesnelerinde anahtar/değer olarak tutulur.
- Portfolyo bölümü şu an soyut çizim (placeholder) ile hazırlanmıştır — gerçek proje fotoğrafları geldiğinde `index.html` içindeki `.portfolio-art` alanlarındaki SVG'ler görsellerle değiştirilebilir.
- İletişim bölümünde form yok; e-posta adresi doğrudan `mailto:` bağlantısı olarak sunulur. İleride bir form eklenmek istenirse Formspree/Web3Forms gibi backend gerektirmeyen bir servisle bağlanabilir.

## Yayınlama

Site statik olduğundan GitHub Pages, Netlify veya benzeri herhangi bir statik hosting ile doğrudan yayınlanabilir (build adımı yok).
