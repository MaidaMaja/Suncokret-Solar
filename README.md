# Suncokret Solar — portfolio sajt

Jednostranični (one-page) sajt za firmu za ugradnju solarnih panela. Rađen kao portfolio primer — statičan HTML/CSS/JS, bez build alata i bez backend-a.

## Struktura

```
index.html        — kompletan sadržaj stranice
style.css          — originalni, čitljiv CSS (menjaj ovaj fajl)
style.min.css      — minifikovana verzija, referencirana u index.html
script.js          — originalni, čitljiv JS (menjaj ovaj fajl)
script.min.js      — minifikovana verzija, referencirana u index.html
image-slot.js      — komponenta za "drag & drop" plejsholdere slika (proizvodi/projekti)
images/            — hero.jpg/webp, tim.jpg/webp
```

## Kako da izmeniš sajt

Uvek menjaj `style.css` i `script.js` (čitljive verzije), pa ručno prenesi izmenu i u `.min` fajl — ili pusti bilo koji CSS/JS minifier (npr. na cssnano.co / minifier.org) da ponovo generiše `.min` fajlove iz izmenjenog originala.

## Napomene

- Slike u sekcijama "Naši proizvodi" i "Referentni projekti" su plejsholderi (`<image-slot>`) — na GitHub Pages-u (statički hosting) drag & drop neće trajno snimiti sliku, pa te slike treba zameniti pravim `<img>` tagovima kada budeš imao fotografije.
- Svi kontakt podaci (telefon, email, adresa) i domen u meta tagovima/Schema.org su placeholder vrednosti — zameni ih pravim podacima ako sajt postane produkcioni.
- Kritični CSS je inline u `<head>` radi brzine učitavanja; ostatak stila (`style.min.css`) učitava se asinhrono.
