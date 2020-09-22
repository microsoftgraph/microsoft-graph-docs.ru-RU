---
title: Тип ресурса office365ActivationsUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 21e18b35dc4e4ff639087617d679ae1583516026
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021226"
---
# <a name="office365activationsusercounts-resource-type"></a>Тип ресурса office365ActivationsUserCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство                 | Тип   | Описание                              |
| :----------------------- | :----- | ---------------------------------------- |
| репортрефрешдате        | Дата   | Самая поздняя дата контента.          |
| продукттипе              | String | Тип продукта, например "Microsoft 365 профессиональный плюс" или "клиент Project". |
| ей                 | Int64  | Количество пользователей, которым назначена лицензия на продукт. |
| активной                | Int64  | Количество пользователей, которые активировали продукт. |
| шаредкомпутерактиватион | Int64  | Количество пользователей, которые использовали продукт на общем компьютере. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "assigned": 1024, 
  "activated": 1024,
  "sharedComputerActivation": 1024
}
```


