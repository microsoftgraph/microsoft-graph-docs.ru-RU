---
title: Тип ресурса Едукатионфидбакк
description: Обратная связь преподавателя с студентом. Это свойство представляет текстовую часть обратной связи вместе с тем, кто.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 7300c5f2d46a3a60a104288d8ee9559e6cf5fd2c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006418"
---
# <a name="educationfeedback-resource-type"></a>Тип ресурса Едукатионфидбакк

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обратная связь преподавателя с студентом. Это свойство представляет текстовую часть обратной связи вместе с тем, кто.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Фидбаккби|[identitySet](identityset.md)|Пользователь, создавший отзыв.|
|Фидбаккдатетиме|DateTimeOffset|Момент времени, когда была выдана обратная связь. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|текст|[itemBody](itembody.md)|Замечания.|

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
