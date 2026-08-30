# Ivybek UZ Short — lead page

Статическая посадочная страница IVYBEK Academy на узбекском языке.

## Состав

| Файл | Что это |
|---|---|
| `index.html` | Сама страница (бывший `Ivybek UZ Short.dc.html`) |
| `support.js` | Рантайм, который отрисовывает страницу в браузере |
| `uploads/` | 12 изображений, которые использует страница |

Больше ничего не нужно — это весь сайт.

## Публикация на GitHub Pages

```bash
git init
git add .
git commit -m "Ivybek UZ short lead page"
git branch -M main
git remote add origin https://github.com/<логин>/<репозиторий>.git
git push -u origin main
```

Дальше в репозитории: **Settings → Pages → Source: Deploy from a branch → Branch: `main` / `(root)` → Save.**
Через минуту страница будет по адресу `https://<логин>.github.io/<репозиторий>/`.

## Локальная проверка

```bash
python3 -m http.server 8000
```

Открыть `http://localhost:8000`. Просто двойным кликом по `index.html` открывать не стоит — часть браузеров блокирует загрузку `support.js` с `file://`.

## Важно знать

- `support.js` подтягивает React и Babel с `unpkg.com`, поэтому для отрисовки нужен интернет. Первая загрузка занимает пару секунд, дальше библиотеки кешируются браузером.
- Форма пока ничего никуда не отправляет: после нажатия кнопки показывается экран «спасибо», но заявка не уходит в CRM. Чтобы лиды доходили, нужно подключить отправку в Google Apps Script или amoCRM.
