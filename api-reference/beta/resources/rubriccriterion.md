---
title: Тип ресурса Рубриккритерион
description: Критерий Rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 60123251d771d06032077231250efe53b35a787c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016116"
---
# <a name="rubriccriterion-resource-type"></a><span data-ttu-id="26a91-103">Тип ресурса Рубриккритерион</span><span class="sxs-lookup"><span data-stu-id="26a91-103">rubricCriterion resource type</span></span>

<span data-ttu-id="26a91-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26a91-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26a91-105">Критерий Rubric.</span><span class="sxs-lookup"><span data-stu-id="26a91-105">A criterion of a rubric.</span></span> <span data-ttu-id="26a91-106">Описание связи между Rubric *качеством*, *уровнями*и *критериями*можно узнать в разделе [едукатионрубрик](educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="26a91-106">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="26a91-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="26a91-107">Properties</span></span>

| <span data-ttu-id="26a91-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="26a91-108">Property</span></span>     | <span data-ttu-id="26a91-109">Тип</span><span class="sxs-lookup"><span data-stu-id="26a91-109">Type</span></span>        | <span data-ttu-id="26a91-110">Описание</span><span class="sxs-lookup"><span data-stu-id="26a91-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="26a91-111">description</span><span class="sxs-lookup"><span data-stu-id="26a91-111">description</span></span>|[<span data-ttu-id="26a91-112">itemBody</span><span class="sxs-lookup"><span data-stu-id="26a91-112">itemBody</span></span>](itembody.md)|<span data-ttu-id="26a91-113">Описание этого критерия.</span><span class="sxs-lookup"><span data-stu-id="26a91-113">The description of this criterion.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="26a91-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="26a91-114">JSON representation</span></span>

<span data-ttu-id="26a91-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26a91-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricCriterion",
  "baseType": null
}-->

```json
{
  "description": {"@odata.type": "microsoft.graph.itemBody"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricCriterion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

