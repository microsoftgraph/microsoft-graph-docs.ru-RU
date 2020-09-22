---
title: Тип ресурса Сеарчаггрегатион
description: Предоставляет сведения о агрегате поиска в ответе поиска.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 480a6f70a2815a174697ff22fc217057053e1f4b
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193964"
---
# <a name="searchaggregation-resource-type"></a><span data-ttu-id="0f4e6-103">Тип ресурса Сеарчаггрегатион</span><span class="sxs-lookup"><span data-stu-id="0f4e6-103">searchAggregation resource type</span></span>

<span data-ttu-id="0f4e6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f4e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f4e6-105">Предоставляет сведения о агрегате поиска в ответе поиска.</span><span class="sxs-lookup"><span data-stu-id="0f4e6-105">Provides the details of the search aggregation in the search response.</span></span>

## <a name="properties"></a><span data-ttu-id="0f4e6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f4e6-106">Properties</span></span>

| <span data-ttu-id="0f4e6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f4e6-107">Property</span></span>     | <span data-ttu-id="0f4e6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0f4e6-108">Type</span></span>        | <span data-ttu-id="0f4e6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0f4e6-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0f4e6-110">displayName</span><span class="sxs-lookup"><span data-stu-id="0f4e6-110">displayName</span></span>|<span data-ttu-id="0f4e6-111">String</span><span class="sxs-lookup"><span data-stu-id="0f4e6-111">String</span></span>| <span data-ttu-id="0f4e6-112">Понятное имя объединения.</span><span class="sxs-lookup"><span data-stu-id="0f4e6-112">The friendly name of the aggregation.</span></span> <span data-ttu-id="0f4e6-113">Это значение было указано во входных данных.</span><span class="sxs-lookup"><span data-stu-id="0f4e6-113">This value was provided in the input.</span></span>|
|<span data-ttu-id="0f4e6-114">поле</span><span class="sxs-lookup"><span data-stu-id="0f4e6-114">field</span></span>|<span data-ttu-id="0f4e6-115">String</span><span class="sxs-lookup"><span data-stu-id="0f4e6-115">String</span></span>| <span data-ttu-id="0f4e6-116">Определяет, для какого поля вычислена агрегация.</span><span class="sxs-lookup"><span data-stu-id="0f4e6-116">Defines on which field the aggregation was computed on.</span></span>|
|<span data-ttu-id="0f4e6-117">buckets</span><span class="sxs-lookup"><span data-stu-id="0f4e6-117">buckets</span></span>|<span data-ttu-id="0f4e6-118">Коллекция [сеарчбуккет](searchbucket.md)</span><span class="sxs-lookup"><span data-stu-id="0f4e6-118">[searchBucket](searchbucket.md) collection</span></span>| <span data-ttu-id="0f4e6-119">Определяет фактические сегменты вычисленной статистической обработки.</span><span class="sxs-lookup"><span data-stu-id="0f4e6-119">Defines the actual buckets of the computed aggregation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f4e6-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f4e6-120">JSON representation</span></span>

<span data-ttu-id="0f4e6-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f4e6-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchAggregation",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "field": "String",  
  "buckets": [{"@odata.type": "microsoft.graph.searchBucket"}]
}
```