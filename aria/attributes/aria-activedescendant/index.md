---
title: 'aria-activedescendant'
attributions:
  - 'Microsoft Developer Network: [[Windows Internet Explorer API reference](http://msdn.microsoft.com/en-us/library/ie/hh828809%28v=vs.85%29.aspx) Article]'
compatibility:
  feature: aria-activedescendant
  topic: aria
notes:
  - 'Needs summary, example, spec reference, standardization status'
readiness: 'Not Ready'
tags:
  - Markup_Attributes
  - ARIA
  - Needs_Summary
  - Needs_Examples
todo_broken_links:
  note: 'During import MediaWiki could not find the following links, please fix and adjust this list.'
  links:
    - dom/events/keypress
uri: aria/attributes/aria-activedescendant

---
<table class="wikitable">
<tr>
<th>
Applies to

</th>
<td>
</td>
</tr>
</table>
## Notes

### Remarks

<table class="wikitable">
<tr>
<th>
Used in Roles

</th>
<td>
<dl>

<dt>
composite

</dt>
<dt>
group

</dt>
<dt>
textbox

</dt>
</dl>
</td>
</tr>
</table>
  To simplify keyboard navigation, an element that gains focus may specify the currently active child element by [**id**](/html/attributes/id).

The container element should change the designated descendant during a [**keypress**](/w/index.php?title=dom/events/keypress&action=edit&redlink=1) event. The container should also ensure that the current child has a style that visibly shows it is active, such as an outline or different background color. **Note**  For cross-browser compatibility, always use the WAI-ARIA attribute syntax to access and modify ARIA properties, for example `object.setAttribute("aria-valuenow", newValue)`.

### Syntax

### Standards information

-   [Accessible Rich Internet Applications (WAI-ARIA) 1.0](http://go.microsoft.com/fwlink/p/?linkid=203793), Section 6.6

## See also

### Related pages

-   Accessible Rich Internet Applications (ARIA)[Accessible Rich Internet Applications (ARIA)](/aria)
