---
{"dg-publish":true,"permalink":"/excel-vydelenie-kazhdoj-vtoroj-stroki-cherez-uslovnoe-formatirovanie/"}
---


⬆:: [[Excel\|Excel]]
⬅:: [[Условное форматирование\|Условное форматирование]]
📅:: [[2023-01-29\|2023-01-29]] 

# Excel - выделение каждой второй строки через условное форматирование


Нашла прикольную "фишку" - форматирование каждой второй строки через условное форматирование:
Прописываем правило:
```
=ОСТАТ(СТРОКА();2)
=MOD(ROW(),2)
```

если значение "правда" (в этом примере - четная строка), то применяется условное форматирование.

![Рис - условное форматирование каждой второй строки excel.png](/img/user/%D0%A0%D0%B8%D1%81%20-%20%D1%83%D1%81%D0%BB%D0%BE%D0%B2%D0%BD%D0%BE%D0%B5%20%D1%84%D0%BE%D1%80%D0%BC%D0%B0%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5%20%D0%BA%D0%B0%D0%B6%D0%B4%D0%BE%D0%B9%20%D0%B2%D1%82%D0%BE%D1%80%D0%BE%D0%B9%20%D1%81%D1%82%D1%80%D0%BE%D0%BA%D0%B8%20excel.png)

Источник: [[_EXCEL DATA ANALYSIS BY EXAMPLES - Thanh Tran\|_EXCEL DATA ANALYSIS BY EXAMPLES - Thanh Tran]]

