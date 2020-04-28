---
title: Тип ресурса alternativeSecurityId
description: Только для внутреннего использования. В будущем этот сложный тип будет устаревшим.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4e3dfae11009000fa89eccb7c0263867fe2a1562
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508333"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="57533-104">Тип ресурса alternativeSecurityId</span><span class="sxs-lookup"><span data-stu-id="57533-104">alternativeSecurityId resource type</span></span>

<span data-ttu-id="57533-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57533-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="57533-106">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="57533-106">For internal use only.</span></span> <span data-ttu-id="57533-107">В будущем этот сложный тип будет устаревшим.</span><span class="sxs-lookup"><span data-stu-id="57533-107">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="57533-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="57533-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="57533-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="57533-109">Properties</span></span>
| <span data-ttu-id="57533-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="57533-110">Property</span></span>         | <span data-ttu-id="57533-111">Тип</span><span class="sxs-lookup"><span data-stu-id="57533-111">Type</span></span>       | <span data-ttu-id="57533-112">Описание</span><span class="sxs-lookup"><span data-stu-id="57533-112">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="57533-113">type</span><span class="sxs-lookup"><span data-stu-id="57533-113">type</span></span>             | <span data-ttu-id="57533-114">Int32</span><span class="sxs-lookup"><span data-stu-id="57533-114">Int32</span></span>      | <span data-ttu-id="57533-115">Только для внутреннего использования</span><span class="sxs-lookup"><span data-stu-id="57533-115">For internal use only</span></span>
| <span data-ttu-id="57533-116">identityProvider</span><span class="sxs-lookup"><span data-stu-id="57533-116">identityProvider</span></span> | <span data-ttu-id="57533-117">string</span><span class="sxs-lookup"><span data-stu-id="57533-117">string</span></span>     | <span data-ttu-id="57533-118">Только для внутреннего использования</span><span class="sxs-lookup"><span data-stu-id="57533-118">For internal use only</span></span>
| <span data-ttu-id="57533-119">ключа</span><span class="sxs-lookup"><span data-stu-id="57533-119">key</span></span>              | <span data-ttu-id="57533-120">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="57533-120">Edm.Binary</span></span> | <span data-ttu-id="57533-121">Только для внутреннего использования</span><span class="sxs-lookup"><span data-stu-id="57533-121">For internal use only</span></span>
