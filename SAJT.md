# TOG Drive: sajt (GitHub Pages)

Statički sajt za TOG Drive: čist HTML i jedan CSS fajl, bez build koraka i bez spoljnog JavaScript-a.
Svetla i tamna tema prate sistem (`prefers-color-scheme`). Font Inter se učitava sa Google Fonts, uz sistemski font kao rezervu.

## Fajlovi

| Fajl | Sadržaj |
|---|---|
| `index.html` | Početna: šta je TOG Drive, mogućnosti, preuzimanje (Windows, macOS, Linux), App Store i Google Play „uskoro“ |
| `uputstvo.html` | Detaljno uputstvo, česta pitanja i rešavanje problema |
| `kako-radi.html` | Kako radi: šifrovanje, gateway, skladište na mreži TOG (sa dva SVG dijagrama) |
| `privatnost.html` | Politika privatnosti; odeljak za brisanje naloga je na `privatnost.html#brisanje-naloga` |
| `en/index.html`, `en/guide.html`, `en/how-it-works.html`, `en/privacy.html` | Engleska verzija (`en/privacy.html#account-deletion`; radi i `#brisanje-naloga`) |
| `404.html` | Stranica za nepostojeće adrese (stil i mali skript su u samom fajlu, jer se servira sa bilo koje putanje) |
| `style.css` | Jedini stylesheet |
| `favicon.svg` | Ikonica |
| `.nojekyll` | Isključuje Jekyll obradu na GitHub Pages |

## Objava

Sajt je predviđen za javni repo `vahidzekic/theonlygrid-drive`, na adresi
https://vahidzekic.github.io/theonlygrid-drive/ .

1. Kopirajte sadržaj ove fascikle u koren grane koju koristi GitHub Pages (na primer `main`, folder `/` ili `/docs`).
2. Settings → Pages → Build and deployment → Source: *Deploy from a branch*, izaberite granu i folder.
3. Dugmad za preuzimanje vode na https://github.com/vahidzekic/theonlygrid-drive/releases/latest , pa je dovoljno da izdanja (Releases) u istom repou imaju fajlove za Windows, macOS i Linux.

Sve unutrašnje veze su relativne, pa sajt radi i na `github.io/theonlygrid-drive/` i na sopstvenom domenu.

## Sopstveni domen (npr. drive.theonlygrid.com)

U ovoj fascikli namerno **nema** fajla `CNAME`: prazan ili pogrešan `CNAME` bi pokvario objavu. Kada domen bude odlučen:

1. Kod DNS provajdera dodajte zapis `CNAME` za `drive` (ili drugi poddomen) koji pokazuje na `vahidzekic.github.io`.
2. U repou dodajte fajl `CNAME` sa jednim redom, samim domenom, na primer `drive.theonlygrid.com` (ili ga upišite u Settings → Pages → Custom domain, što napravi isti fajl).
3. Uključite *Enforce HTTPS* kada se pojavi.

Napomena: ako `drive.theonlygrid.com` bude i adresa Drive gateway-a (javni linkovi `https://<host>/l/...`), sajt treba staviti na drugi poddomen.

## Pre objave

- Popunite sve oznake `[...]` (u HTML-u imaju klasu `ph` i istaknute su ružičasto): naziv firme, adresa, e-mail adrese, rokovi čuvanja, lokacija servera, mehanizam prenosa podataka, datum.
- Pregledajte politiku privatnosti sa advokatom.
- Kada izađu mobilne aplikacije, zamenite dugmad „uskoro“ zvaničnim bedževima App Store i Google Play (prema pravilima Apple-a i Google-a za korišćenje bedževa) i linkovima ka prodavnicama.
