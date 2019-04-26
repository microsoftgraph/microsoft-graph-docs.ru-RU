---
title: Тип ресурса alternativeSecurityId
description: Только для внутреннего использования.
localization_priority: Normal
ms.openlocfilehash: 60e45c6d914c64f92b9f15f78fda22372a23e91f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345843"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="b7e47-103">Тип ресурса alternativeSecurityId</span><span class="sxs-lookup"><span data-stu-id="b7e47-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="b7e47-104">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="b7e47-104">For internal use only.</span></span> <span data-ttu-id="b7e47-105">В будущем этот сложный тип будет устаревшим.</span><span class="sxs-lookup"><span data-stu-id="b7e47-105">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7e47-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b7e47-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b7e47-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b7e47-107">Properties</span></span>
| <span data-ttu-id="b7e47-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7e47-108">Property</span></span>         | <span data-ttu-id="b7e47-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b7e47-109">Type</span></span>       | <span data-ttu-id="b7e47-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b7e47-110">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="b7e47-111">type</span><span class="sxs-lookup"><span data-stu-id="b7e47-111">type</span></span>             | <span data-ttu-id="b7e47-112">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e47-112">Int32</span></span>      | <span data-ttu-id="b7e47-113">Только для внутреннего использования</span><span class="sxs-lookup"><span data-stu-id="b7e47-113">For internal use only</span></span>
| <span data-ttu-id="b7e47-114">identityProvider</span><span class="sxs-lookup"><span data-stu-id="b7e47-114">identityProvider</span></span> | <span data-ttu-id="b7e47-115">строка</span><span class="sxs-lookup"><span data-stu-id="b7e47-115">string</span></span>     | <span data-ttu-id="b7e47-116">Только для внутреннего использования</span><span class="sxs-lookup"><span data-stu-id="b7e47-116">For internal use only</span></span>
| <span data-ttu-id="b7e47-117">ключа</span><span class="sxs-lookup"><span data-stu-id="b7e47-117">key</span></span>              | <span data-ttu-id="b7e47-118">EDM. binary</span><span class="sxs-lookup"><span data-stu-id="b7e47-118">Edm.Binary</span></span> | <span data-ttu-id="b7e47-119">Только для внутреннего использования</span><span class="sxs-lookup"><span data-stu-id="b7e47-119">For internal use only</span></span>
