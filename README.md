# Кафе «Старе Місто» — сайт-меню

Односторінковий сайт кафе «Старе Місто» (м. Хмільник, вул. Шевченка, 30).

- Один самодостатній `index.html` — без збірки, без залежностей (шрифти з Google Fonts, всі фото вшиті base64)
- Повне меню кухні та бару (~250 позицій) з фото страв, пошуком і навігацією по категоріях
- 5 банкетних меню, галерея, контакти
- Mobile-first: нижня таб-панель, safe-area, лайтбокс фото з ціною та вагою

## Деплой

- **Прод:** https://staremisto.nemesis.industries — VPS NEMESIS, nginx роздає `/home/deploy/stare-misto` (vhost у `nemesis-army/infra/nginx-portals.conf`), Cloudflare проксований A-запис `staremisto`.
- **Оновити прод:** `ssh nemesis-deploy 'cd /home/deploy/stare-misto && git pull'` (nginx reload не потрібен).
- **Стейджинг:** GitHub Pages з `main` — https://sikator228.github.io/stare-misto/ (оновлюється кожним push автоматично).
