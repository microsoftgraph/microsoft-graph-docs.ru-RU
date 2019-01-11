---
title: Тип ресурса participantMixerLevel
description: Конфигурация микшер уровни для заданного звука участников
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 8a7b77c07240fbb5face70eb8ea21be55b85f1fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874139"
---
# <a name="participantmixerlevel-resource-type"></a><span data-ttu-id="b4003-103">Тип ресурса participantMixerLevel</span><span class="sxs-lookup"><span data-stu-id="b4003-103">participantMixerLevel resource type</span></span>

> <span data-ttu-id="b4003-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b4003-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4003-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4003-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b4003-106">Конфигурация микшер уровни для заданного звука участников</span><span class="sxs-lookup"><span data-stu-id="b4003-106">Configuration of mixer levels for given audio participant</span></span>

## <a name="properties"></a><span data-ttu-id="b4003-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b4003-107">Properties</span></span>

| <span data-ttu-id="b4003-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4003-108">Property</span></span>               | <span data-ttu-id="b4003-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b4003-109">Type</span></span>                                                      | <span data-ttu-id="b4003-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b4003-110">Description</span></span>                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b4003-111">Уклонение от</span><span class="sxs-lookup"><span data-stu-id="b4003-111">ducking</span></span>                | [<span data-ttu-id="b4003-112">audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="b4003-112">audioDuckingConfiguration</span></span>](audioduckingconfiguration.md) | <span data-ttu-id="b4003-113">Конфигурация (синхронизацию и) из других источников для этой partipant пользовательский набор Уклонение от.</span><span class="sxs-lookup"><span data-stu-id="b4003-113">Configuration of ducking (phasing in and out) of other sources for this partipant custom mix.</span></span>       |
| <span data-ttu-id="b4003-114">exclusiveMode</span><span class="sxs-lookup"><span data-stu-id="b4003-114">exclusiveMode</span></span>          | <span data-ttu-id="b4003-115">boolean</span><span class="sxs-lookup"><span data-stu-id="b4003-115">boolean</span></span>                                                   | <span data-ttu-id="b4003-116">Является ли источники без явного источника уровня необходимо удалить из набора.</span><span class="sxs-lookup"><span data-stu-id="b4003-116">Whether sources without explicit source level should be removed from the mix.</span></span>                       |
| <span data-ttu-id="b4003-117">Участник</span><span class="sxs-lookup"><span data-stu-id="b4003-117">participant</span></span>            | <span data-ttu-id="b4003-118">Строка</span><span class="sxs-lookup"><span data-stu-id="b4003-118">String</span></span>                                                    | <span data-ttu-id="b4003-119">Участник, для которого настраивается микшера.</span><span class="sxs-lookup"><span data-stu-id="b4003-119">The participant for whom the mixer is being configured.</span></span>                                             |
| <span data-ttu-id="b4003-120">sourceLevels</span><span class="sxs-lookup"><span data-stu-id="b4003-120">sourceLevels</span></span>           | <span data-ttu-id="b4003-121">[audioSourceLevel](audiosourcelevel.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="b4003-121">[audioSourceLevel](audiosourcelevel.md) collection</span></span>        | <span data-ttu-id="b4003-122">Конфигурации уровня для других источников.</span><span class="sxs-lookup"><span data-stu-id="b4003-122">Level configuration for other sources.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="b4003-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b4003-123">JSON representation</span></span>

<span data-ttu-id="b4003-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4003-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.participantMixerLevel"
}-->
```json
{
  "ducking": { "@odata.type": "#microsoft.graph.audioDuckingConfiguration" },
  "exclusiveMode": true,
  "participant": "String",
  "sourceLevels": [ { "@odata.type": "#microsoft.graph.audioSourceLevel" } ]
}
```

## <a name="example---mixer-level"></a><span data-ttu-id="b4003-125">Пример — уровень микшер</span><span class="sxs-lookup"><span data-stu-id="b4003-125">Example - Mixer level</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.participantMixerLevel"
}-->
```json
{
  "ducking": {
    "@odata.type": "#microsoft.graph.audioDuckingParameters",
    "rampActive": 1000,
    "rampInactive": 1000,
    "lowerLevel": 20,
    "upperLevel": 100
  },
  "exclusiveMode": true,
  "participant": "123456W77E24E4D85F80597083CB830",
  "sourceLevels": [
    {
      "@odata.type": "#microsoft.graph.audioSourceLevel",
      "duckOthers": false,
      "level": 100,
      "participant": "8A34A46B3D174ADC8DCEDC4E7D572698"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participantMixerLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
