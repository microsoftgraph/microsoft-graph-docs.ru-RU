---
title: Тип ресурса Маилбоксусажестораже
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 636417b5ec299bb11f82c406abecdebe72ee45de
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473417"
---
# <a name="mailboxusagestorage-resource-type"></a>Тип ресурса Маилбоксусажестораже

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство           | Тип   |
| :----------------- | :----- |
| репортрефрешдате  | Дата   |
| сторажеусединбитес | Int64  |
| reportDate         | Дата   |
| репортпериод       | String |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
