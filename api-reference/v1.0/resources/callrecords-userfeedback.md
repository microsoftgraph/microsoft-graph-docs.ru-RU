---
title: Тип ресурса Усерфидбакк
description: Тип Усерфидбакк.
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 468f6a58d3e70a37b15c1b18663958ea5193d59a
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44492122"
---
# <a name="userfeedback-resource-type"></a><span data-ttu-id="3b332-103">Тип ресурса Усерфидбакк</span><span class="sxs-lookup"><span data-stu-id="3b332-103">userFeedback resource type</span></span>

<span data-ttu-id="3b332-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="3b332-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="3b332-105">Представляет обратную связь, предоставленную пользователем конечной точкой относительно качества сеанса.</span><span class="sxs-lookup"><span data-stu-id="3b332-105">Represents the feedback provided by the user an endpoint about the quality of the session.</span></span>

## <a name="properties"></a><span data-ttu-id="3b332-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3b332-106">Properties</span></span>

| <span data-ttu-id="3b332-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b332-107">Property</span></span>     | <span data-ttu-id="3b332-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3b332-108">Type</span></span>        | <span data-ttu-id="3b332-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3b332-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3b332-110">расчета</span><span class="sxs-lookup"><span data-stu-id="3b332-110">rating</span></span>|<span data-ttu-id="3b332-111">Microsoft. Graph. Каллрекордс. Усерфидбаккратинг</span><span class="sxs-lookup"><span data-stu-id="3b332-111">microsoft.graph.callRecords.userFeedbackRating</span></span>|<span data-ttu-id="3b332-112">Оценка, предоставленная пользователем этой конечной точки относительно качества этого сеанса.</span><span class="sxs-lookup"><span data-stu-id="3b332-112">The rating provided by the user of this endpoint about the quality of this Session.</span></span> <span data-ttu-id="3b332-113">Возможные значения: `notRated`, `bad`, `poor`, `fair`, `good`, `excellent`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="3b332-113">Possible values are: `notRated`, `bad`, `poor`, `fair`, `good`, `excellent`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="3b332-114">текст</span><span class="sxs-lookup"><span data-stu-id="3b332-114">text</span></span>|<span data-ttu-id="3b332-115">String</span><span class="sxs-lookup"><span data-stu-id="3b332-115">String</span></span>|<span data-ttu-id="3b332-116">Текст отзыва, предоставленный пользователем этой конечной точки для сеанса.</span><span class="sxs-lookup"><span data-stu-id="3b332-116">The feedback text provided by the user of this endpoint for the session.</span></span>|
|<span data-ttu-id="3b332-117">обнаружения</span><span class="sxs-lookup"><span data-stu-id="3b332-117">tokens</span></span>|[<span data-ttu-id="3b332-118">Microsoft. Graph. Каллрекордс. Фидбакктокенсет</span><span class="sxs-lookup"><span data-stu-id="3b332-118">microsoft.graph.callRecords.feedbackTokenSet</span></span>](callrecords-feedbacktokenset.md)|<span data-ttu-id="3b332-119">Набор маркеров отзывов, предоставленных пользователем данной конечной точки для сеанса.</span><span class="sxs-lookup"><span data-stu-id="3b332-119">The set of feedback tokens provided by the user of this endpoint for the session.</span></span> <span data-ttu-id="3b332-120">Это набор логических свойств.</span><span class="sxs-lookup"><span data-stu-id="3b332-120">This is a set of Boolean properties.</span></span> <span data-ttu-id="3b332-121">Не следует полагаться на имена свойств, так как они могут изменяться в зависимости от того, какие маркеры предлагаются пользователю.</span><span class="sxs-lookup"><span data-stu-id="3b332-121">The property names should not be relied upon since they may change depending on what tokens are offered to the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3b332-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3b332-122">JSON representation</span></span>

<span data-ttu-id="3b332-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b332-123">The following is a JSON representation of the resource.</span></span>

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