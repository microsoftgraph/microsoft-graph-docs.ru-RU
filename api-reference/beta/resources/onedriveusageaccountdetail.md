---
title: Тип ресурса Онедривеусажеаккаунтдетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: cc80110a2f8f755ef984b2f993ea660798a86743
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966470"
---
# <a name="onedriveusageaccountdetail-resource-type"></a>Тип ресурса Онедривеусажеаккаунтдетаил

## <a name="properties"></a>Свойства

| Свойство                | Тип    |
| :---------------------- | :------ |
| Репортрефрешдате       | Дата    |
| siteUrl                 | String  |
| Овнердисплайнаме        | String  |
| ОвнерпринЦипалнаме      | String  |
| isDeleted               | Boolean |
| Ластактивитидате        | Дата    |
| Филекаунт               | Int64   |
| Активефилекаунт         | Int64   |
| Сторажеусединбитес      | Int64   |
| Сторажеаллокатединбитес | Int64   |
| Репортпериод            | String  |

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
