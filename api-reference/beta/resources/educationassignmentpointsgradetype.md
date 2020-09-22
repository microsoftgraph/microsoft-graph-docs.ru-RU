---
title: Тип ресурса Едукатионассигнментпоинтсградетипе
description: Используется с свойством **назначений. ступенчато** . Это подкласс Едукатионассигнментградетипе.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b11ba94bba2147e2ef1d084a66cd7628371a57fa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998890"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a>Тип ресурса Едукатионассигнментпоинтсградетипе

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется с свойством **назначений. ступенчато** . Это подкласс [едукатионассигнментградетипе](educationassignmentgradetype.md).

Это означает, что назначение обладает повышенными уровнями и сохраняет максимальное число баллов, которое каждый учащийся может выполнить для этого рабочего элемента. Если этот параметр задан для назначения, при каждой отправке будет получено свойство [едукатионассигнментпоинтсграде](educationassignmentpointsgrade.md) , связанное с ним для хранения точек каждого учащегося.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|макспоинтс|Одинарное| Максимальное число баллов, которое можно сделать для этого назначения.  |

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


