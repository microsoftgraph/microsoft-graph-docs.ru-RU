---
title: Тип ресурса Усерфидбакк
description: Тип Усерфидбакк.
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5bc315bcb1cd780cb725b2586b8e02e109aa2868
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601505"
---
# <a name="userfeedback-resource-type"></a>Тип ресурса Усерфидбакк

Пространство имен: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет обратную связь, предоставленную пользователем конечной точкой относительно качества сеанса.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|расчета|Microsoft. Graph. Каллрекордс. Усерфидбаккратинг|Оценка, предоставленная пользователем этой конечной точки относительно качества этого сеанса. Возможные значения: `notRated`, `bad`, `poor`, `fair`, `good`, `excellent`, `unknownFutureValue`.|
|текст|String|Текст отзыва, предоставленный пользователем этой конечной точки для сеанса.|
|обнаружения|[Microsoft. Graph. Каллрекордс. Фидбакктокенсет](callrecords-feedbacktokenset.md)|Набор маркеров отзывов, предоставленных пользователем данной конечной точки для сеанса. Это набор логических свойств. Не следует полагаться на имена свойств, так как они могут изменяться в зависимости от того, какие маркеры предлагаются пользователю.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.userFeedback",
  "baseType": null
}-->

```json
{
  "rating": "String",
  "text": "String",
  "tokens": {"@odata.type": "microsoft.graph.callRecords.feedbackTokenSet"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userFeedback resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

