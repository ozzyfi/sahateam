# saha.team — Landing Page

Saha ekibinizin WhatsApp hafızası. Statik landing page.

## Yapı

Tek dosya statik site — tüm CSS, HTML ve JS tek bir `index.html`'de inline.

```
/
├── index.html        # Sayfanın tamamı
├── og-image.png      # Open Graph / Twitter Card görseli (1200×630)
├── robots.txt        # Crawl yönergeleri
└── sitemap.xml       # Site haritası
```

## Yerel geliştirme

```bash
# Sadece statik dosyaları serve et
python3 -m http.server 8000
# veya
npx serve .
```

Tarayıcıda `http://localhost:8000`.

## Deploy

Bu repo **Cloudflare Pages** üzerinden host edilir. Her `git push` otomatik deploy tetikler.

`main` branch → production
Diğer branch'ler → preview URL

## SEO & Erişilebilirlik

- Open Graph + Twitter Card meta
- Schema.org-friendly HTML
- ARIA labels, focus trap, skip link
- `aria-describedby` ile form hata mesajları
- `prefers-reduced-motion` desteği
- Klavye navigasyonu (drawer + modal)

## İletişim

- Email: hi@saha.team
- WhatsApp: [WhatsApp Business](https://api.whatsapp.com/send/?phone=358415773392)
