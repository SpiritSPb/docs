---
title: 'finish'
attributions:
  - 'Microsoft Developer Network: [[Windows Internet Explorer API reference](http://msdn.microsoft.com/en-us/library/ie/hh828809%28v=vs.85%29.aspx) Article]'
code_samples:
  - 'http://samples.msdn.microsoft.com/workshop/samples/author/dhtml/refs/onfinishEX.htm'
notes:
  - 'Needs summary, spec reference, standardization status'
readiness: 'In Progress'
tags:
  - Events
  - DOM
  - Needs_Summary
uri: dom/Event/finish

---
## Overview Table

<table class="wikitable">
<tr>
<th>
Synchronous

</th>
<td>
No

</td>
</tr>
<tr>
<th>
Bubbles

</th>
<td>
No

</td>
</tr>
<tr>
<th>
Target

</th>
<td>
dom/Element

</td>
</tr>
<tr>
<th>
Cancelable

</th>
<td>
No

</td>
</tr>
<tr>
<th>
Default action

</th>
<td>
 ?

</td>
</tr>
</table>
## Examples

The example uses the **srcElement** property of the event object to determine which marquee has fired the **onfinish** event.

``` html
<body>
<label>mqLooper1</label>
<marquee id="mqLooper1" loop="2"
    onfinish="alert(event.srcElement.id + ' finished looping.')">
this marquee loops twice </marquee>
<hr>
<label>mqLooper2</label>
<marquee id="mqLooper2" loop="5"
onfinish="alert(event.srcElement.id + ' finished looping.')">
this marquee loops five times </marquee>
</body>
```

[View live example](http://samples.msdn.microsoft.com/workshop/samples/author/dhtml/refs/onfinishEX.htm)

## Notes

### Remarks

A value greater than 1 and less than infinity must be set on the [**LOOP**](/html/attributes/loop) attribute for this event to fire. Marquee ceases to loop. To invoke this event, do one of the following:

-   Specify a value for the [**LOOP**](/html/attributes/loop) attribute of the **marquee** object.

The *pEvtObj* parameter is required for the following interfaces:

-   **HTMLAnchorEvents2**
-   **HTMLAreaEvents2**
-   **HTMLButtonElementEvents2**
-   **HTMLControlElementEvents2**
-   **HTMLDocumentEvents2**
-   **HTMLElementEvents2**
-   **HTMLFormElementEvents2**
-   **HTMLImgEvents2**
-   **HTMLFrameSiteEvents2**
-   **HTMLInputFileElementEvents2**
-   **HTMLInputImageEvents2**
-   **HTMLInputTextElementEvents2**
-   **HTMLLabelEvents2**
-   **HTMLLinkElementEvents2**
-   **HTMLMapEvents2**
-   **HTMLMarqueeElementEvents2**
-   **HTMLObjectElementEvents2**
-   **HTMLOptionButtonElementEvents2**
-   **HTMLScriptEvents2**
-   **HTMLSelectElementEvents2**
-   **HTMLStyleElementEvents2**
-   **HTMLTableEvents2**
-   **HTMLTextContainerEvents2**
-   **HTMLWindowEvents2**

### Syntax

### Standards information

There are no standards that apply here.

### Event handler parameters

*pEvtObj* [in]
:   Type: ****IHTMLEventObj****
