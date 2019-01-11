---
title: Тип ресурса educationAssignmentPointsGradeType
description: Используется совместно со свойством **assignments.grading** . Это подкласс educationAssignmentGradeType.
localization_priority: Normal
ms.openlocfilehash: f00014eab1dbf7bc8eb78a8898c6abba9977e8a2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860972"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a>Тип ресурса educationAssignmentPointsGradeType

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Используется совместно со свойством **assignments.grading** . Это подкласс [educationAssignmentGradeType](educationassignmentgradetype.md).

Это означает, что назначения выражаемым числом и сохраняет максимальное число пунктов, которые можно достичь каждого студента на этот рабочий элемент. Если это назначения, каждой отправки будет [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) свойства, связанного с ним для хранения каждого студента точек.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|maxPoints|Single| Максимальное число точек можно для данного назначения.  |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGradeType"
}-->

```json
{
  "maxPoints": "Single"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGradeType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
