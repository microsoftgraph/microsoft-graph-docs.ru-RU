---
title: Тип ресурса Тимеранже
description: Ресурс диапазона времени с временем начала и окончания.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0e91f08e9f421a348f5ec7c2ebf5e2f23d4e9377
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952316"
---
# <a name="timerange-resource-type"></a><span data-ttu-id="cfa60-103">Тип ресурса Тимеранже</span><span class="sxs-lookup"><span data-stu-id="cfa60-103">timeRange resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfa60-104">Ресурс диапазона времени с временем начала и окончания.</span><span class="sxs-lookup"><span data-stu-id="cfa60-104">A time range resource with a start and end time.</span></span>

## <a name="properties"></a><span data-ttu-id="cfa60-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="cfa60-105">Properties</span></span>

| <span data-ttu-id="cfa60-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="cfa60-106">Property</span></span>     | <span data-ttu-id="cfa60-107">Тип</span><span class="sxs-lookup"><span data-stu-id="cfa60-107">Type</span></span>        | <span data-ttu-id="cfa60-108">Описание</span><span class="sxs-lookup"><span data-stu-id="cfa60-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cfa60-109">endTime</span><span class="sxs-lookup"><span data-stu-id="cfa60-109">endTime</span></span>|<span data-ttu-id="cfa60-110">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="cfa60-110">TimeOfDay</span></span>|<span data-ttu-id="cfa60-111">Время окончания для диапазона времени.</span><span class="sxs-lookup"><span data-stu-id="cfa60-111">End time for the time range.</span></span>|
|<span data-ttu-id="cfa60-112">startTime</span><span class="sxs-lookup"><span data-stu-id="cfa60-112">startTime</span></span>|<span data-ttu-id="cfa60-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="cfa60-113">TimeOfDay</span></span>|<span data-ttu-id="cfa60-114">Время начала для диапазона времени.</span><span class="sxs-lookup"><span data-stu-id="cfa60-114">Start time for the time range.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cfa60-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cfa60-115">JSON representation</span></span>

<span data-ttu-id="cfa60-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cfa60-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeRange",
  "baseType": null
}-->

```json
{
  "endTime": "String (timestamp)",
  "startTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->