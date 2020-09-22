---
title: Тип ресурса Аггрегатионоптион
description: Указывает объект Аггрегатионоптион
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c18cc1801e5eac76d2fa4396f809ff68f59a78fe
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193971"
---
# <a name="aggregationoption-resource-type"></a><span data-ttu-id="06c25-103">Тип ресурса Аггрегатионоптион</span><span class="sxs-lookup"><span data-stu-id="06c25-103">aggregationOption resource type</span></span>

<span data-ttu-id="06c25-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06c25-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06c25-105">Указывает, какие статистические выражения должны возвращаться вместе с результатами поиска.</span><span class="sxs-lookup"><span data-stu-id="06c25-105">Specifies which aggregations should be returned alongside the search results.</span></span>

## <a name="properties"></a><span data-ttu-id="06c25-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="06c25-106">Properties</span></span>

| <span data-ttu-id="06c25-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="06c25-107">Property</span></span>     | <span data-ttu-id="06c25-108">Тип</span><span class="sxs-lookup"><span data-stu-id="06c25-108">Type</span></span>        | <span data-ttu-id="06c25-109">Описание</span><span class="sxs-lookup"><span data-stu-id="06c25-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="06c25-110">поле</span><span class="sxs-lookup"><span data-stu-id="06c25-110">field</span></span>|<span data-ttu-id="06c25-111">String</span><span class="sxs-lookup"><span data-stu-id="06c25-111">String</span></span>|<span data-ttu-id="06c25-112">Задает поле в схеме указанного типа сущностей, для которого необходимо вычислить статистическое выражение.</span><span class="sxs-lookup"><span data-stu-id="06c25-112">Specifies the field in the schema of the specified entity type that aggregation should be computed on.</span></span> <span data-ttu-id="06c25-113">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="06c25-113">Required.</span></span>|
|<span data-ttu-id="06c25-114">size</span><span class="sxs-lookup"><span data-stu-id="06c25-114">size</span></span>|<span data-ttu-id="06c25-115">Int32</span><span class="sxs-lookup"><span data-stu-id="06c25-115">Int32</span></span>|<span data-ttu-id="06c25-116">Число возвращаемых ресурсов [сеарчбуккет](searchBucket.md) .</span><span class="sxs-lookup"><span data-stu-id="06c25-116">The number of [searchBucket](searchBucket.md) resources to be returned.</span></span> <span data-ttu-id="06c25-117">Этот параметр не является обязательным, если диапазон предоставляется вручную в запросе поиска.</span><span class="sxs-lookup"><span data-stu-id="06c25-117">This is not required when the range is provided manually in the search request.</span></span> <span data-ttu-id="06c25-118">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="06c25-118">Optional.</span></span>|
|<span data-ttu-id="06c25-119">буккетдефинитион</span><span class="sxs-lookup"><span data-stu-id="06c25-119">bucketDefinition</span></span>|[<span data-ttu-id="06c25-120">буккетаггрегатиондефинитион</span><span class="sxs-lookup"><span data-stu-id="06c25-120">bucketAggregationDefinition</span></span>](bucketaggregationdefinition.md)|<span data-ttu-id="06c25-121">Задает критерии для вычисления агрегата.</span><span class="sxs-lookup"><span data-stu-id="06c25-121">Specifies the criteria to compute an aggregation.</span></span> <span data-ttu-id="06c25-122">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="06c25-122">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06c25-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="06c25-123">JSON representation</span></span>

<span data-ttu-id="06c25-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06c25-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.aggregationOption",
  "baseType": null
}-->

```json
{
  "field": "String",
  "size": 1024,
  "bucketDefinition": {"@odata.type": "microsoft.graph.bucketAggregationDefinition"}
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