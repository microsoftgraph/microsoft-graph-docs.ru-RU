---
title: тип ресурса feedbackTokenSet
description: Тип feedbackTokenSet
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2422c0d00e85d1cb6d7d6cf5934d4e498e796013
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59025561"
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
