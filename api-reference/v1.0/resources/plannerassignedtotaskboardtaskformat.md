---
title: PlannerAssignedToTaskBoardTaskFormat type
description: Ресурс **plannerAssignedToTaskBoardTaskFormat** представляет сведения, используемые для правильного отрисовки задачи в представлении AssignedTo в совете задач (представление, организованное пользователями, которым назначены задачи). Каждая задача будет иметь один **объект plannerAssignedToTaskBoardTaskFormat,** связанный с ним.
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: f244c9ff4cd4e9801c1ecef0e1e1170e35f699c0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044393"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a>PlannerAssignedToTaskBoardTaskFormat type

Пространство имен: microsoft.graph

Ресурс **plannerAssignedToTaskBoardTaskFormat** представляет сведения, используемые для правильного отрисовки задачи в представлении AssignedTo в совете задач (представление, организованное пользователями, которым назначены задачи). Каждая [задача](plannertask.md) будет иметь один **объект plannerAssignedToTaskBoardTaskFormat,** связанный с ним.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerAssignedToTaskBoardTaskFormat](../api/plannerassignedtotaskboardtaskformat-get.md) | [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) |Чтение свойств и связей **объекта plannerAssignedToTaskBoardTaskFormat.**|
|[Обновление](../api/plannerassignedtotaskboardtaskformat-update.md) | [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)  |Объект **Update PlannerAssignedToTaskBoardTaskFormat.** |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. ID ресурса. Содержит 28 знаков, учитывается регистр. [Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.|
|orderHintsByAssignee|[plannerOrderHintsByAssignee](plannerorderhintsbyassignee.md)|Словарь указаний, используемых для упорядочения задач в представлении AssignedTo доски задач. Ключ каждой записи — один из пользователей, которому назначена задача, а значение — указание порядка. Формат каждого значения описан [здесь](planner-order-hint-format.md).|
|unassignedOrderHint|Строка|Указание, используемое для расположения задачи в окне "Кому назначено" доски задач, когда задача никому не назначена, или если в словаре orderHintsByAssignee нет указания order для пользователя, которому назначена задача. Формат определяется, как описано [здесь](planner-order-hint-format.md).|

## <a name="relationships"></a>Отношения
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

