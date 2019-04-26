---
title: Тип ресурса ПартиЦипантмиксерлевел
description: Настройка уровней микшера для данного участника аудио
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 14804e02766e375568fac03cb97d2eaf76142353
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568626"
---
# <a name="participantmixerlevel-resource-type"></a><span data-ttu-id="566d2-103">Тип ресурса ПартиЦипантмиксерлевел</span><span class="sxs-lookup"><span data-stu-id="566d2-103">participantMixerLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="566d2-104">Настройка уровней микшера для данного участника аудио</span><span class="sxs-lookup"><span data-stu-id="566d2-104">Configuration of mixer levels for given audio participant</span></span>

## <a name="properties"></a><span data-ttu-id="566d2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="566d2-105">Properties</span></span>

| <span data-ttu-id="566d2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="566d2-106">Property</span></span>               | <span data-ttu-id="566d2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="566d2-107">Type</span></span>                                                      | <span data-ttu-id="566d2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="566d2-108">Description</span></span>                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="566d2-109">дуккинг</span><span class="sxs-lookup"><span data-stu-id="566d2-109">ducking</span></span>                | [<span data-ttu-id="566d2-110">Аудиодуккингконфигуратион</span><span class="sxs-lookup"><span data-stu-id="566d2-110">audioDuckingConfiguration</span></span>](audioduckingconfiguration.md) | <span data-ttu-id="566d2-111">Конфигурация дуккинг (фасинг in и out) других источников для этого партипант настраиваемого набора.</span><span class="sxs-lookup"><span data-stu-id="566d2-111">Configuration of ducking (phasing in and out) of other sources for this partipant custom mix.</span></span>       |
| <span data-ttu-id="566d2-112">Ексклусивемоде</span><span class="sxs-lookup"><span data-stu-id="566d2-112">exclusiveMode</span></span>          | <span data-ttu-id="566d2-113">boolean</span><span class="sxs-lookup"><span data-stu-id="566d2-113">boolean</span></span>                                                   | <span data-ttu-id="566d2-114">Следует ли удалять источники без явного исходного уровня из набора.</span><span class="sxs-lookup"><span data-stu-id="566d2-114">Whether sources without explicit source level should be removed from the mix.</span></span>                       |
| <span data-ttu-id="566d2-115">абонент</span><span class="sxs-lookup"><span data-stu-id="566d2-115">participant</span></span>            | <span data-ttu-id="566d2-116">String</span><span class="sxs-lookup"><span data-stu-id="566d2-116">String</span></span>                                                    | <span data-ttu-id="566d2-117">Участник, для которого настраивается микшер.</span><span class="sxs-lookup"><span data-stu-id="566d2-117">The participant for whom the mixer is being configured.</span></span>                                             |
| <span data-ttu-id="566d2-118">Саурцелевелс</span><span class="sxs-lookup"><span data-stu-id="566d2-118">sourceLevels</span></span>           | <span data-ttu-id="566d2-119">Коллекция [аудиосаурцелевел](audiosourcelevel.md)</span><span class="sxs-lookup"><span data-stu-id="566d2-119">[audioSourceLevel](audiosourcelevel.md) collection</span></span>        | <span data-ttu-id="566d2-120">Настройка уровня для других источников.</span><span class="sxs-lookup"><span data-stu-id="566d2-120">Level configuration for other sources.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="566d2-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="566d2-121">JSON representation</span></span>

<span data-ttu-id="566d2-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="566d2-122">The following is a JSON representation of the resource.</span></span>

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

## <a name="example---mixer-level"></a><span data-ttu-id="566d2-123">Пример — уровень микшера</span><span class="sxs-lookup"><span data-stu-id="566d2-123">Example - Mixer level</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/participantmixerlevel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
