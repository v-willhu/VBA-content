
# ChartFont Object (Word)

Contains the font attributes (font name, font size, color, and so on) for an object chart.


## Remarks

If you do not want to format all the text in an  **[AxisTitle](ec746a05-40df-95cc-c017-40ef150504cf.md)** , **[ChartTitle](fc8ca540-0a29-123b-2fdf-b16aaa1f940c.md)** , **[DataLabel](b955596d-ac94-1e18-4e72-cdf090fc1f9e.md)** , or **[DisplayUnitLabel](9b028f6c-fd66-f767-f3d1-09de0fbdc148.md)** object the same way, use the **Characters** property of that object to first return a subset of the text as a **[ChartCharacters](cffe50a7-3fdc-75ad-2e32-081ba2310c1d.md)** object. Then use the **[Font](bb7f3c4a-be15-7215-f50f-3ecaabcbc454.md)** property of the **ChartCharacters** object to return a **ChartFont** object you can use to format the subset of text, as needed.


## Example

The following example formats the title of the first chart as bold. Use the  **Font** property to return the **ChartFont** object.


```vb
With ActiveDocument.InlineShapes(1).Chart 
 .AxisTitle.Font.Bold = True 
End With
```


## See also


#### Other resources



[Word Object Model Reference](http://msdn.microsoft.com/library/be452561-b436-bb9b-6f94-3faa9a74a6fd%28Office.15%29.aspx)
