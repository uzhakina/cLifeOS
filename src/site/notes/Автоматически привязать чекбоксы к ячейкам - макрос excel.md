---
{"dg-publish":true,"permalink":"/avtomaticheski-privyazat-chekboksy-k-yachejkam-makros-excel/"}
---


⬆::
⬅::
📅:: [[2023-02-26\|2023-02-26]] 

# Автоматически привязать чекбоксы к ячейкам - макрос excel
Источник:: https://youtu.be/cqq6lS23lGM

![Pasted image 20230226231908.png](/img/user/Pasted%20image%2020230226231908.png)



👉 VBA Code: 
```
Sub LinkCheckBoxes() 
Dim chk As CheckBox 
Dim lCol As Long 
lCol = 3 'number of columns to the right of checkbox 
For Each chk In ActiveSheet.CheckBoxes 
	With chk 
		.LinkedCell = _ .TopLeftCell.Offset(0, lCol).Address 
	End With 
Next chk 
End Sub
```


