# Katkıda Bulunma Rehberi

> Org üyeleri: repo, ruleset, test komutları, CI ve deploy ayrıntıları [ekip rehberinde](https://github.com/Garage-Group-Turkiye/.github-private/blob/main/CONTRIBUTING.md).

## Başlamadan Önce

Bir issue aç veya mevcut issue'yu üstlen. `main` branch'i korumalıdır; değişiklikler yalnızca onaylı PR ile girer.

## İş Akışı

```
1. main'den yeni branch aç
   git checkout -b feature/aciklayici-isim

2. Kodunu yaz, branch'ine push et
   git push origin feature/aciklayici-isim

3. GitHub'da PR aç → check'leri bekle → review iste

4. Onay geldikten ve yorumlar çözüldükten sonra merge et
```

## Branch İsimlendirme

| Tür | Format | Örnek |
|-----|--------|-------|
| Yeni özellik | `feature/...` | `feature/hepsiemlak-entegrasyonu` |
| Bug fix | `fix/...` | `fix/login-yonlendirme` |
| Küçük düzeltme | `chore/...` | `chore/console-log-temizle` |

## Commit Mesajı Formatı

```
<tip>: <açıklama>
```

Tipler: `feat`, `fix`, `refactor`, `docs`, `test`, `chore`, `perf`, `ci`

Örnekler:
- `feat: hepsiemlak haber entegrasyonu eklendi`
- `fix: anasayfa yönlendirme hatası düzeltildi`
- `docs: CONTRIBUTING güncellendi`

## PR Açarken

- PR template'ini eksiksiz doldur
- Testleri yerelde çalıştır ve PR açıklamasına yaz
- Web projelerinde önizleme URL'ini PR'a ekle
- `console.log` bırakma
- Secret/API key commit'leme; secret'lar sadece GitHub Secrets'ta tutulur
