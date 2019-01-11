---
title: Тип ресурса alternativeSecurityId
description: Только для внутреннего использования.
localization_priority: Normal
ms.openlocfilehash: 23ef74085a4a3cc383f0854e9139c9a0b63e3d40
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853804"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="e24ba-103">Тип ресурса alternativeSecurityId</span><span class="sxs-lookup"><span data-stu-id="e24ba-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="e24ba-104">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="e24ba-104">For internal use only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e24ba-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e24ba-105">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.alternativeSecurityId"
}-->

```json
{
  "type": 12345,
  "identityProvider": "string",
  "key": {"@odata.type": "Edm.Binary"}
}
```

## <a name="properties"></a><span data-ttu-id="e24ba-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e24ba-106">Properties</span></span>
| <span data-ttu-id="e24ba-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e24ba-107">Property</span></span>         | <span data-ttu-id="e24ba-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e24ba-108">Type</span></span>       | <span data-ttu-id="e24ba-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e24ba-109">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="e24ba-110">type</span><span class="sxs-lookup"><span data-stu-id="e24ba-110">type</span></span>             | <span data-ttu-id="e24ba-111">Int32</span><span class="sxs-lookup"><span data-stu-id="e24ba-111">Int32</span></span>      | <span data-ttu-id="e24ba-112">Только для внутреннего использования</span><span class="sxs-lookup"><span data-stu-id="e24ba-112">For internal use only</span></span>
| <span data-ttu-id="e24ba-113">identityProvider</span><span class="sxs-lookup"><span data-stu-id="e24ba-113">identityProvider</span></span> | <span data-ttu-id="e24ba-114">string</span><span class="sxs-lookup"><span data-stu-id="e24ba-114">string</span></span>     | <span data-ttu-id="e24ba-115">Только для внутреннего использования</span><span class="sxs-lookup"><span data-stu-id="e24ba-115">For internal use only</span></span>
| <span data-ttu-id="e24ba-116">key</span><span class="sxs-lookup"><span data-stu-id="e24ba-116">key</span></span>              | <span data-ttu-id="e24ba-117">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="e24ba-117">Edm.Binary</span></span> | <span data-ttu-id="e24ba-118">Только для внутреннего использования</span><span class="sxs-lookup"><span data-stu-id="e24ba-118">For internal use only</span></span>
