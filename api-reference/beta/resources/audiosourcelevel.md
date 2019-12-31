---
title: Тип ресурса Аудиосаурцелевел
description: Настройка уровня для других источников.
author: ananmishr
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 35997bfcae7f33cc9bf8e62121c5dc2a724c95be
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913746"
---
# <a name="audiosourcelevel-resource-type"></a>Тип ресурса Аудиосаурцелевел

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Настройка уровня для других источников.

## <a name="properties"></a>Свойства

| Свойство               | Тип    | Описание                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| дуккосерс             | Boolean | Позволяет этому источнику дукк другие источники в активном состоянии. Если задано значение true, необходимо задать уровень дуккинг.|
| степень                  | Int64   | Дуккинг уровень источника, если `duckOthers` задано значение. `true`                                     |
| participant            | String  | Поток звука участника источника.                                                                |

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
