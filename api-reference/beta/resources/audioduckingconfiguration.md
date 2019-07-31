---
title: Тип ресурса Аудиодуккингконфигуратион
description: Параметры дуккинг других источников (фасинг в других источниках и из них).
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cfff0ca240a13c9c4396d605def05a52e1916778
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013222"
---
# <a name="audioduckingconfiguration-resource-type"></a><span data-ttu-id="6ab2f-103">Тип ресурса Аудиодуккингконфигуратион</span><span class="sxs-lookup"><span data-stu-id="6ab2f-103">audioDuckingConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ab2f-104">Параметры дуккинг других источников (фасинг в других источниках и из них).</span><span class="sxs-lookup"><span data-stu-id="6ab2f-104">Parameters for ducking of other sources (phasing in and out of other sources.)</span></span>

## <a name="properties"></a><span data-ttu-id="6ab2f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ab2f-105">Properties</span></span>

| <span data-ttu-id="6ab2f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ab2f-106">Property</span></span>      | <span data-ttu-id="6ab2f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6ab2f-107">Type</span></span>     | <span data-ttu-id="6ab2f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6ab2f-108">Description</span></span>                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="6ab2f-109">Ловерлевел</span><span class="sxs-lookup"><span data-stu-id="6ab2f-109">lowerLevel</span></span>    | <span data-ttu-id="6ab2f-110">Int64</span><span class="sxs-lookup"><span data-stu-id="6ab2f-110">Int64</span></span>    | <span data-ttu-id="6ab2f-111">Объем источников в процентах при дуккед источников.</span><span class="sxs-lookup"><span data-stu-id="6ab2f-111">The volume of sources in percent when the sources are being ducked.</span></span>             |
| <span data-ttu-id="6ab2f-112">Рампактиве</span><span class="sxs-lookup"><span data-stu-id="6ab2f-112">rampActive</span></span>    | <span data-ttu-id="6ab2f-113">Int64</span><span class="sxs-lookup"><span data-stu-id="6ab2f-113">Int64</span></span>    | <span data-ttu-id="6ab2f-114">Период времени (в миллисекундах), который требуется для дуккед источников.</span><span class="sxs-lookup"><span data-stu-id="6ab2f-114">The amount of time (in milliseconds) it takes for ducked sources to "fade out".</span></span> |
| <span data-ttu-id="6ab2f-115">Рампинактиве</span><span class="sxs-lookup"><span data-stu-id="6ab2f-115">rampInactive</span></span>  | <span data-ttu-id="6ab2f-116">Int64</span><span class="sxs-lookup"><span data-stu-id="6ab2f-116">Int64</span></span>    | <span data-ttu-id="6ab2f-117">Период времени (в миллисекундах), который требуется для дуккед источников.</span><span class="sxs-lookup"><span data-stu-id="6ab2f-117">The amount of time (in milliseconds) it takes for ducked sources to "fade in".</span></span>  |
| <span data-ttu-id="6ab2f-118">Упперлевел</span><span class="sxs-lookup"><span data-stu-id="6ab2f-118">upperLevel</span></span>    | <span data-ttu-id="6ab2f-119">Int64</span><span class="sxs-lookup"><span data-stu-id="6ab2f-119">Int64</span></span>    | <span data-ttu-id="6ab2f-120">Объем источников в процентах, когда источники не дуккед.</span><span class="sxs-lookup"><span data-stu-id="6ab2f-120">The volume of sources in percent when the sources are not being ducked.</span></span>         |

> <span data-ttu-id="6ab2f-121">**Примечание:** Длительность увеличения не может превышать 5 000 миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="6ab2f-121">**Note:** Ramp duration cannot be more than 5,000 milliseconds.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ab2f-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6ab2f-122">JSON representation</span></span>

<span data-ttu-id="6ab2f-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ab2f-123">The following is a JSON representation of the resource.</span></span>

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
