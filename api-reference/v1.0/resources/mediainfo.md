---
title: тип ресурса mediaInfo
description: Сведения о средствах массовой информации, используемые в действиях для подсказок.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 40bde8c230843156d51b90db64a7e210686886f4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59108956"
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

