---
title: Тип ресурса Шарепоинтситеусажедетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 4cb53d65d505e47fa2fed85c3bdc3b263dd21dff
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520683"
---
# <a name="sharepointsiteusagedetail-resource-type"></a>Тип ресурса Шарепоинтситеусажедетаил

Пространство имен: Microsoft. Graph

## <a name="properties"></a>Свойства

| Свойство                | Тип    |
| :---------------------- | :------ |
| репортрефрешдате       | Дата    |
| siteId                  | GUID  |
| siteUrl                 | String  |
| овнердисплайнаме        | String  |
| овнерпринЦипалнаме      | String  |
| isDeleted               | Логический |
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
