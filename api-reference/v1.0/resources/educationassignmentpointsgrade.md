---
title: Тип ресурса educationAssignmentPointsGrade
description: Если для задания задано значение типа оценки баллов, каждый объект каждой отправки будет связан со **свойством submission.grade** .
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8019915e246a1b219357887ead1ee9ec8e7627d6
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2022
ms.locfileid: "64684671"
---
# <a name="educationassignmentpointsgrade-resource-type"></a>Тип ресурса educationAssignmentPointsGrade

Пространство имен: microsoft.graph

Если для задания задано значение типа оценки баллов, каждый объект каждой отправки будет связан со **свойством submission.grade** . При этом создается подкласс [из educationAssignmentGrade](educationassignmentgrade.md), который добавляет данные who в это свойство. Максимальные точки хранятся в **свойстве assignments.grading** .


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|points|Одинарное|Количество точек, которые преподаватель предоставляет этому объекту отправки.|
|gradedBy|[identitySet](identityset.md)| Пользователь, выполнивший проверку. |
|gradedDateTime|DateTimeOffset| Момент времени, когда оценка была применена к этому объекту отправки. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
}-->

```json
{
  "points": "Double",
  "gradedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "gradedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


