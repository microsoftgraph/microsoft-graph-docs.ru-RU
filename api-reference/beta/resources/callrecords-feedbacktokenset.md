---
title: Тип ресурса Фидбакктокенсет
description: Тип Фидбакктокенсет
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cbf09c70e1df854f1ccba8cb4f8a5fa61c0c24aa
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405612"
---
# <a name="feedbacktokenset-resource-type"></a><span data-ttu-id="59e62-103">Тип ресурса Фидбакктокенсет</span><span class="sxs-lookup"><span data-stu-id="59e62-103">feedbackTokenSet resource type</span></span>

<span data-ttu-id="59e62-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="59e62-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59e62-105">Это _открытый тип_ , представляющий набор маркеров отзывов, предоставленных пользователем данной конечной точки для сеанса.</span><span class="sxs-lookup"><span data-stu-id="59e62-105">This is an _open type_ that represents the set of feedback tokens provided by the user of this endpoint for the Session.</span></span> <span data-ttu-id="59e62-106">Это набор логических свойств.</span><span class="sxs-lookup"><span data-stu-id="59e62-106">This is a set of Boolean properties.</span></span> <span data-ttu-id="59e62-107">Не следует полагаться на имена свойств, так как они могут изменяться в зависимости от того, какие маркеры предлагаются пользователю.</span><span class="sxs-lookup"><span data-stu-id="59e62-107">The property names should not be relied upon since they may change depending on what tokens are offered to the user.</span></span>

## <a name="properties"></a><span data-ttu-id="59e62-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="59e62-108">Properties</span></span>

<span data-ttu-id="59e62-109">Явные имена свойств не задокументированы, так как имена маркеров отзывов могут изменяться, поэтому это [открытый тип](/aspnet/web-api/overview/odata-support-in-aspnet-web-api/odata-v4/use-open-types-in-odata-v4).</span><span class="sxs-lookup"><span data-stu-id="59e62-109">Explicit property names will not be documented since the feedback token names can change, hence this is an [open type](/aspnet/web-api/overview/odata-support-in-aspnet-web-api/odata-v4/use-open-types-in-odata-v4).</span></span>

## <a name="json-representation"></a><span data-ttu-id="59e62-110">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="59e62-110">JSON representation</span></span>

<span data-ttu-id="59e62-111">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59e62-111">The following is a JSON representation of the resource.</span></span>

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