---
title: Тип ресурса Тимеранже
description: Ресурс диапазона времени с временем начала и окончания.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: eb06c09a85d36ab8702b253fd48d7cf5144ce664
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075479"
---
# <a name="timerange-resource-type"></a><span data-ttu-id="53dda-103">Тип ресурса Тимеранже</span><span class="sxs-lookup"><span data-stu-id="53dda-103">timeRange resource type</span></span>

<span data-ttu-id="53dda-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53dda-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53dda-105">Ресурс диапазона времени с временем начала и окончания.</span><span class="sxs-lookup"><span data-stu-id="53dda-105">A time range resource with a start and end time.</span></span>

## <a name="properties"></a><span data-ttu-id="53dda-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="53dda-106">Properties</span></span>

| <span data-ttu-id="53dda-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="53dda-107">Property</span></span>     | <span data-ttu-id="53dda-108">Тип</span><span class="sxs-lookup"><span data-stu-id="53dda-108">Type</span></span>        | <span data-ttu-id="53dda-109">Описание</span><span class="sxs-lookup"><span data-stu-id="53dda-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="53dda-110">endTime</span><span class="sxs-lookup"><span data-stu-id="53dda-110">endTime</span></span>|<span data-ttu-id="53dda-111">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="53dda-111">TimeOfDay</span></span>|<span data-ttu-id="53dda-112">Время окончания для диапазона времени.</span><span class="sxs-lookup"><span data-stu-id="53dda-112">End time for the time range.</span></span>|
|<span data-ttu-id="53dda-113">startTime</span><span class="sxs-lookup"><span data-stu-id="53dda-113">startTime</span></span>|<span data-ttu-id="53dda-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="53dda-114">TimeOfDay</span></span>|<span data-ttu-id="53dda-115">Время начала для диапазона времени.</span><span class="sxs-lookup"><span data-stu-id="53dda-115">Start time for the time range.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="53dda-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="53dda-116">JSON representation</span></span>

<span data-ttu-id="53dda-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53dda-117">The following is a JSON representation of the resource.</span></span>

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

