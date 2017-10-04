﻿---
title: CustomerInfo Data Object
ms.service: bing-ads-customer-management
ms.topic: article
author: eric-urban
ms.author: eur
---
# CustomerInfo Data Object
Defines a customer identification object that contains information that identifies a customer.

## Syntax
```xml
<xs:complexType name="CustomerInfo" xmlns:xs="http://www.w3.org/2001/XMLSchema">
  <xs:sequence>
    <xs:element minOccurs="0" name="Id" nillable="true" type="xs:long" />
    <xs:element minOccurs="0" name="Name" nillable="true" type="xs:string" />
  </xs:sequence>
</xs:complexType>
```

## <a name="elements"></a>Elements

|Element|Description|Data Type|
|-----------|---------------|-------------|
|<a name="id"></a>Id|The system generated identifier of the customer.|**long**|
|<a name="name"></a>Name|The name of the customer.|**string**|

## Requirements
Service: [CustomerManagementService.svc v11](https://clientcenter.api.bingads.microsoft.com/Api/CustomerManagement/v11/CustomerManagementService.svc)  
Namespace: https://bingads.microsoft.com/Customer/v11/Entities  

## Used By
[AdvertiserAccount](advertiseraccount.md)  
[GetCustomersInfo](getcustomersinfo.md)  