---
title: Тип ресурса Тимеранже
description: Ресурс диапазона времени с временем начала и окончания.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 12cdae2407ea985b28afb658c7fd7517fdbb687c
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154166"
---
# <a name="timerange-resource-type"></a><span data-ttu-id="15a41-103">Тип ресурса Тимеранже</span><span class="sxs-lookup"><span data-stu-id="15a41-103">timeRange resource type</span></span>

<span data-ttu-id="15a41-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15a41-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="15a41-105">Ресурс диапазона времени с временем начала и окончания.</span><span class="sxs-lookup"><span data-stu-id="15a41-105">A time range resource with a start and end time.</span></span>

## <a name="properties"></a><span data-ttu-id="15a41-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="15a41-106">Properties</span></span>

| <span data-ttu-id="15a41-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="15a41-107">Property</span></span>     | <span data-ttu-id="15a41-108">Тип</span><span class="sxs-lookup"><span data-stu-id="15a41-108">Type</span></span>        | <span data-ttu-id="15a41-109">Описание</span><span class="sxs-lookup"><span data-stu-id="15a41-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="15a41-110">endTime</span><span class="sxs-lookup"><span data-stu-id="15a41-110">endTime</span></span>|<span data-ttu-id="15a41-111">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="15a41-111">TimeOfDay</span></span>|<span data-ttu-id="15a41-112">Время окончания для диапазона времени.</span><span class="sxs-lookup"><span data-stu-id="15a41-112">End time for the time range.</span></span>|
|<span data-ttu-id="15a41-113">startTime</span><span class="sxs-lookup"><span data-stu-id="15a41-113">startTime</span></span>|<span data-ttu-id="15a41-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="15a41-114">TimeOfDay</span></span>|<span data-ttu-id="15a41-115">Время начала для диапазона времени.</span><span class="sxs-lookup"><span data-stu-id="15a41-115">Start time for the time range.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="15a41-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15a41-116">JSON representation</span></span>

<span data-ttu-id="15a41-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15a41-117">The following is a JSON representation of the resource.</span></span>

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