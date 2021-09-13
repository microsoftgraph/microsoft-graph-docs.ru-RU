---
title: rubricQualityFeedbackModel type
description: Обратная связь, связанная с определенным качеством образованияRubric.
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0ca3a8877573751187f251b0a179498c44c0add8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117755"
---
# <a name="rubricqualityfeedbackmodel-resource-type"></a>rubricQualityFeedbackModel type

Пространство имен: microsoft.graph

Отзывы, связанные с [определенным качеством](rubricquality.md) [образованияRubric](educationrubric.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|feedback|[itemBody](itembody.md)|Конкретные отзывы по одному качеству этой рубрики.|
|qualityId|Строка|ID [рубрикQuality,](rubricquality.md) с чем связана эта обратная связь.|

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

