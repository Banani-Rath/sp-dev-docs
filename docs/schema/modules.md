---
ms.author: rickki
author: rickki
manager: soliver
ms.date: 12/7/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4f43e194-322e-4eca-9c96-8ad9f13818bd
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
<td align="left"># Modules</td>
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

**Last modified:** December 07, 2015

***Applies to:** SharePoint 2016 | SharePoint Foundation 2013 |
SharePoint Online | SharePoint Server 2013*

Modules are defined in an element manifest similarly to how they are
defined in an
[Onet.xml](http://msdn.microsoft.com/library/b99d6657-d9ae-4135-a43c-c58cdfcdc6c1(Office.15).aspx)
file to specify files with which to provision SharePoint sites.

Zero or more [File](file-element-module.htm) elements
are allowed as a child of the
[Module](module-element-module.htm) element. Use the
[AllUsersWebPart](alluserswebpart-element-module.htm) element to
specify a Web Part instance inside a given page except for a list view
Web Part. The [View](view-element-module.htm) element
specifies list view Web Parts to use on site pages. The
[NavBarPage](navbarpage-element-module.htm) element declares
that the page containing this element should participate in the
navigation bar structure. The
[Property](property-element-module.htm) element allows you
to specify custom properties for a Feature.

An element manifest uses the following schema:

[Elements](elements-element-module.htm)

  [Module](module-element-module.htm)

    [File](file-element-module.htm)

      [View](view-element-module.htm)

      [AllUsersWebPart](alluserswebpart-element-module.htm)

      [NavBarPage](navbarpage-element-module.htm)

      [Property](property-element-module.htm)

The following schema is used within an
[Onet.xml](http://msdn.microsoft.com/library/b99d6657-d9ae-4135-a43c-c58cdfcdc6c1(Office.15).aspx)
file:

[Configuration](configuration-element-site.htm)

  [Modules](modules-element-site.htm)

    [Module](module-element-site.htm)

      [File](file-element.htm)

        [View](view-element-module.htm)

        [AllUsersWebPart](alluserswebpart-element-site.htm)

        [NavBarPage](navbarpage-element-sitemodule.htm)

        [Property](property-element-sitemodule.htm)


--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

The following example registers a Web Part Feature that specifies custom
properties:

<span codelanguage="xmlLang"></span>
XML 
<span class="copyCode" onclick="CopyCode(this)"
onkeypress="CopyCode_CheckKey(this, event)"
onmouseover="ChangeCopyCodeIcon(this)"
onmouseout="ChangeCopyCodeIcon(this)" tabindex="0">![Copy
code](../icons/copycode.gif "Copy code")Copy code</span>
    <?xml version="1.0" encoding="utf-8" ?>
    <Elements xmlns="http://schemas.microsoft.com/sharepoint/">
      <Module Name="WebPartPopulation" Url="_catalogs/wp" RootWebOnly="TRUE">
        <File Url="MyWebPart.webpart" Type="GhostableInLibrary">
          <Property Name="MyGroup" Value="Business Information" />
          <Property Name="MyLocation" Value="Middle Right" />
        </File>
      </Module>
    </Elements>

The next example registers a Feature that includes two files and that
specifies a list view to display on one of the pages.

<span codelanguage="xmlLang"></span>
XML 
<span class="copyCode" onclick="CopyCode(this)"
onkeypress="CopyCode_CheckKey(this, event)"
onmouseover="ChangeCopyCodeIcon(this)"
onmouseout="ChangeCopyCodeIcon(this)" tabindex="0">![Copy
code](../icons/copycode.gif "Copy code")Copy code</span>
    <?xml version="1.0" encoding="utf-8" ?>
    <Elements xmlns="http://schemas.microsoft.com/sharepoint/">
      <Module Name="KnowledgeBasePages" Url="" Path="KnowledgeBaseFolder">
        <File Url="KnowledgeBases.aspx">
          <View List="KnowledgeBaseList" BaseViewID="0" WebPartZoneID="Left" WebPartOrder="0" />
        </File>
        <File Url="KnowledgeBaseLink.aspx"/>
      </Module>
    </Elements>


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

#### Other resources

[Module](http://msdn.microsoft.com/library/e5eeed6e-d785-496d-82b5-08d153588045(Office.15).aspx)

[How to: Provision a
File](http://msdn.microsoft.com/library/438d5a75-7f39-4fa9-a365-d86e8ba967b6(Office.15).aspx)

![Footer](../icons/footer.gif "Footer")

[© 2013 Microsoft Corporation. All rights
reserved.](office-2013-documentation-copyright-notice.htm)



