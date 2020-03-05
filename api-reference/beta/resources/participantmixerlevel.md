---
title: Тип ресурса ПартиЦипантмиксерлевел
description: Настройка уровней микшера для данного участника аудио
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 31e4ec08014907480cfe7bafaa21b061ec1434b6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522027"
---
# <a name="participantmixerlevel-resource-type"></a><span data-ttu-id="4b123-103">Тип ресурса ПартиЦипантмиксерлевел</span><span class="sxs-lookup"><span data-stu-id="4b123-103">participantMixerLevel resource type</span></span>

<span data-ttu-id="4b123-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4b123-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b123-105">Настройка уровней микшера для данного участника аудио</span><span class="sxs-lookup"><span data-stu-id="4b123-105">Configuration of mixer levels for given audio participant</span></span>

## <a name="properties"></a><span data-ttu-id="4b123-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b123-106">Properties</span></span>

| <span data-ttu-id="4b123-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b123-107">Property</span></span>               | <span data-ttu-id="4b123-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4b123-108">Type</span></span>                                                      | <span data-ttu-id="4b123-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4b123-109">Description</span></span>                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4b123-110">дуккинг</span><span class="sxs-lookup"><span data-stu-id="4b123-110">ducking</span></span>                | [<span data-ttu-id="4b123-111">аудиодуккингконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4b123-111">audioDuckingConfiguration</span></span>](audioduckingconfiguration.md) | <span data-ttu-id="4b123-112">Конфигурация дуккинг (фасинг in и out) других источников для этого партипант настраиваемого набора.</span><span class="sxs-lookup"><span data-stu-id="4b123-112">Configuration of ducking (phasing in and out) of other sources for this partipant custom mix.</span></span>       |
| <span data-ttu-id="4b123-113">ексклусивемоде</span><span class="sxs-lookup"><span data-stu-id="4b123-113">exclusiveMode</span></span>          | <span data-ttu-id="4b123-114">boolean</span><span class="sxs-lookup"><span data-stu-id="4b123-114">boolean</span></span>                                                   | <span data-ttu-id="4b123-115">Следует ли удалять источники без явного исходного уровня из набора.</span><span class="sxs-lookup"><span data-stu-id="4b123-115">Whether sources without explicit source level should be removed from the mix.</span></span>                       |
| <span data-ttu-id="4b123-116">participant</span><span class="sxs-lookup"><span data-stu-id="4b123-116">participant</span></span>            | <span data-ttu-id="4b123-117">String</span><span class="sxs-lookup"><span data-stu-id="4b123-117">String</span></span>                                                    | <span data-ttu-id="4b123-118">Участник, для которого настраивается микшер.</span><span class="sxs-lookup"><span data-stu-id="4b123-118">The participant for whom the mixer is being configured.</span></span>                                             |
| <span data-ttu-id="4b123-119">саурцелевелс</span><span class="sxs-lookup"><span data-stu-id="4b123-119">sourceLevels</span></span>           | <span data-ttu-id="4b123-120">Коллекция [аудиосаурцелевел](audiosourcelevel.md)</span><span class="sxs-lookup"><span data-stu-id="4b123-120">[audioSourceLevel](audiosourcelevel.md) collection</span></span>        | <span data-ttu-id="4b123-121">Настройка уровня для других источников.</span><span class="sxs-lookup"><span data-stu-id="4b123-121">Level configuration for other sources.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="4b123-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4b123-122">JSON representation</span></span>

<span data-ttu-id="4b123-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b123-123">The following is a JSON representation of the resource.</span></span>

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

## <a name="example---mixer-level"></a><span data-ttu-id="4b123-124">Пример — уровень микшера</span><span class="sxs-lookup"><span data-stu-id="4b123-124">Example - Mixer level</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "participantMixerLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
