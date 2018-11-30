---
title: тип ресурса website
description: Представляет веб-сайт.
ms.openlocfilehash: 14934aae418581f4c75c880be67bf51fd0bc293c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024938"
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
