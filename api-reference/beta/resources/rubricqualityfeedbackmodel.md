---
title: Тип ресурса Рубриккуалитифидбаккмодел
description: Обратная связь, связанная с определенным качеством Едукатионрубрик
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 56fea149446c79dd95e50e1b5d152cc8610dc0dd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016067"
---
# <a name="rubricqualityfeedbackmodel-resource-type"></a>Тип ресурса Рубриккуалитифидбаккмодел

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обратная связь, связанная с определенным [качеством](rubricquality.md) [едукатионрубрик](educationrubric.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|feedback|[itemBody](itembody.md)|Особая обратная связь для одного качества этого Rubric.|
|куалитид|String|Идентификатор [рубриккуалити](rubricquality.md) , с которым связана эта обратная связь.|

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

