---
title: Тип ресурса Буккетаггрегатиондефинитион
description: Предоставляет подробные сведения о том, как должны создаваться агрегатионс в результатах.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1f9fdadefc43b99b8772217db9a9b101357a1c9c
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193985"
---
# <a name="bucketaggregationdefinition-resource-type"></a><span data-ttu-id="cd911-103">Тип ресурса Буккетаггрегатиондефинитион</span><span class="sxs-lookup"><span data-stu-id="cd911-103">bucketAggregationDefinition resource type</span></span>

<span data-ttu-id="cd911-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd911-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd911-105">Задает сведения для агрегирования результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="cd911-105">Specifies details to aggregate search results.</span></span>

## <a name="properties"></a><span data-ttu-id="cd911-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd911-106">Properties</span></span>

| <span data-ttu-id="cd911-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd911-107">Property</span></span>     | <span data-ttu-id="cd911-108">Тип</span><span class="sxs-lookup"><span data-stu-id="cd911-108">Type</span></span>        | <span data-ttu-id="cd911-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cd911-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cd911-110">sortBy</span><span class="sxs-lookup"><span data-stu-id="cd911-110">sortBy</span></span>|<span data-ttu-id="cd911-111">буккетаггрегатионсортпроперти</span><span class="sxs-lookup"><span data-stu-id="cd911-111">bucketAggregationSortProperty</span></span>| <span data-ttu-id="cd911-112">Возможные значения: `count` Сортировать по количеству совпадений в агрегате, чтобы отсортировать их по алфавиту в соответствии с ключом в агрегате `keyAsString` , `keyAsNumber` для числовой сортировки на основе ключа в агрегате.</span><span class="sxs-lookup"><span data-stu-id="cd911-112">The possible values are `count` to sort by the number of matches in the aggregation, `keyAsString`to sort alphabeticaly based on the key in the aggregation, `keyAsNumber` for numerical sorting based on the key in the aggregation.</span></span> <span data-ttu-id="cd911-113">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="cd911-113">Required.</span></span>
|<span data-ttu-id="cd911-114">по убыванию</span><span class="sxs-lookup"><span data-stu-id="cd911-114">isDescending</span></span>|<span data-ttu-id="cd911-115">Логическое</span><span class="sxs-lookup"><span data-stu-id="cd911-115">Boolean</span></span>|<span data-ttu-id="cd911-116">`True` , чтобы указать порядок сортировки по убыванию.</span><span class="sxs-lookup"><span data-stu-id="cd911-116">`True` to specify the sort order as descending.</span></span> <span data-ttu-id="cd911-117">По умолчанию используется `false` порядок сортировки по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="cd911-117">The default is `false`, with the sort order as ascending.</span></span> <span data-ttu-id="cd911-118">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="cd911-118">Optional.</span></span>|
|<span data-ttu-id="cd911-119">префиксфилтер</span><span class="sxs-lookup"><span data-stu-id="cd911-119">prefixFilter</span></span>|<span data-ttu-id="cd911-120">String</span><span class="sxs-lookup"><span data-stu-id="cd911-120">String</span></span>|<span data-ttu-id="cd911-121">Фильтр для определения условия соответствия.</span><span class="sxs-lookup"><span data-stu-id="cd911-121">A filter to define a matching criteria.</span></span> <span data-ttu-id="cd911-122">Ключ должен начинаться с указанного префикса, возвращаемого в ответе.</span><span class="sxs-lookup"><span data-stu-id="cd911-122">The key should start with the specified prefix to be returned in the response.</span></span> <span data-ttu-id="cd911-123">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="cd911-123">Optional.</span></span>|
|<span data-ttu-id="cd911-124">минимумкаунт</span><span class="sxs-lookup"><span data-stu-id="cd911-124">minimumCount</span></span>|<span data-ttu-id="cd911-125">Int32</span><span class="sxs-lookup"><span data-stu-id="cd911-125">Int32</span></span>|<span data-ttu-id="cd911-126">Минимальное количество элементов, которые должны присутствовать в агрегате для возврата в сегменте.</span><span class="sxs-lookup"><span data-stu-id="cd911-126">The minimum number of items that should be present in the aggregation to be returned in a bucket.</span></span> <span data-ttu-id="cd911-127">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="cd911-127">Optional.</span></span>|
|<span data-ttu-id="cd911-128">ranges</span><span class="sxs-lookup"><span data-stu-id="cd911-128">ranges</span></span>|<span data-ttu-id="cd911-129">Коллекция [буккетаггрегатионранже](bucketaggregationrange.md)</span><span class="sxs-lookup"><span data-stu-id="cd911-129">[bucketAggregationRange](bucketaggregationrange.md) collection</span></span>|<span data-ttu-id="cd911-130">Задает диапазоны ручных вычислений для вычисления агрегатов.</span><span class="sxs-lookup"><span data-stu-id="cd911-130">Specifies the manual ranges to compute the aggregations.</span></span> <span data-ttu-id="cd911-131">Это допустимо только для уточнений, не являющихся строками даты или числового типа.</span><span class="sxs-lookup"><span data-stu-id="cd911-131">This is only valid for non-string refiners of date or numeric type.</span></span> <span data-ttu-id="cd911-132">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="cd911-132">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd911-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd911-133">JSON representation</span></span>

<span data-ttu-id="cd911-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd911-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bucketAggregationDefinition",
  "baseType": null
}-->

```json
{
  "sortBy": "String",
  "isDescending": true,
  "prefixFilter": "String",
  "minimumCount": 1024,
  "ranges": [{"@odata.type": "microsoft.graph.bucketAggregationRange"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sortProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->