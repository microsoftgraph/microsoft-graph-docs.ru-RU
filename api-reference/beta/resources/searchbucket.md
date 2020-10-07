---
title: Тип ресурса Сеарчбуккет
description: Предоставляет определенную статистическую функцию в отклике, значение определенного сегмента.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a6b26c01133f519b0308ffee430d85c9df6d868b
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373855"
---
# <a name="searchbucket-resource-type"></a><span data-ttu-id="c47c5-103">Тип ресурса Сеарчбуккет</span><span class="sxs-lookup"><span data-stu-id="c47c5-103">searchBucket resource type</span></span>

<span data-ttu-id="c47c5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c47c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c47c5-105">Представляет контейнер для одного или нескольких результатов поиска, которые имеют одно и то же значение для поля сущности, в котором они объединены.</span><span class="sxs-lookup"><span data-stu-id="c47c5-105">Represents a container for one or more search results that share the same value for the entity field that aggregates them.</span></span> 

## <a name="properties"></a><span data-ttu-id="c47c5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c47c5-106">Properties</span></span>

| <span data-ttu-id="c47c5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c47c5-107">Property</span></span>     | <span data-ttu-id="c47c5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c47c5-108">Type</span></span>        | <span data-ttu-id="c47c5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c47c5-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c47c5-110">key</span><span class="sxs-lookup"><span data-stu-id="c47c5-110">key</span></span>|<span data-ttu-id="c47c5-111">String</span><span class="sxs-lookup"><span data-stu-id="c47c5-111">String</span></span>| <span data-ttu-id="c47c5-112">Дискретное значение поля, для которого рассчитано агрегирование.</span><span class="sxs-lookup"><span data-stu-id="c47c5-112">The discrete value of the field that an aggregation was computed on.</span></span>|
|<span data-ttu-id="c47c5-113">count</span><span class="sxs-lookup"><span data-stu-id="c47c5-113">count</span></span>|<span data-ttu-id="c47c5-114">Int32</span><span class="sxs-lookup"><span data-stu-id="c47c5-114">Int32</span></span>| <span data-ttu-id="c47c5-115">Приблизительное количество совпадений поиска с одинаковым значением, указанным в свойстве **Key** .</span><span class="sxs-lookup"><span data-stu-id="c47c5-115">The approximate number of search matches that share the same value specified in the **key** property.</span></span> <span data-ttu-id="c47c5-116">Обратите внимание, что это число не является точным числом совпадений.</span><span class="sxs-lookup"><span data-stu-id="c47c5-116">Note that this number is not the exact number of matches.</span></span>|
|<span data-ttu-id="c47c5-117">аггрегатионфилтертокен</span><span class="sxs-lookup"><span data-stu-id="c47c5-117">aggregationFilterToken</span></span>|<span data-ttu-id="c47c5-118">String</span><span class="sxs-lookup"><span data-stu-id="c47c5-118">String</span></span>| <span data-ttu-id="c47c5-119">Маркер, содержащий закодированный фильтр для объединения результатов поиска по определенному значению **ключа** .</span><span class="sxs-lookup"><span data-stu-id="c47c5-119">A token containing the encoded filter to aggregate search matches by the specific **key** value.</span></span> <span data-ttu-id="c47c5-120">Чтобы использовать фильтр, передайте маркер в качестве части свойства **аггрегатионфилтер** объекта **сеарчрекуест** в формате **"{Field}: \\ " {аггрегатионфилтертокен} \\ ""**.</span><span class="sxs-lookup"><span data-stu-id="c47c5-120">To use the filter, pass the token as part of the **aggregationFilter** property in a **searchRequest** object, in the format **"{field}:\\"{aggregationFilterToken}\\""**.</span></span> <span data-ttu-id="c47c5-121">См. [пример](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request).</span><span class="sxs-lookup"><span data-stu-id="c47c5-121">See an [example](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c47c5-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c47c5-122">JSON representation</span></span>

<span data-ttu-id="c47c5-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c47c5-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchBucket",
  "baseType": null
}-->

```json
{
  "key": "String",
  "count": "10",  
  "aggregationFilterToken": "String"
}
```
