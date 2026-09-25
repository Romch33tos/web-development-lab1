# Словарь токенов проекта Talking Travel

## 1. Ширина макета и контейнер

| Параметр | Значение | Токен | Где |
|----------|----------|-------|-----|
| Ширина макета | 1440 px | — | справочно |
| Ширина макета (блог) | 1427.64 px | — | расхождение из-за скроллбара |
| Ширина контейнера (главная) | 1202 px | `--container` | главная |
| Ширина контейнера (блог) | 911.64 px | `--container-narrow` | блог |
| Padding контейнера (шапка, Discover) | 119 px | `--container-padding` | обе |
| Padding контейнера (Featured, Recent, подвал) | 120 px | `--container-padding` | обе |
| Padding статьи блога по бокам | 258 px | `--article-padding` | блог |
| Ширина формы Join | 611.36 px | `--form-width` | обе |

**Примечание:** расхождение 1440 и 1427.64 px вызвано наличием скроллбара в Figma. Используется 1440 px как базовая ширина.

---

## 2. Сетка

| Параметр | Значение | Токен |
|----------|----------|-------|
| Промежуток в навигации | 18 px | `--space-4` |
| Промежуток в hero | 34 px | `--space-6` |
| Промежуток в заголовках секций | 15 px | `--space-3` |
| Промежуток между карточками Discover | 0 px | — |
| Промежуток между малыми Story | 16 px | `--space-3` |
| Промежуток между highlight | 15 px | `--space-3` |
| Промежуток в коллаже | 15–16 px | `--space-3` |

**Сетки по секциям:**

| Секция | Раскладка |
|--------|-----------|
| Шапка | flex row, space-between |
| Hero главной | 2 зоны: контент 765 px + изображение |
| Featured | flex row: изображение 540 px + текст 520 px |
| Discover | 4 карточки по 300.5 px |
| Join | форма 617 px по центру |
| Recent | 2 колонки: 600 px + 600 px |
| Статья блога | 1 колонка 911.64 px, padding 46/258 |
| Статья: hero | заголовок 721 px + автор справа |
| Статья: callout | 2 колонки: коллаж 455.82 px + текст 455.82 px |
| Статья: highlights | 3 карточки по 303.88 px |
| Подвал | flex row, space-between |

---

## 3. Типографика

### 3.1. Семейства шрифтов

| Назначение | Значение | Токен | Где |
|------------|----------|-------|-----|
| Заголовки | Changa One, cursive | `--font-heading` | обе |
| Основной текст | Roboto, sans-serif | `--font-body` | обе |
| Декоративный (The Matterhorn) | Black Signature PERSONAL USE ONLY | — | только блог, требует замены |

**Подключение Google Fonts:**

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Changa+One:ital@0;1&family=Roboto:ital,wght@0,400;0,700;1,400&display=swap" rel="stylesheet">
```

**Замена шрифта для «The Matterhorn»:** используется Caveat или Dancing Script (оба доступны в Google Fonts). Решение фиксируется в разделе 13.

### 3.2. Размеры и начертания

| Элемент | Шрифт | Размер | Начертание | Интерлиньяж | Tracking | Цвет | Токен |
|---------|-------|--------|------------|-------------|----------|------|-------|
| `h1` hero главной | Changa One | 73 px | 400 | 84 px | -0.01em | #8A53FF | `--step-6` |
| `h1` статьи блога | Changa One | 50 px | 400 | 54 px | -0.03em | #434343 | `--step-5` |
| Цитата (callout) | Changa One | 42 px | 400 italic | 47 px | -0.04em | #434343 | `--step-5` |
| `h2` секций главной | Changa One | 39 px | 400 | 40 px | normal | #434343 | `--step-5` |
| Подзаголовки (Clincher, Highlights) | Changa One | 32 px | 400 | 36 px | normal | #434343 | `--step-4` |
| `h3` карточек | Changa One | 24 px | 400 | 36 px | normal | #434343 | `--step-3` |
| «Share your travels» (форма) | Changa One | 24 px | 400 | 36 px | normal | #434343 | `--step-3` |
| Надзаголовок (eyebrow) | Roboto | 18 px | 700 | 21 px | 0.06em | #8A53FF | `--step-1` |
| Описание в hero | Roboto | 22 px | 400 | 36 px | normal | #434343 | `--step-2` |
| Основной текст | Roboto | 18 px | 400 | 33 px | normal | #434343 | `--step-1` |
| Текст статьи блога | Roboto | 16 px | 400 | 26 px | normal | #434343 | `--step-0` |
| Disclaimer | Roboto | 16 px | 700 | 26 px | normal | #434343 | `--step-0` |
| Описание в карточках | Roboto | 16 px | 400 | 26 px | normal | #576074 | `--step-0` |
| Имя автора | Roboto | 16 px | 400 | 19 px | normal | #495367 | `--step-0` |
| Роль автора | Roboto | 14 px | 400 italic | 16 px | normal | #A2A7B1 | `--step--1` |
| Подписи под highlights | Roboto | 14 px | 400 italic | 22 px | normal | #828181 | `--step--1` |
| Пункт навигации | Roboto | 16 px | 400 | 19 px | normal | #495367 / #8A53FF | `--step-0` |
| Кнопка | Roboto | 16 px | 400 | 19 px | normal | #FFFFFF | `--step-0` |
| Поле формы | Roboto | 16 px | 400 | 24 px | 0.15px | rgba(0,0,0,0.6) | `--step-0` |
| Копирайт | Roboto | 14 px | 400 | 16 px | normal | #939EB4 | `--step--1` |
| «The Matterhorn» | Black Signature | 70 px | 400 italic | 92 px | normal | #FFFFFF | требует замены |

### 3.3. Регистр и разрядка

| Элемент | Регистр | Tracking |
|---------|---------|----------|
| Надзаголовок (eyebrow) | uppercase | 0.06em |
| `h1` hero главной | normal | -0.01em |
| `h1` статьи | normal | -0.03em |
| Цитата | normal | -0.04em |
| Остальное | normal | normal |

---

## 4. Палитра

| Назначение | Значение | Токен | Где |
|------------|----------|-------|-----|
| Акцент | #8A53FF | `--color-accent` | обе |
| Акцент hover | #7B45E8 | `--color-accent-hover` | обе |
| Основной текст | #434343 | `--color-text` | обе |
| Приглушённый текст | #576074 | `--color-text-muted` | обе |
| Текст навигации | #495367 | `--color-text-nav` | обе |
| Текст копирайта | #939EB4 | `--color-text-faint` | обе |
| Роль автора | #A2A7B1 | `--color-text-faintest` | блог |
| Подписи под highlights | #828181 | `--color-text-caption` | блог |
| Фон страницы | #FFFFFF | `--color-surface` | обе |
| Фон секции Join | #F7F8F9 + паттерн | `--color-surface-alt` | обе |
| Фон больших карточек Story | #F9F9F9 | `--color-surface-card` | обе |
| Фон Disclaimer | #FAFAFA | `--color-surface-disclaimer` | блог |
| Границы полей | rgba(0, 0, 0, 0.23) | `--color-border` | обе |
| Разделитель в шапке | #EEEEEE | `--color-border-light` | обе |
| Тёмный в логотипе | #3E3E3E | `--color-logo-dark` | обе |
| Текст на акценте | #FFFFFF | `--color-on-accent` | обе |
| Плейсхолдер | rgba(0, 0, 0, 0.6) | `--color-placeholder` | обе |

---

## 5. Шаг отступов

Точные значения из макета:

| Значение | Где используется |
|----------|------------------|
| 3 px | label + input |
| 6 px | заголовок + описание |
| 8 px | между надзаголовком и заголовком |
| 10 px | внутренние отступы карточек |
| 12 px | в hero texts, под highlight |
| 14 px | padding body большой Story |
| 15 px | зазор в заголовках, между highlight |
| 16 px | внутренние отступы малых Story |
| 17 px | между полями формы |
| 18 px | промежуток в навигации |
| 19 px | padding Disclaimer |
| 20 px | padding формы, зазор в hero статьи |
| 24 px | зазор между кнопками |
| 28 px | padding формы внутри |
| 29 px | padding Disclaimer по бокам |
| 30 px | padding blurb, зазор в форме Join |
| 32 px | padding подвала |
| 34 px | зазор в hero content главной, padding callout |
| 35 px | зазор в статье блога |
| 36 px | padding callout по вертикали |
| 40 px | padding hero |
| 46 px | padding статьи блога |
| 48 px | зазор в Discover |
| 70 px | padding снизу Discover |
| 83 px | padding Recent |
| 107 px | padding Featured |
| 119 px | padding контейнера |
| 120 px | padding контейнера |
| 140 px | padding hero content |
| 258 px | padding статьи блога по бокам |

**Сгруппированная шкала для вёрстки:**

| Токен | Значение | Какие исходные значения покрывает |
|-------|----------|-----------------------------------|
| `--space-0` | 0.25rem (4 px) | 3 px |
| `--space-1` | 0.5rem (8 px) | 6, 8 px |
| `--space-2` | 0.75rem (12 px) | 10, 12, 14 px |
| `--space-3` | 1rem (16 px) | 15, 16, 17, 18 px |
| `--space-4` | 1.25rem (20 px) | 19, 20, 24 px |
| `--space-5` | 1.5rem (24 px) | 28, 29, 30 px |
| `--space-6` | 2rem (32 px) | 32, 34, 35, 36 px |
| `--space-7` | 2.5rem (40 px) | 40, 46, 48 px |
| `--space-8` | 5rem (80 px) | 70, 83 px |
| `--space-9` | 7.5rem (120 px) | 107, 119, 120, 140, 258 px |

Округление фиксируется в разделе 13.

---

## 6. Радиусы скругления

| Значение | Токен | Где используется |
|----------|-------|------------------|
| 2 px | `--radius-xs` | иконка play (внутренняя) |
| 3 px | `--radius-xs` | polygon в большой play (блог) |
| 4 px | `--radius-sm` | кнопки, поля, логотип, disclaimer, малые Story |
| 8 px | `--radius-md` | Featured, Discover, Big Story, article hero |
| 12 px | `--radius-lg` | форма Join |
| 50% | `--radius-full` | аватары, play |

---

## 7. Тени и границы

| Параметр | Значение | Токен | Где |
|----------|----------|-------|-----|
| Тень шапки | 0 4px 16px rgba(0, 0, 0, 0.04) | `--shadow-header` | обе |
| Тень формы | 0 0 24px rgba(0, 0, 0, 0.03) | `--shadow-form` | обе |
| Граница поля | 1px solid rgba(0, 0, 0, 0.23) | `--border-input` | обе |
| Разделитель | 1px solid #EEEEEE | `--border-light` | обе |
| Оверлей на изображении статьи | linear-gradient(0deg, rgba(0,0,0,0.06), rgba(0,0,0,0.06)) | `--overlay-hero` | блог |

---

## 8. Повторяющиеся элементы

| Элемент | Класс | Точные размеры |
|---------|-------|----------------|
| Кнопка | `.button` | 46 px высота, radius 4 px |
| Карточка направления | `.card` | 300.5×410 px, изображение 268.5×317 px |
| Карточка поста (малая) | `.post-card` | 600×148 px, изображение 200×128 px |
| Карточка поста (большая) | `.post-card--featured` | 560×476 px, изображение 560×358 px |
| Надзаголовок | `.eyebrow` | Roboto 18/21, tracking 0.06em, uppercase |
| Заголовок секции | `h2` | Changa One 39/40 |
| Пункт навигации | `.site-nav__link` | Roboto 16/19 |
| Кнопка play (Featured) | `.play-button` | 36×36 px |
| Кнопка play (Big Story) | `.play-button--lg` | 48×48 px |
| Кнопка play (Article) | `.play-button--xl` | 104.67×105.63 px |
| Поле формы | `.field` | 56 px (input/select), 102 px (textarea) |
| Карточка Highlight | `.highlight` | 303.88×380.55 px, изображение 288.88×346.55 px |
| Disclaimer | `.disclaimer` | 911.64×220 px, фон #FAFAFA, radius 4 px |
| Callout (цитата) | `.callout` | 2 колонки: 455.82 px + 455.82 px |
| Avatar автора | `.post__author-avatar` | 35×35 px |

---

## 9. Состояния элементов

| Элемент | Hover | Focus | Active |
|---------|-------|-------|--------|
| Кнопка `--primary` | фон #7B45E8 | обводка #8A53FF | затемнение |
| Кнопка `--ghost` | фон rgba(138, 83, 255, 0.08) | обводка #8A53FF | — |
| Ссылка в навигации | цвет #8A53FF | обводка #8A53FF | — |
| Поле формы | граница #8A53FF | обводка #8A53FF | — |

**Правило:** обводка фокуса не отключается без замены на собственный видимый стиль.

---

## 10. Изображения и иконки

| Параметр | Значение | Где |
|----------|----------|-----|
| Логотип | 100×64 px, SVG | обе |
| Иконка поиска | 20×20 px, SVG, обводка 2 px #8A53FF | обе |
| Иконка профиля | 24×24 px, SVG, заливка #8A53FF | обе |
| Hamburger | 46×46 px | обе |
| Featured | 540×338 px, radius 8 px | главная |
| Discover | 268.5×317.05 px, radius 8 px | главная |
| Big Story | 560×358.11 px, radius 8 px 8px 0 0 | главная |
| Small Story | 200×128 px, radius 4 px | главная |
| Play (Featured) | 36×36 px | главная |
| Play (Big Story) | 48×48 px | главная |
| Article hero | 911.64×540 px, radius 8 px | блог |
| Play (Article) | 104.67×105.63 px | блог |
| Callout коллаж (вертикальное) | 220.41×481 px, radius 8 px | блог |
| Callout коллаж (горизонтальные) | 220.41×261.47 и 220.41×201.56 px, radius 8 px | блог |
| Highlight | 288.88×346.55 px, radius 8 px | блог |
| Avatar автора | 35×35 px | блог |

**Правило:** все изображения получают `width`, `height`, `max-width: 100%`, `height: auto`. Для изображений ниже первого экрана — `loading="lazy"`. Для крупных иллюстраций — `srcset`/`sizes`.

---

## 11. Точки перехода

| Ширина | Токен | Что меняется |
|--------|-------|--------------|
| 360 px | базовая | одна колонка, мобильная навигация |
| 768 px | `@media (min-width: 48em)` | две колонки, сетка 2×2 |
| 1280 px | `@media (min-width: 80em)` | полная раскладка |

**Правило:** точки перехода назначаются по содержимому, а не по названиям устройств. Базовые стили описывают узкий экран, условия расширяют раскладку.

---

## 12. Что макет не задаёт

Решения по этим пунктам фиксируются в README:

- поведение на промежуточных ширинах между 360, 768 и 1280;
- вид мобильной навигации (бургер-меню или перенос);
- состояния hover, focus, active для большинства элементов;
- поведение длинных заголовков и абзацев в карточках;
- что происходит после отправки формы (страница без логики → заглушка);
- куда ведут ссылки «Gallery» и «Contact Us» (страниц нет → `#`);
- что происходит при клике на кнопку play (видео-плеер, модальное окно или заглушка);
- куда ведёт «View full gallery» (страница галереи или якорь);
- fallback-изображение, если видео не загрузилось;
- что происходит с hero-изображением на мобильном (обрезается, заменяется, скрывается).

---

## 13. Принятые решения

1. **Шрифт Black Signature PERSONAL USE ONLY** заменяется на **Caveat** (Google Fonts). Причина: лицензия не позволяет коммерческое использование. Применяется только для надписи «The Matterhorn» поверх видео.

2. **Шаг отступов** в макете нерегулярный (3, 6, 8, 10, 12, 14, 15, 16, 17, 18, 19, 20, 24, 28, 29, 30, 32, 34, 35, 36, 40, 46, 48, 70, 83, 107, 119, 120, 140, 258 px). Округлён до 10 значений: `--space-0` … `--space-9`.

3. **Ширина макета** указана как 1440 px для главной и 1427.64 px для блога — расхождение из-за скроллбара. Используется 1440 px как базовая.

4. **Контейнер** главной 1202 px, блога 911.64 px — используются как `--container` и `--container-narrow`.

5. **Padding статьи блога** 258 px — на узких экранах заменяется на `--space-6`.

6. **Надпись «The Matterhorn»** — уточнить при вёрстке, часть ли это изображения или отдельный слой. Если отдельный — реализуется через HTML-текст с `--font-signature`.

7. **Разделение стилей** — на базовые и компонентные, если объём превышает несколько сотен строк.

---

## 14. Сводка токенов для :root

```css
:root {
  /* Контейнер */
  --container: 1202px;
  --container-narrow: 912px;
  --article-padding: 258px;
  --form-width: 611px;
  --grid-gap: 24px;

  /* Типографика */
  --font-heading: 'Changa One', cursive;
  --font-body: 'Roboto', sans-serif;
  --font-signature: 'Caveat', cursive;

  --step--1: 0.875rem;   /* 14px */
  --step-0: 1rem;        /* 16px */
  --step-1: 1.125rem;    /* 18px */
  --step-2: 1.375rem;    /* 22px */
  --step-3: 1.5rem;      /* 24px */
  --step-4: 2rem;        /* 32px */
  --step-5: 2.4375rem;   /* 39px */
  --step-6: 4.5625rem;   /* 73px */

  --tracking-tight: -0.01em;
  --tracking-tighter: -0.03em;
  --tracking-tightest: -0.04em;
  --tracking-wide: 0.06em;

  /* Цвета */
  --color-accent: #8A53FF;
  --color-accent-hover: #7B45E8;
  --color-text: #434343;
  --color-text-muted: #576074;
  --color-text-nav: #495367;
  --color-text-faint: #939EB4;
  --color-text-faintest: #A2A7B1;
  --color-text-caption: #828181;
  --color-surface: #FFFFFF;
  --color-surface-alt: #F7F8F9;
  --color-surface-card: #F9F9F9;
  --color-surface-disclaimer: #FAFAFA;
  --color-border: rgba(0, 0, 0, 0.23);
  --color-border-light: #EEEEEE;
  --color-logo-dark: #3E3E3E;
  --color-on-accent: #FFFFFF;
  --color-placeholder: rgba(0, 0, 0, 0.6);

  /* Отступы (сгруппированные) */
  --space-0: 0.25rem;
  --space-1: 0.5rem;
  --space-2: 0.75rem;
  --space-3: 1rem;
  --space-4: 1.25rem;
  --space-5: 1.5rem;
  --space-6: 2rem;
  --space-7: 2.5rem;
  --space-8: 5rem;
  --space-9: 7.5rem;

  /* Радиусы */
  --radius-xs: 2px;
  --radius-sm: 4px;
  --radius-md: 8px;
  --radius-lg: 12px;
  --radius-full: 50%;

  /* Тени и границы */
  --shadow-header: 0 4px 16px rgba(0, 0, 0, 0.04);
  --shadow-form: 0 0 24px rgba(0, 0, 0, 0.03);
  --border-input: 1px solid rgba(0, 0, 0, 0.23);
  --border-light: 1px solid #EEEEEE;
  --overlay-hero: linear-gradient(0deg, rgba(0, 0, 0, 0.06), rgba(0, 0, 0, 0.06));
}
```
