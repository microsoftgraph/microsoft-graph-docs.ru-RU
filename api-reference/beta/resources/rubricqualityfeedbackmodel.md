---
title: Тип ресурса Рубриккуалитифидбаккмодел
description: Обратная связь, связанная с определенным качеством Едукатионрубрик
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0a7c2b80a2cef18b50157ae9a54c66d35822fa51
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173302"
---
# <a name="rubricqualityfeedbackmodel-resource-type"></a>Тип ресурса Рубриккуалитифидбаккмодел

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обратная связь, связанная с определенным [качеством](rubricquality.md) [едукатионрубрик](educationrubric.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|feedback|[itemBody](itembody.md)|Особая обратная связь для одного качества этого Rubric.|
|Куалитид|String|Идентификатор [рубриккуалити](rubricquality.md) , с которым связана эта обратная связь.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQualityFeedbackModel",
  "baseType": null
}-->

```json
{
  "feedback": {"@odata.type": "microsoft.graph.itemBody"},
  "qualityId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQualityFeedbackModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->