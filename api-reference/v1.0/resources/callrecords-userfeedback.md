---
title: тип ресурса userFeedback
description: Тип userFeedback.
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4f38484219f33432aa5f4c215869c5f6df33aba133d38bcc79ce4f52a28eb2c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180889"
---
# <a name="userfeedback-resource-type"></a>тип ресурса userFeedback

Пространство имен: microsoft.graph.callRecords

Представляет обратную связь, предоставляемую пользователем, конечную точку о качестве сеанса.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|оценка|microsoft.graph.callRecords.userFeedbackRating|Оценка, предоставляемая пользователем этой конечной точки, о качестве этого сеанса. Возможные значения: `notRated`, `bad`, `poor`, `fair`, `good`, `excellent`, `unknownFutureValue`.|
|текст|String|Текст обратной связи, предоставленный пользователем этой конечной точки для сеанса.|
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
