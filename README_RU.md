# Портфолио: CSS Layout and Visual Effects

Распакуйте ZIP целиком и откройте index.html в браузере. Установка пакетов и интернет не нужны. В VS Code можно использовать Live Server. JavaScript в проекте не используется.

Это учебное портфолио с вымышленным автором и примерами проектов. Студенты заменяют имя, текст и иллюстрации своими материалами и продолжают собственную работу.

## Файлы

- index.html — структура и небольшой пример внутренних стилей в head.
- style.css — оформление, макет, эффекты, адаптивность. Комментарии SLIDE связывают код со слайдами.
- typography.css — шрифты и line-height, подключён через @import.
- media — локальные SVG-иллюстрации и повторяемый узор.

## Соответствие презентации (24 слайда)

| Слайд | Тема | Найти в проекте |
| --- | --- | --- |
| 2 | div, display:block | .block-example, две строки лаборатории |
| 3 | float:right | .about-photo и .about с flow-root |
| 4 | box-shadow | .project-card |
| 5 | border-radius | .project-card и .about-photo |
| 6 | overflow | .preview, прокручиваемый текст |
| 7 | display:flex | nav и .header-inner |
| 8 | grid-template-columns | .projects |
| 9 | :hover, :focus-visible | ссылки и клавиатурный фокус |
| 10 | display:none | .draft-project — скрытая четвёртая карточка |
| 11 | transition | .project-card, подъём при наведении |
| 12 | @keyframes и animation | appear, .hero-content |
| 13 | центр Flexbox | .hero-content |
| 14 | line-height | body в typography.css |
| 15 | position:fixed | .back-to-top |
| 16 | position:sticky | .site-header |
| 17 | rgba и альфа | .alpha-example и фон hero::before |
| 18 | z-index | .badge и .layer-front/.layer-back |
| 19 | background-repeat | .pattern |
| 20 | text-shadow | .hero h1 |
| 21 | background-size | hero, .sample-cover и .sample-contain |
| 22 | @import | первая инструкция style.css |
| 23 | inline и inline-block | span и ссылка в лаборатории |
| 24 | итоговая практика | доработка портфолио |

В .projects используется repeat(3, minmax(0, 1fr)) — вариант трёх гибких колонок, разрешающий трекам сжиматься до нуля. В презентации приведена базовая запись repeat(3, 1fr).

В .hero-content направление column: justify-content центрирует по вертикали, align-items — по горизонтали. В примере презентации использован row, поэтому направления осей другие.

## Как показывать

1. Откройте страницу и прокрутите её: шапка sticky остаётся сверху, ссылка Top fixed — в углу экрана.
2. About: фотография справа, текст обтекает её. На телефоне float отключается.
3. Work: наведите на карточку, затем пройдите ссылки клавишей Tab.
4. В style.css измените .draft-project с display:none на block. Появится четвёртая карточка. Верните none.
5. В лаборатории прокрутите заметку и сравните cover/contain.
6. Измените background-repeat:repeat на repeat-x или no-repeat.
7. Поменяйте z-index двух .layer, чтобы поменять порядок перекрытия.
8. Сравните фон с альфа-каналом и opacity всего элемента.
9. Обновите страницу: hero плавно появляется. В режиме уменьшенного движения анимация отключается.
10. Измените текст поля и нажмите Reset goal: кнопка действительно сбрасывает значение без JS. Данные никуда не отправляются.
11. Проверьте ширину около 375px, 640px, 900px и 1100px.

## Задание на 25 минут

Продолжить собственное портфолио: добавить скругления и спокойную тень, эффект hover с transition, видимый фокус, sticky-шапку и настроенный фон. Проверить телефонную ширину. Объяснить пять CSS-объявлений. Дополнительно — короткая анимация с отключением при prefers-reduced-motion.
