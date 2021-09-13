---
title: тип ресурса callMediaState
description: Представляет состояние мультимедиа для вызова.
author: ananmishr
ms.prod: cloud-communications
ms.localizationpriority: medium
doc_type: resourcePageType
ms.openlocfilehash: d07562bfaf14a69175535f8b38b73f56fdb0faa8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59104364"
---
# <a name="callmediastate-resource-type"></a>тип ресурса callMediaState

Пространство имен: microsoft.graph


Представляет состояние мультимедиа для [вызова.](call.md)

## <a name="properties"></a>Свойства

| Свойство            | Тип    | Описание                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| audio           | mediaState  | Состояние аудио мультимедиа. Возможные значения: `active`, `inactive`, `unknownFutureValue`. |

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

