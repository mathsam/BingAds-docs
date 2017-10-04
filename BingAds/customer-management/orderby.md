﻿---
title: OrderBy Data Object
ms.service: bing-ads-customer-management
ms.topic: article
author: eric-urban
ms.author: eur
---
# OrderBy Data Object
Defines an order for the list of entities returned using one of the search operations, for example [SearchAccounts](../customer-management/searchaccounts.md), [SearchClientLinks](../customer-management/searchclientlinks.md), or [SearchCustomers](../customer-management/searchcustomers.md).

## Syntax
```xml
<xs:complexType name="OrderBy" xmlns:xs="http://www.w3.org/2001/XMLSchema">
  <xs:sequence>
    <xs:element minOccurs="0" name="Field" type="tns:OrderByField" />
    <xs:element minOccurs="0" name="Order" type="tns:SortOrder" />
  </xs:sequence>
</xs:complexType>
```

## <a name="elements"></a>Elements

|Element|Description|Data Type|
|-----------|---------------|-------------|
|<a name="field"></a>Field|Determines the field to order the results. For example order the results by *Id*.|[OrderByField](orderbyfield.md)|
|<a name="order"></a>Order|Determines whether the results are ascending or descending.|[SortOrder](sortorder.md)|

## Requirements
Service: [CustomerManagementService.svc v11](https://clientcenter.api.bingads.microsoft.com/Api/CustomerManagement/v11/CustomerManagementService.svc)  
Namespace: https://bingads.microsoft.com/Customer/v11/Entities  

## Used By
[SearchAccounts](searchaccounts.md)  
[SearchClientLinks](searchclientlinks.md)  
[SearchCustomers](searchcustomers.md)  