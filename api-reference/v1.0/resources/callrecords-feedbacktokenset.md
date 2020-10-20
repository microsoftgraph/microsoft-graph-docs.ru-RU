---
title: Тип ресурса Фидбакктокенсет
description: Тип Фидбакктокенсет
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0e978bc25615d3fe0f4f39e0e1c5f50d3d5b2ffb
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601337"
---
# <a name="feedbacktokenset-resource-type"></a>Тип ресурса Фидбакктокенсет

Пространство имен: microsoft.graph.callRecords

Это _открытый тип_ , представляющий набор маркеров отзывов, предоставленных пользователем данной конечной точки для сеанса. Это набор логических свойств. Не следует полагаться на имена свойств, так как они могут изменяться в зависимости от того, какие маркеры предлагаются пользователю.

## <a name="properties"></a>Свойства

Явные имена свойств не задокументированы, так как имена маркеров отзывов могут изменяться, поэтому это [открытый тип](/aspnet/web-api/overview/odata-support-in-aspnet-web-api/odata-v4/use-open-types-in-odata-v4).

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.feedbackTokenSet",
  "baseType": null
}-->

```json
{
  "DistortedSpeech": true,
  "ElectronicFeedback": false,
  "BackgroundNoise": true,
  "MuffledSpeech": true,
  "Echo": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "feedbackTokenSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->