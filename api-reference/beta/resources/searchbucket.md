---
title: Тип ресурса Сеарчбуккет
description: Предоставляет определенную статистическую функцию в отклике, значение определенного сегмента.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3fe375ca2e9695a237b60e30cdd9e98a9e545d35
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193960"
---
# <a name="searchbucket-resource-type"></a><span data-ttu-id="affb0-103">Тип ресурса Сеарчбуккет</span><span class="sxs-lookup"><span data-stu-id="affb0-103">searchBucket resource type</span></span>

<span data-ttu-id="affb0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="affb0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="affb0-105">Представляет контейнер для одного или нескольких результатов поиска, которые имеют одно и то же значение для поля сущности, в котором они объединены.</span><span class="sxs-lookup"><span data-stu-id="affb0-105">Represents a container for one or more search results that share the same value for the entity field that aggregates them.</span></span> 



## <a name="properties"></a><span data-ttu-id="affb0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="affb0-106">Properties</span></span>

| <span data-ttu-id="affb0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="affb0-107">Property</span></span>     | <span data-ttu-id="affb0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="affb0-108">Type</span></span>        | <span data-ttu-id="affb0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="affb0-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="affb0-110">key</span><span class="sxs-lookup"><span data-stu-id="affb0-110">key</span></span>|<span data-ttu-id="affb0-111">String</span><span class="sxs-lookup"><span data-stu-id="affb0-111">String</span></span>| <span data-ttu-id="affb0-112">Дискретное значение поля, для которого рассчитано агрегирование.</span><span class="sxs-lookup"><span data-stu-id="affb0-112">The discrete value of the field that an aggregation was computed on.</span></span>|
|<span data-ttu-id="affb0-113">count</span><span class="sxs-lookup"><span data-stu-id="affb0-113">count</span></span>|<span data-ttu-id="affb0-114">Int32</span><span class="sxs-lookup"><span data-stu-id="affb0-114">Int32</span></span>| <span data-ttu-id="affb0-115">Количество совпадений поиска, имеющих одно и то же значение, указанное в свойстве **Key** .</span><span class="sxs-lookup"><span data-stu-id="affb0-115">The number of search matches that share the same value specified in the **key** property.</span></span> |
|<span data-ttu-id="affb0-116">аггрегатионфилтертокен</span><span class="sxs-lookup"><span data-stu-id="affb0-116">aggregationFilterToken</span></span>|<span data-ttu-id="affb0-117">String</span><span class="sxs-lookup"><span data-stu-id="affb0-117">String</span></span>| <span data-ttu-id="affb0-118">Маркер, содержащий закодированный фильтр для объединения результатов поиска по определенному значению **ключа** .</span><span class="sxs-lookup"><span data-stu-id="affb0-118">A token containing the encoded filter to aggregate search matches by the specific **key** value.</span></span> <span data-ttu-id="affb0-119">Чтобы использовать фильтр, передайте маркер в качестве части свойства **аггрегатионфилтер** объекта **сеарчрекуест** в формате **"{Field}: \\ " {аггрегатионфилтертокен} \\ ""**.</span><span class="sxs-lookup"><span data-stu-id="affb0-119">To use the filter, pass the token as part of the **aggregationFilter** property in a **searchRequest** object, in the format **"{field}:\\"{aggregationFilterToken}\\""**.</span></span> <span data-ttu-id="affb0-120">См. [пример](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request).</span><span class="sxs-lookup"><span data-stu-id="affb0-120">See an [example](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="affb0-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="affb0-121">JSON representation</span></span>

<span data-ttu-id="affb0-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="affb0-122">The following is a JSON representation of the resource.</span></span>

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
