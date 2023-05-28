---
{"dg-publish":true,"permalink":"/power-bi-calendar/"}
---


⬆:: [[Power BI\|Power BI]]
⬅::
📅:: [[2023-04-24\|2023-04-24]] 

# Power BI - Calendar

#### Код из книги:

[[DAX для профессионалов\|DAX для профессионалов]]

![Pasted image 20230424124806.png](/img/user/Pasted%20image%2020230424124806.png)

```
Date table with CALENDARAUTO =

ADDCOLUMNS(

    CALENDARAUTO(),

    "Year", YEAR([Date]),

    "MthNr", MONTH([Date]),

    "Mth", FORMAT([Date],"mmmm"),

    "Year Month", FORMAT([Date], "yyyy-mm")

)
```


```
Date table with CALENDARAUTO =

ADDCOLUMNS(

    CALENDARAUTO(),

    "Год", YEAR([Date]),

    "Номер месяца", MONTH([Date]),

    "Месяц", FORMAT([Date],"mmmm"),

    "Год и Месяцh", FORMAT([Date], "yyyy-mm")

)
```



#### Календарь + русские названия месяцев:

```
Date table with CALENDARAUTO = 
ADDCOLUMNS(
    CALENDARAUTO(),
    "Year", YEAR([Date]),
    "MthNr", MONTH([Date]),
    "Mth", FORMAT([Date],"mmmm"),
    "Year Month", FORMAT([Date], "yyyy-mm"),
    "RusMonth", SWITCH(MONTH([Date]), 1, "янв", 2, "фев", 3, "мар", 4, "апр", 5, "май", 6, "июн", 7, "июл", 8, "авг", 9, "сен", 10, "окт", 11, "ноя", 12, "дек", "нет" )
)
```

