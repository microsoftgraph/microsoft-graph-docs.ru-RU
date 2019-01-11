---
title: тип ресурса website
description: Представляет веб-сайт.
localization_priority: Normal
ms.openlocfilehash: 1ffbee8a67527aac97bb4f60b7f8b1637ba1ebe5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851368"
---
# <a name="website-resource-type"></a>тип ресурса website

Представляет веб-сайт.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|type|websiteType| Возможные значения: `other`, `home`, `work`, `blog`, `profile`.|
|address|string|URL-адрес веб-сайта.|
|displayName|строка|Отображаемое имя веб-сайта.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.website"
}-->

```json
{
  "type": "String",
  "address": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "webSite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
