# О продукте

ПО **NLP Analytics** (наименование программы для ЭВМ по продукту **WordPulse**) используется для просмотра и анализа любого вида коммуникаций с клиентами. Результаты анализа позволяют выработать дальнейшее понимание того, как улучшить работу ботов и / или операторов.

ПО **NLP Analytics** устанавливается у заказчика силами сотрудников правообладателя или партнера.

# Начало работы

## Авторизация 

Чтобы начать работу с веб-клиентом **NLP Analytics**, выполните следующие действия:

1. Откройте адрес клиента в браузере,
2. Когда появится окно авторизации, введите данные вашей учетной записи (имя пользователя и пароль) или войдите через MTS ISSO.

При успешной авторизации откроется главная страница веб-клиента.

![](https://raw.githubusercontent.com/mts-ai/wordpulse/main/pictures/1.1.Start/1_Start.png)

## Импорт сессий

Чтобы посмотреть и проанализировать сессии клиентов, необходимо импортировать логи сессий вручную, либо настроить автоматический импорт из различных систем заказчика.

После добавления логов веб-клиент анализирует их и показывает результаты анализа в соответствующих разделах.

## Разделы NLP Analytics

ПО **NLP Analytics** состоит из трёх разделов:

1.  Раздел **Аналитика**, в котором Вы можете:
    - посмотреть содержимое сессий, применить различные фильтры для отображения только интересующих вас сессий во вкладке **Сессии**,
    - посмотреть результаты анализа по различным метрикам во вкладке **Метрики**,
    - посмотреть визуализированные результаты аналитики в динамике во вкладке **Дашборды**,
2.  Раздел **Настройка**, в котором Вы можете создать скрипты, словари и теги в соответствующих вкладках для маркирования сессий по заданным условиям,
3.  Раздел **Администрирование**, в котором можно управлять доступами других пользователей, группами и т.д.

# Раздел Аналитика

## Сессии

Веб-клиент анализирует загруженные логи и отображает все сессии клиентов на вкладке **Сессии**.

![](https://raw.githubusercontent.com/mts-ai/wordpulse/main/pictures/1.2.Sessions/1_Sessions.png)

В строке каждой сессии доступна следующая информация:

- ID сессии,
- время начала сессии,
- имя оператор и клиента,
- количество сообщений за всю сессию,
- сентимент - тональность сессии (позитивная / нейтральная / негативная).

Также можно посмотреть параметры каждой реплики: информацию о дате и времени реплики, тональности и добавленных к реплике тегах.

### Точки перелома тональности реплики

Возле каждой реплики клиента, оператора / бота находится иконка-смайлик, которая показывает тональность реплики. Расчет тональности происходит по голосу и по тексту. Если тональность сообщений клиента изменяет свой характер (например, переходит с позитивного на нейтральный или в негативный) вне зависимости от наличия реплик оператора / бота, то рядом с сообщением отобразится точка перелома в виде иконки-стрелки.

![](https://raw.githubusercontent.com/mts-ai/wordpulse/main/pictures/1.2.Sessions/13_Bad_dialogue_tone.png)

### Аналитика по NPS

На вкладке **Сессии** пользователь может просматривать метрики удовлетворенности клиентским сервисом, например, NPS - показатель приверженности потребителей товару или компании.

![](https://raw.githubusercontent.com/mts-ai/wordpulse/main/pictures/1.2.Sessions/14_tNPS.png)

## Применение фильтров

С помощью различных фильтров можно отобразить только те сессии, которые вас интересуют. Вы можете фильтровать сессии, например, по:

- наличию/отсутствию слов и фраз,
- тону общения и точкам перелома тональности,
- по индексу потребительской лояльности,
- по тематике, параметрам сессии,
- количеству реплик участников сессии.

![](https://raw.githubusercontent.com/mts-ai/wordpulse/main/pictures/1.3.Filter/2_Sidebar.png)

Чтобы каждый раз заново не выбирать нужные параметры для фильтрации, можно создать набор наиболее часто используемых фильтров (сет фильтров).

## Применение запросов

С помощью запросов можно формировать выборки сессий с несколькими уровнями детализации и просматривать статистику по ним.

![](https://raw.githubusercontent.com/mts-ai/wordpulse/main/pictures/1.4.Request/1.Sidebar_requests.png)

### Сравнение фильтров

Чтобы найти интересную для дальнейшего анализа лексику, можно воспользоваться сравнением запросов.

![](https://raw.githubusercontent.com/mts-ai/wordpulse/main/pictures/1.4.Request/15_Matching_words.png)

В каждом запросе отобразятся "Топ слов" или "Топ фраз", количество сессий, в которых эти слова встречаются, и процентное соотношение от общего числа сессий.

### Экспорт сессий

Проанализированные сессии можно экспортировать в файл формата CSV. Это может понадобиться, если необходимо, например, выгрузить сессии за один день, только с определенным клиентом и / или посмотреть сентимент по сессиям.

## Метрики

Результаты анализа сессий можно посмотреть на вкладке **Метрики**.

![](https://raw.githubusercontent.com/mts-ai/wordpulse/main/pictures/2.Metric/4_Metrics.png)

Меню над графиком и боковая панель фильтров позволяет менять отображение графика под нужды пользователя.

### Типы метрик

Анализ проводится по различным метрикам и отображается в виде графика. На текущий момент существует 5 типов метрик:

- **Дефолтная**: позволяет проанализировать сессии по различным параметрам (точный набор доступных метрик зависит от реализации продукта под конкретного заказчика);

![](https://raw.githubusercontent.com/mts-ai/wordpulse/main/pictures/2.Metric/5_Default.png)

- **Сентимент анализ**: анализирует сессии по тону общения, например:
  - **Net sentiment** - разница между сессиями с позитивным и негативным сентиментом,
  - **Доля сессий с переломами**: отношение количества сессий, в которых есть точки перелома, к общему числу сессий.

- **Семантический анализ**: используется для определения ключевых слов и фраз, а также частоты их появления в сессиях.

![](https://raw.githubusercontent.com/mts-ai/wordpulse/main/pictures/2.Metric/7_Semantic_words.png)

- **ABSA**: аспектно-ориентированный анализ настроений, позволяющий выделять:
  - **Аспекты**: сущности, отношение к которым оценивает участники сессии,
  - **Оценки**: слова или словосочетания, определяющие отношение к аспекту,
  - **Тональность аспектов**: качественная характеристика оценки аспекта (позитивный, негативный).

![](https://raw.githubusercontent.com/mts-ai/wordpulse/main/pictures/2.Metric/11.3_ToneABSA.png)

- **Голосовая**: позволяет проанализировать сессии с аудиозаписью по различным параметрам.

![](https://raw.githubusercontent.com/mts-ai/wordpulse/main/pictures/2.Metric/12_Voice_metric.png)

### Экспорт графиков

Любой график и облако слов / фраз вкладки **Метрики** можно скачать в формате PNG. Кроме того, все сессии, входящие в графики из раздела дефолтных метрик, сентимент анализа и голосовых метрик, можно скачать в CSV формате.

## Дашборды

Дашборды служат для визуализации результатов аналитики с помощью различных метрик на одном экране. В каждый дашборд можно добавить до четырех графиков для анализа.

![](https://raw.githubusercontent.com/mts-ai/wordpulse/main/pictures/3.Dashboard/1_Dashboards.png)

# Раздел Настройки

## Скрипты

Скрипты описывают то, как будут анализироваться сессии для выполнения конкретной бизнес-задачи.

![](https://raw.githubusercontent.com/mts-ai/wordpulse/main/pictures/6.Script/1_Scripts_edit.png)

Скрипт состоит из **Входных условий** и **Правил**.

![](https://raw.githubusercontent.com/mts-ai/wordpulse/main/pictures/6.Script/2_New_script_window.png)

## Словари

Словари могут использоваться в фильтре поиска, а также при создании условий внутри скрипта, например, условия на содержание в сессии тех или иных элементов из словаря.  

![](https://raw.githubusercontent.com/mts-ai/wordpulse/main/pictures/4.Dict/1_Dictionary.png)

Значения в словаре можно импортировать и экспортировать в формате CSV.

![](https://raw.githubusercontent.com/mts-ai/wordpulse/main/pictures/4.Dict/7_New_words_to_dict.png)

## Теги

Тег – сущность, в которой хранится дополнительная информация о сессии.

![](https://raw.githubusercontent.com/mts-ai/wordpulse/main/pictures/5.Tag/4_Two_tags.png)

Тег может быть связан с сессией или с конкретными фразами внутри неё.

![](https://raw.githubusercontent.com/mts-ai/wordpulse/main/pictures/5.Tag/8_Tag-on-dialog.png)

# Раздел Администрирование

В разделе Администрирования пользователь может управлять доступами других пользователей, группами, ролями и воркспейсами.

![](https://raw.githubusercontent.com/mts-ai/wordpulse/main/pictures/7.Admin/1_Administration.png)