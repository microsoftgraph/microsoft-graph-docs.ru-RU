---
title: Тип ресурса participantMixerLevel
description: Конфигурация микшер уровни для заданного звука участников
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 14804e02766e375568fac03cb97d2eaf76142353
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513769"
---
# <a name="participantmixerlevel-resource-type"></a>Тип ресурса participantMixerLevel

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Конфигурация микшер уровни для заданного звука участников

## <a name="properties"></a>Свойства

| Свойство               | Тип                                                      | Описание                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| Уклонение от                | [audioDuckingConfiguration](audioduckingconfiguration.md) | Конфигурация (синхронизацию и) из других источников для этой partipant пользовательский набор Уклонение от.       |
| exclusiveMode          | boolean                                                   | Является ли источники без явного источника уровня необходимо удалить из набора.                       |
| Участник            | String                                                    | Участник, для которого настраивается микшера.                                             |
| sourceLevels           | [audioSourceLevel](audiosourcelevel.md) коллекции        | Конфигурации уровня для других источников.                                                              |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

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

## <a name="example---mixer-level"></a>Пример — уровень микшер

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
