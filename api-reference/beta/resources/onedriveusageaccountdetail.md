---
title: Тип ресурса oneDriveUsageAccountDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 92695f509302ede4b3ce64320e8f4ed42418f7e5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842611"
---
# <a name="onedriveusageaccountdetail-resource-type"></a>Тип ресурса oneDriveUsageAccountDetail

## <a name="properties"></a>Свойства

| Свойство                | Тип    |
| :---------------------- | :------ |
| reportRefreshDate       | Date    |
| siteUrl                 | Строка  |
| ownerDisplayName        | Строка  |
| isDeleted               | Логический |
| lastActivityDate        | Date    |
| fileCount               | Int64   |
| activeFileCount         | Int64   |
| storageUsedInBytes      | Int64   |
| storageAllocatedInBytes | Int64   |
| reportPeriod            | String  |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteUrl": "String", 
  "ownerDisplayName": "String", 
  "isDeleted": true, 
  "lastActivityDate": "Date", 
  "fileCount": 1024, 
  "activeFileCount": 1024, 
  "storageUsedInBytes": 1024, 
  "storageAllocatedInBytes": 1024, 
  "reportPeriod": "String"
}
```
