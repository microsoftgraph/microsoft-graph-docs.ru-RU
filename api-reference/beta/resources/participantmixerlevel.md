---
title: Тип ресурса ПартиЦипантмиксерлевел
description: Настройка уровней микшера для данного участника аудио
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cc305274d619a3686d4d391516947f1d06b92745
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006587"
---
# <a name="participantmixerlevel-resource-type"></a><span data-ttu-id="82fe0-103">Тип ресурса ПартиЦипантмиксерлевел</span><span class="sxs-lookup"><span data-stu-id="82fe0-103">participantMixerLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82fe0-104">Настройка уровней микшера для данного участника аудио</span><span class="sxs-lookup"><span data-stu-id="82fe0-104">Configuration of mixer levels for given audio participant</span></span>

## <a name="properties"></a><span data-ttu-id="82fe0-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="82fe0-105">Properties</span></span>

| <span data-ttu-id="82fe0-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="82fe0-106">Property</span></span>               | <span data-ttu-id="82fe0-107">Тип</span><span class="sxs-lookup"><span data-stu-id="82fe0-107">Type</span></span>                                                      | <span data-ttu-id="82fe0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="82fe0-108">Description</span></span>                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="82fe0-109">дуккинг</span><span class="sxs-lookup"><span data-stu-id="82fe0-109">ducking</span></span>                | [<span data-ttu-id="82fe0-110">аудиодуккингконфигуратион</span><span class="sxs-lookup"><span data-stu-id="82fe0-110">audioDuckingConfiguration</span></span>](audioduckingconfiguration.md) | <span data-ttu-id="82fe0-111">Конфигурация дуккинг (фасинг in и out) других источников для этого партипант настраиваемого набора.</span><span class="sxs-lookup"><span data-stu-id="82fe0-111">Configuration of ducking (phasing in and out) of other sources for this partipant custom mix.</span></span>       |
| <span data-ttu-id="82fe0-112">ексклусивемоде</span><span class="sxs-lookup"><span data-stu-id="82fe0-112">exclusiveMode</span></span>          | <span data-ttu-id="82fe0-113">boolean</span><span class="sxs-lookup"><span data-stu-id="82fe0-113">boolean</span></span>                                                   | <span data-ttu-id="82fe0-114">Следует ли удалять источники без явного исходного уровня из набора.</span><span class="sxs-lookup"><span data-stu-id="82fe0-114">Whether sources without explicit source level should be removed from the mix.</span></span>                       |
| <span data-ttu-id="82fe0-115">participant</span><span class="sxs-lookup"><span data-stu-id="82fe0-115">participant</span></span>            | <span data-ttu-id="82fe0-116">String</span><span class="sxs-lookup"><span data-stu-id="82fe0-116">String</span></span>                                                    | <span data-ttu-id="82fe0-117">Участник, для которого настраивается микшер.</span><span class="sxs-lookup"><span data-stu-id="82fe0-117">The participant for whom the mixer is being configured.</span></span>                                             |
| <span data-ttu-id="82fe0-118">саурцелевелс</span><span class="sxs-lookup"><span data-stu-id="82fe0-118">sourceLevels</span></span>           | <span data-ttu-id="82fe0-119">Коллекция [аудиосаурцелевел](audiosourcelevel.md)</span><span class="sxs-lookup"><span data-stu-id="82fe0-119">[audioSourceLevel](audiosourcelevel.md) collection</span></span>        | <span data-ttu-id="82fe0-120">Настройка уровня для других источников.</span><span class="sxs-lookup"><span data-stu-id="82fe0-120">Level configuration for other sources.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="82fe0-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="82fe0-121">JSON representation</span></span>

<span data-ttu-id="82fe0-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82fe0-122">The following is a JSON representation of the resource.</span></span>

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

## <a name="example---mixer-level"></a><span data-ttu-id="82fe0-123">Пример — уровень микшера</span><span class="sxs-lookup"><span data-stu-id="82fe0-123">Example - Mixer level</span></span>

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
