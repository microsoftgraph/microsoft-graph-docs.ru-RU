---
title: Тип ресурса Сервицехостедмедиаконфиг
description: Удаленно размещенный носитель.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 405f6b40260908d7492a3b02c8535588c8475ca8
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870091"
---
# <a name="servicehostedmediaconfig-resource-type"></a>Тип ресурса Сервицехостедмедиаконфиг

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удаленно размещенный носитель. Это наследуется от [медиаконфиг](mediaconfig.md).

## <a name="properties"></a>Свойства

| Свойство                    | Тип                                                        | Описание                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| префетчмедиа               | Коллекция [медиаинфо](mediainfo.md)                        | Список носителей для предварительной загрузки.                   |
| ремовефромдефаултаудиограуп | Логический                                                     | Удаление самостоятельного участника из группы "звук" по умолчанию. |

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
