---


manager: soliver
ms.date: 3/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Server Ribbon schema
api_type:
- schema
ms.assetid: 596d39c6-ee39-41d4-92d6-c99942a6438f
---

![Collapse
section]![Expand
section] "Expand section")![]()![])![]![]()![Copy
code] "Copy code")![Copy code
hover]( "Copy code hover")
<table>
<tbody>
<tr class="odd">
<td align="left"></td>
</tr>
</tbody>
</table>

Visual Basic  
C\#  
C++  
JavaScript  

<table>
<tbody>
<tr class="odd">
<td align="left"><span id="runningHeaderText"></span></td>
</tr>
<tr class="even">
<td align="left"># ToggleButton Element</td>
</tr>
<tr class="odd">
<td align="left"><span id="headfeedbackarea" class="feedbackhead"><a href="javascript:SubmitFeedback(&#39;docthis@Microsoft.com&#39;,&#39;&#39;,&#39;&#39;,&#39;&#39;,&#39;1.0.18082.1225&#39;,&#39;%0\dThank%20you%20for%20your%20feedback.%20The%20developer%20writing%20teams%20use%20your%20feedback%20to%20improve%20documentation.%20While%20we%20are%20reviewing%20your%20feedback,%20we%20may%20send%20you%20e-mail%20to%20ask%20for%20clarification%20or%20feedback%20on%20a%20solution.%20We%20do%20not%20use%20your%20e-mail%20address%20for%20any%20other%20purpose%20and%20we%20delete%20it%20after%20we%20finish%20our%20review.%0\AFor%20further%20information%20about%20the%20privacy%20policies%20of%20Microsoft,%20please%20see%20http://privacy.microsoft.com/en-us/default.aspx.%0\A%0\d&#39;,&#39;Customer%20feedback&#39;);">Send feedback</a></span></td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"></td>
</tr>
</tbody>
</table>

**Last modified:** March 09, 2015

**Applies to**: SharePoint 2016 | SharePoint Foundation 2013 |
SharePoint Online | SharePoint Server 2013

Defines a button that is used to switch states.

<span codelanguage="other"></span>
<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><pre><code>&lt;ToggleButton
  Alt=&quot;Text&quot;
  Command=&quot;Text &quot;
  CommandValueId=&quot;Text&quot;
  Description=&quot;Text&quot;
  Id=&quot;Text&quot;
  LabelCss=&quot;CSS Class Selector&quot;
  LabelText=&quot;Text&quot;
  Image32by32=&quot;Url&quot;
  Image32by32Class=&quot;CSS Class Selector&quot;
  Image32by32Left=&quot;Negative Integer&quot;
  Image32by32Top=&quot;Negative Integer&quot;
  Image16by16=&quot;Url&quot;
  Image16by16Class=&quot;CSS Class Selector&quot;
  Image16by16Left=&quot;Negative Integer&quot;
  Image16by16Top=&quot;Negative Integer&quot;
  MenuItemId=&quot;Text&quot;
  QueryCommand=&quot;Text&quot;
  Sequence=&quot;Integer&quot;
  TemplateAlias=&quot;Text&quot;
  ToolTipImage32by32=&quot;Url&quot;
  ToolTipImage32by32Class=&quot;CSS Selector&quot;
  ToolTipImage32by32Left=&quot;Negative Integer&quot;
  ToolTipImage32by32Top=&quot;Negative Integer&quot;
  ToolTipTitle=&quot;Text&quot;
  ToolTipDescription=&quot;Text&quot;
  ToolTipHelpKeyWord=&quot;Text&quot;
  ToolTipShortcutKey=&quot;Text&quot;
/&gt;</code></pre></td>
</tr>
</tbody>
</table>


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left"><p>Attribute</p></th>
<th align="left"><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>**Alt**</p></td>
<td align="left"><p>Optional. Alternative text that is used for the control.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**Command**</p></td>
<td align="left"><p>Optional. The name of the command to execute when the control is clicked. If the control is in a <a href="commanduidefinition-element.htm">CommandUIDefinition</a> element, the value of the **Command</span> attribute of the control should be the same as the value of the <span class="keyword">Command** attribute of a corresponding <a href="commanduihandler-element.htm">CommandUIHandler</a> element.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**CommandValueId**</p></td>
<td align="left"><p>Optional. A string that is sent with the command event when the button is clicked.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**Description**</p></td>
<td align="left"><p>Optional. A string that describes the button.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**Id**</p></td>
<td align="left"><p>Required. A string that identifies the control, such as &quot;Ribbon.Library.ViewFormat.Standard&quot;.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**LabelCss**</p></td>
<td align="left"><p>Optional. The name of a CSS class selector to be applied to the control's label.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**LabelText**</p></td>
<td align="left"><p>Optional. Text to label the control.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**Image32by32**</p></td>
<td align="left"><p>Optional. A server-relative URL to a file that contains a 32-by-32-pixel image to be used as an icon, such as &quot;/_layouts/1033/images/formatmap32x32.png&quot;.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**Image32by32Class**</p></td>
<td align="left"><p>Optional. The name of a CSS class selector to be applied to the image.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**Image32by32Left**</p></td>
<td align="left"><p>Optional. A negative integer that represents an offset for the left edge of the image. Use this attribute when the **Image32by32** attribute points to an image file that contains images for many icons.</p>
<p>The value of the **Image32by32Left</span> attribute is used to set the CSS <span class="keyword">left</span> attribute for the inline style of an HTML <span class="keyword">img</span> tag. For example, setting the <span class="keyword">Image32by32Left</span> attribute to &quot;<span class="input">-160</span>&quot; and the <span class="keyword">Image32by32Top</span> attribute to &quot;<span class="input">-448**&quot; results in an inline style that is similar to the one in the following HTML markup:</p>
<div class="code">
<span codelanguage="html"></span>
HTML 
<span class="copyCode" onclick="CopyCode(this)" onkeypress="CopyCode_CheckKey(this, event)" onmouseover="ChangeCopyCodeIcon(this)" onmouseout="ChangeCopyCodeIcon(this)" tabindex="0"><img src="../icons/copycode.gif" title="Copy code" alt="Copy code" />Copy code</span>
<pre><code>&lt;img src=&quot;/_layouts/1033/images/formatmap32x32.png&quot; style=&quot;position: absolute;left: -160px;top: -448px;&quot; /&gt;</code></pre>
</div></td>
</tr>
<tr class="odd">
<td align="left"><p>**Image32by32Top**</p></td>
<td align="left"><p>Optional. A negative integer that represents an offset for the top edge of the image. Use this attribute when the **Image32by32</span> attribute points to an image file that contains the images for many icons. The value of the <span class="keyword">Image32by32Top</span> attribute is used to set the CSS <span class="keyword">top</span> attribute for the inline style of an HTML <span class="keyword">img** tag.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**Image16by16**</p></td>
<td align="left"><p>Optional. A server-relative URL to a file that contains a 16-by-16-pixel image to be used as an icon, such as &quot;/_layouts/1033/images/formatmap16x16.png&quot;.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**Image16by16Class**</p></td>
<td align="left"><p>Optional. The name of a CSS class selector to be applied to the image.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**Image16by16Left**</p></td>
<td align="left"><p>Optional. A negative integer that represents an offset for the left edge of the image. Use this attribute when the **Image16by16</span> attribute points to an image file that contains images for many icons. The value of the <span class="keyword">Image16by16Left</span> attribute is used to set the CSS <span class="keyword">left</span> attribute for the inline style of an HTML <span class="keyword">img** tag.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**Image16by16Top**</p></td>
<td align="left"><p>Optional. A negative integer that represents an offset for the top edge of the image. Use this attribute when the **Image16by16</span> attribute points to an image file that contains images for many icons. The value of the <span class="keyword">Image16by16Top</span> attribute is used to set the CSS <span class="keyword">top</span> attribute for the inline style of an HTML <span class="keyword">img** tag.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**MenuItemId**</p></td>
<td align="left"><p>Optional. A string that identifies the menu item where the button is located.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**QueryCommand**</p></td>
<td align="left"><p>Optional. The name of the command to execute when polling for state information.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**Sequence**</p></td>
<td align="left"><p>Optional. An integer that specifies the order of placement among sibling XML nodes.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**TemplateAlias**</p></td>
<td align="left"><p>Optional. A string that matches the value of the **TemplateAlias</span> attribute for a <a href="controlref-element.htm">ControlRef</a> element, an <a href="overflowarea-element.htm">OverflowArea</a> element, or an <a href="overflowsection-element.htm">OverflowSection</a> element in a <a href="grouptemplate-element.htm">GroupTemplate</a> element. The <span class="keyword">TemplateAlias** attribute is used to size and position controls within a group when a template is applied to the group.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**ToolTipImage32by32**</p></td>
<td align="left"><p>Optional. A server-relative URL to a file that contains a 32-by-32-pixel image to be used in the tooltip, such as &quot;/_layouts/1033/images/formatmap32x32.png&quot;.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**ToolTipImage32by32Class**</p></td>
<td align="left"><p>Optional. The name of a CSS class selector to be applied to the tooltip image.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**ToolTipImage32by32Left**</p></td>
<td align="left"><p>Optional. A negative integer that represents an offset for the left edge of the image. Use this attribute when the **ToolTipImage32by32</span> attribute points to an image file that contains images for many icons. The value of the <span class="keyword">ToolTipImage32by32Left</span> attribute is used to set the CSS <span class="keyword">left</span> attribute for the inline style of an HTML <span class="keyword">img** tag when the page is created.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**ToolTipImage32by32Top**</p></td>
<td align="left"><p>Optional. A negative integer that represents an offset for the top edge of the image. Use this attribute when the **ToolTipImage32by32</span> attribute points to an image file that contains the images for many icons. The value of the <span class="keyword">ToolTipImage32by32Top</span> attribute is used to set the CSS <span class="keyword">top</span> attribute for the inline style of an HTML <span class="keyword">img** tag when the page is created.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**ToolTipTitle**</p></td>
<td align="left"><p>Optional. The text that appears as the title of the tooltip.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**ToolTipDescription**</p></td>
<td align="left"><p>Optional. The text that displays in the body of the tooltip.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**ToolTipHelpKeyWord**</p></td>
<td align="left"><p>Optional. The keyword that is used by context-sensitive Help.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**ToolTipShortcutKey**</p></td>
<td align="left"><p>Optional. The text to display for the shortcut key in the tooltip. For example, if the shortcut key for the control is ALT + J, the value for this attribute is &quot;ALT + J&quot;. The tooltip displays the text for the shortcut key in parentheses after the tooltip title: &quot;(ALT + J)&quot;.</p></td>
</tr>
</tbody>
</table>


---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

None


----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p><a href="commanduidefinition-element.htm">CommandUIDefinition</a></p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="controls-element-group.htm">Controls</a></p></td>
</tr>
</tbody>
</table>


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p>Minimum: 0</p>
<p>Maximum: unbounded</p></td>
</tr>
</tbody>
</table>







