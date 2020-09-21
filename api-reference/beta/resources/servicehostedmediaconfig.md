---
title: Тип ресурса Сервицехостедмедиаконфиг
description: Удаленно размещенный носитель.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d006a4417401859c0c385f9537656993f985198d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023958"
---
# <a name="servicehostedmediaconfig-resource-type"></a>Тип ресурса Сервицехостедмедиаконфиг

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удаленно размещенный носитель. Это наследуется от [медиаконфиг](mediaconfig.md).

## <a name="properties"></a>Свойства

| Свойство                    | Тип                                                        | Описание                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| префетчмедиа               | Коллекция [медиаинфо](mediainfo.md)                        | Список носителей для предварительной загрузки.                   |
| ремовефромдефаултаудиограуп | Boolean                                                     | Удаление самостоятельного участника из группы "звук" по умолчанию. |

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
  "preFetchMedia": [ { "@odata.type": "microsoft.graph.mediaInfo" } ],
  "removeFromDefaultAudioGroup": true
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


