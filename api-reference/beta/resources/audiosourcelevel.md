---
title: Тип ресурса audioSourceLevel
description: Конфигурации уровня для других источников.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 79ad56c11e8b277a1354ffc3a6292a0434466c8a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947654"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="e3ce5-103">Тип ресурса audioSourceLevel</span><span class="sxs-lookup"><span data-stu-id="e3ce5-103">audioSourceLevel resource type</span></span>

> <span data-ttu-id="e3ce5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e3ce5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3ce5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3ce5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e3ce5-106">Конфигурации уровня для других источников.</span><span class="sxs-lookup"><span data-stu-id="e3ce5-106">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="e3ce5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3ce5-107">Properties</span></span>

| <span data-ttu-id="e3ce5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3ce5-108">Property</span></span>               | <span data-ttu-id="e3ce5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e3ce5-109">Type</span></span>    | <span data-ttu-id="e3ce5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e3ce5-110">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e3ce5-111">duckOthers</span><span class="sxs-lookup"><span data-stu-id="e3ce5-111">duckOthers</span></span>             | <span data-ttu-id="e3ce5-112">Логический</span><span class="sxs-lookup"><span data-stu-id="e3ce5-112">Boolean</span></span> | <span data-ttu-id="e3ce5-113">Включение этого источника для duck другие источники при активный.</span><span class="sxs-lookup"><span data-stu-id="e3ce5-113">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="e3ce5-114">Если значение равно true, Уклонение от уровня должно быть задано.</span><span class="sxs-lookup"><span data-stu-id="e3ce5-114">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="e3ce5-115">level</span><span class="sxs-lookup"><span data-stu-id="e3ce5-115">level</span></span>                  | <span data-ttu-id="e3ce5-116">Int64</span><span class="sxs-lookup"><span data-stu-id="e3ce5-116">Int64</span></span>   | <span data-ttu-id="e3ce5-117">Уклонение от уровня источника, если `duckOthers` задано значение `true`.</span><span class="sxs-lookup"><span data-stu-id="e3ce5-117">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="e3ce5-118">Участник</span><span class="sxs-lookup"><span data-stu-id="e3ce5-118">participant</span></span>            | <span data-ttu-id="e3ce5-119">Строка</span><span class="sxs-lookup"><span data-stu-id="e3ce5-119">String</span></span>  | <span data-ttu-id="e3ce5-120">Источник участников аудиопотока.</span><span class="sxs-lookup"><span data-stu-id="e3ce5-120">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="e3ce5-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e3ce5-121">JSON representation</span></span>

<span data-ttu-id="e3ce5-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3ce5-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioSourceLevel"
}-->
```json
{
  "duckOthers": true,
  "level": 100,
  "participant": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "audioSourceLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
