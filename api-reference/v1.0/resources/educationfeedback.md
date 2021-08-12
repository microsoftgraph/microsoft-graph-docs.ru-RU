---
title: тип ресурса educationFeedback
description: Обратная связь от преподавателя к учащемуся.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 87aba918c8766434c3bfc18e3020c2d05517d612887179f04c3bf3a427be1aef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218739"
---
# <a name="educationfeedback-resource-type"></a>тип ресурса educationFeedback

Пространство имен: microsoft.graph

Обратная связь от преподавателя к учащемуся. 

Это свойство представляет как текстовую часть отзывов, так и тех, кто предоставил обратную связь.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|feedbackBy|[identitySet](identityset.md)|Пользователь, создавший отзыв.|
|feedbackDateTime|DateTimeOffset|Момент времени, когда была дана обратная связь. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|текст|[itemBody](itembody.md)|Обратная связь.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedback"
}-->

```json
{
  "feedbackBy": {"@odata.type": "microsoft.graph.identitySet"},
  "feedbackDateTime": "String",
  "text": {"@odata.type": "microsoft.graph.itemBody"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationFeedback resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


