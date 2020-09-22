---
title: Тип ресурса Едукатионпоинтсауткоме
description: Объект Едукатионауткоме, который дает числовой уровень
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: eb8c95fa7d13f57cca2c2fe19d7b992e6e2cab98
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049753"
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

