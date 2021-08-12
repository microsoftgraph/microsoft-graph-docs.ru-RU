---
title: Тип ресурса plannerAssignment
description: Ресурс **plannerAssignment** представляет назначение задачи пользователю. Этот тип используется в планировщиках открытого типаAssignments.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 23677678d6f31be3ec24630947c6adc41a2e3bf8cbd35c606365d2adfd50b16d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126377"
---
# <a name="plannerassignment-resource-type"></a>Тип ресурса plannerAssignment

Пространство имен: microsoft.graph

Ресурс **plannerAssignment** представляет назначение задачи пользователю. Этот тип используется в планировщиках открытого [типаAssignments.](plannerassignments.md)


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|assignedBy|[identitySet](identityset.md)|Удостоверение пользователя, который выполнил назначение задачи, то есть назначителя.|
|assignedDateTime|DateTimeOffset|Время, в которое была назначена задача. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|orderHint|String|Подсказка, используемая для заказа назначаемой задачи. Формат определяется как описанный [здесь](planner-order-hint-format.md).|

## <a name="json-representation"></a>Представление JSON
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

