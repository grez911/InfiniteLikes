# Предназначение

Данный скрипт автоматизирует выполнение заданий с сайта [likes.fm](https://likes.fm/).

# Использование

1. Сохранить файл `InfiniteLikes.user.js`. Для этого кликнуть правой кнопкой мыши [сюда](https://github.com/grez911/InfiniteLikes/raw/master/InfiniteLikes.user.js) и выбрать "Сохранить ссылку как...".
2. Получить токен в [vk.com](https://vk.com). Для этого необходимо зайти в аккаунт, с которого будет осуществляться выполнение заданий, и перейти по [этой ссылке](https://oauth.vk.com/authorize?client_id=3682744&v=5.7&scope=wall,friends,groups,offline&redirect_uri=http://oauth.vk.com/blank.html&display=page&response_type=token). Токен будет записан в адресной строке после `access_token=` и до символа `&`. Скопировать его.
3. Открыть файл `InfiniteLikes.user.js`, вставить токен в переменную `access_token` в самом начале скрипта и сохранить его.
4. Установить скрит:
  * Chromium/Chrome: открыть страницу с расширениями (chrome://extensions/) и перетащить туда файл `InfiniteLikes.user.js`.
  * Firefox: установить [Greasemonkey](https://addons.mozilla.org/ru/firefox/addon/greasemonkey/) и перетащить файл `InfiniteLikes.user.js` в окно Firefox.

# Несколько советов

* Не выполнять задания на нескольких аккаунтах, но с одного ip адреса. [likes.fm](https://likes.fm/) блокирует такие аккаунты. Используйте, например, [менеджер профилей Firefox](https://support.mozilla.org/ru/kb/upravlenie-profilyami) для одновременного запуска нескольких браузеров с разными прокси.
* Делать заказы выгоднее мелкими партиями. Если заказать 2 подписчика, обычно на страницу подписывается от 2 до 6 пользователей. Большие заказы не так выгодны, на 30 заказанных подписчиков, подписывается обычно 30-35. Поэтому лучше делать 15 заказов по 2 подписчика, чем один на 30. [Пишите в лс](https://vk.com/id33333349), я поделюсь скриптом, помогающим это автоматизировать.
* Во время выполнения скрипта стоит держать консоль браузера открытой и просматривать выводимые в неё сообщения (CTRL+SHIFT+J в Chromium/Chrome, CTRL+SHIFT+K в Firefox).
