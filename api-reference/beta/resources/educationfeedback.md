---
title: Тип ресурса educationFeedback
description: Отзывы учитель студента. Это свойство представляет часть текста обратной связи, а также who.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 0d08f3bc5c7b4882693cdcbba41b364734c6ccef
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873565"
---
# <a name="educationfeedback-resource-type"></a>Тип ресурса educationFeedback

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Отзывы учитель студента. Это свойство представляет часть текста обратной связи, а также who.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|feedbackBy|[identitySet](identityset.md)|Пользователь, создавший свои отзывы и предложения.|
|feedbackDateTime|DateTimeOffset|Момент времени, когда был задан свои отзывы и предложения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|text|[itemBody](itembody.md)|Обратная связь.|

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
  "feedbackDateTime": "String (timestamp)",
  "text": {"@odata.type": "microsoft.graph.itemBody"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationFeedback resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
