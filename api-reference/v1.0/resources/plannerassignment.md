---
title: Тип ресурса plannerAssignment
description: Ресурс **plannerAssignment** представляет назначение задачи пользователю. Этот тип используется в планировщиках открытого типаAssignments.
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: ea71ff05e4c649712e9e37566dc8cc71e3529c76
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044365"
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

