---
title: Тип ресурса Упдатевиндов
description: Тип ресурса Упдатевиндов.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d0f509accba2cb73709a4a5fa504a5d2a716b038
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519584"
---
# <a name="updatewindow-resource-type"></a><span data-ttu-id="0604e-103">Тип ресурса Упдатевиндов</span><span class="sxs-lookup"><span data-stu-id="0604e-103">updateWindow resource type</span></span>

<span data-ttu-id="0604e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0604e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0604e-105">Представляет окно времени, в течение которого [агенты](onpremisesagent.md) могут получать обновления.</span><span class="sxs-lookup"><span data-stu-id="0604e-105">Represents time window during which [agents](onpremisesagent.md) can receive updates.</span></span>

## <a name="properties"></a><span data-ttu-id="0604e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0604e-106">Properties</span></span>

| <span data-ttu-id="0604e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0604e-107">Property</span></span>     | <span data-ttu-id="0604e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0604e-108">Type</span></span>        | <span data-ttu-id="0604e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0604e-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0604e-110">упдатевиндовендтиме</span><span class="sxs-lookup"><span data-stu-id="0604e-110">updateWindowEndTime</span></span>|<span data-ttu-id="0604e-111">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="0604e-111">TimeOfDay</span></span>|<span data-ttu-id="0604e-112">Конец интервала времени, в течение которого агенты могут получать обновления</span><span class="sxs-lookup"><span data-stu-id="0604e-112">End of a time window during which agents can receive updates</span></span>|
|<span data-ttu-id="0604e-113">упдатевиндовстарттиме</span><span class="sxs-lookup"><span data-stu-id="0604e-113">updateWindowStartTime</span></span>|<span data-ttu-id="0604e-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="0604e-114">TimeOfDay</span></span>|<span data-ttu-id="0604e-115">Начало периода времени, в течение которого агенты могут получать обновления</span><span class="sxs-lookup"><span data-stu-id="0604e-115">Start of a time window during which agents can receive updates</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0604e-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0604e-116">JSON representation</span></span>

<span data-ttu-id="0604e-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0604e-117">The following is a JSON representation of the resource.</span></span>

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
