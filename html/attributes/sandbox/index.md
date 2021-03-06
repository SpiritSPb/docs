---
title: 'sandbox'
attributions:
  - 'Microsoft Developer Network: [[Windows Internet Explorer API reference](http://msdn.microsoft.com/en-us/library/ie/hh828809%28v=vs.85%29.aspx) Article]'
compatibility:
  feature: sandbox
  topic: html
notes:
  - 'Review import; Remove MS bias; Update/improve example; Update descriptions; Fix lists & compatibility info'
readiness: 'Not Ready'
tags:
  - Markup_Attributes
  - HTML
  - Needs_Summary
uri: html/attributes/sandbox

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

The following example shows how to use the **sandbox** attribute to enable sandbox restrictions.

``` html
<iframe sandbox src="frame1.html"></iframe>
```

The following example shows a sandboxed **iframe** element that uses customization flags to customize the restrictions for the content in the element.

``` html
<iframe sandbox="allow-forms allow-same-origin" src="frame1.html"></iframe>
```

## Notes

### Remarks

When the **sandbox** attribute is specified for an **iframe** element, the content in the **iframe** element is said to be *sandboxed.* In addition, the following restrictions are applied to the **iframe** element:

-   Sandboxed content cannot open pop-up windows or new browser windows. Methods that open pop-up windows (such as **createPopup**(), **showModalDialog**(), **showModelessDialog**(), and **window.open**()) , fail silently.
-   Links cannot be opened in new windows.
-   Sandboxed content is considered to be from a unique domain, which prevents access to APIs that are protected by the same-origin policy such as cookies, local storage, and the Document Object Model (DOM) of other documents.
-   The top window cannot be navigated by sandboxed content.
-   Sandboxed content cannot submit form data.
-   Plugins (**object**, **applet**, **embed**, or **frame**) do not instantiate.
-   Automatic element behavior is disabled, including **audio** and **video** elements.
-   Selected features proprietary to Windows Internet Explorer are disabled for sandboxed content, including HTML Components (HTCs), binary behaviors, databinding, and **window.external**.

To customize sandbox restrictions for a given **iframe** element, specify one or more of the possible values as the value for the **sandbox** attribute. Use spaces to separate multiple values.

### Syntax

## See also

### Related pages

-   `HTMLIFrameElement`
