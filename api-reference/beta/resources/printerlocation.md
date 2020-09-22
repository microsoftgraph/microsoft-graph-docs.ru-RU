---
title: Тип ресурса Принтерлокатион
description: Представляет физическое и иерархическое расположение принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 49b5221d31951ae35d72422dd4cb88ec254b4b82
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048829"
---
# <a name="printerlocation-resource-type"></a>Тип ресурса Принтерлокатион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет физическое и иерархическое расположение принтера.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|latitude|Double|Широта, в которой расположен принтер.|
|longitude|Double|Долгота, на которой расположен принтер.|
|алтитудеинметерс|Int32|Высота в метрах, на которой расположен принтер.|
|streetAddress|String|Почтовый адрес, где расположен принтер.|
|подединица|Коллекция String|Иерархия подразделений, в которой расположен принтер. Элементы должны находиться в иерархическом порядке. Например, если Кампус делится на несколько разделов, иерархия может выглядеть следующим образом: `["East Wing", "Block A"]`|
|city|String|Город, в котором находится принтер.|
|postalCode|String|Почтовый индекс, в котором находится принтер.|
|countryOrRegion|String|Страна или регион, в котором находится принтер.|
|site|Строка|Сайт, в котором находится принтер.|
|создания|Строка|Построение, в котором находится принтер.|
|флурнумбер|Int32|Номер этажа, на котором расположен принтер.|
|флурдескриптион|Строка|Описание основания, в котором находится принтер.|
|румнумбер|Int32|Номер комнаты, в которой находится принтер.|
|румдескриптион|Строка|Описание комнаты, в которой находится принтер.|
|organization;|Коллекция String|Организационная иерархия, к которой относится принтер. Элементы должны находиться в иерархическом порядке.|
|подразделение|Коллекция String|Подразделение, в котором находится принтер. Элементы должны находиться в иерархическом порядке.|
|stateOrProvince|Строка|Область или край, в котором находится принтер.|

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
    "floorNumber": 123456,
    "floorDescription": "String",
    "roomNumber": 123456,
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

