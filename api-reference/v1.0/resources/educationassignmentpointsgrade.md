---
title: тип ресурса educationAssignmentPointsGrade
description: Когда назначение заданной типу класса точек, каждый отправка будет иметь этот объект, связанный с **свойством submission.grade.**
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 131aad8f86e639c4002fed73a7221bcdc1d828b6e40d7b3e534aff3ef33ca5db
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152749"
---
# <a name="educationassignmentpointsgrade-resource-type"></a>тип ресурса educationAssignmentPointsGrade

Пространство имен: microsoft.graph

Когда назначение заданной типу класса точек, каждый отправка будет иметь этот объект, связанный с **свойством submission.grade.** Это создает подкласс из [educationAssignmentGrade,](educationassignmentgrade.md)который добавит данные who к этому свойству. Максимальные точки хранятся в **свойстве assignments.grading.**


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|points|Одинарное|Количество точек, которые учитель дает этому объекту отправки.|

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


