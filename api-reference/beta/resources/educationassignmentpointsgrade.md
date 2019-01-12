---
title: Тип ресурса educationAssignmentPointsGrade
description: Если тип марки точек назначения, каждой отправки будут иметь этот объект, связанный со свойством **submission.grade** . Это создаст подкласс из educationAssignmentGrade,
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: d96b84380bc7a6d2298117b5dfeaee25d943efb2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982388"
---
# <a name="educationassignmentpointsgrade-resource-type"></a>Тип ресурса educationAssignmentPointsGrade

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Если тип марки точек назначения, каждой отправки будут иметь этот объект, связанный со свойством **submission.grade** . Это создаст подкласс из [educationAssignmentGrade](educationassignmentgrade.md), который добавит who данных этого свойства. Max точек хранится в свойстве **assignments.grading** .


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|points|Single|Число точек a учитель передается объект отправки.|

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
  "points": "Single"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
