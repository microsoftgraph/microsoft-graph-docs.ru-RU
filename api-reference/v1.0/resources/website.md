---
title: Тип ресурса веб-сайта
description: Представляет веб-сайт.
localization_priority: Normal
author: AAmatino
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f6e237756f96df9ed0592ab38cf7af04e0fb43f90323e1b63ffc9902d4a329a1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196462"
---
# <a name="website-resource-type"></a>Тип ресурса веб-сайта

Пространство имен: microsoft.graph

Представляет веб-сайт.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|type|websiteType| Допустимые значения: `other`, `home`, `work`, `blog`, `profile`.|
|address|string|URL-адрес веб-сайта.|
|displayName|string|Отображение имени веб-сайта.|

## <a name="json-representation"></a>Представление JSON

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

