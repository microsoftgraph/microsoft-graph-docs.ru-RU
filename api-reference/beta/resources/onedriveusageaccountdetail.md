---
title: Тип ресурса Онедривеусажеаккаунтдетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: bcf75fad8c39a543e69fc378546a2621f24eaeab
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2019
ms.locfileid: "34344929"
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
