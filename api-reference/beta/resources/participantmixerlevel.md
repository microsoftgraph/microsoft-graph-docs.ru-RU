---
title: Тип ресурса participantMixerLevel
description: Конфигурация микшер уровни для заданного звука участников
ms.openlocfilehash: 920c22cf423391d2efcdf7177fdc7491250d0f19
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082461"
---
# <a name="participantmixerlevel-resource-type"></a>Тип ресурса participantMixerLevel

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Конфигурация микшер уровни для заданного звука участников

## <a name="properties"></a>Свойства

| Свойство               | Тип                                                      | Description                                                                                         |
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
<!-- {
  "type": "#page.annotation",
  "description": "participantMixerLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
