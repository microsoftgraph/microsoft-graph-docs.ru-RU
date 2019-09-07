---
title: Тип ресурса Каллмедиастате
description: Представляет состояние мультимедиа для вызова.
author: VinodRavichandran
ms.prod: microsoft-teams
localization_priority: Normal
doc_type: resourcePageType
ms.openlocfilehash: 6b092598c50663ec9e7803a13332798d05fe095b
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36793035"
---
# <a name="audioconferencing-resource-type"></a>Тип ресурса АудиоконференЦинг

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет состояние [звонка для вызова](call.md).

## <a name="properties"></a>Свойства

| Свойство            | Тип    | Описание                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| audio           | String.  | Состояние звукового носителя. Возможные значения: `active`, `inactive`. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callMediaState"
}-->
```json
{
  "audio": "active | inactive",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callMediaState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
