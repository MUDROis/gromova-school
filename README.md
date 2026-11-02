# Официальный сайт ИП Громовой Анны Александровны

Статический сайт образовательной организации (индивидуальный предприниматель).
Собран вручную на HTML/CSS без внешних зависимостей, размещается на GitHub Pages.

## Структура

```
site/
├── index.html                    — главная страница
├── css/style.css                 — общие стили
├── docs/                         — документы (PDF)
│   ├── vypiska-egrip.pdf
│   ├── vypiska-reestr-litsenziy.pdf
│   ├── uvedomlenie-o-predostavlenii-litsenziy.pdf
│   └── obrazovatelnaya-programma-angliyskiy-yazyk.pdf
└── svedeniya/                    — раздел «Сведения об образовательной организации»
    ├── index.html                — список подразделов
    ├── 01-osnovnye-svedeniya.html
    ├── 02-struktura.html
    ├── 03-dokumenty.html
    ├── 04-obrazovanie.html
    ├── 05-standarty.html
    ├── 06-rukovodstvo.html
    ├── 07-pedagogicheskiy-sostav.html
    ├── 08-mto.html
    ├── 09-platnye-uslugi.html
    ├── 10-finansy.html
    ├── 11-vakantnye-mesta.html
    ├── 12-stipendii.html
    ├── 13-mezhdunarodnoe.html
    └── 14-pitanie.html
```

## Деплой на GitHub Pages

1. Создайте репозиторий на GitHub (например, `gromova-school`), публичный или приватный (для Pages теперь работает и приватный).
2. Загрузите содержимое папки `site/` в корень репозитория (все файлы и папки, включая `index.html`).
3. В репозитории: **Settings → Pages → Source: Deploy from a branch → Branch: main / (root) → Save**.
4. Через 1–2 минуты сайт будет доступен по адресу:
   `https://<ваш-логин>.github.io/<имя-репозитория>/`
   (например, `https://gromova.github.io/gromova-school/`).

### Если нужно через командную строку

```bash
cd site
git init
git add .
git commit -m "Официальный сайт ИП Громовой А.А."
git branch -M main
git remote add origin https://github.com/<логин>/<репозиторий>.git
git push -u origin main
```

Затем включите GitHub Pages в настройках репозитория, как описано выше.

## Обновление информации

Информация размещается и обновляется в течение 10 рабочих дней со дня изменения сведений
(ч. 3 ст. 29 Федерального закона № 273-ФЗ). Правила обновления:

- редактируете файл соответствующего подраздела (или `docs/` — добавляете документ);
- сохраняете и делаете `git add` / `git commit` / `git push`;
- GitHub Pages публикует изменения автоматически в течение 1–2 минут.

## Что добавить в будущем

- Оформленные и подписанные локальные нормативные акты (правила внутреннего распорядка,
  положения, приказ о стоимости обучения, образец договора об оказании платных услуг,
  отчёт о результатах самообследования) — в папку `docs/` со ссылками из раздела «Документы».
- При желании — собственный домен (например, `gromova-school.ru`): купить домен, добавить
  запись CNAME, указать домен в Settings → Pages → Custom domain.
