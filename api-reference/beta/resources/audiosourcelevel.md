---
title: Тип ресурса Аудиосаурцелевел
description: Настройка уровня для других источников.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bc2b0c11b18a3cf8120cab0bb9c745ae8880cfc6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339068"
---
# <a name="audiosourcelevel-resource-type"></a>Тип ресурса Аудиосаурцелевел

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Настройка уровня для других источников.

## <a name="properties"></a>Свойства

| Свойство               | Тип    | Описание                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| Дуккосерс             | Логический | Позволяет этому источнику дукк другие источники в активном состоянии. Если задано значение true, необходимо задать уровень дуккинг.|
| степень                  | Int64   | Дуккинг уровень источника, если `duckOthers` задано значение. `true`                                     |
| абонент            | String  | Поток звука участника источника.                                                                |

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
<!--
{
  "type": "#page.annotation",
  "description": "audioSourceLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
