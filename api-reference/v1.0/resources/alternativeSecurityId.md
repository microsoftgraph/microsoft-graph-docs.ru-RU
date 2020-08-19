---
title: Тип ресурса alternativeSecurityId
description: Только для внутреннего использования.
localization_priority: Normal
author: spunukol
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 151de4ee90d715ffb6619908ea17cd6ba5e52ed4
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807852"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="52b46-103">Тип ресурса alternativeSecurityId</span><span class="sxs-lookup"><span data-stu-id="52b46-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="52b46-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52b46-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="52b46-105">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="52b46-105">For internal use only.</span></span> <span data-ttu-id="52b46-106">В будущем этот сложный тип будет устаревшим.</span><span class="sxs-lookup"><span data-stu-id="52b46-106">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="52b46-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52b46-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="52b46-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="52b46-108">Properties</span></span>
| <span data-ttu-id="52b46-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="52b46-109">Property</span></span>         | <span data-ttu-id="52b46-110">Тип</span><span class="sxs-lookup"><span data-stu-id="52b46-110">Type</span></span>       | <span data-ttu-id="52b46-111">Описание</span><span class="sxs-lookup"><span data-stu-id="52b46-111">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="52b46-112">type</span><span class="sxs-lookup"><span data-stu-id="52b46-112">type</span></span>             | <span data-ttu-id="52b46-113">Int32</span><span class="sxs-lookup"><span data-stu-id="52b46-113">Int32</span></span>      | <span data-ttu-id="52b46-114">Только для внутреннего использования</span><span class="sxs-lookup"><span data-stu-id="52b46-114">For internal use only</span></span>
| <span data-ttu-id="52b46-115">identityProvider</span><span class="sxs-lookup"><span data-stu-id="52b46-115">identityProvider</span></span> | <span data-ttu-id="52b46-116">string</span><span class="sxs-lookup"><span data-stu-id="52b46-116">string</span></span>     | <span data-ttu-id="52b46-117">Только для внутреннего использования</span><span class="sxs-lookup"><span data-stu-id="52b46-117">For internal use only</span></span>
| <span data-ttu-id="52b46-118">ключа</span><span class="sxs-lookup"><span data-stu-id="52b46-118">key</span></span>              | <span data-ttu-id="52b46-119">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="52b46-119">Edm.Binary</span></span> | <span data-ttu-id="52b46-120">Только для внутреннего использования</span><span class="sxs-lookup"><span data-stu-id="52b46-120">For internal use only</span></span>
