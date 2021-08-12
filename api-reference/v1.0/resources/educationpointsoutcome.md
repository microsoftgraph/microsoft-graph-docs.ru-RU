---
title: тип ресурсов educationPointsOutcome
description: EducationOutcome, который дает числовую оценку.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a5c35216015038252b52b4f16819d4dabf552ff19faf8f5be0d75bade52122af
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178481"
---
# <a name="educationpointsoutcome-resource-type"></a>тип ресурсов educationPointsOutcome

Пространство имен: microsoft.graph

[EducationOutcome,](educationoutcome.md) который дает числовую оценку.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Обновление educationOutcome](../api/educationoutcome-update.md) | [educationOutcome](educationoutcome.md) | Обновление объекта educationOutcome. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|points|[educationAssignmentPointsGrade](educationassignmentpointsgrade.md)|Числовая оценка, предоставленная преподавателем для этого задания.|
|publishedPoints|[educationAssignmentPointsGrade](educationassignmentpointsgrade.md)|Копия свойства точек, которое будет сделано после выпуска класса для учащегося.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPointsOutcome",
  "keyProperty": "id"
}-->

```json
{
  "points": {"@odata.type": "microsoft.graph.educationAssignmentPointsGrade"},
  "publishedPoints": {"@odata.type": "microsoft.graph.educationAssignmentPointsGrade"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationPointsOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

