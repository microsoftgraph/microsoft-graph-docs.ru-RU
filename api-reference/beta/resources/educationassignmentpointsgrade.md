---
title: Тип ресурса Едукатионассигнментпоинтсграде
description: Если для назначения задан тип уровня баллов, то каждая отправка будет иметь этот объект, связанный с свойством **отправку. Grade** . При этом создается подкласс из Едукатионассигнментграде,
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c2ef014c3e9e2954dba5fb759fcf3f86b3681b68
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502510"
---
# <a name="educationassignmentpointsgrade-resource-type"></a>Тип ресурса Едукатионассигнментпоинтсграде

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Если для назначения задан тип уровня баллов, то каждая отправка будет иметь этот объект, связанный с свойством **отправку. Grade** . При этом создается подкласс из [едукатионассигнментграде](educationassignmentgrade.md), который добавляет к этому свойству данные. Максимальные точки хранятся в свойстве **назначений. ступенчато** .


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|points|Одинарное|Количество баллов, на которые преподаватель предоставляет этот объект отправки.|

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
