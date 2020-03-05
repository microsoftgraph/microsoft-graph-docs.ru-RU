---
title: Тип ресурса Едукатионфидбаккауткоме
description: Объект Едукатионауткоме, который дает отзыв в виде текста.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 3dd9dd01c19306d66ac91578a5430ff26667b0e3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502132"
---
# <a name="educationfeedbackoutcome-resource-type"></a>Тип ресурса Едукатионфидбаккауткоме

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет обратную связь для объекта [едукатионауткоме](educationoutcome.md) в виде текста. 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Обновление Едукатионауткоме](../api/educationoutcome-update.md) | [едукатионауткоме](educationoutcome.md) | Обновление объекта Едукатионауткоме. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|feedback|[едукатионфидбакк](educationfeedback.md)|Письменный отзыв учащегося.|
|публишедфидбакк|[едукатионфидбакк](educationfeedback.md)|Копия свойства обратной связи, выполняемого при отпадении оценки на учащийся.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedbackOutcome",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "feedback": {"@odata.type": "microsoft.graph.educationFeedback"},
  "publishedFeedback": {"@odata.type": "microsoft.graph.educationFeedback"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationFeedbackOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->