---
title: Тип ресурса Упдатевиндов
description: Тип ресурса Упдатевиндов.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b2aa61d5d815d912caa47fd63d5907b62f882d36
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003453"
---
# <a name="updatewindow-resource-type"></a><span data-ttu-id="9ab53-103">Тип ресурса Упдатевиндов</span><span class="sxs-lookup"><span data-stu-id="9ab53-103">updateWindow resource type</span></span>

<span data-ttu-id="9ab53-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ab53-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ab53-105">Представляет окно времени, в течение которого [агенты](onpremisesagent.md) могут получать обновления.</span><span class="sxs-lookup"><span data-stu-id="9ab53-105">Represents time window during which [agents](onpremisesagent.md) can receive updates.</span></span>

## <a name="properties"></a><span data-ttu-id="9ab53-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9ab53-106">Properties</span></span>

| <span data-ttu-id="9ab53-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ab53-107">Property</span></span>     | <span data-ttu-id="9ab53-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9ab53-108">Type</span></span>        | <span data-ttu-id="9ab53-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9ab53-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9ab53-110">упдатевиндовендтиме</span><span class="sxs-lookup"><span data-stu-id="9ab53-110">updateWindowEndTime</span></span>|<span data-ttu-id="9ab53-111">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="9ab53-111">TimeOfDay</span></span>|<span data-ttu-id="9ab53-112">Конец интервала времени, в течение которого агенты могут получать обновления</span><span class="sxs-lookup"><span data-stu-id="9ab53-112">End of a time window during which agents can receive updates</span></span>|
|<span data-ttu-id="9ab53-113">упдатевиндовстарттиме</span><span class="sxs-lookup"><span data-stu-id="9ab53-113">updateWindowStartTime</span></span>|<span data-ttu-id="9ab53-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="9ab53-114">TimeOfDay</span></span>|<span data-ttu-id="9ab53-115">Начало периода времени, в течение которого агенты могут получать обновления</span><span class="sxs-lookup"><span data-stu-id="9ab53-115">Start of a time window during which agents can receive updates</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ab53-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9ab53-116">JSON representation</span></span>

<span data-ttu-id="9ab53-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ab53-117">The following is a JSON representation of the resource.</span></span>

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


