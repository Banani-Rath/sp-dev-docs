---


manager: soliver
ms.date: 3/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- View schema
api_type:
- schema
ms.assetid: 491dd867-2dea-485e-a0b8-b33e53094bba
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
<td align="left"># Field Element (View)</td>
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

Returns the formatted value of a field for use within a view definition.

<span codelanguage="other"></span>
<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><pre><code>&lt;Field
  AutoHyperLink = &quot;TRUE&quot; | &quot;FALSE&quot;
  AutoHyperLinkNoEncoding = &quot;TRUE&quot; | &quot;FALSE&quot;
  AutoNewLine = &quot;TRUE&quot; | &quot;FALSE&quot;
  HTMLEncode = &quot;TRUE&quot; | &quot;FALSE&quot;
  Name = &quot;Text&quot;
  StripWS = &quot;TRUE&quot; | &quot;FALSE&quot;
  URLEncode = &quot;TRUE&quot; | &quot;FALSE&quot;
  URLEncodeAsURL = &quot;TRUE&quot; | &quot;FALSE&quot;&gt;
&lt;/Field&gt;</code></pre></td>
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
<td align="left"><p>**AutoHyperLink**</p></td>
<td align="left"><p>Optional **Boolean</span>. <span class="keyword">TRUE** to surround text with &lt;A&gt; tags if the text appears to be a hyperlink (for example, www.microsoft.com).</p></td>
</tr>
<tr class="even">
<td align="left"><p>**AutoHyperLinkNoEncoding**</p></td>
<td align="left"><p>Optional **Boolean</span>. <span class="keyword">TRUE** to surround text with &lt;A&gt; tags if the text appears to be a hyperlink (for example, www.microsoft.com) but without HTML encoding.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**AutoNewLine**</p></td>
<td align="left"><p>Optional **Boolean</span>. <span class="keyword">TRUE** to insert &lt;BR&gt; tags into the text stream and to replace multiple spaces with a nonbreaking space (&amp;nbsp;).</p></td>
</tr>
<tr class="even">
<td align="left"><p>**HTMLEncode**</p></td>
<td align="left"><p>Optional **Boolean</span>. <span class="keyword">TRUE** to convert embedded characters so that they are displayed as text in the browser. In other words, characters that could be confused with HTML tags are converted to entities.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**Name**</p></td>
<td align="left"><p>Optional **Text</span>. Allows the <span class="keyword">Field</span> element to be used outside the field rendering context by supplying an ID (for example, <span class="code">&lt;Field Name=&quot;</span><span class="placeholder">ID</span><span class="code">&quot;/&gt;**).</p></td>
</tr>
<tr class="even">
<td align="left"><p>**StripWS**</p></td>
<td align="left"><p>Optional **Boolean</span>. <span class="keyword">TRUE** to remove white space from the beginning and end of the value returned by the element.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**URLEncode**</p></td>
<td align="left"><p>Optional **Boolean</span>. <span class="keyword">TRUE** to convert special characters, such as spaces, to quoted UTF-8 format (for example, %c3%ab for character ë).</p></td>
</tr>
<tr class="even">
<td align="left"><p>**URLEncodeAsURL**</p></td>
<td align="left"><p>Optional **Boolean</span>. Like <span class="keyword">URLEncode</span>, but <span class="keyword">TRUE** to specify that the string to encode is a path component of a URL so that forward slashes (&quot;/&quot;) are not encoded.</p></td>
</tr>
</tbody>
</table>


---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p>None</p></td>
</tr>
</tbody>
</table>


----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p>Numerous</p></td>
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
<p>Maximum: Unbounded (1 within <a href="urlbasename-element-view.htm">UrlBaseName</a>)</p></td>
</tr>
</tbody>
</table>


----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Use the **Field (View)** element to return a
formatted field value for display within a view, and use the
[Column](column-element-view.md) element to return the
raw data value of the field. The **Field**
element does not specify attributes when it is used within
[UrlBaseName](urlbasename-element-view.md), and only <span
class="keyword">Name</span> is specified when it is used within
[Expr1](expr1-element-view.md),
[Expr2](expr2-element-view.md), or
[Row](row-element-site.md).

To create a custom field definition as a pluggable Feature that is based
on a default SharePoint Foundation field type and that can be reused
across sites and lists, use the [Field
(Field)](field-element-field.md) element to define a
custom [site
column](http://msdn.microsoft.com/library/0402b3a7-3665-43df-9769-85e3aa1b2432(Office.15).aspx).
To create a custom field definition for a list definition based on a
default field type, use the [Field (List -
Definition)](field-element-list.md) element within a
[Schema.xml](http://msdn.microsoft.com/library/c2f01064-80d8-47ee-b602-ecf4c480ac56(Office.15).aspx)
file. To create a [custom field
type](http://msdn.microsoft.com/library/1345b345-226d-443a-918f-af123a3c7b13(Office.15).aspx)
that implements a custom class for special data validation and field
rendering, use the [Field (Field
Types)](field-element-field-types.md) element.







