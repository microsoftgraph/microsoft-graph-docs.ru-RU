---
title: Тип ресурса Фидбакктокенсет
description: Тип Фидбакктокенсет
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e3f4b0f58fbe2fcd9a920181ccbfca0c5a8c8dad
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394852"
---
# <a name="feedbacktokenset-resource-type"></a>Тип ресурса Фидбакктокенсет

Пространство имен: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Это _открытый тип_ , представляющий набор маркеров отзывов, предоставленных пользователем данной конечной точки для сеанса. Это набор логических свойств. Не следует полагаться на имена свойств, так как они могут изменяться в зависимости от того, какие маркеры предлагаются пользователю.

## <a name="properties"></a>Свойства

Явные имена свойств не задокументированы, так как имена маркеров отзывов могут изменяться, поэтому это [открытый тип](https://docs.microsoft.com/aspnet/web-api/overview/odata-support-in-aspnet-web-api/odata-v4/use-open-types-in-odata-v4).

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