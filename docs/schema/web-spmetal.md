---


manager: soliver
ms.date: 3/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SPMetal Parameters XML
api_type:
- schema
ms.assetid: 96f7c4e1-530d-4148-ac5c-8132565ece1d
---

![Collapse
section](../icons/collapse_all.gif "Collapse section")![Expand
section](../icons/expand_all.gif "Expand section")![](../icons/collapse_all.gif)![](../icons/expand_all.gif)![](../icons/dropdown.gif)![](../icons/dropdownHover.gif)![Copy
code](../icons/copycode.gif "Copy code")![Copy code
hover](../icons/copycodeHighlight.gif "Copy code hover")
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
<td align="left"># Web (SPMetal)</td>
</tr>
<tr class="odd">
<td align="left"><a href="#exampleToggle">Example</a>  <a href="#seeAlsoToggle">See also</a>  <span id="headfeedbackarea" class="feedbackhead"><a href="javascript:SubmitFeedback(&#39;docthis@Microsoft.com&#39;,&#39;&#39;,&#39;&#39;,&#39;&#39;,&#39;1.0.18082.1225&#39;,&#39;%0\dThank%20you%20for%20your%20feedback.%20The%20developer%20writing%20teams%20use%20your%20feedback%20to%20improve%20documentation.%20While%20we%20are%20reviewing%20your%20feedback,%20we%20may%20send%20you%20e-mail%20to%20ask%20for%20clarification%20or%20feedback%20on%20a%20solution.%20We%20do%20not%20use%20your%20e-mail%20address%20for%20any%20other%20purpose%20and%20we%20delete%20it%20after%20we%20finish%20our%20review.%0\AFor%20further%20information%20about%20the%20privacy%20policies%20of%20Microsoft,%20please%20see%20http://privacy.microsoft.com/en-us/default.aspx.%0\A%0\d&#39;,&#39;Customer%20feedback&#39;);">Send feedback</a></span></td>
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

***Applies to:** SharePoint 2016 | SharePoint Foundation 2013 |
SharePoint Online | SharePoint Server 2013*

Specifies the name and access level (public or internal) of the class
(derived from <span sdata="cer"
target="T:Microsoft.SharePoint.Linq.DataContext"><span
class="nolink">DataContext</span></span>) that SPMetal generates.

For information about the default behavior of SPMetal when an optional
element or attribute is not present, see [SPMetal Default Code
Generation
Rules](http://msdn.microsoft.com/library/873ac65e-425e-40f3-9ef6-753d3cda1436(Office.15).aspx).

<span sdata="link">[Web
(SPMetal)](web-spmetal.htm)</span>  
<span codelanguage="xmlLang"></span>
<table>
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">XML</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><pre><code>&lt;Web Class=&quot;TeamSite&quot; AccessModifier=&quot;Internal&quot;&gt; ... &lt;/Web&gt;</code></pre></td>
</tr>
</tbody>
</table>

**Complex**


--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

The following sections describe attributes, child elements, and parent
elements.

#### Attributes

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
<td align="left"><p>Class (optional)</p></td>
<td align="left"><p>Specifies a name for the class (derived from <span sdata="cer" target="T:Microsoft.SharePoint.Linq.DataContext"><span class="nolink">DataContext</span></span>) that SPMetal generates.</p></td>
</tr>
<tr class="even">
<td align="left"><p>AccessModifier (optional)</p></td>
<td align="left"><p>Specifies whether the class (derived from <span sdata="cer" target="T:Microsoft.SharePoint.Linq.DataContext"><span class="nolink">DataContext</span></span>) is public or internal.</p></td>
</tr>
</tbody>
</table>

#### AccessModifier Attribute Possible Values:

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left"><p>Value</p></th>
<th align="left"><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Internal</p></td>
<td align="left"><p>The class will be **internal</span> (<span class="keyword">Friend** in Visual Basic).</p></td>
</tr>
<tr class="even">
<td align="left"><p>Public</p></td>
<td align="left"><p>DEFAULT: The class will be **public</span> (<span class="keyword">Public** in Visual Basic).</p></td>
</tr>
</tbody>
</table>

#### Child elements

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left"><p>Element</p></th>
<th align="left"><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p><a href="contenttype-spmetal.htm">ContentType</a></p></td>
<td align="left"><p>Includes a content type for code generation and modifies which fields (columns) in the content type are included in code generation.</p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="excludecontenttype-spmetal.htm">ExcludeContentType</a></p></td>
<td align="left"><p>Excludes a content type from code generation.</p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="excludeothercontenttypes-spmetal.htm">ExcludeOtherContentTypes</a></p></td>
<td align="left"><p>Excludes from code generation all content types not explicitly included in a ContentType element.</p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="includehiddencontenttypes-spmetal.htm">IncludeHiddenContentTypes</a></p></td>
<td align="left"><p>Includes hidden content types in code generation.</p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="list-spmetal.htm">List</a></p></td>
<td align="left"><p>Includes a list for code generation and modifies which content types in the list are included in code generation.</p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="excludelist-spmetal.htm">ExcludeList</a></p></td>
<td align="left"><p>Excludes a list from code generation.</p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="excludeotherlists-spmetal.htm">ExcludeOtherLists</a></p></td>
<td align="left"><p>Excludes from code generation all lists not explicitly included in a List element.</p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="includehiddenlists-spmetal.htm">IncludeHiddenLists</a></p></td>
<td align="left"><p>Includes hidden lists in code generation.</p></td>
</tr>
</tbody>
</table>

#### Parent elements

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left"><p>Element</p></th>
<th align="left"><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>None</p></td>
<td align="left"></td>
</tr>
</tbody>
</table>


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

A Web element cannot have both a ContentType element and an
ExcludeContentType element that name the same content type. An
ExcludeContentType element that names a hidden content type may not be
present in the same Web element that has an IncludeHiddenContentTypes
element. Finally, a Web element cannot have both an
ExcludeOtherContentTypes element and an IncludeHiddenContentTypes
element.


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

The following is an example of a Web element.

<span codelanguage="xmlLang"></span>
XML 
<span class="copyCode" onclick="CopyCode(this)"
onkeypress="CopyCode_CheckKey(this, event)"
onmouseover="ChangeCopyCodeIcon(this)"
onmouseout="ChangeCopyCodeIcon(this)" tabindex="0">![Copy
code](../icons/copycode.gif "Copy code")Copy code</span>
    <?xml version="1.0" encoding="utf-8"?>
    <Web AccessModifier="Internal" xmlns="http://schemas.microsoft.com/SharePoint/2009/spmetal">
      <ContentType Name="Contact" Class="Contact">
        <Column Name="ContId" Member="ContactId" />
        <Column Name="ContactName" Member="ContactName1" />
        <Column Name="Category" Member="Cat" Type="String"/>
        <ExcludeColumn Name="HomeTelephone" />
      </ContentType>
      <ExcludeContentType Name="Order"/>
      <List Name="Team Members" Type="TeamMember">
        <ContentType Name="Item" Class="TeamMember" />
      </List>
    </Web>


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

#### Other resources

[SPMetal Default Code Generation
Rules](http://msdn.microsoft.com/library/873ac65e-425e-40f3-9ef6-753d3cda1436(Office.15).aspx)

[Overriding SPMetal Defaults by Using a Parameters XML
File](http://msdn.microsoft.com/library/209359b2-bd46-47b6-837d-3c0c2005cb19(Office.15).aspx)







