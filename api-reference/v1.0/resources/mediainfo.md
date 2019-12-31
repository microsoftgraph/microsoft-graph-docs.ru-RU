---
title: Тип ресурса Медиаинфо
description: Сведения о мультимедиа, используемые в действиях для запросов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 20134131dba64ad48effa1c95e5d81ab81102805
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913207"
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
