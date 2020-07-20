---
title: Тип ресурса Фидбакктокенсет
description: Тип Фидбакктокенсет
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 307a50c7a29be3857ec1b6b2addf2fafe2189323
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44492050"
---
# <a name="feedbacktokenset-resource-type"></a><span data-ttu-id="d64cf-103">Тип ресурса Фидбакктокенсет</span><span class="sxs-lookup"><span data-stu-id="d64cf-103">feedbackTokenSet resource type</span></span>

<span data-ttu-id="d64cf-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="d64cf-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="d64cf-105">Это _открытый тип_ , представляющий набор маркеров отзывов, предоставленных пользователем данной конечной точки для сеанса.</span><span class="sxs-lookup"><span data-stu-id="d64cf-105">This is an _open type_ that represents the set of feedback tokens provided by the user of this endpoint for the Session.</span></span> <span data-ttu-id="d64cf-106">Это набор логических свойств.</span><span class="sxs-lookup"><span data-stu-id="d64cf-106">This is a set of Boolean properties.</span></span> <span data-ttu-id="d64cf-107">Не следует полагаться на имена свойств, так как они могут изменяться в зависимости от того, какие маркеры предлагаются пользователю.</span><span class="sxs-lookup"><span data-stu-id="d64cf-107">The property names should not be relied upon since they may change depending on what tokens are offered to the user.</span></span>

## <a name="properties"></a><span data-ttu-id="d64cf-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d64cf-108">Properties</span></span>

<span data-ttu-id="d64cf-109">Явные имена свойств не задокументированы, так как имена маркеров отзывов могут изменяться, поэтому это [открытый тип](https://docs.microsoft.com/aspnet/web-api/overview/odata-support-in-aspnet-web-api/odata-v4/use-open-types-in-odata-v4).</span><span class="sxs-lookup"><span data-stu-id="d64cf-109">Explicit property names will not be documented since the feedback token names can change, hence this is an [open type](https://docs.microsoft.com/aspnet/web-api/overview/odata-support-in-aspnet-web-api/odata-v4/use-open-types-in-odata-v4).</span></span>

## <a name="json-representation"></a><span data-ttu-id="d64cf-110">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d64cf-110">JSON representation</span></span>

<span data-ttu-id="d64cf-111">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d64cf-111">The following is a JSON representation of the resource.</span></span>

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