---
title: Тип ресурса Едукатионпоинтсауткоме
description: Объект Едукатионауткоме, который дает числовой уровень
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 51f57683e06f90e877b4cd72e62d0898d0ef8013
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501432"
---
# <a name="educationpointsoutcome-resource-type"></a>Тип ресурса Едукатионпоинтсауткоме

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Едукатионауткоме](educationoutcome.md) , который предоставляет числовой уровень.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Обновление Едукатионауткоме](../api/educationoutcome-update.md) | [едукатионауткоме](educationoutcome.md) | Обновление объекта Едукатионауткоме. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|points|[едукатионассигнментпоинтсграде](educationassignmentpointsgrade.md)|Числовое значение, которое преподаватель приделил студенту для этого назначения.|
|публишедпоинтс|[едукатионассигнментпоинтсграде](educationassignmentpointsgrade.md)|Копия свойства Points, которое устанавливается при отпадении уровня на учащийся.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPointsOutcome",
  "baseType": "",
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