---
title: Тип ресурса Медиаинфо
description: Сведения о мультимедиа, используемые в действиях для запросов.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9d9b8f4709d3379afda8e30fec2b7db64a474a0e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866267"
---
# <a name="mediainfo-resource-type"></a>Тип ресурса Медиаинфо

Сведения о мультимедиа, используемые в действиях для запросов.

## <a name="properties"></a>Свойства
| Свойство       | Тип    | Описание                      |
|:---------------|:--------|:---------------------------------|
| resourceId     | String  | Необязательный параметр. Используется для уникальной идентификации ресурса. Если передается, URI приглашения кэшируется для этого resourceId в качестве ключа. |
| URI            | String  | Путь к приглашению, который будет воспроизводиться. В настоящее время поддерживается только формат волнового файла (WAV), одноканальный 16-разрядный пример с частотой выборки 16 000 (16 кГц). |


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
<!--
{
  "type": "#page.annotation",
  "description": "mediaInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
