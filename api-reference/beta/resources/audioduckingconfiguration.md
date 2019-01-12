---
title: Тип ресурса audioDuckingConfiguration
description: Параметры для Уклонение от других источников, (синхронизацию и выходить из нее других источников).
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b4132946573342976bb1f20c593454a8e18030d2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916875"
---
# <a name="audioduckingconfiguration-resource-type"></a><span data-ttu-id="419ef-103">Тип ресурса audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="419ef-103">audioDuckingConfiguration resource type</span></span>

> <span data-ttu-id="419ef-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="419ef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="419ef-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="419ef-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="419ef-106">Параметры для Уклонение от других источников, (синхронизацию и выходить из нее других источников).</span><span class="sxs-lookup"><span data-stu-id="419ef-106">Parameters for ducking of other sources (phasing in and out of other sources.)</span></span>

## <a name="properties"></a><span data-ttu-id="419ef-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="419ef-107">Properties</span></span>

| <span data-ttu-id="419ef-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="419ef-108">Property</span></span>      | <span data-ttu-id="419ef-109">Тип</span><span class="sxs-lookup"><span data-stu-id="419ef-109">Type</span></span>     | <span data-ttu-id="419ef-110">Описание</span><span class="sxs-lookup"><span data-stu-id="419ef-110">Description</span></span>                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="419ef-111">lowerLevel</span><span class="sxs-lookup"><span data-stu-id="419ef-111">lowerLevel</span></span>    | <span data-ttu-id="419ef-112">Int64</span><span class="sxs-lookup"><span data-stu-id="419ef-112">Int64</span></span>    | <span data-ttu-id="419ef-113">Объем источников в процентах, когда источники которые ducked.</span><span class="sxs-lookup"><span data-stu-id="419ef-113">The volume of sources in percent when the sources are being ducked.</span></span>             |
| <span data-ttu-id="419ef-114">rampActive</span><span class="sxs-lookup"><span data-stu-id="419ef-114">rampActive</span></span>    | <span data-ttu-id="419ef-115">Int64</span><span class="sxs-lookup"><span data-stu-id="419ef-115">Int64</span></span>    | <span data-ttu-id="419ef-116">Количество времени (в миллисекундах), необходимое для ducked источников, чтобы «сделать».</span><span class="sxs-lookup"><span data-stu-id="419ef-116">The amount of time (in milliseconds) it takes for ducked sources to "fade out".</span></span> |
| <span data-ttu-id="419ef-117">rampInactive</span><span class="sxs-lookup"><span data-stu-id="419ef-117">rampInactive</span></span>  | <span data-ttu-id="419ef-118">Int64</span><span class="sxs-lookup"><span data-stu-id="419ef-118">Int64</span></span>    | <span data-ttu-id="419ef-119">Количество времени (в миллисекундах), необходимое для ducked источников «увеличение».</span><span class="sxs-lookup"><span data-stu-id="419ef-119">The amount of time (in milliseconds) it takes for ducked sources to "fade in".</span></span>  |
| <span data-ttu-id="419ef-120">upperLevel</span><span class="sxs-lookup"><span data-stu-id="419ef-120">upperLevel</span></span>    | <span data-ttu-id="419ef-121">Int64</span><span class="sxs-lookup"><span data-stu-id="419ef-121">Int64</span></span>    | <span data-ttu-id="419ef-122">Объем источников в процентах, когда ducked источников не выполняется.</span><span class="sxs-lookup"><span data-stu-id="419ef-122">The volume of sources in percent when the sources are not being ducked.</span></span>         |

> <span data-ttu-id="419ef-123">**Примечание:** Продолжительность расширение путь не может быть более 5000 миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="419ef-123">**Note:** Ramp duration cannot be more than 5,000 milliseconds.</span></span>

## <a name="json-representation"></a><span data-ttu-id="419ef-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="419ef-124">JSON representation</span></span>

<span data-ttu-id="419ef-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="419ef-125">The following is a JSON representation of the resource.</span></span>

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
