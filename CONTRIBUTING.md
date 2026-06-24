# Katkıda Bulunma Rehberi

## Başlamadan Önce

Bir issue aç veya mevcut issue'yu üstlen. Reviewer onayı olmadan main'e merge yapılmaz.

## İş Akışı

```
1. main'den yeni branch aç
   git checkout -b feature/aciklayici-isim

2. Kodunu yaz, branch'ine push et
   git push origin feature/aciklayici-isim

3. GitHub'da PR aç → Firebase check'i bekle → Reviewer onayını bekle

4. Reviewer merge eder
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
- Firebase preview URL'ini PR'a ekle
- `console.log` bırakma
- Reviewer atanmasını bekle, kendin merge etme
