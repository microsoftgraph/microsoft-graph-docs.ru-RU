---
title: Тип ресурса Усерфидбакк
description: Тип Усерфидбакк.
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 63cfdedd0b8902426e86aa1943cbeead669f92b3
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353801"
---
# <a name="userfeedback-resource-type"></a><span data-ttu-id="f240c-103">Тип ресурса Усерфидбакк</span><span class="sxs-lookup"><span data-stu-id="f240c-103">userFeedback resource type</span></span>

<span data-ttu-id="f240c-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="f240c-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f240c-105">Представляет обратную связь, предоставленную пользователем конечной точкой относительно качества сеанса.</span><span class="sxs-lookup"><span data-stu-id="f240c-105">Represents the feedback provided by the user an endpoint about the quality of the session.</span></span>

## <a name="properties"></a><span data-ttu-id="f240c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f240c-106">Properties</span></span>

| <span data-ttu-id="f240c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f240c-107">Property</span></span>     | <span data-ttu-id="f240c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f240c-108">Type</span></span>        | <span data-ttu-id="f240c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f240c-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f240c-110">расчета</span><span class="sxs-lookup"><span data-stu-id="f240c-110">rating</span></span>|<span data-ttu-id="f240c-111">Microsoft. Graph. Каллрекордс. Усерфидбаккратинг</span><span class="sxs-lookup"><span data-stu-id="f240c-111">microsoft.graph.callRecords.userFeedbackRating</span></span>|<span data-ttu-id="f240c-112">Оценка, предоставленная пользователем этой конечной точки относительно качества этого сеанса.</span><span class="sxs-lookup"><span data-stu-id="f240c-112">The rating provided by the user of this endpoint about the quality of this Session.</span></span> <span data-ttu-id="f240c-113">Возможные значения: `notRated`, `bad`, `poor`, `fair`, `good`, `excellent`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f240c-113">Possible values are: `notRated`, `bad`, `poor`, `fair`, `good`, `excellent`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="f240c-114">текст</span><span class="sxs-lookup"><span data-stu-id="f240c-114">text</span></span>|<span data-ttu-id="f240c-115">String</span><span class="sxs-lookup"><span data-stu-id="f240c-115">String</span></span>|<span data-ttu-id="f240c-116">Текст отзыва, предоставленный пользователем этой конечной точки для сеанса.</span><span class="sxs-lookup"><span data-stu-id="f240c-116">The feedback text provided by the user of this endpoint for the session.</span></span>|
|<span data-ttu-id="f240c-117">обнаружения</span><span class="sxs-lookup"><span data-stu-id="f240c-117">tokens</span></span>|[<span data-ttu-id="f240c-118">Microsoft. Graph. Каллрекордс. Фидбакктокенсет</span><span class="sxs-lookup"><span data-stu-id="f240c-118">microsoft.graph.callRecords.feedbackTokenSet</span></span>](callrecords-feedbacktokenset.md)|<span data-ttu-id="f240c-119">Набор маркеров отзывов, предоставленных пользователем данной конечной точки для сеанса.</span><span class="sxs-lookup"><span data-stu-id="f240c-119">The set of feedback tokens provided by the user of this endpoint for the session.</span></span> <span data-ttu-id="f240c-120">Это набор логических свойств.</span><span class="sxs-lookup"><span data-stu-id="f240c-120">This is a set of Boolean properties.</span></span> <span data-ttu-id="f240c-121">Не следует полагаться на имена свойств, так как они могут изменяться в зависимости от того, какие маркеры предлагаются пользователю.</span><span class="sxs-lookup"><span data-stu-id="f240c-121">The property names should not be relied upon since they may change depending on what tokens are offered to the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f240c-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f240c-122">JSON representation</span></span>

<span data-ttu-id="f240c-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f240c-123">The following is a JSON representation of the resource.</span></span>

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