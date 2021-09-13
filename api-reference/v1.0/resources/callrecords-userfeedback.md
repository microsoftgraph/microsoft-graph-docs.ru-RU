---
title: тип ресурса userFeedback
description: Тип userFeedback.
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 830b279c4021ec08677a4a5ebaf637bc73b7beaf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084666"
---
# <a name="userfeedback-resource-type"></a>тип ресурса userFeedback

Пространство имен: microsoft.graph.callRecords

Представляет обратную связь, предоставляемую пользователем, конечную точку о качестве сеанса.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|оценка|microsoft.graph.callRecords.userFeedbackRating|Оценка, предоставляемая пользователем этой конечной точки, о качестве этого сеанса. Возможные значения: `notRated`, `bad`, `poor`, `fair`, `good`, `excellent`, `unknownFutureValue`.|
|текст|Строка|Текст обратной связи, предоставленный пользователем этой конечной точки для сеанса.|
|маркеры|[microsoft.graph.callRecords.feedbackTokenSet](callrecords-feedbacktokenset.md)|Набор маркеров обратной связи, предоставленных пользователем этой конечной точки для сеанса. Это набор свойств Boolean. Имена свойств не следует использовать, так как они могут изменяться в зависимости от того, какие маркеры предлагаются пользователю.|

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
