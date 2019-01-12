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
# <a name="audiosourcelevel-resource-type"></a>Тип ресурса audioSourceLevel

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Конфигурации уровня для других источников.

## <a name="properties"></a>Свойства

| Свойство               | Тип    | Описание                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| duckOthers             | Логический | Включение этого источника для duck другие источники при активный. Если значение равно true, Уклонение от уровня должно быть задано.|
| level                  | Int64   | Уклонение от уровня источника, если `duckOthers` задано значение `true`.                                     |
| Участник            | Строка  | Источник участников аудиопотока.                                                                |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

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
