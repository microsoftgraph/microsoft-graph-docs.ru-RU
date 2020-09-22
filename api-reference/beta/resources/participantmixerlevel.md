---
title: Тип ресурса ПартиЦипантмиксерлевел
description: Настройка уровней микшера для данного участника аудио
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: fdec09b80eddfc4a4ea3f87425c211ed49f22ded
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998238"
---
# <a name="participantmixerlevel-resource-type"></a>Тип ресурса ПартиЦипантмиксерлевел

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Настройка уровней микшера для данного участника аудио

## <a name="properties"></a>Свойства

| Свойство               | Тип                                                      | Описание                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| дуккинг                | [аудиодуккингконфигуратион](audioduckingconfiguration.md) | Конфигурация дуккинг (фасинг in и out) других источников для этого партипант настраиваемого набора.       |
| ексклусивемоде          | boolean                                                   | Следует ли удалять источники без явного исходного уровня из набора.                       |
| participant            | String                                                    | Участник, для которого настраивается микшер.                                             |
| саурцелевелс           | Коллекция [аудиосаурцелевел](audiosourcelevel.md)        | Настройка уровня для других источников.                                                              |

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

## <a name="example---mixer-level"></a>Пример — уровень микшера

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


