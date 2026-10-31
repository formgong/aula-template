# AULA: a premium interior design studio site with Formgong forms

**Live demo:** https://aula.formgong.com · Download: the [latest release](https://github.com/formgong/aula-template/releases/latest) zip.

[![Deploy to Cloudflare](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/formgong/aula-template) [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fformgong%2Faula-template&project-name=aula&repository-name=aula)

Each button copies the site to your GitHub and publishes it. Then replace every `fk_your_access_key` in `index.html` of your copy with your Formgong access key (free at https://formgong.com/new) and commit: the host republishes on its own.

Сайт преміальної студії дизайну інтер'єру з формами Формгонг

A one-page template for an interior design studio, in a single `index.html`. The demo studio, AULA, its address and projects are fictional.

- **Header.** A dark bar that stays on top. It has a menu button, the tagline, an "about" button that opens a panel with the studio text, a centred wordmark, a "discuss a project" pill and the phone number. The menu slides in from the left, and Projects opens a sub-list.
- **Tiles.** Eight square photos in a 4 × 2 grid under a dark veil: about us, projects, services, pricing, awards, press, furnishing, contacts. On hover the photo zooms, the veil lifts and a short line of text opens. "Services" and "furnishing" scroll to the request form and tick that service.
- **Latest projects.** Five full-width rows, photo and text side by side, swapping sides on every row. Each project has its own colour (`--pc`), used for the tag, the details, the title and the "view" link. "view" opens the photo large.
- **Request form.** On the dark footer: chips for type of space and area (pick one each) and for services (pick several), name, phone and email, and a "send request" pill.
- **Call button.** A round phone button that shakes on hover. It opens a small window with the number and a call-back form.

## English

**Set up the forms**

1. Create a form in the Formgong dashboard and copy its access key.
2. In `index.html`, replace every `fk_your_access_key` with that key. There are two forms, project request and call back.
3. Each form sends a hidden `request` field. Several ticked services arrive as several `services` values.

A form shows thanks only when Formgong answers `success: true`. If the answer is anything else, it shows the error and keeps what was typed.

**Edit**

- Colours are at the top of the styles: `--dark` for the header and footer, and `--pill` for the buttons. Each project row sets its own `--pc` in its `style` attribute.
- The wordmark is one SVG `<symbol id="wordmark">` near the top of `<body>`.
- Point the tiles and menu links at your own pages if your site has more than one page.

**Images.** The thirteen photos were generated for this template with ChatGPT image generation (OpenAI) and saved as WebP, about 1.8 MB in all. You may use them in your own site. Replace them with your own projects, keeping the file names.

The "Powered by Formgong" links point to `https://formgong.com/review-page/fk_your_access_key`, so the same find and replace covers them. Once your key is in, the first click from your published site makes your own public review page on Formgong, where clients read and leave reviews, and every later click opens it. Switch the page off in Formgong (Reviews → your site → Settings) or change those links.

## Українська

Односторінковий шаблон для студії дизайну інтер'єру. Студія AULA, адреса й проєкти вигадані.

На сторінці:

- темна шапка з бічним меню і панеллю «про нас»;
- вісім квадратних плиток із фото: під курсором фото збільшується, темна вуаль зникає і з'являється короткий текст;
- п'ять проєктів рядами, кожен зі своїм кольором, фото відкривається великим;
- форма запиту з чипами (тип приміщення, площа, послуги);
- кругла кнопка дзвінка з віконцем зворотного дзвінка.

**Налаштування.** Створіть форму в кабінеті Formgong і замініть усі `fk_your_access_key` у `index.html` на свій ключ (форм дві). Подяка з'являється лише тоді, коли Formgong відповідає `success: true`.

**Зображення:** тринадцять фото згенеровано для цього шаблону в ChatGPT (OpenAI) і збережено у WebP, разом близько 1,8 МБ. Їх можна використовувати на своєму сайті.

MIT license.

Посилання «Powered by Formgong» ведуть на `https://formgong.com/review-page/fk_your_access_key`, тож та сама заміна ключа оновить і їх. Коли ключ стоїть, перший перехід з вашого опублікованого сайту створює вашу публічну сторінку відгуків на Formgong, де клієнти читають і залишають відгуки; далі посилання відкриває її. Вимкнути сторінку можна у Formgong (Відгуки → ваш сайт → Налаштування) або змінити ці посилання.
