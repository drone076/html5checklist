#Чеклист верстки

Для того чтобы отдавать вёрстку клиенту, достаточно соблюдения первых 5 пунктов.
Для выдачи в продакшен — первых 6.


1. **Соответствие макету**
2. **Кроссбраузерность, кодировка и DOCTYPE**
3. **Валидность, доступность, микроформаты**
4. **Независимость блоков в CSS: минимизация каскада, использование техник БЭМ/MCSS/SMACSS**
5. **Сайт должен нормально смотреться во всех стандартных разрешениях от 1024 и выше, не иметь горизонтального скролла и вписываться в экран мобильных устройств**
 

6. Корректная работа при вбивании реального текста, надёжность вёрстки
7. Проверка и оптимизация скорости загрузки
8. Наличие Win/Mac/Linux-аналогов шрифтов
9. Доступность при выключенных(загружающихся) картинках
10. HTML5 формы, линковка, валидация
11. Семантичность. Отсутствие глупостей в html и css, единообразие, аккуратность
12. Правильная структура заголовков (H1,H2,… и т.д. и TITLE)
13. Работоспособность при выключенном (незагруженном) JavaScript
14. Работоспособность при выключенном Flash
15. Отсутствие багов при увеличенном шрифте

Подробности по каждому пункту: http://habrahabr.ru/post/114256/

##Важные мелочи
 - Лого на внутряках должно вести на титулку. На титулке logo = h1, на внутряках H1=заголовок контента, а Logo=div
 - У каждой страницы должен быть свой уникальный TITLE формата <title>About Us - %CompanyName%</title>
 - Все страницы должны быть слинкованы и проверены на наличие битых ссылок.
 - Все ссылки должны как-то реагировать на :hover, :active и :focus — показыванием/убиранием подчёркивания, сменой цвета, чем угодно. У всех ссылок, кроме пунктов меню, должна быть реакция на :visited
 - Проверять что все интерактивные элементы страницы что должны работать — работают.
 - «Контент в начале страницы» — содержимое страницы должно идти в начале кода, до всяких сайдбаров и прочего.
 - Копирайт должен быть написан правильно.
 - Должны быть favicon.ico (желательно с включенными внутрь неё 32x32, 48x48 и 64×64 вариациями) и apple-touch-icon
 - В вёрстке не должны оставаться закомментированные «на всякий случай» куски кода, лишние неиспользуемые файлы, старые версии файлов и т.п. Все бекапы можно вытянуть из системы контроля версий (например SVN), а на живом проекте «мусор» потом мешает разобраться как что работает.
 - Размеры для блоков, чьи размеры зависят от содержащегося в них текста, нужно задавать в em, а не px.
 - Если url ссылки неизвестен, то он должен быть равен её анкору, написанному латиницей с заменой пробелов/спецсимволов на тире.
 - Skype-плагин не должен ломать вёрстку
 - Ресайз textarea не должен ломать вёрстку
 - При проверке frontend в целом — 404-страница должна отдаваться с кодом 404 а не 200.
 - Нужно подстраховываться фиксируя в css размеры картинок, выводящихся программно.
 - Проверка орфографии Word'ом или Орфографом, желательно — оттипографить контент.
 - Ссылки на чужие сайты должны быть с target=«blank», желательно выделять их иконкой «внешняя ссылка».
 - Разумеется картинки должны быть в отдельной папке, css — в отдельной и js — в отдельной.
