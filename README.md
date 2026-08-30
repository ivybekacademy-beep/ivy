# IVYBEK — yangi sayt (ivy.uz)

Qisqa lead-lending (uz) + eski saytning ishchi logikasi. Sof statika — build kerak emas.

## Tarkib

| Fayl | Nima |
|---|---|
| `index.html` | Asosiy sahifa: qisqa dizayn + Meta Pixel, Telegram Pixel, Apps Script'ga yuborish, telefon maskasi, UTM |
| `en.html` | Inglizcha versiya (eski saytdan o'zgarishsiz, /en va /admissions-eng shu yerga olib keladi) |
| `vercel.json` | Kanal linklari: /admissions-ig, -lev, -fb, -yt, -tg, -tgads, -google, /en — UTM teglar bilan |
| `uploads/` | Karusel rasmlari (webp, 368 KB jami) |
| `og.jpg` | Havola ulashilganda ko'rinadigan rasm |
| qolgan `.webp/.woff2` | en.html uchun assetlar |

## Deploy (yangi akkauntlar)

1. Yangi GitHub'da repo yarating → shu papkani push qiling.
2. Yangi Vercel → Add New Project → repo'ni import → Deploy (sozlash kerak emas, statika).
3. Vercel'da Domains → `ivy.uz` qo'shing → ko'rsatilgan A/TXT yozuvlarni registrator panelida o'rnating.
4. Yangi Gmail'da Apps Script qayta deploy qilingach — `index.html` va `en.html` ichidagi `ENDPOINT` (AKfycb... URL) yangisiga almashtiriladi. Boshqa hech narsa o'zgarmaydi.

Pixel ID'lar (Meta `2283622125504650`, Telegram `4HGABMb6`) reklama kabinetlariga bog'liq — ular O'ZGARMAYDI.
