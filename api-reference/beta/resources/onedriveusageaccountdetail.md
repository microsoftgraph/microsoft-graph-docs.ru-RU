---
title: тип ресурса oneDriveUsageAccountDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 210728ee77bb013a4894156aef79d35248e7d2f32eed129baf8905655f192f5a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54155976"
---
# <a name="onedriveusageaccountdetail-resource-type"></a>тип ресурса oneDriveUsageAccountDetail

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство                | Тип    |
| :---------------------- | :------ |
| reportRefreshDate       | Дата    |
| siteUrl                 | Строка  |
| ownerDisplayName        | Строка  |
| ownerPrincipalName      | Строка  |
| isDeleted               | Логический |
| lastActivityDate        | Дата    |
| fileCount               | Int64   |
| activeFileCount         | Int64   |
| storageUsedInBytes      | Int64   |
| storageAllocatedInBytes | Int64   |
| reportPeriod            | Строка  |

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
  "ownerPrincipalName": "String",
  "isDeleted": true,
  "lastActivityDate": "Date",
  "fileCount": 1024,
  "activeFileCount": 1024,
  "storageUsedInBytes": 1024,
  "storageAllocatedInBytes": 1024,
  "reportPeriod": "String"
}
```


