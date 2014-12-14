## Словарь терминов

Список определений закрепленных в терминологии БЭМ.

| Термин | Определение | Пример упоминания в документации |
| ----------- | ------------------- | -------------------- |
| <a name="base_tech"></a>**Базовая технология** | [Node.js](http://nodejs.org/)-модуль, с помощью которого инструмент [bem-tools](#bem-tools) реализует свою базовую функциональность. Может быть переопределен с помощью [модулей технологий](#tech_module). | [Модули технологий](http://ru.bem.info/tools/bem/bem-tools/tech-modules/#Особенности-архитектуры-пакета-bem-tools) |
| <a name="base_tech_com"></a>**Базовая технология команды** | Цепочка методов [базовой технологии](#base_tech), вызываемых в процессе выполнения конкретной команды. | [Модули технологий](http://ru.bem.info/tools/bem/bem-tools/tech-modules/#Приложение-3--Базовая-технология-bem-tools) |
| <a name="bundle"></a>**Бандл** | Набор итоговых [файлов технологий](#file_tech), собранных из файлов технологий [блоков](#block), составляющих отдельную функциональную часть сайта. | [Модули технологий](http://ru.bem.info/tools/bem/bem-tools/tech-modules/#Особенности-архитектуры-пакета-bem-tools) |
| <a name="bundle_tech"></a>**Бандл технологии** | Отдельный файл [бандла](#bundle), соответствующий конкретной технологии. | [Модули технологий](http://ru.bem.info/tools/bem/bem-tools/tech-modules/#Технологии-в-bem-tools) |
| <a name="block"></a>**Блок** | Часть дизайна страницы со своим специфическим и уникальным значением, определенным семантически или визуально (к примеру, шапка сайта или форма поиска). | [Единая предметная область](http://ru.bem.info/method/definitions/#Единая-предметная-область) |
| <a name="block-mix"></a>**Блок-микс** | [Блок](#block), не участвующий в цепочке наследования. | [Блоки-миксы](http://ru.bem.info/technology/i-bem/current/i-bem-js/#Блоки-миксы) |
| <a name="bem-tree"></a>**БЭМ-дерево** | Структура [БЭМ-сущностей](#entity) страницы, учитывающая их вложенность (обычно описывается в формате [BEMJSON](#bemjson)). | [Средства описания страницы](http://ru.bem.info/method/definitions/#Средства-описания-страницы-и-шаблоны) |
| <a name="bem_not"></a>**БЭМ-нотация** | JavaScript-объект, обозначающий [БЭМ-сущность](#entity) и участвующий в формировании ее строкового представления. | [BEMHTML](http://ru.bem.info/technology/bemhtml/2.3.0/rationale/#HTML-CSS-—-ассемблер-для-веба) |
| <a name="bem-event"></a>**БЭМ-событие** | Событие, генерируемое [блоком](#block) и организующее API для взаимодействия с ним других блоков. | [i-bem.js](http://ru.bem.info/technology/i-bem/2.3.0/i-bem-js/) |
| <a name="entity"></a>**БЭМ-сущность** | [Блок](#block) или [элемент](#elem) с [модификаторами](#mod), соответствующий определенной части интерфейса. | [BEMHTML](http://ru.bem.info/technology/bemhtml/2.3.0/rationale/#HTML-CSS-—-ассемблер-для-веба) |
| <a name="build_valid"></a>**Валидация файла** | Процесс определения актуальности файла при [сборке](#build). | [Модули технологий](http://ru.bem.info/tools/bem/bem-tools/tech-modules/#Валидация-файлов-при-последующих-сборках) |
| <a name="decl"></a>**Декларация** | Структура [бандла](#bundle) или страницы, описанная в терминах [блоков](#block), [элементов](#elem) и [модификаторов](#mod) (к примеру, с помощью XML, JSON или [BEMJSON](#bemjson)). | [О структуре проекта](http://ru.bem.info/tutorials/start-with-project-stub/#Кратко-о-структуре-проекта) |
| <a name="dyn_build"></a>**Динамическая сборка** | Предварительная [сборка](#build) статических файлов (CSS, JavaScript, шаблоны), с последующим формированием в runtime динамического [БЭМ-дерева](#bem-tree), на которое при этом накладываются [шаблоны](#template). | [Зависимости](http://ru.bem.info/tools/bem/bem-tools/depsjs/) |
| <a name="freeze"></a>**Заморозка** | Процесс преобразования URL файла, при котором URL заменяется на хеш от контента файла. | [borschik](http://ru.bem.info/articles/borschik/#«Заморозка»-статических-ресурсов--freeze-) |
| <a name="live"></a>**Ленивая инициализация** | Методика запуска инициализации JavaScript-объектов только в тот момент, когда их функциональность запрашивается пользователем: например, по клику на [блоке](#block). | [Ленивая инициализация](http://ru.bem.info/tutorials/bem-js-tutorial/03-live-initialization/) |
| <a name="mix"></a>**Микс** | Техника размещения нескольких [блоков](#block) на одном HTML-элементе. | [i-bem.js](http://ru.bem.info/technology/i-bem/2.3.0/i-bem-js/#Один-HTML-элемент-—-несколько-JS-блоков) |
| <a name="moda"></a>**Мода** | Отдельная фаза, проходимая циклом генерации HTML-элемента при шаблонизации. Каждая мода отвечает за определенный фрагмент генерируемого элемента: тег, атрибуты, класс и т.д. | [Справочное руководство по BEMHTML](http://ru.bem.info/technology/bemhtml/2.3.0/reference/#Мода) |
| <a name="default_mode"></a>**Мода default** | [Мода](#moda), в рамках которой целиком формируется выходной HTML-элемент, соответствующий входной БЭМ-сущности. | [Справочное руководство по BEMHTML](http://ru.bem.info/technology/bemhtml/2.3.0/reference/#default) |
| <a name="mod"></a>**Модификатор** | Свойство [блока](#block) или [элемента](#elem), меняющее его внешний вид или поведение. | [Модифицируемость блоков](http://ru.bem.info/method/definitions/#Модифицируемость-блоков) |
| <a name="tech_module"></a>**Модуль технологии** | [Node.js](http://nodejs.org/)-модуль, выполняющий операции над [файлами технологий](#file_tech). Для каждого типа данных существует отдельный модуль технологии. | [Модули технологий](http://ru.bem.info/tools/bem/bem-tools/tech-modules/#Технологии-в-bem-tools) |
| <a name="multilingv"></a>**Мультилингвальность** | Принцип описания внешнего вида и поведения [блока](#block) во всех [технологиях](#tech), необходимых для его работы. | [Консистентность блока](http://ru.bem.info/method/definitions/#Консистентность-блока) |
| <a name="ind_block"></a>**Независимый блок** | [Блок](#block), реализованный так, чтобы его можно было вставить в любое место на странице, в том числе и в другой блок. | [Независимость блоков](http://ru.bem.info/method/definitions/#Независимость-блоков) |
| <a name="prefix"></a>**Префикс** | Путь и имя файла без [суффикса](#suffix). | [Создание и преобразование файлов технологий](http://ru.bem.info/tools/bem/bem-tools/tech-modules/#Создание-и-преобразование-файлов-технологий) |
| <a name="build"></a>**Сборка страницы** | Формирование оптимизированного кода страницы в различных [технологиях](#tech) на основе ее [декларации](#decl). | [Сборка страниц](http://ru.bem.info/method/filesystem/#Сборка-страниц) |
| <a name="stat_build"></a>**Статическая сборка** | Полная [сборка](#build) статической страницы и публикация готового результата. | [Зависимости](http://ru.bem.info/tools/bem/bem-tools/depsjs/) |
| <a name="suffix"></a>**Суффикс** | Часть имени файла, следующая после первой точки в его названии. | [Модули технологий](http://ru.bem.info/tools/bem/bem-tools/tech-modules/#Технологии-в-bem-tools) |
| <a name="tech"></a>**Технологии** | Средства, с помощью которых описывается внешний вид и функциональность [блока](#block), [элемента](#elem) или [модификатора](#mod) (к примеру, HTML, CSS, JavaScript). | [Модули технологий](http://ru.bem.info/tools/bem/bem-tools/tech-modules/) |
| <a name="level"></a>**Уровень переопределения** | Набор реализаций [блоков](#block), сгруппированных в одну директорию. Позволяет при необходимости переопределять и доопределять блоки в разных технологиях, не затрагивая исходный код блоков. | [Уровни переопределения](http://ru.bem.info/method/filesystem/#Уровни-переопределения) |
| <a name="file_tech"></a>**Файл технологии** | Файл, содержащий все относящиеся к [БЭМ-сущности](#entity) данные определенного типа. Каждый такой файл соответствует конкретной [технологии](#tech), используемой для реализации сущности. | [Модули технологий](http://ru.bem.info/tools/bem/bem-tools/tech-modules/#Технологии-в-bem-tools) |
| <a name="template"></a>**Шаблон BEMHTML** | Утверждение, связывающее [БЭМ-сущность](#entity) с соответствующим ей HTML-элементом. Состоит из **предиката** (условий для применения шаблона) и **тела** (инструкций по генерации выходного HTML).| [Шаблонизатор BEMHTML](http://ru.bem.info/technology/bemhtml/2.3.0/reference/#Шаблон) |
| <a name="elem"></a>**Элемент** | Часть [блока](#block), отвечающая за отдельную функцию и не имеющая смысла в отрыве от блока. | [Единая предметная область](http://ru.bem.info/method/definitions/#Единая-предметная-область) |
|  |  |  |
|  |  |  |
| <a name="tech_api"></a>**API технологии** | Набор методов для работы с [технологиями](#tech). Может быть переопределен с помощью [модулей технологий](#tech_module). | [Модули технологий](http://ru.bem.info/tools/bem/bem-tools/tech-modules/#Особенности-архитектуры-пакета-bem-tools) |
| <a name="freeze"></a>**Freeze** | См. [Заморозка](#freeze) |  |
| <a name="live_init"></a>**Live-инициализация** | См. [Ленивая инициализация](#live) |  |
| <a name="merged-bundle"></a>**Merged-бандл** | [Бандл](#bundle), объединяющий в себе [декларации](#decl) (и, в итоге, результирующие файлы [сборки](#build)) всех бандлов [уровня](#level). | [Сборка merged-бандла](http://ru.bem.info/tools/bem/bem-tools/customization/#Сборка-`merged`-бандла--раньше-так-же-назывался-`common`-) |

## Инструментарий БЭМ

Краткое описание собственных инструментов, библиотек и технологий платформы БЭМ.

| Название | Определение |
| ----------- | ------ |
| <a name="bemhtml"></a>[BEMHTML](http://ru.bem.info/technology/bemhtml/current/intro/) | Шаблонный движок для веб-разработки в рамках БЭМ-методологии. |
| <a name="bemjson"></a>[BEMJSON](http://ru.bem.info/technology/bemjson/current/bemjson/) | Cтандартный формат представления [БЭМ-дерева](#bem-tree) - объект JavaScript с набором дополнительных соглашений о представлении [БЭМ-сущностей](#entity). |
| <a name="bemtree"></a>[BEMTREE](http://ru.bem.info/technology/bemtree/current/bemtree/) | [BEM-XJST](#bemxjst)-шаблонизатор, поэлементно преобразующий [БЭМ-дерево](#bem-tree) в HTML-документ. |
| <a name="bh"></a>[BH](http://ru.bem.info/technology/bh/) | [BEMJSON](#bemjson)-процессор, который превращает BEMJSON в HTML. |
| <a name="bem-bl"></a>[bem-bl](http://ru.bem.info/libs/bem-bl/) | Расширенная библиотека, которая помимо базовых вариантов [блоков](#block) включает реализации некоторых универсальных решений для меню, текста, логотипа, поисковой строки, таблиц и т.д. |
| <a name="bem-comp"></a>[bem-components](http://ru.bem.info/libs/bem-components/) | Библиотека [блоков](#block), предоставляющая готовые элементы управления форм и некоторые другие блоки. |
| <a name="bem-core"></a>[bem-core](http://ru.bem.info/libs/bem-core/) | Базовая библиотека [блоков](#block) для разработки веб-интерфейсов, cодержащая необходимый минимум для разработки клиентского JavaScript и HTML-шаблонов. |
| <a name="bem-history"></a>[bem-history](http://ru.bem.info/libs/bem-history/) | БЭМ-обертка над [History API](http://www.w3.org/html/wg/drafts/html/master/browsers.html#history). |
| <a name="bem-mvc"></a>[bem-mvc](http://ru.bem.info/libs/bem-mvc/) | Набор [i-bem](#i-bem)-блоков для реализации [MVC](http://www.asp.net/mvc)-паттерна, предоставляющий API для работы с моделями и блоки для автоматического провязывания моделей с интерфейсом. |
| <a name="bem-naming"></a>[bem-naming](http://ru.bem.info/tools/bem/bem-naming/) | Инструмент, позволяющий получать информацию о [БЭМ-сущности](#entity) по строке или на основе [БЭМ-нотации](#bem_not). |
| <a name="bem-tools"></a>[bem-tools](http://ru.bem.info/tools/bem/bem-tools/) | Набор инструментов для работы с файлами по БЭМ-методологии. |
| [bem-tools-autoprefixer](http://ru.bem.info/tools/bem/autoprefixer/) | Расширение для [bem-tools](#bem-tools), использующее [autoprefixer](http://ru.bem.info/tools/bem/autoprefixer/) во время процесса сборки. |
| <a name="bemxjst"></a>[BEM-XJST](http://ru.bem.info/tools/templating-engines/bemxjst/) | Компилятор БЭМ-специфичных [шаблонов](#template), основанный на [XJST](#xjst). |
| <a name="borschik"></a>[borschik](http://ru.bem.info/tools/optimizers/borschik/) | Расширяемый сборщик файлов текстовых форматов, основная задача которого - [сборка](#stat_build) статических файлов веб-проектов (CSS, JS и т.д.). |
| <a name="bower-npm-install"></a>[bower-npm-install](http://ru.bem.info/tools/bem/bower-npm-install/) | Инструмент для запуска команды `npm install` для всех зависимостей [bower](http://bower.io/). |
| <a name="ccso"></a>[CCSO](http://ru.bem.info/tools/optimizers/csso/) (CSS Optimizer) | Минимизатор CSS, выполняющий как минимизацию без изменения структуры, так и структурную минимизацию с целью получения наиболее короткого кода. |
| <a name="enb"></a>[ENB](http://enb-make.info/) | Сборщик проектов, построенных на модели `node`/`target`. |
| <a name="enb-bemxjst"></a>[enb-bemxjst](http://ru.bem.info/tools/bem/enb-bemxjst/) | Модуль, обеспечивающий поддержку технологий, основанных на [BEM-XJST](#bemxjst), для [ENB](#enb). |
| <a name="enb-bem-docs"></a>[enb-bem-docs](http://ru.bem.info/tools/bem/enb-bem-docs/) | Модуль создания документации в [ENB](#enb). |
| <a name="enb-bem-examples"></a>[enb-bem-examples](http://ru.bem.info/tools/bem/enb-bem-examples/) | Инструмент для генерации сетов примеров БЭМ-блоков с помощью [ENB](#enb). |
| <a name="enb-bem-pseudo-levels"></a>[enb-bem-pseudo-levels](http://ru.bem.info/tools/bem/enb-bem-pseudo-levels/) | Инструмент для манипуляции [уровнями переопределений](#level) для [ENB](#enb), позволяющий создавать уровни на основе уже существующих. |
| <a name="enb-bem-specs"></a>[enb-bem-specs](http://ru.bem.info/tools/bem/enb-bem-specs/) | Инструмент, используемый [ENB](#enb) для [сборки](#build) и запуска тестов (спеков) на клиентский JavaScript. |
| <a name="enb-bem-techs"></a>[enb-bem-techs](http://ru.bem.info/tools/bem/enb-bem-techs/) | Пакет [ENB](#enb), предоставляющий набор базовых технологий для [сборки](#build) проектов, в основе которых лежит БЭМ-методология. |
| <a name="enb-bem-tmpl-specs"></a>[enb-bem-tmpl-specs](http://ru.bem.info/tools/bem/enb-bem-tmpl-specs/) | Инструмент для [сборки](#build) и запуска тестов на [шаблоны](#template) в [ENB](#enb). |
| <a name="enb-bh"></a>[enb-bh](http://ru.bem.info/tools/bem/enb-bh/) | Модуль, обеспечивающий поддержку [BH](#bh) в [ENB](#enb). |
| <a name="enb-xjst"></a>[enb-xjst](http://ru.bem.info/tools/bem/enb-xjst/) | Модуль, обеспечивающий поддержку технологий, основанных на [XJST](#XJST), в [ENB](#enb). |
| <a name="gemini"></a>[Gemini](http://ru.bem.info/tools/testing/gemini/) | Утилита для регрессионного тестирования отображения веб-страниц. |
| <a name="generator-bem-stub"></a>[generator-bem-stub](http://ru.bem.info/tools/bem/bem-stub/) | Генератор БЭМ-проектов на [Yeoman](http://yeoman.io/). |
| <a name="gonzales"></a>[Gonzales](https://github.com/css/gonzales) | Быстрый парсер CSS. |
| <a name="html-differ"></a>[html-differ](http://ru.bem.info/tools/testing/html-differ/) | Инструмент для сравнения HTML-документов. |
| <a name="i-bem"></a>[i-bem.js](http://ru.bem.info/technology/i-bem/2.3.0/i-bem-js/) | Специализированный JavaScript-фреймворк для веб-разработки в рамках БЭМ-методологии. |
| <a name="ometajs"></a>[OmetaJS](https://github.com/veged/ometa-js#ometajs-) | JavaScript-версия объектно-ориентированного языка [OMeta](http://tinlizzie.org/ometa/). |
| <a name="project-stub"></a>[project-stub](https://github.com/bem/project-stub) | Шаблонный репозиторий используемый для создания БЭМ-проектов. |
| <a name="setochka"></a>[setochka](https://github.com/afelix/setochka) | Инструмент для выделения CSS-свойств исходного CSS в отдельные файлы. |
| <a name="shmakowiki"></a>[Shmakowiki](https://github.com/veged/shmakowiki) | Вариация формата wiki-разметки. |
| <a name="svgo"></a>[SVGO](http://ru.bem.info/tools/optimizers/svgo/svgo/) | Инструмент для оптимизации векторной графики в формате [SVG](http://www.w3schools.com/svg/), написанный на [Node.js](http://nodejs.org/). |
| <a name="xjst"></a>[XJST](http://bem.info/tools/templating-engines/xjst/) | Низкоуровневый JavaScript-шаблонизатор. |
| <a name="ymodules"></a>[YModules](http://ru.bem.info/tools/bem/modules/) | Модульная система, хорошо себя зарекомендовавшая в связке с БЭМ. |
