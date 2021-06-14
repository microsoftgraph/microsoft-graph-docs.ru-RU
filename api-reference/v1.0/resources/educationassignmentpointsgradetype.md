---
title: тип ресурсов educationAssignmentPointsGradeType
description: Тип ресурса, используемый с **свойством assignments.grading.** Это подкласс educationAssignmentGradeType.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ca5a6ba0dd6674d55b4659fbdb1e2c288a65eb12
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912865"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a>тип ресурсов educationAssignmentPointsGradeType

Пространство имен: microsoft.graph

Тип ресурса, используемый с **свойством assignments.grading.** Это подкласс [educationAssignmentGradeType](educationassignmentgradetype.md).

Это указывает на то, что назначение имеет оценку и сохраняет максимальное количество баллов, которые каждый учащийся может достичь в этом элементе работы. При назначении каждая отправка получит свойство [educationAssignmentPointsGrade,](educationassignmentpointsgrade.md) связанное с ним для хранения баллов каждого учащегося.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|maxPoints|Одинарное| Max указывает возможное для этого назначения.  |

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
  "maxPoints": "Double"
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
  "suppressions": []
}
-->


