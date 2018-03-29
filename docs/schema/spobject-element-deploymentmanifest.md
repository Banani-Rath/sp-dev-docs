---


manager: soliver
ms.date: 3/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1bdc823e-d556-4273-a091-92d41d9d9ace
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
<td align="left"># SPObject Element (DeploymentManifest)</td>
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

**Applies to**: SharePoint 2016 | SharePoint Foundation 2013 |
SharePoint Online | SharePoint Server 2013

Represents an instance of a top-level Windows SharePoint Services 3.0
object (**SPGenericObject**).

<span codelanguage="other"></span>
<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><pre><code>DECLARATION
&lt;xs:element name=&quot;SPObject&quot; 
        type=&quot;SPGenericObject&quot; 
        minOccurs=&quot;0&quot; maxOccurs=&quot;unbounded&quot; 
/&gt;

USAGE
&lt;SPObjects&gt;
        &lt;SPObject
                ObjectType=&quot;SPObjectType&quot;
                Id=&quot;Guid&quot;
                ParentId=&quot;Guid&quot;
                Name=&quot;xs:string&quot;
                IsDeleted=&quot;xs:boolean&quot;
                ParentWebId=&quot;Guid&quot;
                ParentWebUrl=&quot;xs:string&quot;
                ContentTypeId=&quot;xs:string&quot;
                Url=&quot;xs:string&quot;
        /&gt;
&lt;/SPObjects&gt;</code></pre></td>
</tr>
</tbody>
</table>


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**SPGenericObject** (<span sdata="cer"
target="T:System.Object">[Object](http://msdn2.microsoft.com/EN-US/library/e5kfa45b)</span>)


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
<td align="left"><p>**ObjectType**</p></td>
<td align="left"><p><span sdata="link"><a href="spobjecttype-simple-type-deploymentmanifest.htm">SPObjectType Simple Type (DeploymentManifest)</a></span></p></td>
<td align="left"><p>Optional. Enumeration that provides values to specify the Windows SharePoint Services 3.0 top-level object type.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**Id**</p></td>
<td align="left"><p><span sdata="link"><a href="guid-simple-type-deploymentmanifest.htm">Guid Simple Type (DeploymentManifest)</a></span></p></td>
<td align="left"><p>Optional. Unique identifier of the Windows SharePoint Services 3.0 object.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**ParentId**</p></td>
<td align="left"><p><span sdata="link"><a href="guid-simple-type-deploymentmanifest.htm">Guid Simple Type (DeploymentManifest)</a></span></p></td>
<td align="left"><p>Optional. Unique identifier of the parent deployment object.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**Name**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. Name of the object.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**IsDeleted**</p></td>
<td align="left"><p>xs:boolean</p></td>
<td align="left"><p>Optional. Specifies whether the object has been deleted.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**ParentWebId**</p></td>
<td align="left"><p><span sdata="link"><a href="guid-simple-type-deploymentmanifest.htm">Guid Simple Type (DeploymentManifest)</a></span></p></td>
<td align="left"><p>Optional. Unique identifier of the parent Web site.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**ParentWebUrl**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. URL to the parent Web site.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**ContenTypeId**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. Specifies the object content type.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**Url**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. URL to the object.</p></td>
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
<td align="left"><p><span sdata="link"><a href="site-element-deploymentmanifest.htm">Site Element (DeploymentManifest)</a></span></p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="web-element-deploymentmanifest.htm">Web Element (DeploymentManifest)</a></span></p></td>
</tr>
<tr class="odd">
<td align="left"><p><span sdata="link"><a href="webtemplate-element-deploymentmanifest.htm">WebTemplate Element (DeploymentManifest)</a></span></p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="list-element-deploymentmanifest.htm">List Element (DeploymentManifest)</a></span></p></td>
</tr>
<tr class="odd">
<td align="left"><p><span sdata="link"><a href="documentlibrary-element-deploymentmanifest.htm">DocumentLibrary Element (DeploymentManifest)</a></span></p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="picturelibrary-element-deploymentmanifest.htm">PictureLibrary Element (DeploymentManifest)</a></span></p></td>
</tr>
<tr class="odd">
<td align="left"><p><span sdata="link"><a href="listitem-element-deploymentmanifestspgenericobject.htm">ListItem Element (DeploymentManifest - SPGenericObject)</a></span></p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="module-element-deploymentmanifest.htm">Module Element (DeploymentManifest)</a></span></p></td>
</tr>
<tr class="odd">
<td align="left"><p><span sdata="link"><a href="documenttemplate-element-deploymentmanifest.htm">DocumentTemplate Element (DeploymentManifest)</a></span></p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="listtemplate-element-deploymentmanifest.htm">ListTemplate Element (DeploymentManifest)</a></span></p></td>
</tr>
<tr class="odd">
<td align="left"><p><span sdata="link"><a href="folder-element-deploymentmanifest.htm">Folder Element (DeploymentManifest)</a></span></p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="file-element-deploymentmanifestspgenericobject.htm">File Element (DeploymentManifest - SPGenericObject)</a></span></p></td>
</tr>
<tr class="odd">
<td align="left"><p><span sdata="link"><a href="contenttype-element-deploymentmanifest.htm">ContentType Element (DeploymentManifest)</a></span></p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="fieldtemplate-element-deploymentmanifest.htm">FieldTemplate Element (DeploymentManifest)</a></span></p></td>
</tr>
<tr class="odd">
<td align="left"><p><span sdata="link"><a href="webstructure-element-deploymentmanifest.htm">WebStructure Element (DeploymentManifest)</a></span></p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="userx-element-deploymentmanifest.htm">UserX Element (DeploymentManifest)</a></span></p></td>
</tr>
<tr class="odd">
<td align="left"><p><span sdata="link"><a href="groupx-element-deploymentmanifest.htm">GroupX Element (DeploymentManifest)</a></span></p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="roles-element-deploymentmanifest.htm">Roles Element (DeploymentManifest)</a></span></p></td>
</tr>
<tr class="odd">
<td align="left"><p><span sdata="link"><a href="rolex-element-deploymentmanifest.htm">RoleX Element (DeploymentManifest)</a></span></p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="roleassignments-element-deploymentmanifest.htm">RoleAssignments Element (DeploymentManifest)</a></span></p></td>
</tr>
<tr class="odd">
<td align="left"><p><span sdata="link"><a href="feature-element-deploymentmanifest.htm">Feature Element (DeploymentManifest)</a></span></p></td>
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
<td align="left"><p><span sdata="link"><a href="spobjects-element-deploymentmanifest.htm">SPObjects Element (DeploymentManifest)</a></span></p></td>
</tr>
</tbody>
</table>


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

#### Reference

<span sdata="cer"
target="T:Microsoft.SharePoint.Deployment.SPDeploymentObject"><span
class="nolink">SPDeploymentObject</span></span>

<span sdata="cer"
target="T:System.Object">[Object](http://msdn2.microsoft.com/EN-US/library/e5kfa45b)</span>

#### Concepts

[DeploymentManifest
Schema](deploymentmanifest-schema.md)</span>







