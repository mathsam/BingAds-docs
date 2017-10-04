﻿---
title: AdExtensionEditorialReasonCollection Data Object
ms.service: bing-ads-campaign-management
ms.topic: article
author: eric-urban
ms.author: eur
---
# AdExtensionEditorialReasonCollection Data Object
Defines a collection of ad extensions that failed editorial review.

## Syntax
```xml
<xs:complexType name="AdExtensionEditorialReasonCollection" xmlns:xs="http://www.w3.org/2001/XMLSchema">
  <xs:sequence>
    <xs:element minOccurs="0" name="AdExtensionId" type="xs:long" />
    <xs:element minOccurs="0" name="Reasons" nillable="true" type="tns:ArrayOfAdExtensionEditorialReason" />
  </xs:sequence>
</xs:complexType>
```

## <a name="elements"></a>Elements

|Element|Description|Data Type|
|-----------|---------------|-------------|
|<a name="adextensionid"></a>AdExtensionId|The identifier of the ad extension that failed editorial review.|**long**|
|<a name="reasons"></a>Reasons|A list of *AdExtensionEditorialReason* objects that identify the component of an ad extension that failed editorial review, and the reason for the failure.|[AdExtensionEditorialReason](adextensioneditorialreason.md) array|

## Requirements
Service: [CampaignManagementService.svc v11](https://campaign.api.bingads.microsoft.com/Api/Advertiser/CampaignManagement/v11/CampaignManagementService.svc)  
Namespace: https://bingads.microsoft.com/CampaignManagement/v11  

## Used By
[GetAdExtensionsEditorialReasons](getadextensionseditorialreasons.md)  