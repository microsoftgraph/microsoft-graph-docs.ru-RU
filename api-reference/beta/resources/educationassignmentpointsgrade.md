---
title: Тип ресурса educationAssignmentPointsGrade
description: Если тип марки точек назначения, каждой отправки будут иметь этот объект, связанный со свойством **submission.grade** . Это создаст подкласс из educationAssignmentGrade,
ms.openlocfilehash: 2439ac8946fea588bd7bc1afe7f1ff1042b9179a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076837"
---
# <a name="educationassignmentpointsgrade-resource-type"></a>Тип ресурса educationAssignmentPointsGrade

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Если тип марки точек назначения, каждой отправки будут иметь этот объект, связанный со свойством **submission.grade** . Это создаст подкласс из [educationAssignmentGrade](educationassignmentgrade.md), который добавит who данных этого свойства. Max точек хранится в свойстве **assignments.grading** .


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
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