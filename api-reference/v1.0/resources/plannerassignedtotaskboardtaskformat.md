---
title: Тип ресурса plannerAssignedToTaskBoardTaskFormat
description: Ресурс **plannerAssignedToTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении AssignedTo на доске задач (представление, упорядоченное по пользователям, которым назначены задачи). C каждой задачей будет сопоставлен один объект **plannerAssignedToTaskBoardTaskFormat**.
localization_priority: Normal
ms.openlocfilehash: 0eee2ffaa08cb227ee1b9fa5fdab129d33ddd2ba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846069"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a>Тип ресурса plannerAssignedToTaskBoardTaskFormat

Ресурс **plannerAssignedToTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении AssignedTo на доске задач (представление, упорядоченное по пользователям, которым назначены задачи). C каждой [задачей](plannertask.md) будет сопоставлен один объект **plannerAssignedToTaskBoardTaskFormat**.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение plannerAssignedToTaskBoardTaskFormat](../api/plannerassignedtotaskboardtaskformat-get.md) | [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) |Чтение свойств и связей объекта **plannerAssignedToTaskBoardTaskFormat**.|
|[Обновление](../api/plannerassignedtotaskboardtaskformat-update.md) | [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)  |Обновление объекта **plannerAssignedToTaskBoardTaskFormat**. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|Строка| Только для чтения. Идентификатор ресурса. Это 28 знаков без учета регистра. [Формат](planner-identifiers-disclaimer.md) проверяются на службу.|
|orderHintsByAssignee|[plannerOrderHintsByAssignee](plannerorderhintsbyassignee.md)|Словарь указаний, используемых для упорядочения задач в представлении AssignedTo доски задач. Ключ каждой записи — один из пользователей, которому назначена задача, а значение — указание порядка. Формат каждого значения описан [здесь](planner-order-hint-format.md).|
|unassignedOrderHint|Строка|Значение указания, используемое для упорядочения задач в представлении AssignedTo доски задач, когда задача не назначена ни одному пользователю либо когда в словаре orderHintsByAssignee нет указания порядка для пользователя, которому назначена задача. Используемый формат описан [здесь](planner-order-hint-format.md).|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHintsByAssignee": {"@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"},
  "unassignedOrderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignedToTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
