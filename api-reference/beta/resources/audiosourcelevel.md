---
title: Тип ресурса Аудиосаурцелевел
description: Настройка уровня для других источников.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c91a4c57b283f7669b2be22bba5de5d958b437ad
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535597"
---
# <a name="audiosourcelevel-resource-type"></a>Тип ресурса Аудиосаурцелевел

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Настройка уровня для других источников.

## <a name="properties"></a>Свойства

| Свойство               | Тип    | Описание                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| Дуккосерс             | Логический | Позволяет этому источнику дукк другие источники в активном состоянии. Если задано значение true, необходимо задать уровень дуккинг.|
| level                  | Int64   | Дуккинг уровень источника, если `duckOthers` задано значение. `true`                                     |
| абонент            | String  | Поток звука участника источника.                                                                |

## <a name="json-representation"></a>Представление в формате JSON

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
  "suppressions": [
    "Error: /api-reference/beta/resources/audiosourcelevel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
