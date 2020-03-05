---
title: Тип ресурса Аудиодуккингконфигуратион
description: Параметры дуккинг других источников (фасинг в других источниках и из них).
author: ananmishr
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 99aa202e0048b328d97453f57d249df749f7bce5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508117"
---
# <a name="audioduckingconfiguration-resource-type"></a><span data-ttu-id="79cf3-103">Тип ресурса Аудиодуккингконфигуратион</span><span class="sxs-lookup"><span data-stu-id="79cf3-103">audioDuckingConfiguration resource type</span></span>

<span data-ttu-id="79cf3-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="79cf3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79cf3-105">Параметры дуккинг других источников (фасинг в других источниках и из них).</span><span class="sxs-lookup"><span data-stu-id="79cf3-105">Parameters for ducking of other sources (phasing in and out of other sources.)</span></span>

## <a name="properties"></a><span data-ttu-id="79cf3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="79cf3-106">Properties</span></span>

| <span data-ttu-id="79cf3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="79cf3-107">Property</span></span>      | <span data-ttu-id="79cf3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="79cf3-108">Type</span></span>     | <span data-ttu-id="79cf3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="79cf3-109">Description</span></span>                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="79cf3-110">ловерлевел</span><span class="sxs-lookup"><span data-stu-id="79cf3-110">lowerLevel</span></span>    | <span data-ttu-id="79cf3-111">Int64</span><span class="sxs-lookup"><span data-stu-id="79cf3-111">Int64</span></span>    | <span data-ttu-id="79cf3-112">Объем источников в процентах при дуккед источников.</span><span class="sxs-lookup"><span data-stu-id="79cf3-112">The volume of sources in percent when the sources are being ducked.</span></span>             |
| <span data-ttu-id="79cf3-113">рампактиве</span><span class="sxs-lookup"><span data-stu-id="79cf3-113">rampActive</span></span>    | <span data-ttu-id="79cf3-114">Int64</span><span class="sxs-lookup"><span data-stu-id="79cf3-114">Int64</span></span>    | <span data-ttu-id="79cf3-115">Период времени (в миллисекундах), который требуется для дуккед источников.</span><span class="sxs-lookup"><span data-stu-id="79cf3-115">The amount of time (in milliseconds) it takes for ducked sources to "fade out".</span></span> |
| <span data-ttu-id="79cf3-116">рампинактиве</span><span class="sxs-lookup"><span data-stu-id="79cf3-116">rampInactive</span></span>  | <span data-ttu-id="79cf3-117">Int64</span><span class="sxs-lookup"><span data-stu-id="79cf3-117">Int64</span></span>    | <span data-ttu-id="79cf3-118">Период времени (в миллисекундах), который требуется для дуккед источников.</span><span class="sxs-lookup"><span data-stu-id="79cf3-118">The amount of time (in milliseconds) it takes for ducked sources to "fade in".</span></span>  |
| <span data-ttu-id="79cf3-119">упперлевел</span><span class="sxs-lookup"><span data-stu-id="79cf3-119">upperLevel</span></span>    | <span data-ttu-id="79cf3-120">Int64</span><span class="sxs-lookup"><span data-stu-id="79cf3-120">Int64</span></span>    | <span data-ttu-id="79cf3-121">Объем источников в процентах, когда источники не дуккед.</span><span class="sxs-lookup"><span data-stu-id="79cf3-121">The volume of sources in percent when the sources are not being ducked.</span></span>         |

> <span data-ttu-id="79cf3-122">**Примечание:** Длительность увеличения не может превышать 5 000 миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="79cf3-122">**Note:** Ramp duration cannot be more than 5,000 milliseconds.</span></span>

## <a name="json-representation"></a><span data-ttu-id="79cf3-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="79cf3-123">JSON representation</span></span>

<span data-ttu-id="79cf3-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79cf3-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioDuckingConfiguration"
}-->
```json
{
  "lowerLevel": 20,
  "rampActive": 1000,
  "rampInactive": 1000,
  "upperLevel": 100
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioDuckingConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
