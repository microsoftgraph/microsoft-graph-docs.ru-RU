---
title: Тип ресурса Опеншифтитем
description: Представляет одно количество открытых смен.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 86392d330403acf667f81c1dce4bbc951bb8185d
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895848"
---
# <a name="openshiftitem-resource-type"></a><span data-ttu-id="7c9f9-103">Тип ресурса Опеншифтитем</span><span class="sxs-lookup"><span data-stu-id="7c9f9-103">openShiftItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c9f9-104">Представляет одно число [опеншифт](../resources/openshift.md).</span><span class="sxs-lookup"><span data-stu-id="7c9f9-104">Represents a single count of an [openshift](../resources/openshift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7c9f9-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c9f9-105">Properties</span></span>

| <span data-ttu-id="7c9f9-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c9f9-106">Property</span></span>     | <span data-ttu-id="7c9f9-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7c9f9-107">Type</span></span>        | <span data-ttu-id="7c9f9-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7c9f9-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7c9f9-109">опенслоткаунт</span><span class="sxs-lookup"><span data-stu-id="7c9f9-109">openSlotCount</span></span>|<span data-ttu-id="7c9f9-110">Int32</span><span class="sxs-lookup"><span data-stu-id="7c9f9-110">Int32</span></span>| <span data-ttu-id="7c9f9-111">Количество слотов для заданной открытой смены.</span><span class="sxs-lookup"><span data-stu-id="7c9f9-111">Count of the number of slots for the given open shift.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7c9f9-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7c9f9-112">JSON representation</span></span>

<span data-ttu-id="7c9f9-113">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c9f9-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShiftItem",
  "baseType": "microsoft.graph.shiftItem"
}-->

```json
{
  "openSlotCount": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShiftItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
