---
title: Тип ресурса office365ActivationsUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 78c21f33352e5f6357638de8dacc4b628b6ef93b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522486"
---
# <a name="office365activationsusercounts-resource-type"></a>Тип ресурса office365ActivationsUserCounts

Пространство имен: Microsoft. Graph

## <a name="properties"></a>Свойства

| Свойство                 | Тип   | Описание                              |
| :----------------------- | :----- | ---------------------------------------- |
| репортрефрешдате        | Дата   | Самая поздняя дата контента.          |
| продукттипе              | String | Тип продукта, например "Office 365 профессиональный плюс", "клиент Project" или "Visio Pro для Office 365". |
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
