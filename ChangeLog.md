# История #
| 2012/10/15 | <a href='http://code.google.com/p/nekopaw/downloads/detail?name=graber11021.zip'>1.1.0.21</a><br />- добавлена опция, позволяющая качать с e/ex-hentai по ссылке альбома. Для этого надо поставить галочку "Album URL" и в поле tags вставить ссылку на альбом. |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 2012/10/12 | 2.0.1.17<br />- исправлен баг, из-за которого в режиме "страница за страницей" загрузка страниц могла внезапно остановиться по середине работы;<br />- добавлен режим получения расширения файла из его содержимого. Нужен если больше нет никаких способов узнать расширение файла. Из-за отсутствия возможности догрузки на большинстве ресурсов (т.е. нельзя прочесть только нужное число байтов), закачка предварительно происходит в память, а затем на винт. Если же докачка работает, то загрузка будет происходить как обычно;<br />- добавлен ресурс seiga.nicovideo.jp. Включена обязательная авторизация; |
| 2012/10/01 | 2.0.1.16<br />- в hentai-foundry теперь работает "дополнительный" фильтр. Теперь можно фильтровать картинки на странице автора без авторизации;<br />- добавлена индикация процесса на панели задач для windows 7;                                              |
| 2012/09/28 | 1.1.0.20<br />- исправлена скачка с exhentai.org ([issue #74](https://code.google.com/p/nekopaw/issues/detail?id=#74));                                                                                                                                         |
| 2012/09/28 | 2.0.1.15<br />- добавлен дополнительный режим поиска на hentai-foundry: теперь можно качать со страницы профиля пользователя. Для этого нужно переключить search mode на by user profile и в поле tags указать имя пользователя (осторожно, регистрозависимый) ([issue #34](https://code.google.com/p/nekopaw/issues/detail?id=#34));<br />- добавлен ресурс furaffinity.net. Можно качать все типы контента (пикчи, текст, флэш, музка). Можно качать со страницы поиска, галереи пользователя, избранных пользователя. Стив, извини, что так долго :) |
| 2012/09/21 | 2.0.1.14<br />- добавлена возможность создавать сложные дополнительные условия для поиска на бордах (с несколькими полями на 1 параметр);<br />- исправлена работа hentai-foundry в соответсвии с новой механикой, в т.ч. добавлен фильтр по автору;            |
| 2012/09/09 | 2.0.1.13<br />- исправлен баг скачки изображений в browse режиме с nabyn.com, а так же листание страниц в нем же;<br />- добавлен hentai-foundry.com;<br />- добавлен strict режим на zerochan.net;                                                             |
| 2012/10/01 | 2.0.1.16<br />- в hentai-foundry теперь работает "дополнительный" фильтр. Теперь можно фильтровать картинки на странице автора без авторизации;<br />- добавлена индикация процесса на панели задач для windows 7;                                              |
| 2012/09/28 | 1.1.0.20<br />- исправлена скачка с exhentai.org ([issue #74](https://code.google.com/p/nekopaw/issues/detail?id=#74));                                                                                                                                         |
| 2012/09/28 | 2.0.1.15<br />- добавлен дополнительный режим поиска на hentai-foundry: теперь можно качать со страницы профиля пользователя. Для этого нужно переключить search mode на by user profile и в поле tags указать имя пользователя (осторожно, регистрозависимый) ([issue #34](https://code.google.com/p/nekopaw/issues/detail?id=#34));<br />- добавлен ресурс furaffinity.net. Можно качать все типы контента (пикчи, текст, флэш, музка). Можно качать со страницы поиска, галереи пользователя, избранных пользователя. Стив, извини, что так долго :) |
| 2012/09/21 | 2.0.1.14<br />- добавлена возможность создавать сложные дополнительные условия для поиска на бордах (с несколькими полями на 1 параметр);<br />- исправлена работа hentai-foundry в соответсвии с новой механикой, в т.ч. добавлен фильтр по автору;            |
| 2012/09/09 | 2.0.1.13<br />- исправлен баг скачки изображений в browse режиме с nabyn.com, а так же листание страниц в нем же;<br />- добавлен hentai-foundry.com;<br />- добавлен strict режим на zerochan.net;                                                             |
| 2012/09/01 | 2.0.1.12<br />- исправлено несколько мелких багов, из-за которых периодически парс страничек происходил криво;<br />- на nabyn.com исправлена скачка изображений, у которых на странице картинки нет ссылки на картинку;<br />- на nabyn.com теперь работает режим поиска "browse"; |
| 2012/08/31 | 2.0.1.11<br />- добавлен режим скачки "страница за страницей", позволяющий качать страницы, не зная заранее их общее количество;<br />- в связи с вводом нового режима, был добавлен первый тестовый ресурс nabyn.com;<br />- теперь после каждого завершения загрузки списка пополняется общий пул тэгов, хранящийся в обычном текстовом файле tagsdump.txt;<br />- теперь при вводе тэга появляется список похожих вариантов для быстрой вставки. Тэги берутся из общего пула, так что первое время тэги могу и не найтись;<br />- сохраняется список последних пяти использовавшихся в редакторе формата имени путей;<br />- все настройки ресурсов теперь сохраняются после завершения списка; |
| 2012/08/10 | 2.0.1.10<br />Без особо заметных обновлений. Продолжение борьбы с [issue #69](https://code.google.com/p/nekopaw/issues/detail?id=#69).                                                                                                                          |
| 2012/08/03 | 2.0.1.9<br />- исправлен баг с санками, вызывающий ошибку при добавлении тэгов, содержащих двойные ковычки (i"s);<br />- попытался исправить проблему с плавающей ошибкой System Error. Code: 5 (ВНЕЗАПНО появилась там, где ее никогда не было);<br />- подправлен баг с изоляцией несуществующих ключей и параметров; |
| 2012/07/30 | 2.0.1.8<br />Добавлены новые ключи для формата пути:<br />- $nn$ - порядковый номер изображения в списке;<br />- $fn$ - порядковый номер в том случае, если имя уже занято;<br />- $fnn`[`(N)`]`$ - порядковый номер относительно директории, в которой указан ключ. Параметром N можно указать, сколько раз повторять число;<br />- $tags`[`(N)`]`$ - тэги изображения. N - количество тэгов, по умолчанию все. Строка ограничена 200 символами, обычная длинна имени файла ~245 символов, так что не увлекайтесь;<br />+ примеры использования новых ключей см. в wiki;<br />- исправлены некоторые баги с торможением и подвисанием при закачке;<br />- прогресс теперь не исчезает после завершения или приостановки закачки. Так же у всех значков статусов теперь есть текстовые аналоги в фильтре;<br />- добавлена горячая кнопка CTRL+W, которая закрывает вкладку; |
| 2012/07/20 | 2.0.1.7<br />- добавлен визуальный редактор для правил поиска дублей (подробнее см. вики). Для него создан соответствующих раздел "Даблы" в настройках;<br />- поиск дублей теперь умеет делать проверку выполнимости нескольких условий для одного правила (т.е. чтобы, например, совпадение происходило по 3м полям, и если хотя бы по одному из них совпадения не будет, то условие выполнено не будет);<br />- исправлен баг с зависанием окна при пропуске большого количества файлов;<br />- добавлена опция, позволяющая перед началом закачки сразу снять галочки со всех элементов списка, которые не соответствую правилам фильтра (т.е. которые не видно в таблице после фильтрации). См. общие настройки ресурсов в настройках или дополнительные возможности на экране таблицы;<br />- исправлена проблема с пробелами в названиях тэгов на derpiboo; |
| 2012/07/17 | 2.0.1.6<br />- теперь программа запоминает размер окна;<br />- запоминает вкладку и ширину боковой панели;<br />- запоминает последний раз использовавшийся набор группировок и столбцов;<br />- исправлена проблема, из-за которой не появлялся список изображений для sankakucomplex;<br />- исправлена проблема с тегами у minitokyo; |
| 2012/07/11 | 2.0.1.5<br />Сделал небольшую паузу в работе над добавлением новых ресурсов и взялся за доработку интерфейса:<br />- исправлен баг, из-за которого не все надписи менялись при изменении языка и нажатии "применить";<br />- добавил кнопку на против "основных" настроек в создании списка. С ее помощью можно убрать из списка все борды;<br />- теперь список, который использовался последний раз, сохраняется;<br />- добавлены быстрые кнопки для путей и ссылок на панели информации об изображении. В поле "путь сохранения" можно сразу открыть изображение программой просмотра по умолчанию (лупа) и открыть каталог с изображением (папка), а так же можно открывать ссылки браузером по умолчанию (лупа);<br />- теперь можно делать описания для полей изображений с возможностью использовать разные языки. Теперь у всех полей изображений есть описание в редакторе формата имени;<br />- добавлен rule63.paheal.net; |
| 2012/07/05 | 2.0.1.4<br />- доделал функционал для работы с бордами вроде minitokyo.net. Можно выбирать, откуда качать арт (wallpapers, indy art, scans), а так же указывать, стоит ли качать все доступные размеры, или только первый доступный (т.е. самый большой);<br />- косметика по мелочи;<br />- подправил проблему с папкой log ([issue #67](https://code.google.com/p/nekopaw/issues/detail?id=#67)), но обещать, что она больше не будет возникать, не буду; |
| 2012/06/27 | 2.0.1.3<br />- добавил простенький редактор для создания пути сохранения, в нем можно посмотреть (или подставить) все доступные переменные и поля изображений (поля пока что без подсказок). Безусловно, переменные можно вообще не использовать, просто указать путь, где сохранять;<br />- добавлен cosplay.paheal.net;<br />- добавлен rule34.paheal.net;<br />- добавлен tentaclerape.net; |
| 2012/06/25 | 2.0.1.2<br />- починил авторизацию на бордах с необязательной авторизацией со страницы настроек;<br />- в ресурсах выставил максимально возможное количество страниц ([issue #65](https://code.google.com/p/nekopaw/issues/detail?id=#65));<br />- реализовал возможность добавлять свои поля на стройках борды для использования в скрипте. В следствии чего на rmart.org теперь можно выставлять рейтинг и отображение пикч без рейтинга; |
| 2012/06/22 | 2.0.1.1<br />- начал вести краткий лог с изменениями в текстовом файле versionlog.txt, который будет обновляться в папке программы. В настройках появилась опция, позволяющая включать отображение содержимого этого файла после каждого обновления;<br />- исправил баг в обработке куки, из-за которого перестал логиниться donmai.us ([issue #64](https://code.google.com/p/nekopaw/issues/detail?id=#64));<br />- исправил проблему, из-за которой не работала авторизация на всех остальных бурах (т.е. тех, где авторизация не обязательна). Замечу, что я по меря добавления борд реализую авторизацию на КАЖДОЙ из них (в отличии от старой версии, где это было довольно геморройным);<br />- добавлен zerochan.net;<br />- добавлен rmart.org. Чуть позже допилю возможность выбирать рейтинг скачиваемого и поиск без рейтинга;<br />- добавил к бордам, где есть возможность выдергивать размер изображений, отношение ширины к длинне, назвал не иначе как "aspect\_ratio" (соотношение сторон) ([issue #65](https://code.google.com/p/nekopaw/issues/detail?id=#65)). По этому полю можно искать изображения определенной формации ака 16:9, 16:10, 4:3 и т.д. Чтобы узнать, какую цифру нужно искать, просто поделите ширину на высоту в соотношении (например 16:9 = 16/9 = ~1.78). Замечу, что при делении чаще всего получаются очень длинные дробные числа, поэтому лучше искать в диапазоне (напр. 1.77-1.79). В дальнейшем я попробую упростить поиск по соотношению сторон. |
| 2012/06/21 | 2.0.1.0<br />Вот и начался отсчет по новой. Новый более менее стабильный релиз, выпуск которого окрещен достаточно расширившимся функционалом для ограбления ресурсов без API и т.п. радостей цивилизации.<br />- в связи с этим добавилось 3 борды: ii.booru.org, lolibooru.com и ponibooru.413chan.net. Со временем создам конфиги для всех имеющихся в данный момент в старой версии борд (за исключением тех, что требуют реализации закачки альбомов, это ожидается только в следующем релизе).<br />Отдельно замечу то, что в большинстве случаев безАПИшные борды не дают возможности на лету получать дополнительную информацию, вроде Ширины, Высоты, Авторе и т.д., не говоря уже о возможности получения MD5 для отсеивания дублей. Sad but true.|
| 2012/06/19 | 2.0.0.21<br />- наследуемый путь теперь корректно изменяется при листании страниц с ресурсами ([issue #58](https://code.google.com/p/nekopaw/issues/detail?id=#58));<br />- в общих настройках ресурсов появилась возможность указать, нужно ли начинать закачку сразу после завершения списка ([issue #60](https://code.google.com/p/nekopaw/issues/detail?id=#60));<br />завершенные ресурсы во время скачки теперь скрываются из списка ресурсов ([issue #57](https://code.google.com/p/nekopaw/issues/detail?id=#57)). |
| 2012/06/15 | 2.0.0.20<br />- исправлен баг конвертирования UString в Double ([issue #54](https://code.google.com/p/nekopaw/issues/detail?id=#54));<br />- исправлен баг, из-за которого не работала авторизация ([issue #55](https://code.google.com/p/nekopaw/issues/detail?id=#55));<br />- теперь можно фильтровать по полю "прогресс" ([issue #57](https://code.google.com/p/nekopaw/issues/detail?id=#57));<br />- исправлено "подвисание" при масштабном пропуске картинок в списке ([issue #56](https://code.google.com/p/nekopaw/issues/detail?id=#56)); |
| 2012/06/14 | 2.0.0.19<br />- добавил возможность массовой расстановки галочек в списке ([issue #48](https://code.google.com/p/nekopaw/issues/detail?id=#48)). Появилось 2 новых пункта - "выбрать" и "убрать". Можно выбрать "все", "выделенное" и "отфильтрованное", а так же "инвертировать".<br />- добавил возможность задания формата для ключей, используемых при создании имени файла ([issue #45](https://code.google.com/p/nekopaw/issues/detail?id=#45)). Формат зависит от типа значения. Если это дата, то будет использоваться формат времени, если же строка или число, то строчно-числовой. Подробностями см. в вики. Пример: %posted:yyyy-mm-dd%, где posted - поле, в котором хранится дата добавления изображения;<br />- кроме того добавил проверку для имен файлов. Многие люди впадают в ступор от необходимости указывать формат файла ($ext$), поэтому я сделал так, чтобы если формат не указан, то он добавляется автоматически (зы: форматом файла считается все, что идет после точки в имени файла). Также если имя файла не было указано, то будет использоваться стандартное $fname$.$ext$; |
| 2012/06/13 | 2.0.0.18<br />- Теперь можно сохранять настройки для каждой отдельной борды (в разделе настроек -> ресурсы). Можно сохранить логин и пароль чтобы не надо было вводить его каждый раз. Пароль сохраняется в profile.ini в зашифрованном виде;<br />- в разделе настроек "основное" теперь можно отключить автопроверку обновлений. Там же есть кнопка "проверить сейчас".<br />1.1.0.19<br />- исправлена проблема с pixiv ([issue #52](https://code.google.com/p/nekopaw/issues/detail?id=#52)). |
| 2012/06/09 | 2.0.0.17<br />- авторизация. Она теперь работает. В связи с чем со спокойной душой добавил donmai.us (старый danbooru) в список. Как я раньше уже говорил, на данбуре запретили пользоваться API без авторизации. Программа пока не умеет сохранять пресеты для ресурсов, поэтому пока что придется вводить логин/пароль каждый раз заново (1 раз после запуска программы и первом запуске скачки с ресурса). В теории также авторизация поддерживается на всех остальных шаблонных бордах. Чтобы авторизоваться надо указать логин и пароль (если не указать хотя бы логин программа посчитает, что нужно войти анонимно). |
| 2012/06/04 | 2.0.0.16<br />- подправил закачку по протоколу https (yande.re,wildcritters.net);<br />1.1.018<br />- исправил скачку с xbooru;<br />- исправил скачку с zerochan (хотфикс [issue #43](https://code.google.com/p/nekopaw/issues/detail?id=#43)).                |
| 2012/04/03 | 1.1.0.17<br />- oreno.imouto.org больше нет, удалил;<br />- добавил yande.re. У них используется протокол HTTPS, так что возможно потребуется скачать библиотеки OpenSSL (см. страницу загрузок);<br />- исправил скачку с rule34.paheal.net;<br />- исправил загрузку не всех альбомов с pixiv.net. |
| 2012/03/16 | 2.0.0.15 (гугл глючит, поэтому апдейт может стать доступным не сразу)<br />- провел стресстест на 20 потоках по 6 ресурсам в размере 544 пикч (хотя мои интернеты не очень пригодны для таких заездов, впрочем, только лучше для тестирования). По результатам теста пофиксил несколько глюков отображения, ошибок "самоотключения" и их зацикливание. В общем, последний тест, прошел успешно, за мелкими исключениями. "Повисшие" скачки в итоге можно просто остановить и начать заново (было 2 таких скачки из 3х тестов);<br />- переделал отображение прогресса, теперь отображается статус (ОК/СКИП/ЕРР и т.д.), позже сделаю, чтобы в процессе таки прогресс выглядел как прогрессбар, а не просто текст;<br />- прикрутил "жесткую" остановку процесса. Для этого надо нажать стоп, и через 5 секунд нажать стоп еще раз;<br />- все jpeg файлы теперь автоматически переименовываются в jpg (у меня использовался %md5%.%ext% формат, а повторы все равно получались, оказалось из-за разницы в одной букве в расширении); <br />- переделал раздел настроек. Язык теперь можно выбрать в настройках. Настройки теперь применяются ко всем вкладкам (точнее, они обновляются каждый раз, когда начинается работа, т.е. прямо в процессе никаких изменений не будет, и не нужно); |
| 2012/03/14 | 1.1.0.16<br />- добавил возможность расставлять опции поиска в е/эксхентае (кнопка options). Можно выбрать, какой контент искать и как (в именах галерей или в тегах);<br />Продинамил описание 1.1.0.15<br />- исправлена скачка с гелбуру;<br />Кроме того отклеилась имоута (из-за переезда на яндере), залью с фиксом позже. |
| 2012/03/13 | 2.0.0.14<br />- исправлена проблема со скачкой с yande.re (добавлена возможность создавать referer-метку);<br />- добавлены chan. и idol.sankakucomplex.com (реализован парс json);                                                                             |
| 2012/03/11 | 2.0.0.12<br />- добавил некоторую индикацию по работе ресурсов (какая страница обрабатывается, сколько пикч скачано с ресурса);<br />- имоута переехала на яндере. На яндере запретили "скачку фулсайзов" (при попытке открыть пикчу напрямую или нажать "download full size" происходит редирект на страницу семплов), поэтому скачка с яндере пока не работает (скачиваются html-файлы вместо пикч);<br />- пофиксил скачку с вилдов, заодно поставил жесткое HTML-кодирование строки тегов.<br />- к апдейтеру прикрутил опцию удаления старых файлов (напр. старый конфиг имоуты); |
| 2012/03/06 | Залил 2.0.0.8 билд (самообновление):<br />- изменил способ хранения пикч, в связи с чем доделал поиск дублей. Теперь он происходит прямо в процессе получения списка;<br />- оптимизировал отображение таблицы;<br />- детали пикчи при нескольких вкладках больше не мерцают;<br />- изоляция в форматах имен исправлена;<br />см. [issue #32](https://code.google.com/p/nekopaw/issues/detail?id=#32) |
| 2012/02/28 | Залил даунлойдер, который в то же время и апдейтер. Он скачает саму последнюю версию кошкограббера (в текущий момент это злостная альфа с кучей неработающих функций).                                                                                          |
| 2012/02/17 | 2я знаменательная дата в истории кошкограббера. Сегодня успешно прошла закачка пикч по полученному списку. Доделаю индикацию процесса, прикручу апдейтер, заклею дырки жвачкой, и можно будет выложить первую сырую альфочку :3                                 |
| 2012/02/10 | Gtaber 1.1.0.14:<br />- прикрутил авторизацию на devianart'е. Тем не менее особенной разницы, что и без авторизации, нет. Для входа надо указать хотя бы логин, иначе загрузка начнется анонимно. Воход происходит по HTTPS, поэтому придется скачать и скинуть в папку с программой библиотеки OpenSSL (см. раздел загрузок);<br />- прикрутил окошко с 10 сек паузой при возникновении баннера на гелбуре. |
| 2012/02/06 | Graber 1.1.0.13:<br />- баннер в GUI gelbooru.org теперь благополучно пропускается ;<br />- с deviantart.com теперь в первую очередь качаются фуллсайзовые картинки ;<br />- таймауты теперь можно настроить. 0 = без таймаута.                                 |
| 2012/01/28 | Новый билд Graber 1.1.0.12<br />- Пофиксил скачку с thedoujin. На doujin`е теперь больше нет тэгов для каждой отдельной пикчи;<br />- попробовал пофиксить обрезки и заблокированные пикчи при насильной остановке;<br />- чуть прокачал обработку ошибки 509 на e/exhentai;<br />- ошибки о нехватке GP и 509 на e/exhentai теперь будут корректно отображаться;<br />- установил дополнительные жесткие таймауты на подключение (5сек) и скачку (10сек). Таймаут подразумевает, что в течении этого времени не было _никакого_ ответа (предположительно подвисло);<br />- пофиксил визуальные глюки при возникновении ошибки или изменении ссылки на пичку (надписи появлялись только на первой строке, а не там, где должны); |
| 2012/01/21<br /><img src='http://img502.imageshack.us/img502/9332/doublesguy.jpg'> <table><thead><th> Залил Graber 1.1.0.11:<br />- выключил возможность не включать интервал запросов (query interval) для е/эксхентай;<br />- выключил возможность не включать интервал запросов между страницами (before getting url) для е/эксхентай;<br />- поставил минимальный интервал = 1;<br />- теперь интервал можно указывать в долях секунд (дробным числом);<br />- добавил обработку предупреждения о слишком быстром листании страниц для е/эксхентай;<br />- добавил обработку "Ваш IP временно заблокирован" для е/эксхентай;<br />- добавил обработку закончившихся GP для е/эксхентай;<br />- добавил обработку пикчки ошибки 509 (наверное, для сравнения использовал размер и MD5 файла). Если все-таки кто-то скажет URL на эту пикчку - буду благодарен.<br />/ казалось бы какие еще могут быть косяки со скачкой с е/эксхентай, но есть человек, который умудрился получить кучу одинаковых пикч с фоткой неизвестной тян азиатской внешности. Если кто-то еще столкнется с подобным - хотелось бы узнать, что он для этого сделал.<br />- "переехал" rule34.booru.org на rule34.xxx;<br />- после ввода логина и пароля через "кнопку с ключиком" старые куки борды будут стерты. </th></thead><tbody>
<tr><td> 2012/01/18 </td><td> Новый релиз Graber 1.1.0.10 (Скорее хотфикс):<br />- оказалось, что за опцию "скачки фуллсайзов" через несколько пикч е/эксхентай начинает хотеть денег, поэтому прикрутил галку "fullsize" чтобы это можно было выключать нафиг (по умолчанию выключено);<br />- Говорят, что иногда начинает навязчиво происходить ошибка "You can not access a file directly without specifying a gallery. Please get the full URL for this image.", но сам я ее так и не смог поймать. Поэтому прокачал обработку этой ошибки в потоках... в общем, сами увидите, и если увидите - то сообщите. </td></tr>
<tr><td> 2012/01/14 </td><td> New Graber 1.1.0.9 release is available<br />- поправил скачку фуллсайзов с e/exhentai (<a href='https://code.google.com/p/nekopaw/issues/detail?id=#24'>issue #24</a>);<br />- добавил tbib.org (<a href='https://code.google.com/p/nekopaw/issues/detail?id=#25'>issue #25</a>);<br />- добавил tentaclerape.net (<a href='https://code.google.com/p/nekopaw/issues/detail?id=#25'>issue #25</a>); </td></tr>
<tr><td> 2012/01/14 WIP </td><td> Историческая дата проекта, ибо сегодня успешно был скачан первый список кошкограббером х) (<a href='https://code.google.com/p/nekopaw/source/detail?r=62'>r62</a>) [<a href='http://img40.imageshack.us/img40/8122/85969878.png'>?</a>]                         </td></tr>
<tr><td> 2012/01/03 </td><td> Залил билд 1.1.0.8<br />- сделал, чтобы рейтинг на стандартнобурах добавлялся в тэги и можно было фильтровать локально (<a href='https://code.google.com/p/nekopaw/issues/detail?id=#23'>issue #23</a>);<br />- сделал, чтобы можно было искать тэги (кнопка с лупой на вкладке метаданных);<br />- разлочил кнопки next, previous и goto в режиме скачки. </td></tr>
<tr><td> <img src='http://img233.imageshack.us/img233/6286/49182402.png'> </td><td> <b>Happy New Year</b><br /> Залил новый новогодний релиз первой версии грабера<br />- под корень перепилил работу с куками из-за неудачного переезда на Delphi XE. "Самая последняя версия" Indy, включенная в поставку, работает с куки через жопу (имена ресурсов с ведущей точкой и "www" не совпадали, некоторые ресурсы не понимали созданных вручную куков, напр. rmart), всвязи с чем пришлось делать ручную обработку. Зато теперь я на 100% уверен в том, как будет выглядеть кука. Судя по всему, я все ближе к написанию своего компонента для скачки;<br />- добавил авторизацию на zerochan.net и minitokyo.net. По дефолту входит в анонимном режиме, для авторизации надо указать как минимум логин (см. кнопку с ключем) (<a href='https://code.google.com/p/nekopaw/issues/detail?id=#22'>issue #22</a>);<br />- добавил флаг "запомнить меня" в pixiv`е чтобы продлить срок действия куков (из-за тупняка с русской отменой зимнего времени) (<a href='https://code.google.com/p/nekopaw/issues/detail?id=#21'>issue #21</a>);<br />- попытался решить проблему с недокачивающимися файлами, сделав проверку на размер файла после скачки пикчи. Тех, кто сталкивался с проблемой, отписаться после тестирования, т.к. сам я эту проблему никак не смог воспроизвести (<a href='https://code.google.com/p/nekopaw/issues/detail?id=#20'>issue #20</a>, <a href='https://code.google.com/p/nekopaw/issues/detail?id=#21'>issue #21</a>). </td></tr>
<tr><td> 2011/12/18 WIP </td><td> Что полезного было сделано на этих выходных: повозился с интерфейсом, разметил вкладочную систему и содержание соотвествующих форм; написал мат. процедуру, благодаря которой теперь в скрипте благополучно производятся все строковые, математикие и логические операции. Если в голову не взбредет ничего странного в течении следующей недели, то начну работу над "проектами" (набор "настройки закачки" + "настройки сохранения" + "пикчи" + "тэги" (для каждой борды отдельно в рамках одного проекта), а следом и механизм закачки. Побыстрее бы праздничные, надоело перебежками по 2 дня писать, хотет засесть на неделю-другую и все доделать до релиза. </td></tr>
<tr><td> 2011/12/11 WIP </td><td> итак, наконец-то хоть какое-то продвижение в работе над некопав граббером. Сегодня благополучно наладил минимальные условия для загрузки скрипта, создание списка скриптов, и, собственно, визуальное отображение этого списка. Еще предстоит прикрутить математический анализатор для обработки условий и определений значений, и можно будет начать работу над скачкой списка и пикч </td></tr>
<tr><td> 2011/12/10 </td><td> удалил архив с исходниками первой версии из загрузок, переместил все исходники в subversion, раздел /trunk/graber/. 2я версия теперь в /trunk/graber2/.                                                                                                         </td></tr>
<tr><td> 2011/12/07 </td><td> На pixiv'е снова поменялась разметка, поэтому заливаю новый релиз graber 1.1.0.6.                                                                                                                                                                               </td></tr>
<tr><td> 2011/12/04 </td><td> не прошло и суток, как заливаю новый билд 1.1.0.5. Прикрутил поддержку minitokyo.net.                                                                                                                                                                           </td></tr>
<tr><td> 2011/12/03 </td><td> новый билд graber 1.1.0.4 с новыми фиксами. Запилил <a href='FirstVersion.md'>полное описание</a> по первому граберу.<br />- пофиксил скачку rating:explicit на e621.net.                                                                                       </td></tr>
<tr><td> 2011/11/29 </td><td> последний апдейт graber 1.1.0.3 в этом месяце.<br />- добавил возможность качать по закладкам авторов с pixiv`а;<br />- галочка autoscroll сохраняется в настройках.                                                                                            </td></tr>
<tr><td> 2011/11/23 </td><td> развернул базу проекта на территории гугла чтобы больше не терроризировать автобус. Завтра залью исходники 1 версии.                                                                                                                                            </td></tr>