---
title: Тип ресурса plannerAssignedToTaskBoardTaskFormat
description: Ресурс **plannerAssignedToTaskBoardTaskFormat** представляет сведения, используемые для корректной визуализации задачи в представлении AssignedTo доски задач (представление, упорядоченное пользователями, которым назначены задачи). Каждой задаче будет назначен один объект **plannerAssignedToTaskBoardTaskFormat** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: aca03e2a82d7fe42aa229c2f53d0c1dd066a30bc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037621"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a>Тип ресурса plannerAssignedToTaskBoardTaskFormat

Пространство имен: microsoft.graph

Ресурс **plannerAssignedToTaskBoardTaskFormat** представляет сведения, используемые для корректной визуализации задачи в представлении AssignedTo доски задач (представление, упорядоченное пользователями, которым назначены задачи). Каждой [задаче](plannertask.md) будет назначен один объект **plannerAssignedToTaskBoardTaskFormat** .


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerAssignedToTaskBoardTaskFormat](../api/plannerassignedtotaskboardtaskformat-get.md) | [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md); |Чтение свойств и связей объекта **plannerAssignedToTaskBoardTaskFormat** .|
|[обновление](../api/plannerassignedtotaskboardtaskformat-update.md). | [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md);  |Обновление объекта **plannerAssignedToTaskBoardTaskFormat** . |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Идентификатор ресурса. Содержит 28 знаков, учитывается регистр. [Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.|
|orderHintsByAssignee|[plannerOrderHintsByAssignee](plannerorderhintsbyassignee.md)|Словарь указаний, используемых для упорядочения задач в представлении AssignedTo доски задач. Ключ каждой записи — один из пользователей, которому назначена задача, а значение — указание порядка. Формат каждого значения описан [здесь](planner-order-hint-format.md).|
|unassignedOrderHint|Строка|Указание, используемое для расположения задачи в окне "Кому назначено" доски задач, когда задача никому не назначена, или если в словаре orderHintsByAssignee нет указания order для пользователя, которому назначена задача. Формат определяется, как описано [здесь](planner-order-hint-format.md).|

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

