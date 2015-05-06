---
layout: doc
title: Редактирование в JOSM
permalink: /ru/beginner/more-about-josm/
lang: ru
category: beginner
---

Редактирование в JOSM
=====================
В предыдущем разделе вы установили JOSM и начали рисовать собственные первые
точки, линии и фигуры. Вы применяли шаблоны для того чтобы добавить информацию
об объектах. И в конце вы начертили собственную карту в JOSM

Вы достаточно попрактиковались и теперь готовы начать редактировать данные в
OpenStreetMap.

В этом разделе мы подробно ознакомимся с интерфейсом JOSM, и с тем как использовать его для создания карты OpenStreetMap.

Цикл редактирования
-------------------
Редактирование OpenStreetMap с помощью JOSM похоже на редактирование в iD, с
которым мы познакомились раньше. Но так как JOSM является отдельным
приложением, он работает несколько иначе. Процесс редактирования и добавления
объектов в OpenStreetMap с помощью JOSM всегда будет следующим:

1. **Загрузка** текущих данных из OSM
2. **Редактирование** данных с использованием спутниковых снимков, GPS,
    Обходных листов (Field Papers) и заметок в качестве подсказок
3. **Сохранение** изменений в OpenStreetMap

Загрузка данных OSM
----------------------
Первым шагом в редактировании является загрузка данных для участка, который вы
хотите улучшить. Помните, что это нужно делать каждый раз, когда вы хотите
изменить карту, так как данные часто обновляются другими участниками.

-	В меню “Файл” (“File”), сверху слева в JOSM, выберите “Скачать с OSM…” (“Download from OSM”). Будет открыто окно для загрузки. Вы также можете открыть это окно просто щёлкнув на значок загрузки на панели инструментов:

![JOSM Download Button][]

- Когда будет открыто окно загрузки вы увидите карту с розовым прямоугольником
  на ней. Если вы не видите карту, щёлкните вкладку “Карта” (“Slippy map”).

![JOSM Download Dialog][]

- Розовый прямоугольник показывает участок на карте, данные из которого будут
  загружены для редактирования. Воспользуйтесь мышью для передвижения и
  изменения масштаба карты до того места, которое вам хорошо известно,
  например, вашего города или района. Управление такое же как и на основной
  карте JOSM. Нажатием правой кнопкой мыши можно перемещать карту, а колёсиком
  изменять масштаб.

>	Если вы работаете на ноутбуке, иногда может быть трудно увеличивать и
> уменьшать масштаб. Работа в JOSM происходит значительно легче, если вы
> используете мышь, но современные ноутбуки позволяют выполнять эти же действия
> с помощью сенсорной панели.

-	Нарисуйте прямоугольник, вокруг места, которое вы хотите загрузить. Чтобы
  начертить прямоугольник заново, щёлкните на карте, нажмите и удерживайте
  левую кнопку мыши и потяните её для создания нового прямоугольника. Отпустите кнопку мыши для завершения выделения участка.
- Если размер и место выделенного участка вас удовлетворяют, нажмите на кнопку
  “Скачать” (“Download”) внизу окна. JOSM загрузит данные для выделенного
  участка с OpenStreetMap и откроет их в основном окне с картой для
  редактирования.

### Добавление снимков
Если вы прочитали предыдущие главы, когда мы добавляли наши первые точки с
помощью редактора iD, вы помните, что кроме данных карты присутствовали
спутниковые снимки, которые помогали нам определять объекты на местности. Эти
снимки предоставлены Microsoft Bing, сервисом который любезно предоставляет их
для участников OpenStreetMap для обрисовывания объектов и улучшение данных
карты.

-	Для добавления спутниковых снимков Bing в JOSM, выберите “Снимок” (“Imagery”) в основном меню JOSM, а затем - “Спутниковые снимки Bing” (“Bing Sat”).

> Если в вашем меню отсутствует пункт “Спутниковые снимки Bing” (“Bing Sat”),
> вам нужно активировать его в настройках JOSM. Перейдите Правка (Edit) ->
> Настройки (Preferences) и перейдите на вкладку “WMS TMS”. Возможно, вам
> придется поискать его в перечне.
>
>	![JOSM Preferences up down][]
>	![JOSM Preferences WMS TMS][]
>
> Выберите “Спутниковые снимки Bing” (“Bing Sat”). Нажмите “Активировать”
> (“Activate”).


### Обзор JOSM
Теперь у вас есть загруженные данные OpenStreetMap, а также слой со спутниковыми
снимками Bing, давайте еще раз посмотрим на интерфейс JOSM.

![JOSM layout][]

Главное окно, с которым вы уже познакомились, является окном карты в котором
происходит большинство действий. Здесь мы будем просматривать, изменять и
добавлять данные OpenStreetMap.

Справа от окна карты находится набор панелей, каждая из которых отвечает за
соответствующую функцию. Обычно, после процесса установки JOSM показывается
несколько типовых панелей, такие как Слои (Layers), Теги/Участие (Properties) и
Выделение (Selection). Когда вы выделяете точку, линию или фигуру на карте, они
появляются на панели Выделение (Selection). Информация показывается на панели
Теги/Участие (Properties), а на панели Авторы (Authors) показывается информация
об участниках, которые последними изменяли выделеные объекты.

Эти панели могут быть открыты или закрыты нажатием кнопок в нижней части панели
инструментов, слева от окна карты в JOSM. Над этими кнопками находятся
инструменты, которыми мы выбираем возможные действия, выполняемые мышью. Вы уже
знакомы с некоторыми из них: инструментом Выделение (Select tool) и
инструментом Рисование (Draw tool). Под ними инструменты, облегчающие
масштабирование, удаление объектов, рисование фигур, или черчение параллельных
линий.

Редактирование
--------------
И так, вы выполнили первый шаг процесса редактирования данных – загрузка. Вы
подготовили в JOSM фоновый слой со спутниковыми снимками, по которым мы будем
рисовать. Следующий шаг – редактирование карты и добавление новых объектов.

В зависимости от местности, которую вы выберете для редактирования, у вас может
быть много или мало внесенных ранее на карту данных. Но обратите внимание, что
это те же типы данных, с которыми мы познакомились ранее – точки, линии и
фигуры, которые представляют местность в реальной жизни.

-	Воспользуйтесь теми же приёмами, которые вы изучили, добавив несколько точек
  на карту в месте, которое хорошо вам известно. Если вы увидели ошибки,
  попробуйте исправить их.
-	Вы не должны слишком усердствовать пока вы учитесь. Если вы не уверены в
  чем-то лучше оставить всё как есть.
-	Если вам нужно передвинуть точку, линию или фигуру используйте инструмент
  **Выделение**. Щелкните на объект и перетащите его в нужное место. Этот прием
  используется для уточнения места положения объектов.

![JOSM select tool][]

-  Используйте инструмент **Рисование** для нанесения новых точек, линий и
  фигур. Описывайте объекты с помощью Заготовок (Presets) из соответствующего
  меню, так, как мы делали это в предыдущем разделе.

>	Никогда не изменяйте карту за пределами загруженных участков. Вы можете
> увидеть, что загруженный участок будет иметь сплошной фон, в то время как,
> незагруженный – будет иметь диагональную штриховку.
>
>	![JOSM area downloaded][]

Сохранение изменений
--------------------
Третий и финальный шаг, завершающий вашу работу – передача сделанных вами
изменений в базу данных OpenStreetMap. Для того, чтобы сохранить изменения
нужно подключиться к Интернету.

- Найдите в меню “Файл” (“File”) пункт “Передать данные на сервер…” (“Upload
  Data”). Появится окно отправки данных. Также его можно вызвать, нажав на
  кнопку отправки данных:

![JOSM Upload Button][]

- В окне отправки данных показывается перечень объектов, которые были
  добавлены, изменены или удалены вами. В нижней части окна вам будет
  предложено ввести описание ваших изменений. Добавьте его.

![JOSM Upload Dialog][]

- Нажмите “Передать изменения на сервер” (“Upload Changes”).

-	Если это ваш первый раз сохранения изменений в OpenStreetMap, вам будет
  предложено ввести ваш логин и пароль OpenStreetMap.
-	Введите их в следующем окне. Если вы поставите флажок, логин и пароль будут
  сохранены в настройках и вам не придется вводить их в будущем вновь. Нажмите
  “Аутентификация” (“Authenticate”).

![JOSM Authenticate][]

-	Вам нужно немного подождать пока ваши изменения отправляются, после чего можно считать, что работа завершена! Вы внесли изменения на карту OpenStreetMap.

>	При редактировании всегда проверяйте отправили ли вы изменения на сервер
> перед тем, как закрыть JOSM. Даже если вам нужно сделать еще много работы,
> отправляйте ваши изменения, чтобы потом вернуться и продолжить работу, когда
> у вас появится время. Вы же не хотите потерять результаты ваших стараний?!

Просмотр ваших правок на карте
------------------------------
-  Откройте ваш веб-обозреватель и перейдите на [http://openstreetmap.org/](http://openstreetmap.org/)
- Переместите карту в место, в котором вы вносили изменения.
- Вы должны увидеть, что ваши изменения появились на карте! Если их не видно,
  попробуйте перезагрузить страничку, нажав CTRL+R. Иногда карта не обновляется
  соответствующим образом и требует перезагрузки.
- Что делать, если вы не видите собственных изменений? Не волнуйтесь – нужно
  чтобы прошло несколько минут, чтобы изменения появились на карте. Также,
  проверьте ваши изменения в JOSM, чтобы убедиться, что вы все сделали верно.
  Общее правило гласит, если вы видите значок на точке в JOSM, то и на карте на
  сайте OpenStreetMap они должны также показываться.

Итоги
-----
Теперь, после того, как вы увидели, как добавлять данные в OpenStreetMap, что
делать дальше? Что ж, редактирование данных – это хорошо, но только им создание
карт не ограничивается. Конечно теперь вам нужно узнать, как в полевых условиях
собирать информацию об объектах на местности.

В следующих главах мы узнаем о двух методах – GPS и Обходные листы (Field
Papers), которые используются для сбора картографической информации.
Информацию, полученную с помощью этих методов можно импортировать в JOSM и
использовать при редактировании карты.

Продвигаемся дальше
-------------------

Перейдите по следующим ссылкам, чтобы узнать об:  

*  [Использовании GPS](/ru/beginner/using-gps/)  
*  [Обходных листах (Field Papers)](/ru/beginner/field-papers/)
*  [Редактировании собранных данных](/ru/beginner/editing-with-josm/)


[JOSM Download Button]: /images/en/beginner/04_more-about-josm/eng_beg_04_more-about-josm_image00_download-button.png
[JOSM Download Dialog]: /images/en/beginner/04_more-about-josm/eng_beg_04_more-about-josm_image01_download-dialog.png
[JOSM Preferences up down]: /images/en/beginner/04_more-about-josm/eng_beg_04_more-about-josm_image02_preferences-up-down.png
[JOSM Preferences WMS TMS]: /images/en/beginner/04_more-about-josm/eng_beg_04_more-about-josm_image03_preferences-wms-tms.png
[JOSM layout]: /images/en/beginner/04_more-about-josm/eng_beg_04_more-about-josm_image04_layout.png
[JOSM select tool]: /images/en/beginner/04_more-about-josm/eng_beg_04_more-about-josm_image05_select-tool.png
[JOSM area downloaded]: /images/en/beginner/04_more-about-josm/eng_beg_04_more-about-josm_image06_area-downloaded.png
[JOSM Upload Button]: /images/en/beginner/04_more-about-josm/eng_beg_04_more-about-josm_image07_upload-button.png
[JOSM Upload Dialog]: /images/en/beginner/04_more-about-josm/eng_beg_04_more-about-josm_image08_upload-dialog.png
[JOSM Authenticate]: /images/en/beginner/04_more-about-josm/eng_beg_04_more-about-josm_image09_authenticate.png