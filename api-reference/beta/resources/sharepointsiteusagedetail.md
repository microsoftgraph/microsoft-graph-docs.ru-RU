---
title: Тип ресурса Шарепоинтситеусажедетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 10b0f83dc6ed69fc3158e7d5ac6f35e242052042
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2019
ms.locfileid: "34344936"
---
# <a name="sharepointsiteusagedetail-resource-type"></a>Тип ресурса Шарепоинтситеусажедетаил

## <a name="properties"></a>Свойства

| Свойство                | Тип    |
| :---------------------- | :------ |
| Репортрефрешдате       | Дата    |
| siteId                  | GUID  |
| siteUrl                 | String  |
| Овнердисплайнаме        | String  |
| ОвнерпринЦипалнаме      | String  |
| isDeleted               | Boolean |
| Ластактивитидате        | Дата    |
| Филекаунт               | Int64   |
| Активефилекаунт         | Int64   |
| Пажевиевкаунт           | Int64   |
| Виситедпажекаунт        | Int64   |
| Сторажеусединбитес      | Int64   |
| Сторажеаллокатединбитес | Int64   |
| Рутвебтемплате         | String  |
| Репортпериод            | String  |

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
