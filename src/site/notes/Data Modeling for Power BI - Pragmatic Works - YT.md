---
{"dg-publish":true,"permalink":"/data-modeling-for-power-bi-pragmatic-works-yt/"}
---


⬆:: [[Power BI\|Power BI]] [[Data Modeling\|Data Modeling]]
⬅::
📅:: [[2023-03-26\|2023-03-26]] 

# Data Modeling for Power BI - Pragmatic Works - YT

Data Modeling for Power BI - Full Course
[https://www.youtube.com/live/MrLnibFTtbA](https://www.youtube.com/live/MrLnibFTtbA)

Download student files - [](https://www.youtube.com/redirect?event=video_description&redir_token=QUFFLUhqa1VxODd4SlBVNERpQjBtRHZqUWgyNWpxQUFVQXxBQ3Jtc0tsdHFoQUFVaEdsZjVaQkpTXzlIRWs4cnhsbHY2OXgzUWxrNnI2RjgtR21DU1JySTdxWnE2ZFJOLVNkRDYxRng1QzZWeWd6aEJpMUtvdk9JVWVZbmhzalA3eWFXVUdpZGNCcUhxdW1BR2Z2aWNyNUYzQQ&q=https%3A%2F%2Fprag.works%2F202208-LWTN-Files&v=MrLnibFTtbA)[https://prag.works/202208-LWTN-Files](https://prag.works/202208-LWTN-Files)

  

**Books recommendations:**

Star Schema The Complete Reference -Christopher Adamson

The Data Warehouse Toolkit The Definitive Guide to Dimensional Modeling - Ralph Kimball, Margy Ross

  

![](https://lh6.googleusercontent.com/yNMikFwBedxf5ZdXB5fz8tYZftSIsmYGIBBn45i_vvS8zy197Nv7SyUJ05vm3jtr4Qi20GSdF-qRRjY8MlYaC7MftLqiTSjc-rSB0KKtINxC3Tz3KuVWstl0AYzkM_fFpzKYnv-xwZeR_G5Yk4oKBCI)

-   be specific what you trying to accomplish -> what you measure
    
-   user problems - what information is missing?
    
-   PBI - put everything in memory - optimize performance - limited amount of data
    
-   with time data will only growth and complex increase
    

![](https://lh3.googleusercontent.com/g1CCWtvZE6qPXmHR2Ph3a2fmYWktpgP4AYBoxixBd6AV0FihkQ6WA0CFhSF9iANye8G6srk2mL6HFJsyoFi3bUFUUqPjrStmEgRUMjr7VCe-eHtXSsBEzngJiHYlSv6Lfn_JhGiQ4glcT8qOoflNq6M)

  

Schemas: 

-   star
    
-   snowflakes
    
-   cube (?)
    

DIM = dimension

  
  

![](https://lh4.googleusercontent.com/YpLJ6LU5bd43ctqO-a_VMoYhI1FlXZ4QUdbWZwMTuReAc-UdvRj8ZXYqxT5h7GnnII_B151QXt68n85KaP8PgBlT392TvIY1R586pVyeUNne6PlT6RV33wksXaE8o7uOQqJ_Qgt8zJ5wSLf_-v3bEME)

  

Лучше не использовать:

![](https://lh4.googleusercontent.com/r9jPWnKDYGIEcGznDTEG6LbGqHwiULwa699ALGksVWBZZonhi2BVMxeRdFdy7KwaRMTEKSSQVTw69UWuG0g31jLX2Lkp6XRGL94OftP72dUDyjg-_c3aOhteAmPYTwxY2ByfJt8mJNG4lLmh4oVzpoo)

  

Start with tables and column data.

![](https://lh6.googleusercontent.com/DqVMpSHOUYmbF4M8nPDgCew3BnCPtjJzneqtOE28Fle-dk0H7CgZxxU-e46CoTyoI4V36JZeS0ZAfvLWMlix5KcK_Qvaiv1JddU8mS9sxsU7B-fCXTY9WatJlT-r9Z0fYQU90eYcougfi2xmi8yPt90)

  
  
  
  

![](https://lh3.googleusercontent.com/GgXDtlU3QagVSGuM0UflVxRUZXceWOpxqUPW2fTU1DzPULh8tXxvW6J8a-mR5wqqIesSqAi_rIXLzMHhqizli1W0rd2EuPiiXT_PvqPJ60rdxIP-7MP7TbDCM9xH1xXfU6WG2n1vTc3nO0E0ABVfywU)

  

![](https://lh3.googleusercontent.com/GBOWoZuYAfGXJ6K-j3cgsriep3SNgKJhB6QoYNW60MT3mc6A3rWOBnuPuPRdsC1KEYueQM07OsQ894MyU5Hf465JFkY9iwLoaLw6a0eqAGVEXlhGacqH8bMzASwXTu3YOHEMS790zRdG-5l-VBnxBdc)

  

![](https://lh5.googleusercontent.com/ldOB-kbsIABKubpauYjRC0cCo3cel3L3OKLXzK-0xNZMlf8zmewIyvTicHxFb9nkeUMo3rxc1yuRXvSt5eXTeggfiAwLcTAs4ngS6ZS86K94CExeGltsdK5bItnuPUUusQFGwzDN5eyA-mgZbsMBS7o)

  

![](https://lh5.googleusercontent.com/kmj8Mb4jjgt0pg5cmOeUy7DpHFZ_b8G5of77gigyREOlKZPtE835DJTGbqhhiB8Ufey0LgcxK-Sf0HrFab0msmVMpLKdDLP3e45wWuRtI887QZY5gQkSFRAwwHheTcUMbAfW9iGiKPSaLL0flBc_dLk)

  

Гранулярность - как можно меньше, мы всегда сможем укрупнить ее (но не сможем измельчить). Построенная модель не сможет отвечать на поставленные вопросы.

  

Если мы знаем, что будет очень много информации, и PBI будет сложно это переварить, то в самом начале важно это понимать.

  

![](https://lh3.googleusercontent.com/TwHsVgw8bqz4rTKNzPCfjt0wu2xdZdMCV5m0CLjB9drS_Oj3v7n07_k3caodnU9z-r9xrHxe53eosh2U9fKGUAhNiKzNkJOTo05ZYpBEOtANOdc-H8y2A-BXQpiYmDRfBdlJdjuAn0cQlYgnxPUs57I)

  

DIM - Это описательные характеристики данных.

  

![](https://lh3.googleusercontent.com/6QpJs0-90D83NhARY5r5eF6IGQF0Iwn3nQupBOt4S4bfUT79Dq7idbyeFORpGj-drTa959PSCfTNSs-lSQ2Bti_xyOhT5mc0Q6OANI8Hgkqmcdm3JMuzkfzWx0_5PjoeuGjJZb3ahpEc2avv4CGJvxg)

Отношения - DAX работает на этом - в описательных не должно быть повторений.

  

![](https://lh4.googleusercontent.com/YkCYbDtyUCeAo1Trij6xXynyEuuFvpqkpp1CIq0DVgsd4PzIib7u-giejtma4oHqzTnCMmdusvgp3-daH1aqqqq0ukzv4YwlsZuOTaYssxMLh3l8LhK_Xi4Y9KKvedOsmntrS7KbgkrzizxBD5WKuAU)

Ошибка - все в одну таблицу - привычка аналитиков из excel.

Одна таблица - меньше гибкости, больше объем.

  

![](https://lh3.googleusercontent.com/1rbdCZEDJb9PHLjgM_48A7z9l0Ni-6y11lfOLjTzArSIQ0J1oCjaymyNu2Vf7_WeSe2j--ljIyYU7RRFbBW5c791mjsxvL7o0uLspkqzxFWitzjJOlnBNGJXSUlW-5cDiuig89K8yA-hvMrmlA6ZW6A)

  

![](https://lh6.googleusercontent.com/FGPOTWpQgAdTtmfW_ctVGGAZU538C4Wvt0fHHIWiKI2Kex7Eelgnjhs6L7fpYr_iEqMHPvJWyZ69_1YAN6VLCkDmNiiob8Ghrb_WVmf7lenhR2XOehEV4oFEugnUnJvUnT9AG6q5c8gT_3AeboaW_7U)

  

Несмотря на наличие уникального ИД мы все равно в PBI добавляем искусственный ИД.

  

Важно, чтобы DIM были действительно описательные, помогали понять информацию (а не коды).

  
  
  

Практическое задание:

  

Начинаем с построения модели - Звезда.

Альтернатива - можно привязать географию к покупателю, тогда получится схема Снежинка.

![](https://lh5.googleusercontent.com/acTdMgp738kOBixvpPdwnQOtzbEt5EZ27fQgsp0mlfK5nKdKGLFc_wU8fBrCl6ZrwTlxmIHY1FH6_itYkm5YoeohveH27woT0VWNHqcqv83AAQppkCztKhAXWyWzBwhuWcLmAAbf0W1Zw92TeO5eew8)

  
  

Power Query - **создание DIM**

-   Лучше дублировать запрос, тогда мы можем позже к ней вернуться (если ссылка - не сможем)
    
-   размножим таблицу, оставим в каждой DIM  только нужные столбцы
    
-   удаляем дубликаты
    
-   Для ИД - добавляем ИНДЕКС столбец, начиная с 1
    
-   теперь нужно вернуться в первую таблицу и подтянуть туда по DIM уникальный созданный ИД
    

  
  

Что такое 3d normal form? Это не лучшая модель для аналитических отчетов в PBI. 

  

PowerQuery Date table:

[https://devinknightsql.com/2015/06/16/creating-a-date-dimension-with-power-query/](https://devinknightsql.com/2015/06/16/creating-a-date-dimension-with-power-query/)

  

(56:00) Запрос создает функцию - указать даны начала и окончания и выполнить - создается таблица - назовем DimDate. Проставить типы данных.

  

Сначала сохраняем модель, только потом применяем! чтобы не потерять настройки.

  

PQ recommendation book: 

Collect, Transform and Combine Data using Power BI and Power Query in Excel - Gil Raviv

хуже: M Is for (Data) Monkey A Guide to the M Language in Excel Power Query - Ken Puls, Miguel Escobar

  

Проверить, что все данные связаны в модели (иначе будут неверные данные).

  

![](https://lh5.googleusercontent.com/X5z6bGDfd3q3CtpJRmX4sh6gtRK-ToxxLMoBbwPlccbIcZkb6faRlf_KTFNaRvvvv5oPi1Jr8zxRhulEvmY6HpbEaOICe0P72O2-wjfmAK5OlC7rSby3ocyzPE-71IqTbqjPQRRxTy1aL3ad-EYV_40)

  

Отдельный FactTable, например, список возвратов, кроме списка продажных транзакций. (остатки на складах, бюджет, прогноз и тп)

![](https://lh3.googleusercontent.com/Y4ouiYHAEA50v5mUCjPfKWM_ov9pNd1r9aW4_-nyZ4LjJzF42QUDSnwd645U1ivp5pPLSihDe6xXj2-DMd5HttMWKQ9Ukhqad8dD3jufMarOZI_uUrxOvnK64_kbuvPgBdwCV3DokmLjGr6jvqIMPw4)

  

It would just be different star schemas. A star schema describes the relationship between 1 fact table and multiple dimensions. So you will have different schemas for every facttable.

  

Программа для рисунков на экране: [https://learn.microsoft.com/en-us/sysinternals/downloads/zoomit](https://learn.microsoft.com/en-us/sysinternals/downloads/zoomit)

  

Другие данные (например, бюджет) могут иметь другую грануляцию (месяц - категория)

  

![](https://lh6.googleusercontent.com/LfweMkpuV_yeH-TPWXg7r66iFcxDMpOKqCbPD8BJa3BnuvvFvTGVMR5lViekOAf5Dw2i8zePLEUIzaTm0C6W6dUDOvptBozWDcHPP7o9ixtOEwAyFnW9FEzaBTSdviNE1FFIT1qtnKyroNe2A94ZpxY)

  

Для создания связей - создать новый DIM - и так как он будет вынесен из таблицы, мы сможем фильтровать по нему сразу обе таблицы!

  

Type 2 dimensions - что то меняется - мы отслеживаем историю.

Чтобы отслеживать - добавляем surogate key - сурогатный ключ.

  

FactTable - сортируем по дате по возратстанию и добавляем ключ SK

  

Важно! ETL idea

После этого добавляем в таблицу продаж этот SK в зависимости от даты транзакции. 

? Как это сделать? нужно найти видео об этом.

Создаем DIM - для категорий из бюджета, потому что сейчас у нас нет такого DIM.

  

Дублируем таблицу и оставляем только 2 столбца - категория и сегмент? удаляем дубликаты, сортируем.

Добавляем SK.

! теперь важно вернуть этот SK снова в ФактТаблицу с продажами.

-   Murge queries - (можно только, если дублировались таблицы!)
    
-   по условию - категория и сегмент
    

  

![](https://lh5.googleusercontent.com/4xYBNiSp_xuKBvg4E8h4ifXbykyGD7f59OKZ_z1KHMwlo3KkbH43NsuninDR2174xV9w-7mi_-OqRjGp2xyoLN4MZ82GLkAJHB2OHK9KE9Ih3gAif0hmYgQgHWvh4b3ogjS2L_Iw3Ws3wSujVvMda8g)

  

![](https://lh4.googleusercontent.com/N2H0HHaGFUdiOSbNR6YDgOl0q1if-g-54AeSuzWBl7DQmMwZWUfYAJ9m-rqAeZ3rRAQFe_mB-T-b3kg0kl0J9tc834IF14B6oTs2tuoRBxdQm-nsHy-pIvNZLtR0duvBUM0gC8mHpSSJqvIFkHaQEGc)

  

теперь из таблицы можем удалить Категории и Сегменты. (reducing redundancy)

  

То же самое проделать для факттаблицы Бюджета.

  

В PBI можно создавать отдельные лейауты для отдельных ФактТаблиц, чтобы было удобнее работать с данными:

![](https://lh4.googleusercontent.com/3oa7Rp01twmjwDKrI5qUt4rRh2hNKjulAh3vkaKuO11Bhnu0OrHroWsT223DN5X4CnwG8il9R2jaEoOojhxTcqH0L2TkFrb1FNvYsMoirThRHfg09rHrCua17XjOWcC--msjMabEgOPrL2c0Wb1xkFo)

  

Roll Playing Tables - 

![](https://lh3.googleusercontent.com/Uqs44UJ2h95-0_WbafgIvOLObP1gN_s_9TOLi6jXG-mPlOiUlwmLxo5tyq51VC6r8PMnsK43oAgSH2HnPmj5NULfv-ZLs81lx4Lou_upoaQ7SAY6767slL0lBAcqeXkoASbNLS0XEWaeatyietockQ0)

Сейчас - фильтрация по дате заказа, а если нужно по дате отгрузки?

Можно добавить дату отгрузки в таблицу заказов.

  

Добавляем 3 Mesures:

![](https://lh4.googleusercontent.com/BUWoRqDLkiu6ntg0Bghbwq67g6j3nbaVnAPuXnBhbNZUI32KGQYPPMB9l-Q6k8RCb8Q0Y-eFq6H6LOfRw5smHdOluRF1hb43dqnWbaC1BTU5hX1ClBGHkBBkJrVR6ILWxkLOIQeQr3sRog7aaeXlyZU)

Total sales

Total costs

Total transactions

YTD sales

  

Вся фильтрация идет по году отгрузки:

![](https://lh5.googleusercontent.com/fLsYSFZ13nzat5wsTCX-YkMu8yKQ-bdqUCdCh8ePKLUQzuap0Iq27l4eb7S4bE5zFziDQlTuQmsMv4knRjO8lppubleZNd5hQGIG66JcikClDZmuEWIhcCnzIOxiJ0gmfOvfBXqveaNiButUDE5cBPE)

  
  

Решение - 

-   создание нескольких DateTables (не всегда приемлемо)
    
-   через DAX (сложность - нужно прописывать для каждого параметра)
    

  

Создаем дополнительную (неактивную) связь.

  

Используя Measures переписать фильтр - 

![](https://lh4.googleusercontent.com/k06IQ94d6DW_KMhXVjtQtnUPVgs2Qw17FpEhi3aiM-76vNI-MNVXX5WgmvhOl-qj-SyiZs68RZVDt2jXtFC1poWWn38yVDQVVgy95RWbXXQHX749tJud5pS0OwYAJjQJg04qmwrGG5MJgMP4NUSODOs)

  

![](https://lh5.googleusercontent.com/bh5CXUx217PD7xTdt6pyDoSnrMM4lNkRc7xIdM4UvOWZ4bhj3lDt6STG75s3IaDv0d8Ls06M3-HLZpJVHtCsMvCcFU2CSJFWuXTWBdyV9HpkYZHGZTvNKT2xTar1-cr-fu8-DMQ2pVhIl5OxAjuwT8c)

  
  

Больше про DAX - [https://www.youtube.com/watch?v=QJw4HkagVWc](https://www.youtube.com/watch?v=QJw4HkagVWc)

  

результат - по 2м параметрам - заказ и отгрузка

![](https://lh5.googleusercontent.com/NIApk5UkWJaiMyGfjjXtXeK-Nu7OyoNbeWUlRQw5KmDBVvXnOSXhkNDrlJ0mnsLDViq3VO3E2AB5Fjp5S7GNjKzWa4QCfsnheyiu3EF0ZlbkphaQQ2qEVWbhzdROgr0oRuVWdKeKEWaor1vMG6O1EsQ)

  

(1:55:00)

Альтернативное решение - Calculation Groups.

(находится в External Tools - Tabular Editor)

  

![](https://lh6.googleusercontent.com/KRRy5XmQJsycL-EgDi8pW3wCIPsTVSk7FDdsL51MzWZLb8OJnLciPQ3IHIYVU_EYoBI5R3KyWOE2nAoFzkpMNQBplvNUaYjQeGHROo565-hi7u0lJDda4q0IEvbA_KthVkZxv4j8C0_M_lVSiuLGYVE)

  

![](https://lh5.googleusercontent.com/uICUBxg3EbvkPm_458i47vuKOwNBFOyHm8Uhxm-jzf_mekcWzi8wRetLVlUqSd9w3by_QNFTGr2fCfkf9NPsqLs7OfvL5JRtt26j9WiIeWn9mvvQjT22mR3gzqWukNByCq0H2dThHM05JaPDPOo-uyE)

  

Создаем в группе - Current measure

![](https://lh3.googleusercontent.com/fZ4Qf_IUQqa4RIrXmIZrSwQi6_99oJ3Zf41GDwTTP47kEyBUKJBQbALY8x5Uyg7l7BMIRVTj73boAvdHZAeJ_ssCO4mABV-88zOM5LUxM4sIaE7l6fnYUd27ftUqrJhrpEZ25lEtdXQQXnyR6DlQ2UE)

  

Новая Calculation Item: byShipDate

![](https://lh5.googleusercontent.com/Cyp3LlRpVWnwOO5E2P4tWdteOWUVWvATQ9dM5dFB6gMPaliGmULLbY06LujqYSxePkpbNs7JI1im2HFRdaQsL6fm3paVV5rYGpNBdsLqn9PS7H7qrKkrO1Zo2GPQcNXLgRiQKPuAyTSk4O0YGeos-0E)

  

Можно перетаскивать изменения в формулу:

![](https://lh4.googleusercontent.com/z-9KjlLxrimkkJJ_RDg_hFI_MEn3mv4-lLat5veJ2OU5b1Nr-2EIjB9_Jrp5sClHIm40Kxg-rnXyw9adyBiow4hy58csDpr8-XnbdtnkCsUpQkOYY13fR2o3I38vXO83VSy7UkYsr2quU8NG8akmTp0)

  

После сохранения: 

  

![](https://lh6.googleusercontent.com/Tfdm7vx5128INHvYP-6mZHcNpP75V3i8ogGFUpu7DE3PYR_I7QgexFW-cLvBQlkER3cYeTU3tm_4FODcy8pECzWAHqUgekm-eqzoue_A96AG2gwDvPvK9vAfx_m3HCoTZ1hLI1uHGxizsGW3M4xDqd8)

  

Это работает теперь для всех измерений:

![](https://lh3.googleusercontent.com/Ey7QG_ZaZFTCOqda1l6uAu7CuiZBAwXDR8hbWm50zX9M2xwJeAmUtq2wonlVh-zF8BQ2znUHHjg3g1__5Kzia_yMzsucCpOsZdI4O73_RP1L9xiVfU_tI52EjdxJV-9hUCtLfrgRKa7oykzuBbUNu8g)

  

Можно также использовать для расчета YTD.

  

Подробнее как с этим работать: 

Leverage Calculation Groups in Power BI to create a single DAX measure for role playing tables - [https://www.youtube.com/watch?v=yGSB4F6-mlY](https://www.youtube.com/watch?v=yGSB4F6-mlY)

  
  

Установить границы начала и конца модели?

  

через Параметры! для фильтра

![](https://lh4.googleusercontent.com/IH7489qim0gN_mYa6rutbmhKvp8ocSTTMo-WobkHss6x9rwWXbvO3-OtX9FUV9XINjiHY63MI-Kt3aRskG96PXNwIkB1d_quXSPdqfHeW_RXWg5JvcdpP5gPxhl0EQP4HM1PUMBcV6fYEScc1JVOj58)

  

создаем параметры для дат

![](https://lh6.googleusercontent.com/nD8q-nQXMvr3q0iE95blfRMBemdZ7YLVtXm0ktVZEGFuZU3e6Cp0SJde3cJMHdvUOy8NxxUgrawFwcPEAQcFHwd8LpwAeu6TuDqdreKqOGeP60tDqw32ZXUtxEIGD-VxeNesvcIi33zvl9XbCnjnEL4)

  

![](https://lh3.googleusercontent.com/3-RMNILKZG9DkUtVWwAGaCW58CQhdikdsVA7QFxJq_iheclRRhCkopxRDKBe5HE0wR7tfNLBEGyO-VZjpZJIynLKeQIU63DIIpJmHHhJM-g98HmSe1sBpIGBRsfxMxdridmFl2ypMYeyj9pd6mp208A)

  

и теперь в фильтре можно выбрать Параметр:

![](https://lh4.googleusercontent.com/n4KGkR9QGZaFK4wzy1CrBrJg7vHaDv04lw3UWRoXeQ1yTDxfaXIaF7Ss6N2YucvNixZVRWVGCpPkiqGVr9znB5KbM49gBB4Fgcm8PIxL4GeOjs3R5Up3_-BXXw1Ks1UFe7cJYTi6VLtP23Z_k3hLXZk)

  

(2:06:00)

Если много данных, это может снизить скорость работы отчета.

Решение - создание Aggregated (snapshot) FactTables.

  

Add data to PQ:

-   import data (aggregated)
    
-   direct query
    
-   live connection to analysis services
    

  

Агрегацию можно делать на сервере через SQL или PQ.

  

PQ:

-   group by
    
-   ![](https://lh5.googleusercontent.com/zXlPLvtUW-d7kDKLXrQXvE9rJv9KZqUKmu2lBFfE14aNdL7TiRCykiGPdISqPXecEad-JvQvfdVZCL4-uzO6Ab6t_C009v_L9I7fm-L4NP5wMuIaoyAbLmxUZR01DgcQe3p7qqt5Vl9HF3QBNgJKt7M)
    
-   уменьшение данных (кол-во транзакций)
    
-   ![](https://lh4.googleusercontent.com/90_BTgmwgTmcrtYUmrcYcKDTVEL7H-d0L52Ra3_-nkk6rw4VZBdPuRj0d-wDdvfR0uAYnpeWKGQKTBwlNt-QsDngx-KfCx6-xJl7rVsbtw-tnZyN48CHh0a3EVv7ffX1AECnfH3lVCV18VRTMC5PgwY)
    
-   такие таблицы быстрее работают для вычислений, чем оригинальные, так как там меньше строк.
    
-   Проблема! теперь фильтрация может не работать, так как мы удалили эту информацию при агрегации
    
-   ![](https://lh3.googleusercontent.com/TpR6Go0Kf1NsFt4gITDpvwV9-DyHqg9ulpDxgHv6C9Djd_r6qYO6QV6okr-3hb7KNNHZs_Y4xD95jsXxCedglKCYD7K0gxTvYZbKpj2iOlVjODm1KXe582j0FSIh7Eq84UzB9EGeZh3f6g-HeA0sgbQ)
    
-   Решение: Aggregation by PBI (изучить отдельно)
    
-   Если исходной таблицы нет, но она все еще используется в отчете, то можно:
    
-   ![](https://lh5.googleusercontent.com/NM8s8usu6_iJIPtipekpyRldyhmiHy0LdDjITYW4qFYF-ruLH69ylhq0ZGsJWCIt_RXE_rnr5sSha2pMihkZqKAHHVXICIuJmBqa7a-9qyYMWJeDqsWl0HJYcECfYnVXxClVUwmn3j0obT3Qdfh440o)
    
-   ![](https://lh5.googleusercontent.com/IB3pov5UetppwDmkUqRGGo-FBhc4bZGBHq8k_ArBTm563TOHaQIrYCx7_ImAttfy284I491N1_HbYdy1hUYpll6WWarVyymHlTZL1gi735wXOTzDfaIQpyA_6cit1lLBP7lam9M6AQoGKufNf9xbp_8)
    
-   через ссылки на direct query
    
-   после сохранения таблица не будет видна пользователям, но будет использоваться при вычислениях (пока мне не очень понятно…)
    

  

В настройках Data Load - отключить Time Intelligence (для всего или для файла) - тогда НЕ будет создаваться автоматическая иерархия для каждой даты.

![](https://lh4.googleusercontent.com/9XLOS8QXhlAG3n6sFDBIgI9nP7S5vH2Kl_PZTrysU59Knb99obSp9Ke-Ghw-36yJSJbcSI65RKrJnYac3ickilhC2P321W456HjVedRTBc9O3hlNYtabj8uDz0CTSqJYsCMa7mxpif9xE-1otq9XN5k)

  

Вместо этого - пометить таблицу как Date Table (через GRV)

![](https://lh4.googleusercontent.com/2ZcttE6N9iZxTWA_FIrQIZQNh67sDaRchf4rQ_3GHzCXWgJevHKIRnY64OOzGfChagfx5KGSmBrzUhdciWGqho8MVSezq2PIT7RWyJr8ZlxsCi3X3qBv2_T7x-s1dzirSd4o9q4LMrWDcoBBWabAhuA)

  

Загрузка в PowerPoint: [https://learn.microsoft.com/en-us/power-platform-release-plan/2022wave1/power-bi/power-bi-integration-powerpoint](https://learn.microsoft.com/en-us/power-platform-release-plan/2022wave1/power-bi/power-bi-integration-powerpoint)

 install an addon in Power Point to be able to imbed Power BI visual. great feature though.

  

Для расчета части бюджета (например с 1го числа по сегодня, когда у нас есть месяц), то используются меры, которые вычисляют дни в месяце, дни на сейчас и берут эту долю. При это мажно, чтобы фильтры тоже остались работающими.

  
  
  
  
**