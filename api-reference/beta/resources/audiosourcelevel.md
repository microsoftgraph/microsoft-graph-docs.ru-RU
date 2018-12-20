---
title: Тип ресурса audioSourceLevel
description: Конфигурации уровня для других источников.
author: VinodRavichandran
ms.openlocfilehash: 5d5abe7eba03891427b30ba1c8f63b15b3707e46
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380242"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="a96b3-103">Тип ресурса audioSourceLevel</span><span class="sxs-lookup"><span data-stu-id="a96b3-103">audioSourceLevel resource type</span></span>

> <span data-ttu-id="a96b3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a96b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a96b3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a96b3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a96b3-106">Конфигурации уровня для других источников.</span><span class="sxs-lookup"><span data-stu-id="a96b3-106">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="a96b3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a96b3-107">Properties</span></span>

| <span data-ttu-id="a96b3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a96b3-108">Property</span></span>               | <span data-ttu-id="a96b3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a96b3-109">Type</span></span>    | <span data-ttu-id="a96b3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a96b3-110">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a96b3-111">duckOthers</span><span class="sxs-lookup"><span data-stu-id="a96b3-111">duckOthers</span></span>             | <span data-ttu-id="a96b3-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="a96b3-112">Boolean</span></span> | <span data-ttu-id="a96b3-113">Включение этого источника для duck другие источники при активный.</span><span class="sxs-lookup"><span data-stu-id="a96b3-113">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="a96b3-114">Если значение равно true, Уклонение от уровня должно быть задано.</span><span class="sxs-lookup"><span data-stu-id="a96b3-114">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="a96b3-115">level</span><span class="sxs-lookup"><span data-stu-id="a96b3-115">level</span></span>                  | <span data-ttu-id="a96b3-116">Int64</span><span class="sxs-lookup"><span data-stu-id="a96b3-116">Int64</span></span>   | <span data-ttu-id="a96b3-117">Уклонение от уровня источника, если `duckOthers` задано значение `true`.</span><span class="sxs-lookup"><span data-stu-id="a96b3-117">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="a96b3-118">Участник</span><span class="sxs-lookup"><span data-stu-id="a96b3-118">participant</span></span>            | <span data-ttu-id="a96b3-119">String</span><span class="sxs-lookup"><span data-stu-id="a96b3-119">String</span></span>  | <span data-ttu-id="a96b3-120">Источник участников аудиопотока.</span><span class="sxs-lookup"><span data-stu-id="a96b3-120">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="a96b3-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a96b3-121">JSON representation</span></span>

<span data-ttu-id="a96b3-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a96b3-122">The following is a JSON representation of the resource.</span></span>

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
