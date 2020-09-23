<div align="center">

## Windows Drawn Drop Shadow


</div>

### Description

Ever wonder how Windows XP draws the drop shadow on menus and tooltips? Now you can draw the drop shadow on forms. Perfect for splash screens. For Windows XP (and Server 2003?) only. Visual Basic .NET. Copy this to your form code.

Update: Thanks to the annonimus coder, now C# ready!
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[The New iSoftware Company\!](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/the-new-isoftware-company.md)
**Level**          |Intermediate
**User Rating**    |4.7 (33 globes from 7 users)
**Compatibility**  |C\#, VB\.NET
**Category**       |[GUIs](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/guis__10-30.md)
**World**          |[\.Net \(C\#, VB\.net\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/net-c-vb-net.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/the-new-isoftware-company-windows-drawn-drop-shadow__10-3392/archive/master.zip)





### Source Code

```
' VB.NET
Protected Overrides ReadOnly Property CreateParams() As System.Windows.Forms.CreateParams
 Get
  Const CS_DROPSHADOW = &H20000
  Dim cp As CreateParams = MyBase.CreateParams
  cp.ClassStyle = cp.ClassStyle Or CS_DROPSHADOW
  Return cp
 End Get
End Property
//C#
///
<summary>
/// This property adds drop shadows to the for(in WinXP+)
///
</summary>
protected override System.Windows.Forms.CreateParams CreateParams
{
 get
 {
  const int CS_DROPSHADOW = 0x20000;
CreateParams cp = base.CreateParams;
 cp.ClassStyle = cp.ClassStyle | CS_DROPSHADOW;
  return cp;
 }
}
```

