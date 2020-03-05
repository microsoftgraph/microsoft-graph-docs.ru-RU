---
title: Тип ресурса Рубриккритерион
description: Критерий Rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e1a2a0550a7e1f9f5865b8381b3f730d31cac6b6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521021"
---
# <a name="rubriccriterion-resource-type"></a><span data-ttu-id="e2e2c-103">Тип ресурса Рубриккритерион</span><span class="sxs-lookup"><span data-stu-id="e2e2c-103">rubricCriterion resource type</span></span>

<span data-ttu-id="e2e2c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e2e2c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2e2c-105">Критерий Rubric.</span><span class="sxs-lookup"><span data-stu-id="e2e2c-105">A criterion of a rubric.</span></span> <span data-ttu-id="e2e2c-106">Описание связи между Rubric *качеством*, *уровнями*и *критериями*можно узнать в разделе [едукатионрубрик](educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="e2e2c-106">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="e2e2c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e2e2c-107">Properties</span></span>

| <span data-ttu-id="e2e2c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2e2c-108">Property</span></span>     | <span data-ttu-id="e2e2c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e2e2c-109">Type</span></span>        | <span data-ttu-id="e2e2c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e2e2c-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e2e2c-111">description</span><span class="sxs-lookup"><span data-stu-id="e2e2c-111">description</span></span>|[<span data-ttu-id="e2e2c-112">itemBody</span><span class="sxs-lookup"><span data-stu-id="e2e2c-112">itemBody</span></span>](itembody.md)|<span data-ttu-id="e2e2c-113">Описание этого критерия.</span><span class="sxs-lookup"><span data-stu-id="e2e2c-113">The description of this criterion.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2e2c-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e2e2c-114">JSON representation</span></span>

<span data-ttu-id="e2e2c-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2e2c-115">The following is a JSON representation of the resource.</span></span>

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