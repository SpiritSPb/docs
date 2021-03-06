---
title: 'value (input elements)'
attributions:
  - 'Microsoft Developer Network: [[Windows Internet Explorer API reference](http://msdn.microsoft.com/en-us/library/ie/hh828809%28v=vs.85%29.aspx) Article]'
compatibility:
  feature: 'value (input elements)'
  topic: html
notes:
  - 'Review import; Remove MS bias; Update/improve example; Update descriptions; Fix lists & compatibility info'
readiness: 'Not Ready'
tags:
  - Markup_Attributes
  - HTML
  - Needs_Summary
uri: 'html/attributes/value (input elements)'

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

This example uses the **input type=text** element to create an empty text control that can contain 15 characters without requiring the user to scroll to read all of the text.

``` html
<INPUT TYPE=text VALUE="" NAME="textbox" SIZE=15>
```

This example uses script to detect the content of the text box and display it in a dialog box.

``` html
<SCRIPT>
function detectEntry()
{
    alert("Your name is " + textbox.value)
}
</SCRIPT>
```

## Notes

### Remarks

The purpose of the **value** property depends on the type of control as described in the following table. {

### Syntax

### Standards information

-   [HTML 4.01 Specification](http://go.microsoft.com/fwlink/p/?linkid=25320), Section 17.4

## See also

### Related pages

-   `input`
-   `input type=checkbox`
-   `input type=password`
-   `input type=text`
-   `input type=file`
-   `input type=hidden`
-   `input type=button`
-   `input type=radio`
-   `input type=reset`
-   `input type=submit`
-   input type=range[input type=range](/html/elements/input/type/range)
-   input type=number[input type=number](/html/elements/input/type/number)
-   input type=email[input type=email](/html/elements/input/type/email)
-   input type=url[input type=url](/html/elements/input/type/url)
-   input type=tel[input type=tel](/html/elements/input/type/tel)
