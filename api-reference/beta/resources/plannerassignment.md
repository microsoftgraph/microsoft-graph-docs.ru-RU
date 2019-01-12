---
title: Тип ресурса plannerAssignment
description: Ресурс **plannerAssignment** представляет назначения задачи для пользователя. Этот тип используется в plannerAssignments открытого типа.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 5eaeb00abf7446db1085a7c0d0916b0a7b5b2434
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963964"
---
# <a name="plannerassignment-resource-type"></a>Тип ресурса plannerAssignment

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Ресурс **plannerAssignment** представляет назначение задачи пользователю. Этот тип используется в открытом типе [plannerAssignments](plannerassignments.md).


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|assignedBy|[identitySet](identityset.md)|Удостоверение пользователя, назначившего задачу.|
|assignedDateTime|DateTimeOffset|Дата и время назначения задачи. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|orderHint|String|Указание, которое позволяет упорядочить назначенных пользователей для задачи. Используемый формат описан [здесь](planner-order-hint-format.md).|

## <a name="json-representation"></a>Представление в формате JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignment"
}-->

```json
{
  "assignedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "assignedDateTime": "String (timestamp)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
