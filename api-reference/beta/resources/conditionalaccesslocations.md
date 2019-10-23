---
title: Тип ресурса Кондитионалакцесслокатионс
description: Представляет расположения, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6997664eb131664bcaaf571398ed393fb13c987c
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638570"
---
# <a name="conditionalaccesslocations-resource-type"></a><span data-ttu-id="7410c-103">Тип ресурса Кондитионалакцесслокатионс</span><span class="sxs-lookup"><span data-stu-id="7410c-103">conditionalAccessLocations resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7410c-104">Представляет расположения, включенные в область политики и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="7410c-104">Represents locations included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="7410c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7410c-105">Properties</span></span>

| <span data-ttu-id="7410c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7410c-106">Property</span></span>     | <span data-ttu-id="7410c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7410c-107">Type</span></span>        | <span data-ttu-id="7410c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7410c-108">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7410c-109">инклуделокатионс</span><span class="sxs-lookup"><span data-stu-id="7410c-109">includeLocations</span></span> | <span data-ttu-id="7410c-110">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7410c-110">String collection</span></span> | <span data-ttu-id="7410c-111">Идентификаторы расположений в области применения политики, если `All`явно не `AllTrusted`исключены, или.</span><span class="sxs-lookup"><span data-stu-id="7410c-111">Location IDs in scope of policy unless explicitly excluded, `All`, or `AllTrusted`.</span></span> |
| <span data-ttu-id="7410c-112">ексклуделокатионс</span><span class="sxs-lookup"><span data-stu-id="7410c-112">excludeLocations</span></span> | <span data-ttu-id="7410c-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7410c-113">String collection</span></span> | <span data-ttu-id="7410c-114">Идентификаторы расположений, исключенные из области применения политики.</span><span class="sxs-lookup"><span data-stu-id="7410c-114">Location IDs excluded from scope of policy.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7410c-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7410c-115">JSON representation</span></span>

<span data-ttu-id="7410c-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7410c-116">The following is a JSON representation of the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="7410c-117">Связи</span><span class="sxs-lookup"><span data-stu-id="7410c-117">Relationships</span></span>

<span data-ttu-id="7410c-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7410c-118">None.</span></span>

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