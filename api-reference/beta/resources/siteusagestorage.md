---
title: тип ресурса siteUsageStorage
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: e00e260bfcab2992ecf892ec66b0d39884a31d477c84b0b6c46d3e004b274485
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54167781"
---
# <a name="siteusagestorage-resource-type"></a>тип ресурса siteUsageStorage

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство           | Тип   |
| :----------------- | :----- |
| reportRefreshDate  | Дата   |
| siteType           | Строка |
| storageUsedInBytes | Int64  |
| reportDate         | Дата   |
| reportPeriod       | String |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date",
  "siteType": "String",
  "storageUsedInBytes": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```


