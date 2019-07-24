---
title: Тип ресурса Упдатевиндов
description: Тип ресурса Упдатевиндов.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 57fb977dd853261300ed09dd8d9b3c343f62bea0
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840956"
---
# <a name="updatewindow-resource-type"></a><span data-ttu-id="244d5-103">Тип ресурса Упдатевиндов</span><span class="sxs-lookup"><span data-stu-id="244d5-103">updateWindow resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="244d5-104">Представляет окно времени, в течение которого [агенты](onpremisesagent.md) могут получать обновления.</span><span class="sxs-lookup"><span data-stu-id="244d5-104">Represents time window during which [agents](onpremisesagent.md) can receive updates.</span></span>

## <a name="properties"></a><span data-ttu-id="244d5-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="244d5-105">Properties</span></span>

| <span data-ttu-id="244d5-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="244d5-106">Property</span></span>     | <span data-ttu-id="244d5-107">Тип</span><span class="sxs-lookup"><span data-stu-id="244d5-107">Type</span></span>        | <span data-ttu-id="244d5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="244d5-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="244d5-109">Упдатевиндовендтиме</span><span class="sxs-lookup"><span data-stu-id="244d5-109">updateWindowEndTime</span></span>|<span data-ttu-id="244d5-110">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="244d5-110">TimeOfDay</span></span>|<span data-ttu-id="244d5-111">Конец интервала времени, в течение которого агенты могут получать обновления</span><span class="sxs-lookup"><span data-stu-id="244d5-111">End of a time window during which agents can receive updates</span></span>|
|<span data-ttu-id="244d5-112">Упдатевиндовстарттиме</span><span class="sxs-lookup"><span data-stu-id="244d5-112">updateWindowStartTime</span></span>|<span data-ttu-id="244d5-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="244d5-113">TimeOfDay</span></span>|<span data-ttu-id="244d5-114">Начало периода времени, в течение которого агенты могут получать обновления</span><span class="sxs-lookup"><span data-stu-id="244d5-114">Start of a time window during which agents can receive updates</span></span>|

## <a name="json-representation"></a><span data-ttu-id="244d5-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="244d5-115">JSON representation</span></span>

<span data-ttu-id="244d5-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="244d5-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.updateWindow",
  "baseType": null
}-->

```json
{
  "updateWindowEndTime": "String (timestamp)",
  "updateWindowStartTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "updateWindow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
