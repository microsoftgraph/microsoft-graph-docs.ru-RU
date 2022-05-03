---
title: Тип ресурса printerLocation
description: Представляет физическое и иерархическое расположение принтера.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 53eeee6e135276ff43e5cd360fbc6615d2df649f
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176610"
---
# <a name="printerlocation-resource-type"></a>Тип ресурса printerLocation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет физическое и иерархическое расположение принтера.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|latitude|Double|Широта принтера.|
|longitude|Double|Долгота, в котором находится принтер.|
|altitudeInMeters|Int32|Высота в метрах, где находится принтер.|
|streetAddress|String|Адрес улицы, где находится принтер.|
|subUnit|Коллекция строк|Иерархия дочерних элементов, в которой расположен принтер. Элементы должны иметь иерархический порядок. Например, если комплекс разделен на разные разделы, иерархия может выглядеть следующим образом: `["East Wing", "Block A"]`|
|city|String|Город, в котором находится принтер.|
|postalCode|String|Почтовый индекс, в котором находится принтер.|
|countryOrRegion|String|Страна или регион, в которых находится принтер.|
|site|Строка|Сайт, на котором находится принтер.|
|Здание|Строка|Здание, в котором находится принтер.|
|floor|Строка|Этаж, на котором находится принтер. Сейчас поддерживаются только числовые значения.|
|floorDescription|Строка|Описание пола, на котором расположен принтер.|
|roomName|Строка|Комната, в котором находится принтер. Сейчас поддерживаются только числовые значения.|
|roomDescription|Строка|Описание комнаты, в котором находится принтер.|
|organization;|Коллекция String|Иерархия организации, к которой принадлежит принтер. Элементы должны иметь иерархический порядок.|
|Подразделение|Коллекция String|Подраздел, в котором находится принтер. Элементы должны иметь иерархический порядок.|
|stateOrProvince|Строка|Штат или край, в котором находится принтер.|

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

