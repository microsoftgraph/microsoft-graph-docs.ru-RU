---
title: Тип ресурса Кондитионалакцесслокатионс
description: Представляет расположения, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2a6b4175decf2d4985d17b64014b09d9299af06e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021961"
---
# <a name="conditionalaccesslocations-resource-type"></a><span data-ttu-id="a938a-103">Тип ресурса Кондитионалакцесслокатионс</span><span class="sxs-lookup"><span data-stu-id="a938a-103">conditionalAccessLocations resource type</span></span>

<span data-ttu-id="a938a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a938a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a938a-105">Представляет расположения, включенные в область политики и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="a938a-105">Represents locations included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="a938a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a938a-106">Properties</span></span>

| <span data-ttu-id="a938a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a938a-107">Property</span></span>     | <span data-ttu-id="a938a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a938a-108">Type</span></span>        | <span data-ttu-id="a938a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a938a-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a938a-110">инклуделокатионс</span><span class="sxs-lookup"><span data-stu-id="a938a-110">includeLocations</span></span> | <span data-ttu-id="a938a-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a938a-111">String collection</span></span> | <span data-ttu-id="a938a-112">Идентификаторы расположений в области применения политики, если явно не исключены, `All` или `AllTrusted` .</span><span class="sxs-lookup"><span data-stu-id="a938a-112">Location IDs in scope of policy unless explicitly excluded, `All`, or `AllTrusted`.</span></span> |
| <span data-ttu-id="a938a-113">ексклуделокатионс</span><span class="sxs-lookup"><span data-stu-id="a938a-113">excludeLocations</span></span> | <span data-ttu-id="a938a-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a938a-114">String collection</span></span> | <span data-ttu-id="a938a-115">Идентификаторы расположений, исключенные из области применения политики.</span><span class="sxs-lookup"><span data-stu-id="a938a-115">Location IDs excluded from scope of policy.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a938a-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a938a-116">JSON representation</span></span>

<span data-ttu-id="a938a-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a938a-117">The following is a JSON representation of the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="a938a-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="a938a-118">Relationships</span></span>

<span data-ttu-id="a938a-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a938a-119">None.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeLocations",
    "excludeLocations"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessLocations",
  "baseType": null
}-->

```json
{
  "excludeLocations": ["String"],
  "includeLocations": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessLocations resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

