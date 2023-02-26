---
{"dg-publish":true,"permalink":"/olap-cube/"}
---


⬆:: [[Работа с данными\|Работа с данными]]
⬅::
📅:: [[2023-02-04\|2023-02-04]] 
Источник: https://www.holistics.io/blog/the-rise-and-fall-of-the-olap-cube/

# OLAP Cube

 - **online analytical processing** - схема (тип) использования баз данных (a type of workload)
	 - куб - это структурирование данных для выполнения работ в рамках OLAP (a specific data structure)
	 - OLAP можно использовать и in a columnar database
 - класс приложений для работы с [[Базы Данных\|Базы Данных]]
 - 1993 - Edgar F. Codd - придумал название
 - Категории Баз данных
	 - OLTP (Online Transaction Processing): using a database to run your business
	 - OLAP: using a database to understand your business
- используются сложные комбинации UNION + GroupBy
-  Kimball dimensional modeling, Inmon-style entity-relationship modeling, or data vault modeling - методы организации информации
- зачем строить кубы, если можно написать простой запрос, например через [[Сводная таблица\|Сводная таблица]] - единственное ограничение - стоимость хранилища и мощностей
- современные облачные хранилища - massively parallel processing (MPP) architecture - запросы распределяются на сотни машин, а не выполняются на одной
- основной прорыв - columnar data warehouses - объясняет возвращение от кубов снова к Базам Данных.
	- бысртрее читается (не нужно загружать всю информацию), лучше сжимается,
- сортировка и индексирование  - в высвобожденном пространстве после сжатия информации
В результате -та же информация и гибкость, что и в кубах, но при этом не нужно писать сложные запросы

Рекомендация автора: 
- большие компании ушли из кубов
	- но OLAP можно использовать:
	- > BigQuery, Redshift and Snowflake will all say that they are well suited for OLAP _workloads_, but will never say they are OLAP cubes
- Study Kimball, Inmon and data vault methodologies, but with an eye to **application in the new paradigm**. Understand the limitations of each of their approaches.





![Рис - OLAP  cube.png](/img/user/%D0%A0%D0%B8%D1%81%20-%20OLAP%20%20cube.png)

![Рис - underlying infrastructure of BigQuery - an MPP database.png](/img/user/%D0%A0%D0%B8%D1%81%20-%20underlying%20infrastructure%20of%20BigQuery%20-%20an%20MPP%20database.png)

![Рис - Difference between a row-based RDBMS and a columnar database.png](/img/user/%D0%A0%D0%B8%D1%81%20-%20Difference%20between%20a%20row-based%20RDBMS%20and%20a%20columnar%20database.png)


