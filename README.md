# kucingops.github.io

Blog pribadi saya, dibuat dengan [Astro](https://astro.build) dan di-deploy otomatis ke GitHub Pages: **https://kucingops.github.io**

## Menulis post baru

1. Buat file baru di `src/content/blog/`, misalnya `belajar-kafka.md`. Nama file menjadi URL: `/blog/belajar-kafka/`.
2. Isi frontmatter di bagian atas:

   ```md
   ---
   title: 'Belajar Kafka dari nol'
   description: 'Ringkasan satu kalimat untuk daftar post dan SEO.'
   pubDate: 2026-11-21
   tags: ['kafka', 'backend']
   draft: false
   ---
   ```

3. Tulis isinya dalam Markdown (atau `.mdx` kalau butuh komponen).
4. Commit dan push ke `main`. GitHub Actions akan build dan deploy dalam 1-2 menit.

Post dengan `draft: true` hanya muncul saat `npm run dev`, tidak ikut dipublikasikan.

## Jalankan di komputer

```sh
npm install
npm run dev      # http://localhost:4321
npm run build    # hasil di dist/
```

## Fitur

- Halaman blog, tag, about, 404
- RSS (`/rss.xml`) dan sitemap otomatis
- Estimasi waktu baca, syntax highlighting
