---
title: Тип ресурса audioDuckingConfiguration
description: Параметры для Уклонение от других источников, (синхронизацию и выходить из нее других источников).
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 713e7012381bf6b727321494f81e75c88c66ebe6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891562"
---
# <a name="audioduckingconfiguration-resource-type"></a><span data-ttu-id="b455d-103">Тип ресурса audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="b455d-103">audioDuckingConfiguration resource type</span></span>

> <span data-ttu-id="b455d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b455d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b455d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b455d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b455d-106">Параметры для Уклонение от других источников, (синхронизацию и выходить из нее других источников).</span><span class="sxs-lookup"><span data-stu-id="b455d-106">Parameters for ducking of other sources (phasing in and out of other sources.)</span></span>

## <a name="properties"></a><span data-ttu-id="b455d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b455d-107">Properties</span></span>

| <span data-ttu-id="b455d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b455d-108">Property</span></span>      | <span data-ttu-id="b455d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b455d-109">Type</span></span>     | <span data-ttu-id="b455d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b455d-110">Description</span></span>                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="b455d-111">lowerLevel</span><span class="sxs-lookup"><span data-stu-id="b455d-111">lowerLevel</span></span>    | <span data-ttu-id="b455d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="b455d-112">Int64</span></span>    | <span data-ttu-id="b455d-113">Объем источников в процентах, когда источники которые ducked.</span><span class="sxs-lookup"><span data-stu-id="b455d-113">The volume of sources in percent when the sources are being ducked.</span></span>             |
| <span data-ttu-id="b455d-114">rampActive</span><span class="sxs-lookup"><span data-stu-id="b455d-114">rampActive</span></span>    | <span data-ttu-id="b455d-115">Int64</span><span class="sxs-lookup"><span data-stu-id="b455d-115">Int64</span></span>    | <span data-ttu-id="b455d-116">Количество времени (в миллисекундах), необходимое для ducked источников, чтобы «сделать».</span><span class="sxs-lookup"><span data-stu-id="b455d-116">The amount of time (in milliseconds) it takes for ducked sources to "fade out".</span></span> |
| <span data-ttu-id="b455d-117">rampInactive</span><span class="sxs-lookup"><span data-stu-id="b455d-117">rampInactive</span></span>  | <span data-ttu-id="b455d-118">Int64</span><span class="sxs-lookup"><span data-stu-id="b455d-118">Int64</span></span>    | <span data-ttu-id="b455d-119">Количество времени (в миллисекундах), необходимое для ducked источников «увеличение».</span><span class="sxs-lookup"><span data-stu-id="b455d-119">The amount of time (in milliseconds) it takes for ducked sources to "fade in".</span></span>  |
| <span data-ttu-id="b455d-120">upperLevel</span><span class="sxs-lookup"><span data-stu-id="b455d-120">upperLevel</span></span>    | <span data-ttu-id="b455d-121">Int64</span><span class="sxs-lookup"><span data-stu-id="b455d-121">Int64</span></span>    | <span data-ttu-id="b455d-122">Объем источников в процентах, когда ducked источников не выполняется.</span><span class="sxs-lookup"><span data-stu-id="b455d-122">The volume of sources in percent when the sources are not being ducked.</span></span>         |

> <span data-ttu-id="b455d-123">**Примечание:** Продолжительность расширение путь не может быть более 5000 миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="b455d-123">**Note:** Ramp duration cannot be more than 5,000 milliseconds.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b455d-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b455d-124">JSON representation</span></span>

<span data-ttu-id="b455d-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b455d-125">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "audioDuckingConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
