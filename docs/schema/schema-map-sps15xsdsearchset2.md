---


manager: arnek
ms.date: 11/16/2014
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a088c6ef-6e66-04d6-5fa4-232a4e513598
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
<td align="left"># Schema map (SPS15XSDSearchSet2)</td>
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

This topic shows the schema definition for <span
class="keyword">schema\_Microsoft.Office.Server.Search.Administration</span>.

**Last modified:** January 13, 2014

<span codelanguage="xmlLang"></span>
XML 
<span class="copyCode" onclick="CopyCode(this)"
onkeypress="CopyCode_CheckKey(this, event)"
onmouseover="ChangeCopyCodeIcon(this)"
onmouseout="ChangeCopyCodeIcon(this)" tabindex="0">![Copy
code](../icons/copycode.gif "Copy code")Copy code</span>
    <xs:schema ser="http://schemas.microsoft.com/2003/10/Serialization/" tns="http://schemas.datacontract.org/2004/07/Microsoft.Office.Server.Search.Administration" elementFormDefault="qualified" targetNamespace="http://schemas.datacontract.org/2004/07/Microsoft.Office.Server.Search.Administration" xmlns:xs="http://www.w3.org/2001/XMLSchema">
        <xs:complexType name="SearchObjectOwner">
            <xs:sequence>
                <xs:element name="DatabaseId" type="ser:guid" minOccurs="0"></xs:element>
                <xs:element name="DisableInheritance" type="xs:boolean" minOccurs="0"></xs:element>
                <xs:element name="SPFarmId" type="ser:guid" minOccurs="0"></xs:element>
                <xs:element name="SPSiteId" type="ser:guid" minOccurs="0"></xs:element>
                <xs:element name="SPSiteSubscriptionId" type="ser:guid" minOccurs="0"></xs:element>
                <xs:element name="SPWebId" type="ser:guid" minOccurs="0"></xs:element>
            </xs:sequence>
        </xs:complexType>
        <xs:element name="SearchObjectOwner" type="tns:SearchObjectOwner"></xs:element>
        <xs:complexType name="ArrayOfResultItemType">
            <xs:sequence>
                <xs:element name="ResultItemType" type="tns:ResultItemType" minOccurs="0" maxOccurs="unbounded"></xs:element>
            </xs:sequence>
        </xs:complexType>
        <xs:element name="ArrayOfResultItemType" type="tns:ArrayOfResultItemType"></xs:element>
        <xs:complexType name="ResultItemType">
            <xs:sequence>
                <xs:element name="BuiltIn" type="xs:boolean" minOccurs="0"></xs:element>
                <xs:element name="DisplayProperties" type="xs:string" minOccurs="0"></xs:element>
                <xs:element name="DisplayTemplateUrl" type="xs:string" minOccurs="0"></xs:element>
                <xs:element name="ID" type="xs:int" minOccurs="0"></xs:element>
                <xs:element name="InternalID" type="ser:guid" minOccurs="0"></xs:element>
                <xs:element name="IsDeleted" type="xs:boolean" minOccurs="0"></xs:element>
                <xs:element name="LastModifiedDate" type="xs:dateTime" minOccurs="0"></xs:element>
                <xs:element name="Name" type="xs:string" minOccurs="0"></xs:element>
                <xs:element name="OptimizeForFrequentUse" type="xs:boolean" minOccurs="0"></xs:element>
                <xs:element name="Owner" type="tns:SearchObjectOwner" minOccurs="0"></xs:element>
                <xs:element name="RulePriority" type="xs:int" minOccurs="0"></xs:element>
                <xs:element name="Rules" type="tns:PropertyRuleCollection" minOccurs="0"></xs:element>
                <xs:element name="SourceID" type="ser:guid" minOccurs="0"></xs:element>
            </xs:sequence>
        </xs:complexType>
        <xs:element name="ResultItemType" type="tns:ResultItemType"></xs:element>
        <xs:complexType name="PropertyRuleCollection">
            <xs:sequence>
                <xs:element name="PropertyRules" type="tns:ArrayOfPropertyRule" minOccurs="0"></xs:element>
            </xs:sequence>
        </xs:complexType>
        <xs:element name="PropertyRuleCollection" type="tns:PropertyRuleCollection"></xs:element>
        <xs:complexType name="ArrayOfPropertyRule">
            <xs:sequence>
                <xs:element name="PropertyRule" type="tns:PropertyRule" minOccurs="0" maxOccurs="unbounded"></xs:element>
            </xs:sequence>
        </xs:complexType>
        <xs:element name="ArrayOfPropertyRule" type="tns:ArrayOfPropertyRule"></xs:element>
        <xs:complexType name="PropertyRule">
            <xs:sequence>
                <xs:element name="PropertyName" type="xs:string" minOccurs="0"></xs:element>
                <xs:element name="PropertyOperator" type="tns:PropertyRuleOperator" minOccurs="0"></xs:element>
                <xs:element name="PropertyValues" type="q1:ArrayOfstring" minOccurs="0"></xs:element>
                <xs:element name="RuleNameLSID" type="q2:LocStringId" minOccurs="0"></xs:element>
            </xs:sequence>
        </xs:complexType>
        <xs:element name="PropertyRule" type="tns:PropertyRule"></xs:element>
        <xs:complexType name="PropertyRuleOperator">
            <xs:sequence>
                <xs:element name="DescriptionLSID" type="q3:LocStringId" minOccurs="0"></xs:element>
                <xs:element name="IsFunction" type="xs:boolean" minOccurs="0"></xs:element>
                <xs:element name="IsQuoted" type="xs:boolean" minOccurs="0"></xs:element>
                <xs:element name="JoinedByOr" type="xs:boolean" minOccurs="0"></xs:element>
                <xs:element name="Name" type="xs:string" minOccurs="0"></xs:element>
                <xs:element name="NameLSID" type="q4:LocStringId" minOccurs="0"></xs:element>
                <xs:element name="Representation" type="xs:string" minOccurs="0"></xs:element>
            </xs:sequence>
        </xs:complexType>
        <xs:element name="PropertyRuleOperator" type="tns:PropertyRuleOperator"></xs:element>
        <xs:complexType name="AuthenticationInformation">
            <xs:sequence>
                <xs:element name="AuthenticationType" type="tns:FederationAuthType" minOccurs="0"></xs:element>
                <xs:element name="Data" type="tns:AuthenticationData" minOccurs="0"></xs:element>
            </xs:sequence>
        </xs:complexType>
        <xs:element name="AuthenticationInformation" type="tns:AuthenticationInformation"></xs:element>
        <xs:simpleType name="FederationAuthType">
            <xs:restriction base="xs:string">
                <xs:enumeration value="Anonymous" />
                <xs:enumeration value="LocalNTAuth" />
                <xs:enumeration value="SingleAccountBasicAuth" />
                <xs:enumeration value="SingleAccountFormsAuthentication" />
                <xs:enumeration value="SingleAccountCookie" />
                <xs:enumeration value="ApplicationPoolIdentity" />
                <xs:enumeration value="Kerberos" />
                <xs:enumeration value="PerUserFormsAuthentication" />
                <xs:enumeration value="PerUserCookie" />
                <xs:enumeration value="SSO" />
                <xs:enumeration value="SingleAccountNTLM" />
                <xs:enumeration value="PerUserNTLM" />
                <xs:enumeration value="SingleAccountDigest" />
                <xs:enumeration value="PerUserDigest" />
                <xs:enumeration value="PerUserBasicAuth" />
                <xs:enumeration value="Custom" />
                <xs:enumeration value="PerUserCustom" />
            </xs:restriction>
        </xs:simpleType>
        <xs:element name="FederationAuthType" type="tns:FederationAuthType"></xs:element>
        <xs:complexType name="AuthenticationData"></xs:complexType>
        <xs:element name="AuthenticationData" type="tns:AuthenticationData"></xs:element>
        <xs:complexType name="SsoAuthData">
            <xs:complexContent>
                <xs:extension base="tns:AuthenticationData">
                    <xs:sequence>
                        <xs:element name="_SsoAppId" type="xs:string" minOccurs="0"></xs:element>
                        <xs:element name="_nameValuePairs" type="q5:ArrayOfKeyValueOfstringstring" minOccurs="0"></xs:element>
                    </xs:sequence>
                </xs:extension>
            </xs:complexContent>
        </xs:complexType>
        <xs:element name="SsoAuthData" type="tns:SsoAuthData"></xs:element>
        <xs:complexType name="CookieAuthData">
            <xs:complexContent>
                <xs:extension base="tns:AuthenticationData">
                    <xs:sequence>
                        <xs:element name="_Cookies" type="q6:CookieCollection" minOccurs="0"></xs:element>
                        <xs:element name="_ErrorPageUrl" type="xs:string" minOccurs="0"></xs:element>
                    </xs:sequence>
                </xs:extension>
            </xs:complexContent>
        </xs:complexType>
        <xs:element name="CookieAuthData" type="tns:CookieAuthData"></xs:element>
        <xs:complexType name="SecurableAuthData">
            <xs:complexContent>
                <xs:extension base="tns:AuthenticationData">
                    <xs:sequence>
                        <xs:element name="_NameValuePairs" type="q7:ArrayOfKeyValueOfstringstring" minOccurs="0"></xs:element>
                        <xs:element name="_SecurableNameValuePairs" type="q8:ArrayOfKeyValueOfstringSecureStringX9wx7DhE" minOccurs="0"></xs:element>
                        <xs:element name="SerializableSecurableNameValuePairs" type="q9:ArrayOfKeyValueOfstringstring" minOccurs="0"></xs:element>
                    </xs:sequence>
                </xs:extension>
            </xs:complexContent>
        </xs:complexType>
        <xs:element name="SecurableAuthData" type="tns:SecurableAuthData"></xs:element>
        <xs:complexType name="AccountAuthCredentials">
            <xs:complexContent>
                <xs:extension base="tns:AuthenticationData">
                    <xs:sequence>
                        <xs:element name="Password" type="xs:string" minOccurs="0"></xs:element>
                        <xs:element name="_UserName" type="xs:string" minOccurs="0"></xs:element>
                    </xs:sequence>
                </xs:extension>
            </xs:complexContent>
        </xs:complexType>
        <xs:element name="AccountAuthCredentials" type="tns:AccountAuthCredentials"></xs:element>
        <xs:complexType name="FormsAuthCredentials">
            <xs:complexContent>
                <xs:extension base="tns:SecurableAuthData">
                    <xs:sequence>
                        <xs:element name="_AuthSchemeName" type="xs:string" minOccurs="0"></xs:element>
                        <xs:element name="_AuthSubmissionMethod" type="xs:string" minOccurs="0"></xs:element>
                        <xs:element name="_AuthSubmissionPath" type="xs:string" minOccurs="0"></xs:element>
                        <xs:element name="_ErrorPageUrl" type="xs:string" minOccurs="0"></xs:element>
                    </xs:sequence>
                </xs:extension>
            </xs:complexContent>
        </xs:complexType>
        <xs:element name="FormsAuthCredentials" type="tns:FormsAuthCredentials"></xs:element>
        <xs:complexType name="AliasInfoCollection"></xs:complexType>
        <xs:element name="AliasInfoCollection" type="tns:AliasInfoCollection"></xs:element>
        <xs:complexType name="BaseInfoCollectionOfAliasInfoTzWWwPjw">
            <xs:sequence>
                <xs:element name="LastItemName" type="xs:string" minOccurs="0"></xs:element>
                <xs:element name="dictionary" type="q10:ArrayOfKeyValueOfstringAliasInfoy6h3NzC8" minOccurs="0"></xs:element>
            </xs:sequence>
        </xs:complexType>
        <xs:element name="BaseInfoCollectionOfAliasInfoTzWWwPjw" type="tns:BaseInfoCollectionOfAliasInfoTzWWwPjw"></xs:element>
        <xs:complexType name="AliasInfo">
            <xs:complexContent>
                <xs:extension base="tns:BaseInfo">
                    <xs:sequence>
                        <xs:element name="ManagedPid" type="xs:int" minOccurs="0"></xs:element>
                        <xs:element name="SchemaId" type="xs:int" minOccurs="0"></xs:element>
                    </xs:sequence>
                </xs:extension>
            </xs:complexContent>
        </xs:complexType>
        <xs:element name="AliasInfo" type="tns:AliasInfo"></xs:element>
        <xs:complexType name="BaseInfo">
            <xs:sequence>
                <xs:element name="Name" type="xs:string" minOccurs="0"></xs:element>
            </xs:sequence>
        </xs:complexType>
        <xs:element name="BaseInfo" type="tns:BaseInfo"></xs:element>
        <xs:complexType name="CrawledPropertyInfoCollection"></xs:complexType>
        <xs:element name="CrawledPropertyInfoCollection" type="tns:CrawledPropertyInfoCollection"></xs:element>
        <xs:complexType name="BaseInfoCollectionOfCrawledPropertyInfoTzWWwPjw">
            <xs:sequence>
                <xs:element name="LastItemName" type="xs:string" minOccurs="0"></xs:element>
                <xs:element name="dictionary" type="q11:ArrayOfKeyValueOfstringCrawledPropertyInfoy6h3NzC8" minOccurs="0"></xs:element>
            </xs:sequence>
        </xs:complexType>
        <xs:element name="BaseInfoCollectionOfCrawledPropertyInfoTzWWwPjw" type="tns:BaseInfoCollectionOfCrawledPropertyInfoTzWWwPjw"></xs:element>
        <xs:complexType name="CrawledPropertyInfo">
            <xs:complexContent>
                <xs:extension base="tns:BaseInfo">
                    <xs:sequence>
                        <xs:element name="CategoryName" type="xs:string" minOccurs="0"></xs:element>
                        <xs:element name="IsMappedToContents" type="xs:boolean" minOccurs="0"></xs:element>
                        <xs:element name="IsNameEnum" type="xs:boolean" minOccurs="0"></xs:element>
                        <xs:element name="MappedManagedProperties" type="tns:ArrayOfManagedPropertyInfo" minOccurs="0"></xs:element>
                        <xs:element name="Propset" type="ser:guid" minOccurs="0"></xs:element>
                        <xs:element name="Samples" type="q12:ArrayOfstring" minOccurs="0"></xs:element>
                        <xs:element name="SchemaId" type="xs:int" minOccurs="0"></xs:element>
                    </xs:sequence>
                </xs:extension>
            </xs:complexContent>
        </xs:complexType>
        <xs:element name="CrawledPropertyInfo" type="tns:CrawledPropertyInfo"></xs:element>
        <xs:complexType name="ArrayOfManagedPropertyInfo">
            <xs:sequence>
                <xs:element name="ManagedPropertyInfo" type="tns:ManagedPropertyInfo" minOccurs="0" maxOccurs="unbounded"></xs:element>
            </xs:sequence>
        </xs:complexType>
        <xs:element name="ArrayOfManagedPropertyInfo" type="tns:ArrayOfManagedPropertyInfo"></xs:element>
        <xs:complexType name="ManagedPropertyInfo">
            <xs:complexContent>
                <xs:extension base="tns:BaseInfo">
                    <xs:sequence>
                        <xs:element name="Aliases" type="q13:ArrayOfstring" minOccurs="0"></xs:element>
                        <xs:element name="CompleteMatching" type="xs:boolean" minOccurs="0"></xs:element>
                        <xs:element name="Context" type="xs:short" minOccurs="0"></xs:element>
                        <xs:element name="DeleteDisallowed" type="xs:boolean" minOccurs="0"></xs:element>
                        <xs:element name="Description" type="xs:string" minOccurs="0"></xs:element>
                        <xs:element name="EnabledForScoping" type="xs:boolean" minOccurs="0"></xs:element>
                        <xs:element name="EntityExtractorBitMap" type="xs:int" minOccurs="0"></xs:element>
                        <xs:element name="FullTextIndex" type="xs:string" minOccurs="0"></xs:element>
                        <xs:element name="HasMultipleValues" type="xs:boolean" minOccurs="0"></xs:element>
                        <xs:element name="IndexOptions" type="xs:int" minOccurs="0"></xs:element>
                        <xs:element name="IsReadOnly" type="xs:boolean" minOccurs="0"></xs:element>
                        <xs:element name="ManagedType" type="tns:ManagedDataType" minOccurs="0"></xs:element>
                        <xs:element name="MappedCrawledProperties" type="tns:ArrayOfCrawledPropertyInfo" minOccurs="0"></xs:element>
                        <xs:element name="MappingDisallowed" type="xs:boolean" minOccurs="0"></xs:element>
                        <xs:element name="Pid" type="xs:int" minOccurs="0"></xs:element>
                        <xs:element name="Queryable" type="xs:boolean" minOccurs="0"></xs:element>
                        <xs:element name="Refinable" type="xs:boolean" minOccurs="0"></xs:element>
                        <xs:element name="RefinerConfiguration" type="tns:RefinerConfiguration" minOccurs="0"></xs:element>
                        <xs:element name="RemoveDuplicates" type="xs:boolean" minOccurs="0"></xs:element>
                        <xs:element name="RespectPriority" type="xs:boolean" minOccurs="0"></xs:element>
                        <xs:element name="Retrievable" type="xs:boolean" minOccurs="0"></xs:element>
                        <xs:element name="SafeForAnonymous" type="xs:boolean" minOccurs="0"></xs:element>
                        <xs:element name="Searchable" type="xs:boolean" minOccurs="0"></xs:element>
                        <xs:element name="Sortable" type="xs:boolean" minOccurs="0"></xs:element>
                        <xs:element name="SortableType" type="tns:SortableType" minOccurs="0"></xs:element>
                        <xs:element name="TokenNormalization" type="xs:boolean" minOccurs="0"></xs:element>
                        <xs:element name="UpdateGroup" type="xs:string" minOccurs="0"></xs:element>
                    </xs:sequence>
                </xs:extension>
            </xs:complexContent>
        </xs:complexType>
        <xs:element name="ManagedPropertyInfo" type="tns:ManagedPropertyInfo"></xs:element>
        <xs:simpleType name="ManagedDataType">
            <xs:restriction base="xs:string">
                <xs:enumeration value="Unsupported" />
                <xs:enumeration value="Text" />
                <xs:enumeration value="Integer" />
                <xs:enumeration value="Decimal" />
                <xs:enumeration value="DateTime" />
                <xs:enumeration value="YesNo" />
                <xs:enumeration value="Binary" />
                <xs:enumeration value="Double" />
            </xs:restriction>
        </xs:simpleType>
        <xs:element name="ManagedDataType" type="tns:ManagedDataType"></xs:element>
        <xs:complexType name="ArrayOfCrawledPropertyInfo">
            <xs:sequence>
                <xs:element name="CrawledPropertyInfo" type="tns:CrawledPropertyInfo" minOccurs="0" maxOccurs="unbounded"></xs:element>
            </xs:sequence>
        </xs:complexType>
        <xs:element name="ArrayOfCrawledPropertyInfo" type="tns:ArrayOfCrawledPropertyInfo"></xs:element>
        <xs:complexType name="RefinerConfiguration">
            <xs:sequence>
                <xs:element name="Anchoring" type="tns:RefinerAnchoring" minOccurs="0"></xs:element>
                <xs:element name="CutoffMaxBuckets" type="xs:int" minOccurs="0"></xs:element>
                <xs:element name="Divisor" type="xs:int" minOccurs="0"></xs:element>
                <xs:element name="Intervals" type="xs:int" minOccurs="0"></xs:element>
                <xs:element name="Resolution" type="xs:int" minOccurs="0"></xs:element>
                <xs:element name="Type" type="tns:RefinerType" minOccurs="0"></xs:element>
            </xs:sequence>
        </xs:complexType>
        <xs:element name="RefinerConfiguration" type="tns:RefinerConfiguration"></xs:element>
        <xs:simpleType name="RefinerAnchoring">
            <xs:restriction base="xs:string">
                <xs:enumeration value="Auto" />
                <xs:enumeration value="None" />
                <xs:enumeration value="Complete" />
                <xs:enumeration value="Prefix" />
                <xs:enumeration value="Suffix" />
            </xs:restriction>
        </xs:simpleType>
        <xs:element name="RefinerAnchoring" type="tns:RefinerAnchoring"></xs:element>
        <xs:simpleType name="RefinerType">
            <xs:restriction base="xs:string">
                <xs:enumeration value="Deep" />
                <xs:enumeration value="Latent" />
                <xs:enumeration value="Shallow" />
            </xs:restriction>
        </xs:simpleType>
        <xs:element name="RefinerType" type="tns:RefinerType"></xs:element>
        <xs:simpleType name="SortableType">
            <xs:restriction base="xs:string">
                <xs:enumeration value="Enabled" />
                <xs:enumeration value="Latent" />
            </xs:restriction>
        </xs:simpleType>
        <xs:element name="SortableType" type="tns:SortableType"></xs:element>
        <xs:complexType name="ManagedPropertyInfoCollection">
            <xs:complexContent>
                <xs:extension base="tns:BaseInfoCollectionOfManagedPropertyInfoTzWWwPjw">
                    <xs:sequence>
                        <xs:element name="TotalCount" type="xs:int" minOccurs="0"></xs:element>
                    </xs:sequence>
                </xs:extension>
            </xs:complexContent>
        </xs:complexType>
        <xs:element name="ManagedPropertyInfoCollection" type="tns:ManagedPropertyInfoCollection"></xs:element>
        <xs:complexType name="BaseInfoCollectionOfManagedPropertyInfoTzWWwPjw">
            <xs:sequence>
                <xs:element name="LastItemName" type="xs:string" minOccurs="0"></xs:element>
                <xs:element name="dictionary" type="q14:ArrayOfKeyValueOfstringManagedPropertyInfoy6h3NzC8" minOccurs="0"></xs:element>
            </xs:sequence>
        </xs:complexType>
        <xs:element name="BaseInfoCollectionOfManagedPropertyInfoTzWWwPjw" type="tns:BaseInfoCollectionOfManagedPropertyInfoTzWWwPjw"></xs:element>
        <xs:complexType name="MappingInfoCollection"></xs:complexType>
        <xs:element name="MappingInfoCollection" type="tns:MappingInfoCollection"></xs:element>
        <xs:complexType name="BaseInfoCollectionOfMappingInfoTzWWwPjw">
            <xs:sequence>
                <xs:element name="LastItemName" type="xs:string" minOccurs="0"></xs:element>
                <xs:element name="dictionary" type="q15:ArrayOfKeyValueOfstringMappingInfoy6h3NzC8" minOccurs="0"></xs:element>
            </xs:sequence>
        </xs:complexType>
        <xs:element name="BaseInfoCollectionOfMappingInfoTzWWwPjw" type="tns:BaseInfoCollectionOfMappingInfoTzWWwPjw"></xs:element>
        <xs:complexType name="MappingInfo">
            <xs:complexContent>
                <xs:extension base="tns:BaseInfo">
                    <xs:sequence>
                        <xs:element name="CrawledPropertyName" type="xs:string" minOccurs="0"></xs:element>
                        <xs:element name="CrawledPropset" type="ser:guid" minOccurs="0"></xs:element>
                        <xs:element name="ManagedPid" type="xs:int" minOccurs="0"></xs:element>
                        <xs:element name="MappingOrder" type="xs:int" minOccurs="0"></xs:element>
                        <xs:element name="SchemaId" type="xs:int" minOccurs="0"></xs:element>
                    </xs:sequence>
                </xs:extension>
            </xs:complexContent>
        </xs:complexType>
        <xs:element name="MappingInfo" type="tns:MappingInfo"></xs:element>
        <xs:complexType name="OverrideInfoCollection"></xs:complexType>
        <xs:element name="OverrideInfoCollection" type="tns:OverrideInfoCollection"></xs:element>
        <xs:complexType name="BaseInfoCollectionOfOverrideInfoTzWWwPjw">
            <xs:sequence>
                <xs:element name="LastItemName" type="xs:string" minOccurs="0"></xs:element>
                <xs:element name="dictionary" type="q16:ArrayOfKeyValueOfstringOverrideInfoy6h3NzC8" minOccurs="0"></xs:element>
            </xs:sequence>
        </xs:complexType>
        <xs:element name="BaseInfoCollectionOfOverrideInfoTzWWwPjw" type="tns:BaseInfoCollectionOfOverrideInfoTzWWwPjw"></xs:element>
        <xs:complexType name="OverrideInfo">
            <xs:complexContent>
                <xs:extension base="tns:BaseInfo">
                    <xs:sequence>
                        <xs:element name="AliasesOverridden" type="xs:boolean" minOccurs="0"></xs:element>
                        <xs:element name="ExtraProperties" type="xs:string" minOccurs="0"></xs:element>
                        <xs:element name="ManagedPid" type="xs:int" minOccurs="0"></xs:element>
                        <xs:element name="MappingsOverridden" type="xs:boolean" minOccurs="0"></xs:element>
                        <xs:element name="SchemaId" type="xs:int" minOccurs="0"></xs:element>
                        <xs:element name="TokenNormalization" type="xs:boolean" minOccurs="0"></xs:element>
                    </xs:sequence>
                </xs:extension>
            </xs:complexContent>
        </xs:complexType>
        <xs:element name="OverrideInfo" type="tns:OverrideInfo"></xs:element>
    </xs:schema>

![Footer](../icons/footer.gif "Footer")

[© 2013 Microsoft Corporation. All rights
reserved.](office-2013-documentation-copyright-notice.htm)



