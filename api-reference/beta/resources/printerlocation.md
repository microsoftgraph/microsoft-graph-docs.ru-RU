---
title: Тип ресурса printerLocation
description: Представляет физическое и иерархическое расположение принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: bfb082571ab1c5ddf2b46a06c6e66b9e31e47309
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664060"
---
# <a name="printerlocation-resource-type"></a>Тип ресурса printerLocation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет физическое и иерархическое расположение принтера.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|latitude|Double|Широта, в которой расположен принтер.|
|longitude|Double|Долгота, в которую находится принтер.|
|altitudeInMeters|Int32|Высота в метрах, в которую расположен принтер.|
|streetAddress|String|Адрес улицы, где расположен принтер.|
|subUnit|Коллекция строк|Иерархия, в которой расположен принтер. Элементы должны быть в иерархическому порядке. Например, если территории разделены на разные разделы, иерархия может выглядеть так: `["East Wing", "Block A"]`|
|city|String|Город, в который находится принтер.|
|postalCode|String|Почтовый индекс, в который находится принтер.|
|countryOrRegion|String|Страна или регион, где находится принтер.|
|site|String|Сайт, на который расположен принтер.|
|building|String|Здание, в которое находится принтер.|
|floor|String|Пол, на который расположен принтер. В настоящее время поддерживаются только числимые значения.|
|floorDescription|String|Описание этажа, на который расположен принтер.|
|roomName|String|Комната, в которую находится принтер. В настоящее время поддерживаются только числимые значения.|
|roomDescription|String|Описание комнаты, в которую находится принтер.|
|organization;|Коллекция строк|Организационная иерархия, к которой принадлежит принтер. Элементы должны быть в иерархическому порядке.|
|subdivision|Коллекция строк|Подраздел, в который находится принтер. Элементы должны быть в иерархическому порядке.|
|stateOrProvince|String|Область или край, где находится принтер.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerLocation"
}-->

```json
{
    "latitude": 80.1,
    "longitude": -170.1,
    "altitudeInMeters": 123456,
    "streetAddress": "String",
    "subUnit": ["String"],
    "city": "String",
    "postalCode": "String",
    "countryOrRegion": "String",
    "site": "String",
    "building": "String",
    "floor": "123456",
    "floorDescription": "String",
    "roomName": "123456",
    "roomDescription": "String",
    "organization": ["String"],
    "subdivision": ["String"],
    "stateOrProvince": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

