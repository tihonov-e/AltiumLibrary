# Библиотека компонентов для Altium Designer
Данная библиотека является открытой и используется автором для работы, а следовательно постоянно пополняется новыми компонентами. Условно-графические обозначения (УГО) компонентов, выполнены в стилистике ЕСКД, но автор не гарантирует полное соответствие. Посадочные места для компонентов выполнены в полном соответствии с группой стандартов IPC. Актуальная рабочая библиотека содержится в ветке *master*, основная часть компонентов в ней проверена на реальных платах. Сложные ответственные компоненты, например, FPGA в корпусах BGA, проходят усиленную проверку и до испытаний в "боевом" проекте находятся в ветке *dev*.

![Пример дизайна](https://habrastorage.org/webt/lv/_v/vo/lv_vvojmxbw4kgr854siiyvor2i.png)

# Структура проекта

* Библиотеки компонентов
    >
    * IC: Logic
    * IC: Comparator
    * IC: Amplifier
    * IC: Sensor
    * IC: MCU
    * IC: FPGA
    * IC: ADC, DAC, DDS
    * IC: Memory
    * IC: RF transceiver
    * IC: Interface
    * IC: Power supply
    * IC: Gate driver
    * Module
    * Electromechanics
    * Transformer
    * Inductor
    * Transistor
    * Diode
    * Connector
    * Oscilator
    * Optoisolator
    * Resistor
    * Capacitor

>

* Шаблоны файлов и правил
    >
    * SchematicPage - стандартные листы для ЕСКД и ISO
    * BoardPCB - шаблоны для печатных плат
    * Rules - правила трассировки для разных классов точности

# Установка библиотеки

Скачайте архив с библиотекой или клонируйте репозиторий к себе на локальный диск:
```
git clone https://github.com/Nordic-Energy/AltiumLibrary.git
```
После этого переходите в папку *LibraryComponents* и видите список файлов библиотеки компонентов:

![Список файлов](https://habrastorage.org/webt/gq/yi/lp/gqyilpiaiied2tomg-plan0nslg.png)

Все библиотеки состоят из четырых файлов: 

* Файлы с расширением .LibPkg - объединяют все последующие файлы проекта
* Файлы с расширением .SchLib - содержат УГО компонентов
* StandartCase.PcbLib - содержит посадочные места для стандартных корпусов, например, LQFP-48 и подобные
* CustomCase.PcbLib - содержит посадочные места для нестандартных компонентов, например, разъемов

Для установки нужной библиотеки откройте файл с расширением ***.LibPkg*** в Altium Designer, например, ***IC. ADC, DAC, DDS.LibPkg*** и у вас в дереве проектов появится библиотека и три файла внутри нее:

![Дерево проектов](https://habrastorage.org/webt/qj/7q/ze/qj7qzea6pmnlmb7regqanuri0ri.png)

Теперь нажимайте правой кнопкой мыши на название проекта и выбирайте пункт ***Compile Integrated Library***:

![Компиляция проекта](https://habrastorage.org/webt/1p/at/nk/1patnk16twt8potkibvg7ey5-ao.png)

После этого у вас скомпилируется проект библиотеки, автоматически подключится к Altium Designer и появится в списке библиотек:

![Скомпилированная библиотека](https://habrastorage.org/webt/io/mk/pp/iomkppp4u4cur8o4izf2q-tpx6u.png)

# Контакты для связи
* Электронная почта: ilya@nordic-energy.org
* Канал на youtube: https://www.youtube.com/NordicEnergy




