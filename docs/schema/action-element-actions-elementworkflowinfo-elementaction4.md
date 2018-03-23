---


manager: laurawi
ms.date: 3/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 98829cd3-8f68-351b-6e33-c0e27e174b58
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
<td align="left"># Action element (Actions element) (WorkflowInfo element) (Action4)</td>
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

Contains the information that is required for Workflow Manager Client
1.0 to process a workflow action's underlying activity or activities.

**Last modified:** March 09, 2015

***Applies to:** SharePoint Server 2013*


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<span codelanguage="xmlLang"></span>
XML 
<span class="copyCode" onclick="CopyCode(this)"
onkeypress="CopyCode_CheckKey(this, event)"
onmouseover="ChangeCopyCodeIcon(this)"
onmouseout="ChangeCopyCodeIcon(this)" tabindex="0">![Copy
code](../icons/copycode.gif "Copy code")Copy code</span>
    <Actions>
        <Action>
            <Parameters />
            <RuleDesigner />
            <DataSources />
            <Modifications>
                <Modification/>
            </Modifications>
            <ActionVariables />
            <ActionBody /
            <ActionConditions />
        </Action>
    </Actions>


--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p><span class="label">Element type</span></p></td>
<td align="left"><p></p></td>
</tr>
<tr class="even">
<td align="left"><p><span class="label">Namespace</span></p></td>
<td align="left"><p></p></td>
</tr>
<tr class="odd">
<td align="left"><p><span class="label">Schema file</span></p></td>
<td align="left"><p>Actions4.xsd</p></td>
</tr>
</tbody>
</table>


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<span codelanguage="xmlLang"></span>
XML 
<span class="copyCode" onclick="CopyCode(this)"
onkeypress="CopyCode_CheckKey(this, event)"
onmouseover="ChangeCopyCodeIcon(this)"
onmouseout="ChangeCopyCodeIcon(this)" tabindex="0">![Copy
code](../icons/copycode.gif "Copy code")Copy code</span>
    <xs:element name="Action" minOccurs="0" maxOccurs="unbounded">
    <xs:complexType>
       <xs:all>
       <xs:element name="Parameters" type="parametersType" minOccurs="0" maxOccurs="1"></xs:element>
       <xs:element name="RuleDesigner" type="ruleDesignerType" minOccurs="1" maxOccurs="1"></xs:element>
       <xs:element name="DataSources" type="dataSourcesType" minOccurs="0" maxOccurs="1"></xs:element>
       <xs:element name="Modifications" minOccurs="0" maxOccurs="1">
       <xs:complexType>
          <xs:sequence>
          <xs:element name="Modification" minOccurs="1" maxOccurs="unbounded">
             <xs:attribute name="TypeId" type="s:string" use="required" />
             <xs:attribute name="NameFormat" type="s:string" use="required" />
             <xs:attribute name="FormURN" type="s:string" use="required" />
          </xs:element>
          </xs:sequence>
       </xs:complexType>
       </xs:element>
       <xs:element name="ActionVariables" minOccurs="0" maxOccurs="1">
       <xs:complexType>
          <xs:sequence>
             <xs:element name="ActionVariables"></xs:element>
          </xs:sequence>
       </xs:complexType>
       </xs:element>
       <xs:element name="ActionBody" minOccurs="0" maxOccurs="1">
       <xs:complexType>
          <xs:sequence>
             <xs:element name="ActionBody"></xs:element>
          </xs:sequence>
                </xs:complexType>
       </xs:element>
       <xs:element name="ActionConditions" minOccurs="0" maxOccurs="1">
       <xs:complexType>
          <xs:sequence>
             <xs:element name="ActionConditions"></xs:element>
          </xs:sequence>
       </xs:complexType>
       </xs:element>
       </xs:all>
         <xs:attribute name="Name" type="s:string" use="required" />
         <xs:attribute name="ClassName" type="s:string" use="required" />
         <xs:attribute name="Assembly" type="s:string" />
         <xs:attribute name="FunctionName" type="s:string" />
         <xs:attribute name="Category" type="s:string" />
         <xs:attribute name="CreatesTask" type="s:boolean" />
         <xs:attribute name="CreatesInList" type="s:string" />
         <xs:attribute name="AppliesTo" type="appliesToTypes" use="required" />
         <xs:attribute name="IsError" type="s:boolean" />
         <xs:attribute name="ListModeration" type="s:boolean" />
         <xs:attribute name="UsesCurrentItem" type="s:boolean" />
         <xs:attribute name="CreatedTaskFormType" type="s:string" />
         <xs:attribute name="__SolutionId" type="s:string" />
         <xs:attribute name="SandboxedFunction" type="s:boolean" />
         <xs:attribute name="ShapeImageUrl" type="s:string" />
       </xs:complexType>
    </xs:element>


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

If the schema defines specific requirements, such as <span
class="keyword">sequence</span>, **minOccurs**,
**maxOccurs**, and <span
class="keyword">choice</span>, see the definition section.

### Parent elements

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th align="left"><p>Element</p></th>
<th align="left"><p>Type</p></th>
<th align="left"><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p><a href="actions-element-workflowinfo-elementaction4.htm">Actions</a></p></td>
<td align="left"><p></p></td>
<td align="left"><p></p></td>
</tr>
</tbody>
</table>

### Child elements

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th align="left"><p>Element</p></th>
<th align="left"><p>Type</p></th>
<th align="left"><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p><a href="actionbody-element-action-elementactions-elementworkflowinfo-elementaction4.htm">ActionBody</a></p></td>
<td align="left"><p></p></td>
<td align="left"><p></p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="actionconditions-element-action-elementactions-elementworkflowinfo-elementaction.htm">ActionConditions</a></p></td>
<td align="left"><p></p></td>
<td align="left"><p></p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="actionvariables-element-action-elementactions-elementworkflowinfo-elementaction4.htm">ActionVariables</a></p></td>
<td align="left"><p></p></td>
<td align="left"><p></p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="datasources-element-action-elementactions-elementworkflowinfo-elementaction4.htm">DataSources</a></p></td>
<td align="left"><p><a href="datasourcestype-complextype-action4.htm">dataSourcesType</a></p></td>
<td align="left"><p></p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="modifications-element-action-elementactions-elementworkflowinfo-elementaction4.htm">Modifications</a></p></td>
<td align="left"><p></p></td>
<td align="left"><p></p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="parameters-element-action-elementactions-elementworkflowinfo-elementaction4.htm">Parameters</a></p></td>
<td align="left"><p><a href="parameterstype-complextype-action4.htm">parametersType</a></p></td>
<td align="left"><p></p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="ruledesigner-element-action-elementactions-elementworkflowinfo-elementaction4.htm">RuleDesigner</a></p></td>
<td align="left"><p><a href="ruledesignertype-complextype-action4.htm">ruleDesignerType</a></p></td>
<td align="left"><p></p></td>
</tr>
</tbody>
</table>

### Attributes

<table>
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th align="left"><p>Attribute</p></th>
<th align="left"><p>Type</p></th>
<th align="left"><p>Required</p></th>
<th align="left"><p>Description</p></th>
<th align="left"><p>Possible values</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>__SolutionId</p></td>
<td align="left"><p>s:string</p></td>
<td align="left"><p>optional</p></td>
<td align="left"><p>Specifies a GUID that the client application writes to the implementation-specific action. The server uses the GUID to help locate the assembly at workflow runtime.</p></td>
<td align="left"><p>Values of the s:string type.</p></td>
</tr>
<tr class="even">
<td align="left"><p>AppliesTo</p></td>
<td align="left"><p><a href="appliestotypes-simpletype-action4.htm">appliesToTypes</a></p></td>
<td align="left"><p>required</p></td>
<td align="left"><p>Indicates whether this workflow action should be. Valid values include <strong>site</strong>, <strong>list</strong>, <strong>doclib</strong>, and <strong>all</strong>. The value <strong>all</strong> means that the action is available under any scope and will always show up in the <span class="ui">Actions</span> list.</p></td>
<td align="left"><p>Values of the appliesToTypes type.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Assembly</p></td>
<td align="left"><p>s:string</p></td>
<td align="left"><p>optional</p></td>
<td align="left"><p>The assembly name that contains instructions for implementing the **Action</span> element. The text should include the <span class="parameter" sdata="paramReference">PublicKeyToken</span>, <span class="parameter" sdata="paramReference">Version</span>, and <span class="parameter" sdata="paramReference">Culture** values.</p></td>
<td align="left"><p>Values of the s:string type.</p></td>
</tr>
<tr class="even">
<td align="left"><p>Category</p></td>
<td align="left"><p>s:string</p></td>
<td align="left"><p>optional</p></td>
<td align="left"><p>Provides a category for the workflow action. This value is used to filter the list of available actions.</p></td>
<td align="left"><p>Values of the s:string type.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>ClassName</p></td>
<td align="left"><p>s:string</p></td>
<td align="left"><p>required</p></td>
<td align="left"><p>Fully qualified name of the class that implements the workflow action.</p></td>
<td align="left"><p>Values of the s:string type.</p></td>
</tr>
<tr class="even">
<td align="left"><p>CreatedTaskFormType</p></td>
<td align="left"><p>s:string</p></td>
<td align="left"><p>optional</p></td>
<td align="left"><p>Specifies the type of a task created. Use **DataCollectTask</span> to create a task that collects data from one user; use <span class="keyword">GroupAssignedTask</span> to create a task that collects data from one or more users; use <span class="keyword">TodoItemTask</span> to create a task that does not collect data from users but only exists for a user to validate that they have done something; use <span class="keyword">TaskProcess** to create a task that has a form that allows for ad-hoc collaboration and might collect data from one or more users.</p></td>
<td align="left"><p>Values of the s:string type.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>CreatesInList</p></td>
<td align="left"><p>s:string</p></td>
<td align="left"><p>optional</p></td>
<td align="left"><p>If set, specifies that the workflow create an item in a list or document library. Values must map to a parameter name that contains the ID of the list or document library.</p></td>
<td align="left"><p>Values of the s:string type.</p></td>
</tr>
<tr class="even">
<td align="left"><p>CreatesTask</p></td>
<td align="left"><p>s:boolean</p></td>
<td align="left"><p>optional</p></td>
<td align="left"><p>If **true</span>, a task list item is created in the workflow. If left blank, the assumption is <span class="keyword">false**, and no task list items are created.</p></td>
<td align="left"><p>Values of the s:boolean type.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>FunctionName</p></td>
<td align="left"><p>s:string</p></td>
<td align="left"><p>optional</p></td>
<td align="left"><p>Specifies the name of a function to call.</p></td>
<td align="left"><p>Values of the s:string type.</p></td>
</tr>
<tr class="even">
<td align="left"><p>IsError</p></td>
<td align="left"><p>s:boolean</p></td>
<td align="left"><p>optional</p></td>
<td align="left"><p>If **true</span>, instances of this <span class="keyword">Action** element are considered an error by the client application</p></td>
<td align="left"><p>Values of the s:boolean type.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>ListModeration</p></td>
<td align="left"><p>s:boolean</p></td>
<td align="left"><p>optional</p></td>
<td align="left"><p>If **true</span>, this <span class="keyword">Action</span> element applies to a list or document library that has content approval enabled. If left blank, the assumption is <span class="keyword">false**.</p></td>
<td align="left"><p>Values of the s:boolean type.</p></td>
</tr>
<tr class="even">
<td align="left"><p>Name</p></td>
<td align="left"><p>s:string</p></td>
<td align="left"><p>required</p></td>
<td align="left"><p>Represents the descriptive name of the workflow action that is displayed to the workflow editor.</p></td>
<td align="left"><p>Values of the s:string type.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>SandboxedFunction</p></td>
<td align="left"><p>s:boolean</p></td>
<td align="left"><p>optional</p></td>
<td align="left"><p>If **true**, the client application inserts an implementation-specific action when this action is selected. The action should be configured to call a function defined by the conjunction of AssemblyName, ClassName, and FunctionName. If set, AssemblyName, ClassName, FunctionName, and __SolutionId must also be set.</p></td>
<td align="left"><p>Values of the s:boolean type.</p></td>
</tr>
<tr class="even">
<td align="left"><p>ShapeImageUrl</p></td>
<td align="left"><p>s:string</p></td>
<td align="left"><p>optional</p></td>
<td align="left"><p>The URL of a default icon shape-image file that is available for customization when creating custom actions or custom conditions.</p></td>
<td align="left"><p>Values of the s:string type.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>UsesCurrentItem</p></td>
<td align="left"><p>s:boolean</p></td>
<td align="left"><p>optional</p></td>
<td align="left"><p>Specifies whether a given workflow action can be used in a &quot;site&quot; workflow. Setting this to **true</span> means that the action cannot be used, and is not available, for site workflows. The copy/paste function on actions is also blocked. If this attribute value is not set, then <span class="keyword">false** is implied.</p></td>
<td align="left"><p>Values of the s:boolean type.</p></td>
</tr>
</tbody>
</table>

![Footer](../icons/footer.gif "Footer")

[© 2013 Microsoft Corporation. All rights
reserved.](office-2013-documentation-copyright-notice.htm)



