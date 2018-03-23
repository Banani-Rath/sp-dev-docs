---
ms.author: nicg
author: nicg
manager: soliver
ms.date: 3/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c7ab084e-e946-45a0-9dc8-ac68eba4e557
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
<td align="left"># View Element (DeploymentManifest)</td>
</tr>
<tr class="odd">
<td align="left"><a href="#seeAlsoToggle">See also</a>  <span id="headfeedbackarea" class="feedbackhead"><a href="javascript:SubmitFeedback(&#39;docthis@Microsoft.com&#39;,&#39;&#39;,&#39;&#39;,&#39;&#39;,&#39;1.0.18082.1225&#39;,&#39;%0\dThank%20you%20for%20your%20feedback.%20The%20developer%20writing%20teams%20use%20your%20feedback%20to%20improve%20documentation.%20While%20we%20are%20reviewing%20your%20feedback,%20we%20may%20send%20you%20e-mail%20to%20ask%20for%20clarification%20or%20feedback%20on%20a%20solution.%20We%20do%20not%20use%20your%20e-mail%20address%20for%20any%20other%20purpose%20and%20we%20delete%20it%20after%20we%20finish%20our%20review.%0\AFor%20further%20information%20about%20the%20privacy%20policies%20of%20Microsoft,%20please%20see%20http://privacy.microsoft.com/en-us/default.aspx.%0\A%0\d&#39;,&#39;Customer%20feedback&#39;);">Send feedback</a></span></td>
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

Represents an instance of a Windows SharePoint Services 3.0 view (<span
sdata="cer" target="T:Microsoft.SharePoint.SPView"><span
class="nolink">SPView</span></span>) object.

<span codelanguage="other"></span>
<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><pre><code>DECLARATION
&lt;xs:element name=&quot;View&quot; type=&quot;SPView&quot; minOccurs=&quot;0&quot; maxOccurs=&quot;unbounded&quot; /&gt;

USAGE
&lt;Views&gt;
        &lt;View&gt;
        &lt;xs:choice minOccurs=&quot;0&quot; maxOccurs=&quot;25&quot;&gt;
                &lt;xs:element name=&quot;Script&quot; /&gt;
                &lt;xs:element name=&quot;PagedRowset&quot; /&gt;
                &lt;xs:element name=&quot;PagedClientCallbackRowset&quot; /&gt;
                &lt;xs:element name=&quot;PagedRecurrenceRowset&quot; /&gt;
                &lt;xs:element name=&quot;ViewFields&quot; /&gt;
                &lt;xs:element name=&quot;ViewData&quot; /&gt;
                &lt;xs:element name=&quot;Query&quot; /&gt;
                &lt;xs:element name=&quot;RowLimit&quot; /&gt;
                &lt;xs:element name=&quot;RowLimitExceeded&quot; /&gt;
                &lt;xs:element name=&quot;Toolbar&quot; /&gt;
                &lt;xs:element name=&quot;Formats&quot; /&gt;
                &lt;xs:element name=&quot;Aggregations&quot; /&gt;
                &lt;xs:element name=&quot;ViewStyle&quot; /&gt;
                &lt;xs:element name=&quot;ViewBody&quot; /&gt;
                &lt;xs:element name=&quot;ViewEmpty&quot; /&gt;
                &lt;xs:element name=&quot;ViewFooter&quot; /&gt;
                &lt;xs:element name=&quot;ViewHeader&quot; /&gt;
                &lt;xs:element name=&quot;ViewBidiHeader&quot; /&gt;
                &lt;xs:element name=&quot;GroupByFooter&quot; /&gt;
                &lt;xs:element name=&quot;GroupByHeader&quot; /&gt;
                &lt;xs:element name=&quot;CalendarViewStyles&quot; /&gt;
                &lt;xs:element name=&quot;ListFormBody&quot; /&gt;
        &lt;/xs:choice&gt;
        &lt;xs:attribute name=&quot;Name&quot; /&gt;
        &lt;xs:attribute name=&quot;DefaultView&quot; /&gt;
        &lt;xs:attribute name=&quot;Type&quot; /&gt;
        &lt;xs:attribute name=&quot;Hidden&quot; /&gt;
        &lt;xs:attribute name=&quot;Threaded&quot; /&gt;
        &lt;xs:attribute name=&quot;FPModified&quot; /&gt;
        &lt;xs:attribute name=&quot;ReadOnly&quot; /&gt;
        &lt;xs:attribute name=&quot;Scope&quot; /&gt;
        &lt;xs:attribute name=&quot;RecurrenceRowset&quot; /&gt;
        &lt;xs:attribute name=&quot;ModerationType&quot; /&gt;
        &lt;xs:attribute name=&quot;Personal&quot; /&gt;
        &lt;xs:attribute name=&quot;OrderedView&quot; /&gt;
        &lt;xs:attribute name=&quot;DisplayName&quot; /&gt;
        &lt;xs:attribute name=&quot;ContentTypeId&quot; /&gt;
        &lt;xs:attribute name=&quot;Url&quot; /&gt;
        &lt;xs:attribute name=&quot;BaseViewID&quot; /&gt;
        &lt;xs:attribute name=&quot;WebPartZoneID&quot; /&gt;
        &lt;/View&gt;
&lt;/Views&gt;</code></pre></td>
</tr>
</tbody>
</table>


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<span sdata="cer" target="T:Microsoft.SharePoint.SPView"><span
class="nolink">SPView</span></span> object.


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th align="left"><p>Attribute</p></th>
<th align="left"><p>Type</p></th>
<th align="left"><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>**BaseViewID**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. Represents the ID of the base view for the view.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**ContentTypeId**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. Represents the ID of a content type that is associated with the view.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**DefaultView**</p></td>
<td align="left"><p>xs:boolean</p></td>
<td align="left"><p>Optional. Specifies whether the view is the default view.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**DisplayName**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. Represents the display name of the view.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**FPModified**</p></td>
<td align="left"><p>xs:boolean</p></td>
<td align="left"><p>Optional. Specifies whether the view was modified in an HTML editor.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**Hidden**</p></td>
<td align="left"><p>xs:boolean</p></td>
<td align="left"><p>Optional. Specifies whether the view is hidden.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**ModerationType**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional.Represents the Content Approval type for the view.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**Name**</p></td>
<td align="left"><p><span sdata="link"><a href="guid-simple-type-deploymentmanifest.htm">Guid Simple Type (DeploymentManifest)</a></span></p></td>
<td align="left"><p>Optional. Unique identifier of the view.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**OrderedView**</p></td>
<td align="left"><p>xs:boolean</p></td>
<td align="left"><p>Optional. Specifies whether the user can reorder items through the user interface.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**Personal**</p></td>
<td align="left"><p>xs:boolean</p></td>
<td align="left"><p>Optional. Specifies whether the view is personalized.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**ReadOnly**</p></td>
<td align="left"><p>xs:boolean</p></td>
<td align="left"><p>Optional. Specifies whether the view is read-only.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**RecurrenceRowset**</p></td>
<td align="left"><p>xs:boolean</p></td>
<td align="left"><p>Optional. Specifies whether the view supports recurrence rowsets.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**Scope**</p></td>
<td align="left"><p><span sdata="link"><a href="spviewscope-simple-type-deploymentmanifest.htm">SPViewScope Simple Type (DeploymentManifest)</a></span></p></td>
<td align="left"><p>Optional. Sets the recursive scope for the view of a document library.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**Threaded**</p></td>
<td align="left"><p>xs:boolean</p></td>
<td align="left"><p>Optional. Specifies whether the view is threaded.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**Type**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. Represetns the type of the view.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**Url**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. Represents the site-relative URL of the page that contains the view.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**WebPartZoneID**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. Identifier of the Web Part zone in which the view is sited.</p></td>
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
<td align="left"><p><span sdata="link"><a href="script-element-deploymentmanifestspview.htm">Script Element (DeploymentManifest - SPView)</a></span></p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="pagedrowset-element-deploymentmanifestspview.htm">PagedRowset Element (DeploymentManifest - SPView)</a></span></p></td>
</tr>
<tr class="odd">
<td align="left"><p><span sdata="link"><a href="pagedclientcallbackrowset-element-deploymentmanifestspview.htm">PagedClientCallbackRowset Element (DeploymentManifest - SPView)</a></span></p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="pagedrecurrencerowset-element-deploymentmanifestspview.htm">PagedRecurrenceRowset Element (DeploymentManifest - SPView)</a></span></p></td>
</tr>
<tr class="odd">
<td align="left"><p><span sdata="link"><a href="viewfields-element-deploymentmanifestspview.htm">ViewFields Element (DeploymentManifest - SPView)</a></span></p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="viewdata-element-deploymentmanifestspview.htm">ViewData Element (DeploymentManifest - SPView)</a></span></p></td>
</tr>
<tr class="odd">
<td align="left"><p><span sdata="link"><a href="query-element-deploymentmanifestspview.htm">Query Element (DeploymentManifest - SPView)</a></span></p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="rowlimit-element-deploymentmanifestspview.htm">RowLimit Element (DeploymentManifest - SPView)</a></span></p></td>
</tr>
<tr class="odd">
<td align="left"><p><span sdata="link"><a href="rowlimitexceeded-element-deploymentmanifestspview.htm">RowLimitExceeded Element (DeploymentManifest - SPView)</a></span></p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="toolbar-element-deploymentmanifestspview.htm">Toolbar Element (DeploymentManifest - SPView)</a></span></p></td>
</tr>
<tr class="odd">
<td align="left"><p><span sdata="link"><a href="formats-element-deploymentmanifestspview.htm">Formats Element (DeploymentManifest - SPView)</a></span></p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="aggregations-element-deployment-manifestspview.htm">Aggregations Element (Deployment Manifest - SPView)</a></span></p></td>
</tr>
<tr class="odd">
<td align="left"><p><span sdata="link"><a href="viewstyle-element-deploymentmanifestspview.htm">ViewStyle Element (DeploymentManifest - SPView)</a></span></p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="view-body-element-deploymentmanifestspview.htm">View Body Element (DeploymentManifest - SPView)</a></span></p></td>
</tr>
<tr class="odd">
<td align="left"><p><span sdata="link"><a href="viewempty-element-deploymentmanifestspview.htm">ViewEmpty Element (DeploymentManifest - SPView)</a></span></p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="viewfooter-element-deploymentmanifestspview.htm">ViewFooter Element (DeploymentManifest - SPView)</a></span></p></td>
</tr>
<tr class="odd">
<td align="left"><p><span sdata="link"><a href="viewheader-element-deploymentmanifestspview.htm">ViewHeader Element (DeploymentManifest - SPView)</a></span></p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="viewbidiheader-element-deploymentmanifestspview.htm">ViewBidiHeader Element (DeploymentManifest - SPView)</a></span></p></td>
</tr>
<tr class="odd">
<td align="left"><p><span sdata="link"><a href="groupbyfooter-element-deploymentmanifestspview.htm">GroupByFooter Element (DeploymentManifest - SPView)</a></span></p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="groupbyheader-deploymentmanifestspview.htm">GroupByHeader (DeploymentManifest - SPView)</a></span></p></td>
</tr>
<tr class="odd">
<td align="left"><p><span sdata="link"><a href="calendarviewstyles-element-deploymentmanifestspview.htm">CalendarViewStyles Element (DeploymentManifest - SPView)</a></span></p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="listformbody-element-deploymentmanifestspview.htm">ListFormBody Element (DeploymentManifest - SPView)</a></span></p></td>
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
<td align="left"><p><span sdata="link"><a href="views-element-deploymentmanifest.htm">Views Element (DeploymentManifest)</a></span></p></td>
</tr>
</tbody>
</table>


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

#### Reference

<span sdata="cer" target="T:Microsoft.SharePoint.SPView"><span
class="nolink">SPView</span></span>

#### Concepts

<span sdata="link">[DeploymentManifest
Schema](deploymentmanifest-schema.htm)</span>

![Footer](../icons/footer.gif "Footer")

[© 2013 Microsoft Corporation. All rights
reserved.](office-2013-documentation-copyright-notice.htm)



