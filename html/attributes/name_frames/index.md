---
title: 'name (frames)'
attributions:
  - 'Microsoft Developer Network: [[Windows Internet Explorer API reference](http://msdn.microsoft.com/en-us/library/ie/hh828809%28v=vs.85%29.aspx) Article]'
compatibility:
  feature: 'name (frames)'
  topic: html
notes:
  - 'Review import; Remove MS bias; Update/improve example; Update descriptions; Fix lists & compatibility info'
readiness: 'Not Ready'
tags:
  - Markup_Attributes
  - HTML
  - Needs_Summary
uri: 'html/attributes/name (frames)'

---
<table class="wikitable">
<tr>
<th>
Applies to

</th>
<td>
 ?

</td>
</tr>
</table>
## Examples

This example uses scripting to set the **name** property of a frame.

``` html
parent.frames[0].name="Left";
```

This example shows how the **NAME** attribute for a window can be persisted in HTML, but only when defined in a frame within a frameset.

``` html
<FRAMESET>
    <FRAME NAME="Left" SRC="blank.htm">
    <FRAME NAME="Right" SRC="contents.htm">
</FRAMESET>
```

## Notes

### Remarks

The **name** property identifies which frame displays the content of a linked document.

### Syntax

## See also

### Related pages

-   `frame`
-   `frameSet`
-   `iframe`
