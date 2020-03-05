---
title: Тип ресурса Тимеранже
description: Ресурс диапазона времени с временем начала и окончания.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e9edfd06ecd65d7e08d6701d1fc885dce9067689
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519710"
---
# <a name="timerange-resource-type"></a><span data-ttu-id="29067-103">Тип ресурса Тимеранже</span><span class="sxs-lookup"><span data-stu-id="29067-103">timeRange resource type</span></span>

<span data-ttu-id="29067-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="29067-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29067-105">Ресурс диапазона времени с временем начала и окончания.</span><span class="sxs-lookup"><span data-stu-id="29067-105">A time range resource with a start and end time.</span></span>

## <a name="properties"></a><span data-ttu-id="29067-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="29067-106">Properties</span></span>

| <span data-ttu-id="29067-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="29067-107">Property</span></span>     | <span data-ttu-id="29067-108">Тип</span><span class="sxs-lookup"><span data-stu-id="29067-108">Type</span></span>        | <span data-ttu-id="29067-109">Описание</span><span class="sxs-lookup"><span data-stu-id="29067-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="29067-110">endTime</span><span class="sxs-lookup"><span data-stu-id="29067-110">endTime</span></span>|<span data-ttu-id="29067-111">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="29067-111">TimeOfDay</span></span>|<span data-ttu-id="29067-112">Время окончания для диапазона времени.</span><span class="sxs-lookup"><span data-stu-id="29067-112">End time for the time range.</span></span>|
|<span data-ttu-id="29067-113">startTime</span><span class="sxs-lookup"><span data-stu-id="29067-113">startTime</span></span>|<span data-ttu-id="29067-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="29067-114">TimeOfDay</span></span>|<span data-ttu-id="29067-115">Время начала для диапазона времени.</span><span class="sxs-lookup"><span data-stu-id="29067-115">Start time for the time range.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29067-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="29067-116">JSON representation</span></span>

<span data-ttu-id="29067-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29067-117">The following is a JSON representation of the resource.</span></span>

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