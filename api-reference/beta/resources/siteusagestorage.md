---
title: Тип ресурса Ситеусажестораже
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 36ca6cc16ec4eeaf399bb8bd49db51c43a9dd8be
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807915"
---
# <a name="siteusagestorage-resource-type"></a>Тип ресурса Ситеусажестораже

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство           | Тип   |
| :----------------- | :----- |
| репортрефрешдате  | Дата   |
| ситетипе           | String |
| сторажеусединбитес | Int64  |
| reportDate         | Дата   |
| репортпериод       | String |

## <a name="json-representation"></a>Представление в формате JSON

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
