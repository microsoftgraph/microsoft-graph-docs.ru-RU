---
title: Тип ресурса Шарепоинтситеусажедетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e0827f6b6b991136198fc174e01e7d0e1f91c259
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584000"
---
# <a name="sharepointsiteusagedetail-resource-type"></a>Тип ресурса Шарепоинтситеусажедетаил

## <a name="properties"></a>Свойства

| Свойство                | Тип    |
| :---------------------- | :------ |
| Репортрефрешдате       | Дата    |
| siteId                  | Guid  |
| siteUrl                 | String  |
| Овнердисплайнаме        | String  |
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
