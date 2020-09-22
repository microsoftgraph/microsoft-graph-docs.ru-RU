---
title: Тип ресурса Онедривеусажеаккаунтдетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 6e355e1f71d493b30ffb2fe41816208dfe4816e9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039288"
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


