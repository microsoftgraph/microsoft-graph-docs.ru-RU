---
title: Тип ресурса Едукатионассигнментпоинтсграде
description: Если для назначения задан тип уровня баллов, то каждая отправка будет иметь этот объект, связанный с свойством **отправку. Grade** . При этом создается подкласс из Едукатионассигнментграде,
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6e74c6bb74c830cb1ceb80e149903282c4da33ae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972819"
---
# <a name="educationassignmentpointsgrade-resource-type"></a>Тип ресурса Едукатионассигнментпоинтсграде

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
  "points": "Single"
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
