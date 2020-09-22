---
title: Тип ресурса Аудиодуккингконфигуратион
description: Параметры дуккинг других источников (фасинг в других источниках и из них).
author: ananmishr
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 795ad9b1740d36a365bea4d99a880c43308a01c8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024438"
---
# <a name="audioduckingconfiguration-resource-type"></a><span data-ttu-id="f1064-103">Тип ресурса Аудиодуккингконфигуратион</span><span class="sxs-lookup"><span data-stu-id="f1064-103">audioDuckingConfiguration resource type</span></span>

<span data-ttu-id="f1064-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1064-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1064-105">Параметры дуккинг других источников (фасинг в других источниках и из них).</span><span class="sxs-lookup"><span data-stu-id="f1064-105">Parameters for ducking of other sources (phasing in and out of other sources.)</span></span>

## <a name="properties"></a><span data-ttu-id="f1064-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1064-106">Properties</span></span>

| <span data-ttu-id="f1064-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1064-107">Property</span></span>      | <span data-ttu-id="f1064-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f1064-108">Type</span></span>     | <span data-ttu-id="f1064-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f1064-109">Description</span></span>                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="f1064-110">ловерлевел</span><span class="sxs-lookup"><span data-stu-id="f1064-110">lowerLevel</span></span>    | <span data-ttu-id="f1064-111">Int64</span><span class="sxs-lookup"><span data-stu-id="f1064-111">Int64</span></span>    | <span data-ttu-id="f1064-112">Объем источников в процентах при дуккед источников.</span><span class="sxs-lookup"><span data-stu-id="f1064-112">The volume of sources in percent when the sources are being ducked.</span></span>             |
| <span data-ttu-id="f1064-113">рампактиве</span><span class="sxs-lookup"><span data-stu-id="f1064-113">rampActive</span></span>    | <span data-ttu-id="f1064-114">Int64</span><span class="sxs-lookup"><span data-stu-id="f1064-114">Int64</span></span>    | <span data-ttu-id="f1064-115">Период времени (в миллисекундах), который требуется для дуккед источников.</span><span class="sxs-lookup"><span data-stu-id="f1064-115">The amount of time (in milliseconds) it takes for ducked sources to "fade out".</span></span> |
| <span data-ttu-id="f1064-116">рампинактиве</span><span class="sxs-lookup"><span data-stu-id="f1064-116">rampInactive</span></span>  | <span data-ttu-id="f1064-117">Int64</span><span class="sxs-lookup"><span data-stu-id="f1064-117">Int64</span></span>    | <span data-ttu-id="f1064-118">Период времени (в миллисекундах), который требуется для дуккед источников.</span><span class="sxs-lookup"><span data-stu-id="f1064-118">The amount of time (in milliseconds) it takes for ducked sources to "fade in".</span></span>  |
| <span data-ttu-id="f1064-119">упперлевел</span><span class="sxs-lookup"><span data-stu-id="f1064-119">upperLevel</span></span>    | <span data-ttu-id="f1064-120">Int64</span><span class="sxs-lookup"><span data-stu-id="f1064-120">Int64</span></span>    | <span data-ttu-id="f1064-121">Объем источников в процентах, когда источники не дуккед.</span><span class="sxs-lookup"><span data-stu-id="f1064-121">The volume of sources in percent when the sources are not being ducked.</span></span>         |

> <span data-ttu-id="f1064-122">**Примечание:** Длительность увеличения не может превышать 5 000 миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="f1064-122">**Note:** Ramp duration cannot be more than 5,000 milliseconds.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1064-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f1064-123">JSON representation</span></span>

<span data-ttu-id="f1064-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1064-124">The following is a JSON representation of the resource.</span></span>

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


