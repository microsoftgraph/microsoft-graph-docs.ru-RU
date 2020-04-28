---
title: Тип ресурса Усерфидбакк
description: Тип Усерфидбакк.
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0ab9c49563bb4715b1736618a939b681178ddae8
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394791"
---
# <a name="userfeedback-resource-type"></a><span data-ttu-id="3d3a8-103">Тип ресурса Усерфидбакк</span><span class="sxs-lookup"><span data-stu-id="3d3a8-103">userFeedback resource type</span></span>

<span data-ttu-id="3d3a8-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="3d3a8-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d3a8-105">Представляет обратную связь, предоставленную пользователем конечной точкой относительно качества сеанса.</span><span class="sxs-lookup"><span data-stu-id="3d3a8-105">Represents the feedback provided by the user an endpoint about the quality of the session.</span></span>

## <a name="properties"></a><span data-ttu-id="3d3a8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3d3a8-106">Properties</span></span>

| <span data-ttu-id="3d3a8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d3a8-107">Property</span></span>     | <span data-ttu-id="3d3a8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3d3a8-108">Type</span></span>        | <span data-ttu-id="3d3a8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3d3a8-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3d3a8-110">расчета</span><span class="sxs-lookup"><span data-stu-id="3d3a8-110">rating</span></span>|<span data-ttu-id="3d3a8-111">String</span><span class="sxs-lookup"><span data-stu-id="3d3a8-111">String</span></span>|<span data-ttu-id="3d3a8-112">Оценка, предоставленная пользователем этой конечной точки относительно качества этого сеанса.</span><span class="sxs-lookup"><span data-stu-id="3d3a8-112">The rating provided by the user of this endpoint about the quality of this Session.</span></span> <span data-ttu-id="3d3a8-113">Возможные значения: `notRated`, `bad`, `poor`, `fair`, `good`, `excellent`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="3d3a8-113">Possible values are: `notRated`, `bad`, `poor`, `fair`, `good`, `excellent`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="3d3a8-114">текст</span><span class="sxs-lookup"><span data-stu-id="3d3a8-114">text</span></span>|<span data-ttu-id="3d3a8-115">String</span><span class="sxs-lookup"><span data-stu-id="3d3a8-115">String</span></span>|<span data-ttu-id="3d3a8-116">Текст отзыва, предоставленный пользователем этой конечной точки для сеанса.</span><span class="sxs-lookup"><span data-stu-id="3d3a8-116">The feedback text provided by the user of this endpoint for the session.</span></span>|
|<span data-ttu-id="3d3a8-117">обнаружения</span><span class="sxs-lookup"><span data-stu-id="3d3a8-117">tokens</span></span>|[<span data-ttu-id="3d3a8-118">Microsoft. Graph. Каллрекордс. Фидбакктокенсет</span><span class="sxs-lookup"><span data-stu-id="3d3a8-118">microsoft.graph.callRecords.feedbackTokenSet</span></span>](callrecords-feedbacktokenset.md)|<span data-ttu-id="3d3a8-119">Набор маркеров отзывов, предоставленных пользователем данной конечной точки для сеанса.</span><span class="sxs-lookup"><span data-stu-id="3d3a8-119">The set of feedback tokens provided by the user of this endpoint for the session.</span></span> <span data-ttu-id="3d3a8-120">Это набор логических свойств.</span><span class="sxs-lookup"><span data-stu-id="3d3a8-120">This is a set of Boolean properties.</span></span> <span data-ttu-id="3d3a8-121">Не следует полагаться на имена свойств, так как они могут изменяться в зависимости от того, какие маркеры предлагаются пользователю.</span><span class="sxs-lookup"><span data-stu-id="3d3a8-121">The property names should not be relied upon since they may change depending on what tokens are offered to the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3d3a8-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3d3a8-122">JSON representation</span></span>

<span data-ttu-id="3d3a8-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d3a8-123">The following is a JSON representation of the resource.</span></span>

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