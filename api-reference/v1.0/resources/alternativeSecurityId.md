---
title: Тип ресурса alternativeSecurityId
description: Только для внутреннего использования.
ms.openlocfilehash: 9d941469da133d9a3e7149dfca55c813f60b3ce8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024421"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="b0ce0-103">Тип ресурса alternativeSecurityId</span><span class="sxs-lookup"><span data-stu-id="b0ce0-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="b0ce0-104">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="b0ce0-104">For internal use only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0ce0-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0ce0-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b0ce0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0ce0-106">Properties</span></span>
| <span data-ttu-id="b0ce0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0ce0-107">Property</span></span>         | <span data-ttu-id="b0ce0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b0ce0-108">Type</span></span>       | <span data-ttu-id="b0ce0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b0ce0-109">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="b0ce0-110">type</span><span class="sxs-lookup"><span data-stu-id="b0ce0-110">type</span></span>             | <span data-ttu-id="b0ce0-111">Int32</span><span class="sxs-lookup"><span data-stu-id="b0ce0-111">Int32</span></span>      | <span data-ttu-id="b0ce0-112">Только для внутреннего использования</span><span class="sxs-lookup"><span data-stu-id="b0ce0-112">For internal use only</span></span>
| <span data-ttu-id="b0ce0-113">identityProvider</span><span class="sxs-lookup"><span data-stu-id="b0ce0-113">identityProvider</span></span> | <span data-ttu-id="b0ce0-114">string</span><span class="sxs-lookup"><span data-stu-id="b0ce0-114">string</span></span>     | <span data-ttu-id="b0ce0-115">Только для внутреннего использования</span><span class="sxs-lookup"><span data-stu-id="b0ce0-115">For internal use only</span></span>
| <span data-ttu-id="b0ce0-116">key</span><span class="sxs-lookup"><span data-stu-id="b0ce0-116">key</span></span>              | <span data-ttu-id="b0ce0-117">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="b0ce0-117">Edm.Binary</span></span> | <span data-ttu-id="b0ce0-118">Только для внутреннего использования</span><span class="sxs-lookup"><span data-stu-id="b0ce0-118">For internal use only</span></span>
