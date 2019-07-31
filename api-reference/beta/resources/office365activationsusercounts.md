---
title: Тип ресурса office365ActivationsUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 33339578f498460aacd24481f166ab717138f8fa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966568"
---
# <a name="office365activationsusercounts-resource-type"></a>Тип ресурса office365ActivationsUserCounts

## <a name="properties"></a>Свойства

| Свойство                 | Тип   | Описание                              |
| :----------------------- | :----- | ---------------------------------------- |
| Репортрефрешдате        | Дата   | Самая поздняя дата контента.          |
| Продукттипе              | String | Тип продукта, например "Office 365 профессиональный плюс", "клиент Project" или "Visio Pro для Office 365". |
| ей                 | Int64  | Количество пользователей, которым назначена лицензия на продукт. |
| активной                | Int64  | Количество пользователей, которые активировали продукт. |
| Шаредкомпутерактиватион | Int64  | Количество пользователей, которые использовали продукт на общем компьютере. |

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
