---
title: Тип ресурса alternativeSecurityId
description: Только для внутреннего использования. В будущем этот сложный тип будет устаревшим.
localization_priority: Normal
ms.openlocfilehash: 31e5501c504b8813f8910a8b8b352a1fa0ce9478
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348420"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="e8f7f-104">Тип ресурса alternativeSecurityId</span><span class="sxs-lookup"><span data-stu-id="e8f7f-104">alternativeSecurityId resource type</span></span>

<span data-ttu-id="e8f7f-105">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="e8f7f-105">For internal use only.</span></span> <span data-ttu-id="e8f7f-106">В будущем этот сложный тип будет устаревшим.</span><span class="sxs-lookup"><span data-stu-id="e8f7f-106">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8f7f-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e8f7f-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="e8f7f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e8f7f-108">Properties</span></span>
| <span data-ttu-id="e8f7f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8f7f-109">Property</span></span>         | <span data-ttu-id="e8f7f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e8f7f-110">Type</span></span>       | <span data-ttu-id="e8f7f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e8f7f-111">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="e8f7f-112">type</span><span class="sxs-lookup"><span data-stu-id="e8f7f-112">type</span></span>             | <span data-ttu-id="e8f7f-113">Int32</span><span class="sxs-lookup"><span data-stu-id="e8f7f-113">Int32</span></span>      | <span data-ttu-id="e8f7f-114">Только для внутреннего использования</span><span class="sxs-lookup"><span data-stu-id="e8f7f-114">For internal use only</span></span>
| <span data-ttu-id="e8f7f-115">identityProvider</span><span class="sxs-lookup"><span data-stu-id="e8f7f-115">identityProvider</span></span> | <span data-ttu-id="e8f7f-116">string</span><span class="sxs-lookup"><span data-stu-id="e8f7f-116">string</span></span>     | <span data-ttu-id="e8f7f-117">Только для внутреннего использования</span><span class="sxs-lookup"><span data-stu-id="e8f7f-117">For internal use only</span></span>
| <span data-ttu-id="e8f7f-118">ключа</span><span class="sxs-lookup"><span data-stu-id="e8f7f-118">key</span></span>              | <span data-ttu-id="e8f7f-119">EDM. binary</span><span class="sxs-lookup"><span data-stu-id="e8f7f-119">Edm.Binary</span></span> | <span data-ttu-id="e8f7f-120">Только для внутреннего использования</span><span class="sxs-lookup"><span data-stu-id="e8f7f-120">For internal use only</span></span>
