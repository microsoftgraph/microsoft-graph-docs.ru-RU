---
title: Тип ресурса Сервицехостедмедиаконфиг
description: Тип Сервицехостедмедиаконфиг.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 35d5754071aa388e300042b9977fd759a38a6b74
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912953"
---
# <a name="servicehostedmediaconfig-resource-type"></a>Тип ресурса Сервицехостедмедиаконфиг

Удаленно размещенный носитель. Это наследуется от [медиаконфиг](mediaconfig.md).

## <a name="properties"></a>Свойства

| Свойство                    | Тип                                                        | Описание                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| префетчмедиа               | Коллекция [медиаинфо](mediainfo.md)                        | Список носителей для предварительной загрузки.                   |


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "preFetchMedia"
  ],
  "baseType": "microsoft.graph.mediaConfig",
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [ { "@odata.type": "microsoft.graph.mediaInfo" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "serviceHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
