<div align="center">

## CSS/VBScript change background\-color of txt\-fields after type in


</div>

### Description

A real good way to show wich txtfields are required in a form!

If you type in some stuff in the txtfield, the color change.

In the example the color change from red to green.
 
### More Info
 
Works only in IE but you dont get a Failure msg or something like that in NS

Create a Textfield like

<input type="text" style="background-color:#FF0000;color:#FFFFFF" onchange="OC(T1)" name="T1" size="20">

Be sure that you've the name of the textfield in  onchange="OC(T1)"  (Here T1)

Put the following Script in the Body-Section of your Page

>>>>>>>>>>

PS: You can use every css attribute if you like to change not only the colors!

If you dont know the Scripting Version for the css attributes (for example html: style="BACKGROUND-COLOR:#FFFFFF" scripting: style.backgroundcolor="#FFFFFF") you will find it under http://msdn.microsoft.com/workshop/author/css/reference/attributes.asp

If you like this easy small script then please vote for me!


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Mathias Stocker](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/mathias-stocker.md)
**Level**          |Beginner
**User Rating**    |4.8 (19 globes from 4 users)
**Compatibility**  |ASP \(Active Server Pages\), HTML, VbScript \(browser/client side\)

**Category**       |[Documents/ Frames](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/documents-frames__4-27.md)
**World**          |[ASP / VbScript](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/asp-vbscript.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/mathias-stocker-css-vbscript-change-background-color-of-txt-fields-after-type-in__4-6546/archive/master.zip)





### Source Code

```
<SCRIPT Language = "vbscript">
Function OC(object)
if len(object.value)>0 then
object.style.backgroundcolor="#00FF00"
object.style.color="#000000"
else
object.style.backgroundcolor="#FF0000"
object.style.color="#FFFFFF"
end if
End Function
</SCRIPT>
```

