---
title: тип ресурса educationAssignmentPointsGrade
description: Когда назначение заданной типу класса точек, каждый отправка будет иметь этот объект, связанный с **свойством submission.grade.**
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 91dbdc6a6a94a296dffafe32d6d6021dd23d3371
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109152"
---
# <a name="educationassignmentpointsgrade-resource-type"></a>тип ресурса educationAssignmentPointsGrade

Пространство имен: microsoft.graph

Когда назначение заданной типу класса точек, каждый отправка будет иметь этот объект, связанный с **свойством submission.grade.** Это создает подкласс из [educationAssignmentGrade,](educationassignmentgrade.md)который добавит данные who к этому свойству. Максимальные точки хранятся в **свойстве assignments.grading.**


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|points|Один|Количество точек, которые учитель дает этому объекту отправки.|

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
  "points": "Double"
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


