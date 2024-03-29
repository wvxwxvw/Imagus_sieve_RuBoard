
![Alt text](https://github.com/wvxwxvw/Imagus_sieve_RuBoard/blob/master/imagus.webp "a title")  
  
Фильтры для Imagus - комплект - оригинальные + с Reddit + c Ru-Board  
  
**Imagus** - это расширение для браузеров которое увеличивает миниатюры и показывает изображения/видео при наведении курсора мыши на ссылки / миниатюры.  
  
**Фильтры** - это правила для получения изображений, мультимедиа или другого содержимого с большим разрешением. Само расширение содержит более 200 правил по умолчанию, которые поддерживают тысячи сайтов по всему Интернету, в том числе такие популярные, как Reddit, Imgur, Википедию (или любой сайт на основе WikiMedia), deviantART, сервисы Google (Картинки, YouTube, G+, Picasa...), Facebook, Twitter, Flickr...  
В этом списке сейчас около 600 фильтров.
  
Для некоторых сайтов может быть несколько фильтров (например YouTube), об особенностях каждого из них читайте в примечании к фильтру: Настройки >> Вкладка "Фильтры" >> щелкните по фильтру >> смотрите поле "note" (нижнее).
  
Множественный выбор фильтров по Ctrl+ЛКМ, далее можете переключить их состояние скопом кнопкой Ø.

  
<a href="https://www.reddit.com/r/Imagus/" target="_blank">Страница Imagus</a>  
<a href="https://addons.mozilla.org/ru/firefox/addon/imagus" target="_blank">Imagus для Firefox</a>  
<a href="https://chrome.google.com/webstore/detail/imagus/immpkjjlgappgfkkfieppnmlhakdmaab" target="_blank">Imagus для Chrome</a>  
  
<a href="https://addons.mozilla.org/firefox/addon/imagus-mod/" target="_blank">Imagus Mod для FireFox</a>  
<a href="https://github.com/TheFantasticWarrior/chrome-extension-imagus/releases" target="_blank">Imagus Mod для Chrome</a>  
  
<a href="https://forum.ru-board.com/topic.cgi?forum=5&topic=48222&glp#lt" target="_blank">Ветка обсуждения и запросов</a>  
<a href="https://forum.ru-board.com/topic.cgi?forum=5&topic=50874&start=0&limit=1&m=6#1" target="_blank">Чаво</a>  
  
---
  
**Как импортировать фильтры из файла:**  
* В настройках Imagus переходим на вкладку "Фильтры"
* Нажимаем кнопку "Импорт" (стрелка вниз)
* Отмечаем параметр "Удалить данные перед импортом"
* Нажимаем кнопку "Из файла", выбираем ранее скачанный файл на диске
* Справа нажимаем кнопку "Сохранить"
  
**Как добавить/обновить фильтр из json-строки:**  

Например -  
`{"B_parovoz.com":{"img":"(parovoz\\.com\\/gallery)\\/icons(\\/[A-Z0-9]+\\/\\d{8}_\\d{6})-s(\\.jpg)","to":"$1$2$3"}}`
* В настройках Imagus переходим на вкладку "Фильтры"
* Нажимаем кнопку "Импорт" (стрелка вниз)
* Отмечаем параметр "Заменить имеющиеся данные"
* В поле ввода вставляем текст фильтра `{"B_parovoz.com":{"img"...}`
* Нажимаем кнопку "Из текста"
* Справа нажимаем кнопку "Сохранить"
  
---
  
**Идентификаторы в названии фильтров:**  
* R_ (Ru-Board) - фильтры с Ру-Борд  
* O_ (Other) - фильтры из других источников (в основном с Reddit)  
* -b (bad) - неисправные фильтры (на данный момент)  
* -x (xxx) - сайты с NSFW-контентом  
  
**Кто разработчик фильтра?**  
  
Автор фильтра указан в самом фильтре в самой первой строке его раздела "notes". Там же указана и ссылка на оригинал фильтра (где он был опубликован). Если же автор не указан, значит это фильтр самого разработчика Imagus (как правило, это самые старые фильтры, они находятся в конце списка на вкладке Фильтры и не имеют префикса).  
  
Сборщик этого комплекта фильтров <a href="https://forum.ru-board.com/profile.cgi?action=show&member=kenko2" target="_blank">**kenko2** (ru-board)</a>.  
Автор многих фильтров ru-board <a href="https://forum.ru-board.com/profile.cgi?action=show&member=Baton34V" target="_blank">**Baton34V** (ru-board)</a>.
  
---
  
### О необходимости Simple Modify Headers
  
Simple Modify Headers это браузерное расширение для подмены рефереров.  
  
Реферер это строка, которая передаётся http-серверу от клиента и определяет источник запроса. Например, если перейти с одной страницы на другую, реферер будет содержать адрес исходной страницы. Бывает что сервер не отдаст полноразмерную картинку, если запрос клиента не будет содержать определенный источник. 
  
Ранее мы использовали Referer Control, но теперь с ним проблемы, поэтому переезжаем на Simple Modify Headers.  
 
<a href="https://chrome.google.com/webstore/detail/simple-modify-headers/gjgiipmpldkpbdfjkgofildhapegmmic?hl=en" target="_blank">Версия для Хрома и хромоклонов</a>  
<a href="https://addons.mozilla.org/ru/firefox/addon/simple-modify-header" target="_blank">Версия для Firefox и лисоклонов</a>
 
На данный момент расширение необходимо для корректной работы фильтров Imagus на сайтах:
```
• 500px.com (для авторизованных пользователей)
• Archived.moe (archiveofsins.com)
• EroMe.com
• Files.fm (failiem.lv)
• Gammacdn.com (Gamma Entertainment)
• Happy-Team.org
• ImageFap.com (видео)
• ImageNpic.com
• ImageShack.com (внутренние альбомы)
• Imageshimage.com
• ImageTwist.com
• ImgHost.pl
• Instagram.com (cdninstagram.com) (внешние ссылки и фреймы)
• Kick.com (VoD)
• Pixiv.net (pximg.net) (внешние ссылки)
• Pixroute.com
• TikTok (внешние ссылки) - возможно, уже не нужен?
• YouTube (4 правила) (внешние ссылки - только для Хромиум-браузеров, в FF фильтр работает и без SMH)
• Zapodaj.net
```
Если вы не пользуетесь этими сайтами или вам не нужны именно эти фильтры, то устанавливать данное расширение необходимости нет.
 
Список правил обновляется аналогично списку фильтров - по мере добавления/удаления правил.
Забрать его можно в последнем архиве папки "archive".
  
!!! Перед импортом все старые правила (если они есть) будут удалены, такова особенность расширения.
