---
title: Тип ресурса educationAssignmentPointsGradeType
description: Используется совместно со свойством **assignments.grading** . Это подкласс educationAssignmentGradeType.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 567bff38f8a20456dffffdd91775a1e32852fe20
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508897"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a>Тип ресурса educationAssignmentPointsGradeType

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGradeType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentpointsgradetype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
