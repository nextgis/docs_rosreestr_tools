.. _ngq_rosreestr_cadaster:

Работа с кадастровой картой
===========================

.. _ngq_rr_add_layer:

Подключение кадастрового слоя
-----------------------------

Вторая иконка модуля **NGQ Rosreestr Tools** |icon_add_layers| позволяет добавлять различные слои данных Росреестра (см. :numref:`add_layers_pkk`) из публичной кадастровой карты (далее - ПКК):

.. |icon_add_layers| image:: _static/icon_add_layers.png
   :width: 6mm

* слой кадастровых кварталов, округа
* слой земельных участков, ОКС (Объекты капитального строительства)
* слой зон с особыми условиями использования

.. figure:: _static/add_layers_pkk_ru.png
   :name: add_layers_pkk
   :align: center
   :width: 12cm
   
   Добавление слоёв из ПКК


.. figure:: _static/pkk_on_map_ru.png
   :name: pkk_on_map
   :align: center
   :width: 20cm
   
   Слой кадастровых кварталов на карте

Добавлять слои данных  Росреестра из ПКК так же можно через Панель “Браузер”.


.. figure:: _static/add_layer_ppk_ru.png
   :name: add_layer_ppk_ru
   :align: center
   :width: 14cm

   Добавление слоёв из ПКК через панель "Браузер"

.. _ngq_rr_indentify:

Идентификация кварталов и участков
----------------------------------

Третья иконка |identificaion_land| позволяет по клику на объект идентифицировать (см. :numref:`identificaion_objects`) атрибутивную информацию по:


* |identificaion_land| земельным участкам
* |identification_oks| кадастровым кварталам
* |identification_quarter| объектам капитального строительства (ОКС)
* |identification_zones| зонам с особыми условиями использования территорий (ЗОУИТ)


.. |identificaion_land| image:: _static/rr_identification_land.png
   :width: 6mm

.. |identification_oks| image:: _static/rr_identification_oks.png
   :width: 6mm

.. |identification_quarter| image:: _static/rr_identification_quarter.png
   :width: 6mm

.. |identification_zones| image:: _static/rr_identification_zones.png
   :width: 6mm

.. figure:: _static/identificaion_objects_ru_2.png
   :name: identificaion_objects
   :align: center
   :width: 14cm
   
   Идентификация объектов Росреестра
   
По клику отображается список объектов выбранного типа, найденных в этой точке. Первый из них будет подсвечен.

.. figure:: _static/objects_on_map_list_ru.png
   :name: objects_on_map_list_pic
   :align: center
   :width: 20cm

   Список найденных кадастровых кварталов и подсветка контура первого из них

Нулевые кварталы соответствуют более крупной единице деления. В примере выше это район и город.

Двойной клик по объекту в списке открывает его карточку. Чтобы переходить между объектами, используйте выпадающее меню сверху.

.. figure:: _static/objects_on_map_ru_3.png
   :name: object_on_map
   :align: center
   :width: 20cm
   
   Отображение карточки найденного объекта и подсветка его контура

При идентификации объект можно сохранить в пользовательский векторный слой, а также создать специальный слой со структурой идентифицируемого объекта. Аналогично при поиске объектов: найденные объекты можно добавлять в пользовательские или специальные векторные слои (см. :numref:`ngq_identification`, :numref:`ngq_temp_layer`).

.. figure:: _static/ngq_identification_ru_3.png
   :name: ngq_identification
   :align: center
   :width: 20cm
   
   Доступные опции при идентификации объекта
   
   
.. figure:: _static/ngq_temp_layer_ru_3.png
   :name: ngq_temp_layer
   :align: center
   :width: 20cm
   
   Добавление объекта во временный пользовательский слой
   
.. figure:: _static/ngq_temp_layer_attributes_ru_3.png
   :name: ngq_temp_layer_attributes
   :align: center
   :width: 20cm
   
   Объект во временном слое. 1 - временный слой, 2 - объект на карте, 3 - таблица атрибутов временного слоя, 4 - карточка информации об объекте
   
Также можно скопировать запись (строку), значение отдельного атрибута или всю карточку.  

Поля, содержащие большие числа и единицы измерения, представлены в атрибутах объекта в двух вариантах: с форматированием и без.

.. figure:: _static/feature_format_ru_2.png
   :name: feature_format_pic
   :align: center
   :width: 20cm

   Поля с визуальным форматированием больших чисел и единиц измерения

.. _ngq_rr_search:

Поиск по кадастровому номеру
----------------------------

Иконка панели поиска |search_icon| позволяет находить объекты, имеющие границы из базы данных Росреестра (см. :numref:`search_object`), по кадастровому номеру.

.. |HighlightFeature| image:: _static/mActionHighlightFeature.png
   :width: 6mm

.. |PanTo| image:: _static/mActionPanTo.png
   :width: 6mm

.. |ZoomTo| image:: _static/mActionZoomTo.png
   :width: 6mm

.. |search_icon| image:: _static/button_RR_search.png
   :width: 6mm

.. figure:: _static/search_object_ru_3.png
   :name: search_object
   :align: center
   :width: 22cm
   
   Отображение списка найденных объектов и подсветка контура выделенного

Вы можете выбрать, как показывать объекты при поиске:

* |HighlightFeature| Отображать все найденные объекты одновременно (объекты подсвечиваются полупрозрачной заливкой и наслаиваются друг на друга);
* |PanTo| Автоматически перемещаться к выбранному объекту;
* |ZoomTo| Автоматически приближать к выбранному объекту.

.. figure:: _static/search_highlight_ru.png
   :name: search_highlight_pic
   :align: center
   :width: 22cm

   Подсвечены одновременно три найденных объекта. Они накладываются друг на друга и отличаются плотностью заливки

Для снятия выделения щелкните по пустому полю под списком.

Дважды щёлкните по объекту в списке, чтобы перейти к его карточке.

В карточке объекта отображается статистика: сколько кварталов, участков и ОКС он включает в себя.

.. figure:: _static/search_object_stat_ru_2.png
   :name: search_object_stat_pic
   :align: center
   :width: 22cm

   Статистические данные квартала

Поддерживается поиск объектов без геометрий. Можно просмотреть карточку объекта и добавить его на слой. Примерное местоположение объекта на карте будет отмечено точкой.

.. figure:: _static/no_geometry_found_ru.png
   :name: no_geometry_card_pic
   :align: center
   :width: 22cm
   
   Отображение карточки найденного объекта без геометрии





Процесс поиска объекта по кадастровому номеру можно посмотреть на этом `видео <https://youtu.be/ig6jreu-I9E>`_.

Также доступно подключение кадастровых сервисов для NextGIS Web on-premise для работы на веб-карте.

