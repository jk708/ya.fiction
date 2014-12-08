## Словарь терминов

Список определений закрепленных в терминологии БЭМ.

| Термин | Определение | Пример упоминания в документации |
| ----------- | ------------------- | -------------------- |
| <a name="base-tech"></a>**Базовая технология** | Модуль на основе технологии [Node.js](http://nodejs.org/), реализующий общую функциональность обработки данных командами `bem create` и `bem build` инструмента [bem-tools](#bem-tools). | [Модули технологий](http://ru.bem.info/tools/bem/bem-tools/tech-modules/#Особенности-архитектуры-пакета-bem-tools) |
| **Базовая технология команды** | Цепочка методов [базовой технологии](#base-tech), вызываемых в процессе выполнения команды. | [Модули технологий](http://ru.bem.info/tools/bem/bem-tools/tech-modules/#Приложение-3--Базовая-технология-bem-tools) |
| <a name="bundle"></a>**Бандл** | Совокупность результирующих [файлов технологий](#file-tech), собранных из файлов технологий [блоков](#block) на [уровнях переопределения](#level). | [Модули технологий](http://ru.bem.info/tools/bem/bem-tools/tech-modules/#Особенности-архитектуры-пакета-bem-tools) |
| **Бандл технологии** | Отдельный результирующий [файл технологии](#file-tech). | [Модули технологий](http://ru.bem.info/tools/bem/bem-tools/tech-modules/#Технологии-в-bem-tools) |
| <a name="block"></a>**Блок** | Часть дизайна страницы или раскладки со своим специфическим и уникальным значением, определенным семантически или визуально. | [Единая предметная область](http://ru.bem.info/method/definitions/#Единая-предметная-область) |
| **Блок-микс** | [Блок](#block), не участвующий в цепочке наследования. | [Блоки-миксы](http://ru.bem.info/technology/i-bem/current/i-bem-js/#Блоки-миксы) |
| <a name="bem-tree"></a>**БЭМ-дерево** | Структура [БЭМ-сущностей](#entity) страницы, с учетом их вложенности (описывается в формате [BEMJSON](#bemjson)). | [Средства описания страницы](http://ru.bem.info/method/definitions/#Средства-описания-страницы-и-шаблоны) |
| **БЭМ-событие** | Собственное событие, генерируемое [блоком](#block) и позволяющее организовать API для взаимодействия с блоком. | [i-bem.js](http://ru.bem.info/technology/i-bem/2.3.0/i-bem-js/) |
| <a name="entity"></a>**БЭМ-сущность** | [Блок](#block) или [элемент](#elem) с [модификаторами](#mod), соответствующий определенной части интерфейса. | [BEMHTML](http://ru.bem.info/technology/bemhtml/2.3.0/rationale/#HTML-CSS-—-ассемблер-для-веба) |
| **Валидация файла** | Процесс определения актуальности файла при [сборке](#build). | [Модули технологий](http://ru.bem.info/tools/bem/bem-tools/tech-modules/#Валидация-файлов-при-последующих-сборках) |
| <a name="decl"></a>**Декларация** | Структура страницы, описанная в терминах [блоков](#block), [элементов](#elem) и [модификаторов](#mod) (к примеру, с помощью XML, JSON или [BEMJSON](#bemjson)). | [О структуре проекта](http://ru.bem.info/tutorials/start-with-project-stub/#Кратко-о-структуре-проекта) |
| **Динамическая сборка** | Предварительная [сборка](#build) статических файлов (CSS, JavaScript, шаблоны), с последующим формированием в runtime динамического [БЭМ-дерева](#bem-tree), на которое накладываются [шаблоны](#template). | [Зависимости](http://ru.bem.info/tools/bem/bem-tools/depsjs/) |
| <a name="freeze"></a>**Заморозка** | Процесс преобразования URL до файла, при котором URL заменяется на хеш от контента файла. | [borschik](http://ru.bem.info/articles/borschik/#«Заморозка»-статических-ресурсов--freeze-) |
| <a name="live"></a>**Ленивая инициализация** | Запуск инициализации JavaScript-объектов только в тот момент, когда их функциональность требуется пользователю: например, по клику на [блоке](#block). | [Ленивая инициализация](http://ru.bem.info/tutorials/bem-js-tutorial/03-live-initialization/) |
| **Микс** | Техника размещения нескольких [блоков](#block) на одном HTML-элементе. | [i-bem.js](http://ru.bem.info/technology/i-bem/2.3.0/i-bem-js/#Один-HTML-элемент-—-несколько-JS-блоков) |
| **Мода** | Ряд фаз, проходимый циклом генерации каждого [элемента](#elem). | [BEMHTML](http://ru.bem.info/technology/bemhtml/2.3.0/reference/#Мода) |
| <a name="mod"></a>**Модификатор** | Свойство [блока](#block) или [элемента](#elem), которое меняет его внешний вид или поведение. | [Модифицируемость блоков](http://ru.bem.info/method/definitions/#Модифицируемость-блоков) |
| **Модуль технологии** | Модуль на основе технологии [Node.js](http://nodejs.org/), который позволяет работать с [файлами технологии](#file-tech) в БЭМ-терминах. | [Модули технологий](http://ru.bem.info/tools/bem/bem-tools/tech-modules/#Технологии-в-bem-tools) |
| **Мультилингвальность** | Описание [блока](#block) на всех языках ([технологиях](#tech)), необходимых для его работы. | [Консистентность блока](http://ru.bem.info/method/definitions/#Консистентность-блока) |
| **Независимый блок** | [Блок](#block), реализованный так, чтобы его можно было вставить в любое место на странице, в том числе и в другой блок. | [Независимость блоков](http://ru.bem.info/method/definitions/#Независимость-блоков) |
| **Префикс** | Путь и имя файла без [суффикса](#suffix). | [Создание и преобразование файлов технологий](http://ru.bem.info/tools/bem/bem-tools/tech-modules/#Создание-и-преобразование-файлов-технологий) |
| <a name="build"></a>**Сборка страницы** | Формирование кода страницы в различных [технологиях](#tech) на основе [декларативного](#decl) описания страницы путем применения реализаций описанных [блоков](#block). | [Сборка страниц](http://ru.bem.info/method/filesystem/#Сборка-страниц) |
| <a name="stat_build"></a>**Статическая сборка** | Полная [сборка](#build) статической страницы и публикация готового результата. | [Зависимости](http://ru.bem.info/tools/bem/bem-tools/depsjs/) |
| <a name="suffix"></a>**Суффикс** | Часть имени файла, следующая после первой точки в его названии. | [Модули технологий](http://ru.bem.info/tools/bem/bem-tools/tech-modules/#Технологии-в-bem-tools) |
| <a name="tech"></a>**Технологии** | Средства, с помощью которых описывается внешний вид и функциональность [блока](#block), [элемента](#elem) или [модификатора](#mod) (к примеру, HTML, CSS, JavaScript). | [Модули технологий](http://ru.bem.info/tools/bem/bem-tools/tech-modules/) |
| <a name="level"></a>**Уровень переопределения** | Набор реализаций [блоков](#block), сгруппированных в одну директорию. | [Уровни переопределения](http://ru.bem.info/method/filesystem/#Уровни-переопределения) |
| <a name="file-tech"></a>**Файл технологии** | Определенный тип данных, относящихся к [БЭМ-сущности](#entity). | [Модули технологий](http://ru.bem.info/tools/bem/bem-tools/tech-modules/#Технологии-в-bem-tools) |
| <a name="template"></a>**Шаблон** | Максимально простое утверждение, сопоставляющее каждому типу [БЭМ-сущности](#entity) нужное HTML-оформление. | [Шаблонизатор BEMHTML](http://ru.bem.info/technology/bemhtml/current/reference/#Входные-данные:-BEMJSON) |
| <a name="elem"></a>**Элемент** | Часть [блока](#block), отвечающая за отдельную функцию и не имеющая смысла в отрыве от блока. | [Единая предметная область](http://ru.bem.info/method/definitions/#Единая-предметная-область) |
|  |  |  |
|  |  |  |
| **API технологии** | Набор методов для работы с [технологиями](#tech), общий для всех подпрограмм пакета [bem-tools](#bem-tools) и модулей [технологий](#tech). | [Модули технологий](http://ru.bem.info/tools/bem/bem-tools/tech-modules/#Особенности-архитектуры-пакета-bem-tools) |
| **Freeze** | См. [Заморозка](#freeze) |  |
| **Live-инициализация** | См. [Ленивая инициализация](#live) |  |
| **Merged-бандл** | [Бандл](#bundle), который объединяет в себе [декларации](#decl) всех бандлов уровня. | [Сборка merged-бандла](http://ru.bem.info/tools/bem/bem-tools/customization/#Сборка-`merged`-бандла--раньше-так-же-назывался-`common`-) |

## Инструментарий БЭМ

Краткое описание собственных инструментов, библиотек и технологий платформы БЭМ.

| Название | Определение |
| ----------- | ------ |
| [BEMHTML](http://ru.bem.info/technology/bemhtml/current/intro/) | Шаблонный движок для веб-разработки в рамках БЭМ-методологии. |
| <a name="bemjson"></a>[BEMJSON](http://ru.bem.info/technology/bemjson/current/bemjson/) | Cтандартный формат представления [БЭМ-дерева](#bem-tree) - объект JavaScript с набором дополнительных соглашений о представлении [БЭМ-сущностей](#entity). |
| [BEMTREE](http://ru.bem.info/technology/bemtree/current/bemtree/) | [BEM-XJST](#bemxjst)-шаблонизатор, поэлементно преобразующий [БЭМ-дерево](#bem-tree) в HTML-документ. |
| [BH](http://ru.bem.info/technology/bh/) | [BEMJSON](#bemjson)-процессор, который превращает BEMJSON в HTML. |
| [bem-bl](http://ru.bem.info/libs/bem-bl/) | Расширенная библиотека, которая помимо базовых вариантов [блоков](#block) включает реализации некоторых универсальных решений для меню, текста, логотипа, поисковой строки, таблиц и т.д. |
| [bem-components](http://ru.bem.info/libs/bem-components/) | Библиотека [блоков](#block), предоставляющая готовые элементы управления форм и некоторые другие блоки. |
| [bem-core](http://ru.bem.info/libs/bem-core/) | Базовая библиотека [блоков](#block) для разработки веб-интерфейсов, cодержащая необходимый минимум для разработки клиентского JavaScript и HTML-шаблонов. |
| [bem-history](http://ru.bem.info/libs/bem-history/) | БЭМ-обертка над [History API](http://www.w3.org/html/wg/drafts/html/master/browsers.html#history). |
| [bem-mvc](http://ru.bem.info/libs/bem-mvc/) | Набор [i-bem](#i-bem)-блоков для реализации [MVC](http://www.asp.net/mvc)-паттерна, предоставляющий API для работы с моделями и блоки для автоматического провязывания моделей с интерфейсом. |
| [bem-naming](http://ru.bem.info/tools/bem/bem-naming/) | Инструмент, позволяющий получать информацию о [БЭМ-сущности](#entity) по строке, а также формировать строковое представление на основе БЭМ-нотации. |
| <a name="bem-tools"></a>[bem-tools](http://ru.bem.info/tools/bem/bem-tools/) | Набор инструментов для работы с файлами по БЭМ-методологии. |
| [bem-tools-autoprefixer](http://ru.bem.info/tools/bem/autoprefixer/) | Расширение для [bem-tools](#bem-tools), использующее [autoprefixer](http://ru.bem.info/tools/bem/autoprefixer/) во время процесса сборки. |
| <a name="bemxjst"></a>[BEM-XJST](http://ru.bem.info/tools/templating-engines/bemxjst/) | Компилятор БЭМ-специфичных [шаблонов](#template), основанный на [XJST](#xjst). |
| [borschik](http://ru.bem.info/tools/optimizers/borschik/) | Расширяемый сборщик файлов текстовых форматов, основная задача которого - [сборка](#stat_build) статических файлов веб-проектов (CSS, JS и т.д.). |
| [bower-npm-install](http://ru.bem.info/tools/bem/bower-npm-install/) | Инструмент для запуска команды `npm install` для всех зависимостей [bower](http://bower.io/). |
| [CCSO](http://ru.bem.info/tools/optimizers/csso/) (CSS Optimizer) | Минимизатор CSS, выполняющий как минимизацию без изменения структуры, так и структурную минимизацию с целью получить как можно меньший текст. |
| <a name="enb"></a>[ENB](http://enb-make.info/) | Сборщик проектов, построенных на модели `node`/`target`. |
| [enb-bemxjst](http://ru.bem.info/tools/bem/enb-bemxjst/) | Поддержка [технологий](#tech), базирующихся на основе [BEM-XJST](#bemxjst), для [ENB](#enb). |
| [enb-bem-docs](http://ru.bem.info/tools/bem/enb-bem-docs/) | Модуль создания документации для [ENB](#enb). |
| [enb-bem-examples](http://ru.bem.info/tools/bem/enb-bem-examples/) | Инструмент для генерации сетов из примеров БЭМ-блоков с помощью [ENB](#enb). |
| [enb-bem-pseudo-levels](http://ru.bem.info/tools/bem/enb-bem-pseudo-levels/) | Инструмент для манипуляции [уровнями переопределений](#level) для [ENB](#enb), позволяющий создавать уровни на основе уже существующих. |
| [enb-bem-specs](http://ru.bem.info/tools/bem/enb-bem-specs/) | Инструмент, используемый [ENB](#enb) для [сборки](#build) и запуска тестов (спеков) на клиентский JavaScript. |
| [enb-bem-techs](http://ru.bem.info/tools/bem/enb-bem-techs/) | Пакет, предоставляющий набор базовых технологий для [сборки](#build) проектов, в основе которых лежит БЭМ-методология, с помощью [ENB](#enb). |
| [enb-bem-tmpl-specs](http://ru.bem.info/tools/bem/enb-bem-tmpl-specs/) | Инструмент для [сборки](#build) и запуска тестов на [шаблоны](#template) в [ENB](#enb). |
| [enb-bh](http://ru.bem.info/tools/bem/enb-bh/) | Модуль, обеспечивающий поддержку [BH](#bh) в [ENB](#enb). |
| [enb-xjst](http://ru.bem.info/tools/bem/enb-xjst/) | Поддержка технологий на основе [XJST](#XJST) в [ENB](#enb). |
| [Gemini](http://ru.bem.info/tools/testing/gemini/) | Утилита для регрессионного тестирования отображения веб-страниц. |
| [generator-bem-stub](http://ru.bem.info/tools/bem/bem-stub/) | Генератор БЭМ-проектов на [Yeoman](http://yeoman.io/). |
| [Gonzales](https://github.com/css/gonzales) | Быстрый парсер CSS. |
| [html-differ](http://ru.bem.info/tools/testing/html-differ/) | Инструмент для сравнения HTML-документов. |
| <a name="i-bem"></a>[i-bem.js](http://ru.bem.info/technology/i-bem/2.3.0/i-bem-js/) | Специализированный JavaScript-фреймворк для веб-разработки в рамках БЭМ-методологии. |
| [OmetaJS](https://github.com/veged/ometa-js#ometajs-) | JavaScript-версия объектно-ориентированного языка [OMeta](http://tinlizzie.org/ometa/). |
| [project-stub](https://github.com/bem/project-stub) | Шаблонный репозиторий используемый для создания БЭМ-проектов. |
| [setochka](https://github.com/afelix/setochka) | Инструмент для выделения CSS-свойств исходного CSS в отдельные файлы. |
| [Shmakowiki](https://github.com/veged/shmakowiki) | Вариация формата wiki-разметки. |
| [SVGO](http://ru.bem.info/tools/optimizers/svgo/svgo/) | Инструмент для оптимизации векторной графики в формате [SVG](http://www.w3schools.com/svg/), написанный на [Node.js](http://nodejs.org/). |
| <a name="xjst"></a>[XJST](http://bem.info/tools/templating-engines/xjst/) | Низкоуровневый JavaScript-шаблонизатор. |
| [YModules](http://ru.bem.info/tools/bem/modules/) | Модульная система. |
