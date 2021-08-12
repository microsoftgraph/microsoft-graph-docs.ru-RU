---
title: тип ресурса feedbackTokenSet
description: Тип feedbackTokenSet
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 054b77c64f61bd100db45ce6ed83772fd6e1fd2c0d502a4e6f578058ec8f097f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205936"
---
# <a name="feedbacktokenset-resource-type"></a>тип ресурса feedbackTokenSet

Пространство имен: microsoft.graph.callRecords

Это _открытый тип,_ который представляет набор маркеров обратной связи, предоставляемых пользователем этой конечной точки для сеанса. Это набор свойств Boolean. Имена свойств не следует использовать, так как они могут изменяться в зависимости от того, какие маркеры предлагаются пользователю.

## <a name="properties"></a>Свойства

Явные имена свойств не будут задокументированы, так как имена маркеров обратной связи могут изменяться, поэтому это [открытый тип.](/aspnet/web-api/overview/odata-support-in-aspnet-web-api/odata-v4/use-open-types-in-odata-v4)

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