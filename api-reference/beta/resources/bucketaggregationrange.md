---
title: Тип ресурса Буккетаггрегатионранже
description: 'Позволяет указать несколько ручных диапазонов в запросе статистической обработки. Это относится только к уточнениям без строки: числа и даты.'
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 77f89503a8f19bd8b057575643ebf89e6dbc43a8
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193980"
---
# <a name="bucketaggregationrange-resource-type"></a><span data-ttu-id="41250-104">Тип ресурса Буккетаггрегатионранже</span><span class="sxs-lookup"><span data-stu-id="41250-104">bucketAggregationRange resource type</span></span>

<span data-ttu-id="41250-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41250-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41250-106">Задает нижнюю и верхнюю границу диапазона для агрегирования результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="41250-106">Specifies the lower and upper limit to a range for aggregating search results.</span></span> <span data-ttu-id="41250-107">Применяется только к уточнениям даты или числового типа.</span><span class="sxs-lookup"><span data-stu-id="41250-107">Applies to only refiners of the date or numeric type.</span></span>

## <a name="properties"></a><span data-ttu-id="41250-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="41250-108">Properties</span></span>

| <span data-ttu-id="41250-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="41250-109">Property</span></span>     | <span data-ttu-id="41250-110">Тип</span><span class="sxs-lookup"><span data-stu-id="41250-110">Type</span></span>        | <span data-ttu-id="41250-111">Описание</span><span class="sxs-lookup"><span data-stu-id="41250-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="41250-112">from</span><span class="sxs-lookup"><span data-stu-id="41250-112">from</span></span>|<span data-ttu-id="41250-113">String</span><span class="sxs-lookup"><span data-stu-id="41250-113">String</span></span>| <span data-ttu-id="41250-114">Определяет нижнюю границу, от которой вычисляется агрегация.</span><span class="sxs-lookup"><span data-stu-id="41250-114">Defines the lower bound from which to compute the aggregation.</span></span> <span data-ttu-id="41250-115">Это может быть числовое значение или строковое представление даты с использованием `YYYY-MM-DDTHH:mm:ss.sssZ` формата.</span><span class="sxs-lookup"><span data-stu-id="41250-115">This can be a numeric value or a string representation of a date using the `YYYY-MM-DDTHH:mm:ss.sssZ` format.</span></span> <span data-ttu-id="41250-116">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="41250-116">Required.</span></span>|
|<span data-ttu-id="41250-117">на</span><span class="sxs-lookup"><span data-stu-id="41250-117">to</span></span>|<span data-ttu-id="41250-118">String</span><span class="sxs-lookup"><span data-stu-id="41250-118">String</span></span>| <span data-ttu-id="41250-119">Определяет верхнюю границу, до которой вычисляется агрегация.</span><span class="sxs-lookup"><span data-stu-id="41250-119">Defines the upper bound up to which to compute the aggregation.</span></span> <span data-ttu-id="41250-120">Это может быть числовое значение или строковое представление даты с использованием `YYYY-MM-DDTHH:mm:ss.sssZ` формата.</span><span class="sxs-lookup"><span data-stu-id="41250-120">This can be a numeric value or a string representation of a date using the `YYYY-MM-DDTHH:mm:ss.sssZ` format.</span></span> <span data-ttu-id="41250-121">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="41250-121">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="41250-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="41250-122">JSON representation</span></span>

<span data-ttu-id="41250-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41250-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bucketAggregationRange",
  "baseType": null
}-->

```json
{
  "from": "String",
  "to": "String"
}
```
