---
title: Тип ресурса Онедривеусажеаккаунтдетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 594339072c683b053ddeb637b6f401bae2aed322
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812073"
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
| isDeleted               | Логический |
| ластактивитидате        | Дата    |
| филекаунт               | Int64   |
| активефилекаунт         | Int64   |
| сторажеусединбитес      | Int64   |
| сторажеаллокатединбитес | Int64   |
| репортпериод            | String  |

## <a name="json-representation"></a>Представление в формате JSON

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
