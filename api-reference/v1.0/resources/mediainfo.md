---
title: тип ресурса mediaInfo
description: Сведения о средствах массовой информации, используемые в действиях для подсказок.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8d3a03604a608963c3d5ead22b523f0b8ce3d0979aa34666f4470bad5b61fad1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141429"
---
# <a name="mediainfo-resource-type"></a>тип ресурса mediaInfo

Пространство имен: microsoft.graph

Сведения о средствах массовой информации, используемые в действиях для подсказок.

## <a name="properties"></a>Свойства
| Свойство       | Тип    | Описание                      |
|:---------------|:--------|:---------------------------------|
| resourceId     | String  | Необязательный параметр. Используется для уникальной идентификации ресурса. Если он будет передан, запросный uri будет кэшным для этого ресурсаId в качестве ключа. |
| uri            | String  | Путь к запросу, который будет играть. В настоящее время поддерживается только формат wave file (.wav), одноканал, 16-разрядные образцы с частотой выборки 16 000 (16 КГц). |


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

