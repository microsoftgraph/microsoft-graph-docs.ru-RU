---
title: Тип ресурса sharePointSiteUsageDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: f8f06cf9fcf1dfc01af3e98c01a79a86426e19ee
ms.sourcegitcommit: 1b01c820be659f85f380fc883bbb36036b7daadf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/05/2021
ms.locfileid: "50115222"
---
# <a name="sharepointsiteusagedetail-resource-type"></a>Тип ресурса sharePointSiteUsageDetail

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство                | Тип    |
| :---------------------- | :------ |
| reportRefreshDate       | Дата    |
| siteId                  | Guid  |
| siteUrl                 | Строка  |
| ownerDisplayName        | Строка  |
| ownerPrincipalName      | Строка  |
| isDeleted               | Boolean |
| lastActivityDate        | Дата    |
| SiteSensitivityLabelId  | Строка  |
| ExternalSharing         | Boolean |
| UnmanagedDevicePolicy   | Строка  |
| GeoLocation             | Строка  |
| fileCount               | Int64   |
| activeFileCount         | Int64   |
| pageViewCount           | Int64   |
| visitedPageCount        | Int64   |
| AnonymousLinkCount      | Int64   |
| CompanyLinkCount        | Int64   |
| SecureLinkForGuestCount | Int64   |
| SecureLinkForMemberCount| Int64   |
| storageUsedInBytes      | Int64   |
| storageAllocatedInBytes | Int64   |
| rootWebTemplate         | Строка  |
| reportPeriod            | Строка  |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointSiteUsageDetail"
} -->

```json
{
  "reportRefreshDate": "Date",
  "siteId": "Guid",
  "siteUrl": "String",
  "ownerDisplayName": "String",
  "ownerPrincipalName": "String",
  "isDeleted": true,
  "lastActivityDate": "Date",
  "lastActivityDate": "2017-09-01", 
  "SiteSensitivityLabelId": "String",
  "ExternalSharing": true,
  "UnmanagedDevicePolicy": "String",
  "GeoLocation": "String",
  "fileCount": 1024,
  "activeFileCount": 1024,
  "pageViewCount": 1024,
  "visitedPageCount": 1024,
  "AnonymousLinkCount": 5,
  "CompanyLinkCount": 8,
  "SecureLinkForGuestCount": 13,
  "SecureLinkForMemberCount": 11,
  "storageUsedInBytes": 1024,
  "storageAllocatedInBytes": 1024,
  "rootWebTemplate": "String",
  "reportPeriod": "String"
}
```


