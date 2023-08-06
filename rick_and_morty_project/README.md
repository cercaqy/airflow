# Работа с [API Rick&Morty](https://rickandmortyapi.com)
## Описание проекта
Даг находит ТОП-N локаций по количеству резидентов в API Rick&Morty и загружает данные в таблицу o_bazan_ram_location в GreenPlum
- Реализация c кастомными операторами
- Идемподентность (свойство при повторном запуске выдавать точно такой же результат, как при первом запуске) реализована полным очищением таблицы перед загрузкой в нее новых данных
  
## Использованные инструменты
Apache Airlow, Python, GreenPlum

## Файлы
**o-bazan_lesson5_with_hook_dag.py** - скрипт DAG-а

**o_bazan_ram_operator.py** - оператор, возвращающий из API Rick&Morty ТОП-N локаций по количеству резидентов

**o_bazan_ram_hook.py** - хук, взаимодействующий с API Rick&Morty