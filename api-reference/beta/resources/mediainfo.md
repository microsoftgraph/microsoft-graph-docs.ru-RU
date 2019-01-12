---
title: Тип ресурса mediaInfo
description: Запрашивает сведения о мультимедиа, используемые в действиях для.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 217b9a5aaa88a1bbf343447fad344b322cfeb611
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924533"
---
# <a name="mediainfo-resource-type"></a>Тип ресурса mediaInfo

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Запрашивает сведения о мультимедиа, используемые в действиях для.

## <a name="properties"></a>Свойства
| Свойство       | Тип    | Описание                      |
|:---------------|:--------|:---------------------------------|
| resourceId     | String  | Уникальный идентификатор ресурса. |
| URI            | Строка  | Путь к ресурсу.            |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaInfo"
}-->
```json
{
  "resourceId": "String",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
