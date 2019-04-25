---
title: Тип ресурса Аудиодуккингконфигуратион
description: Параметры дуккинг других источников (фасинг в других источниках и из них).
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d61e4150250df25e020f45a65676d1c55c0e4c9d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544141"
---
# <a name="audioduckingconfiguration-resource-type"></a><span data-ttu-id="93f10-103">Тип ресурса Аудиодуккингконфигуратион</span><span class="sxs-lookup"><span data-stu-id="93f10-103">audioDuckingConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93f10-104">Параметры дуккинг других источников (фасинг в других источниках и из них).</span><span class="sxs-lookup"><span data-stu-id="93f10-104">Parameters for ducking of other sources (phasing in and out of other sources.)</span></span>

## <a name="properties"></a><span data-ttu-id="93f10-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="93f10-105">Properties</span></span>

| <span data-ttu-id="93f10-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="93f10-106">Property</span></span>      | <span data-ttu-id="93f10-107">Тип</span><span class="sxs-lookup"><span data-stu-id="93f10-107">Type</span></span>     | <span data-ttu-id="93f10-108">Описание</span><span class="sxs-lookup"><span data-stu-id="93f10-108">Description</span></span>                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="93f10-109">Ловерлевел</span><span class="sxs-lookup"><span data-stu-id="93f10-109">lowerLevel</span></span>    | <span data-ttu-id="93f10-110">Int64</span><span class="sxs-lookup"><span data-stu-id="93f10-110">Int64</span></span>    | <span data-ttu-id="93f10-111">Объем источников в процентах при дуккед источников.</span><span class="sxs-lookup"><span data-stu-id="93f10-111">The volume of sources in percent when the sources are being ducked.</span></span>             |
| <span data-ttu-id="93f10-112">Рампактиве</span><span class="sxs-lookup"><span data-stu-id="93f10-112">rampActive</span></span>    | <span data-ttu-id="93f10-113">Int64</span><span class="sxs-lookup"><span data-stu-id="93f10-113">Int64</span></span>    | <span data-ttu-id="93f10-114">Период времени (в миллисекундах), который требуется для дуккед источников.</span><span class="sxs-lookup"><span data-stu-id="93f10-114">The amount of time (in milliseconds) it takes for ducked sources to "fade out".</span></span> |
| <span data-ttu-id="93f10-115">Рампинактиве</span><span class="sxs-lookup"><span data-stu-id="93f10-115">rampInactive</span></span>  | <span data-ttu-id="93f10-116">Int64</span><span class="sxs-lookup"><span data-stu-id="93f10-116">Int64</span></span>    | <span data-ttu-id="93f10-117">Период времени (в миллисекундах), который требуется для дуккед источников.</span><span class="sxs-lookup"><span data-stu-id="93f10-117">The amount of time (in milliseconds) it takes for ducked sources to "fade in".</span></span>  |
| <span data-ttu-id="93f10-118">Упперлевел</span><span class="sxs-lookup"><span data-stu-id="93f10-118">upperLevel</span></span>    | <span data-ttu-id="93f10-119">Int64</span><span class="sxs-lookup"><span data-stu-id="93f10-119">Int64</span></span>    | <span data-ttu-id="93f10-120">Объем источников в процентах, когда источники не дуккед.</span><span class="sxs-lookup"><span data-stu-id="93f10-120">The volume of sources in percent when the sources are not being ducked.</span></span>         |

> <span data-ttu-id="93f10-121">**Примечание:** Длительность увеличения не может превышать 5 000 миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="93f10-121">**Note:** Ramp duration cannot be more than 5,000 milliseconds.</span></span>

## <a name="json-representation"></a><span data-ttu-id="93f10-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="93f10-122">JSON representation</span></span>

<span data-ttu-id="93f10-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93f10-123">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/audioduckingconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
