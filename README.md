# Решение задания 2 — сверстать макет

Решение тестового задания по вёрстке для [14-й Школы разработки интерфейсов](https://academy.yandex.ru/events/frontend/shri_msk-2018-2).

Выложено на https://anton-kobzev.github.io/shri-2018-entrance-task-2/.
Сохраняет адекватный вид при любом размере экрана.

## Используемые инструменты

В проекте используются:

1. `browserlist` для задания набора поддерживаемых браузеров.
2. `autoprefixer`, `postcss-preset-env`: для транспиляции нового CSS в старый.
3. `SCSS` для вложенности и миксинов. Классы именуются по БЭМ.
4. `prettier` для поддержания стиля кода JS и CSS.
5. `stylelint` с набором предустановок для проверки правильности CSS. В том числе проверяет, не используются ли свойства,
   не поддерживаемые в заявленном наборе браузеров.
6. При коммите срабатывают `prettier` и `stylelint` и пытаются привести код в порядок.

## Используемые библиотеки

1. D3 используется для упрощения динамической отрисовки SVG для крутилки регулятора температуры.

## Мысли

1. Анимацию открытия попапа сделал немного другой. Та, что предложена в задании, предполагает скрытие элемента, по которому
   нажали. На главном экране iOS это выглядит естественно, но в нашем случае мне это показалось нелогичным.
2. По-хорошему, блоки избранных сценариев должны быть такого же размера, как остальные (200x120), у них, как и у остальных,
   может быть заголовок в две строки и подзаголовок. На макете это не предусмотрено, и размер сделан 200x100. Для простоты
   проверки сделал как на макете.
