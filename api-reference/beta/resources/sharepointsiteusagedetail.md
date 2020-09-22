---
title: Тип ресурса Шарепоинтситеусажедетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 1b61321dfeb0a9aa14651e7d13ad7184b30c3423
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997790"
---
# <a name="sharepointsiteusagedetail-resource-type"></a>Тип ресурса Шарепоинтситеусажедетаил

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство                | Тип    |
| :---------------------- | :------ |
| репортрефрешдате       | Дата    |
| siteId                  | Guid  |
| siteUrl                 | String  |
| овнердисплайнаме        | String  |
| овнерпринЦипалнаме      | String  |
| isDeleted               | Boolean |
| ластактивитидате        | Дата    |
| филекаунт               | Int64   |
| активефилекаунт         | Int64   |
| пажевиевкаунт           | Int64   |
| виситедпажекаунт        | Int64   |
| сторажеусединбитес      | Int64   |
| сторажеаллокатединбитес | Int64   |
| рутвебтемплате         | String  |
| репортпериод            | String  |

## <a name="json-representation"></a>Представление JSON

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
  "fileCount": 1024,
  "activeFileCount": 1024,
  "pageViewCount": 1024,
  "visitedPageCount": 1024,
  "storageUsedInBytes": 1024,
  "storageAllocatedInBytes": 1024,
  "rootWebTemplate": "String",
  "reportPeriod": "String"
}
```


