---
title: Тип ресурса Каллмедиастате
description: Представляет состояние мультимедиа для вызова.
author: ananmishr
ms.prod: cloud-communications
localization_priority: Normal
doc_type: resourcePageType
ms.openlocfilehash: b73f6110639cfb158bef8e5f529d9a2c65b34689
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913466"
---
# <a name="callmediastate-resource-type"></a>Тип ресурса Каллмедиастате


Представляет состояние мультимедиа для [вызова](call.md).

## <a name="properties"></a>Свойства

| Свойство            | Тип    | Описание                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| audio           | String  | Состояние звукового носителя. Возможные значения: `active`, `inactive`. |

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
