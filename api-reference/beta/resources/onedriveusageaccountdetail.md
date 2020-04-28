---
title: Тип ресурса Онедривеусажеаккаунтдетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 21bc509fd2364365e29d1e35bcbe78d67fdc40c8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522381"
---
# <a name="onedriveusageaccountdetail-resource-type"></a>Тип ресурса Онедривеусажеаккаунтдетаил

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство                | Тип    |
| :---------------------- | :------ |
| репортрефрешдате       | Дата    |
| siteUrl                 | String  |
| овнердисплайнаме        | String  |
| овнерпринЦипалнаме      | String  |
| isDeleted               | Boolean |
| ластактивитидате        | Дата    |
| филекаунт               | Int64   |
| активефилекаунт         | Int64   |
| сторажеусединбитес      | Int64   |
| сторажеаллокатединбитес | Int64   |
| репортпериод            | String  |

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
