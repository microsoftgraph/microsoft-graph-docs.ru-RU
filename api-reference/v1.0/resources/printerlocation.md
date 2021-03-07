---
title: тип ресурса printerLocation
description: Представляет физическое и иерархическое расположение принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: f357ab3b33182ac6ffb2f8ae705a359a0e955eed
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517367"
---
# <a name="printerlocation-resource-type"></a>тип ресурса printerLocation

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Представляет физическое и иерархическое расположение принтера.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|latitude|Double|Широта, на которой расположен принтер.|
|longitude|Double|Долгота, на которую расположен принтер.|
|altitudeInMeters|Int32|Высота в метрах, на которую расположен принтер.|
|streetAddress|String|Адрес улицы, где расположен принтер.|
|subUnit|Коллекция строк|Иерархия подразделения, в которой расположен принтер. Элементы должны быть в иерархичном порядке. Например, если кампус разделен на разные разделы, иерархия может выглядеть так: `["East Wing", "Block A"]`|
|city|String|Город, в который расположен принтер.|
|postalCode|String|Почтовый код, в который находится принтер.|
|countryOrRegion|String|Страна или область, в которую расположен принтер.|
|site|Строка|Сайт, на который расположен принтер.|
|здание|Строка|Здание, в которое расположен принтер.|
|floor|Строка|Пол, на который расположен принтер. Сейчас поддерживаются только численное значение.|
|floorDescription|Строка|Описание пола, на который расположен принтер.|
|имя roomName|Строка|Комната, в которую расположен принтер. Сейчас поддерживаются только численное значение.|
|roomDescription|Строка|Описание комнаты, в которую расположен принтер.|
|organization;|Коллекция строк|Иерархия организации, к которой принадлежит принтер. Элементы должны быть в иерархичном порядке.|
|подразделение|Коллекция строк|Подразделение, в которое расположен принтер. Элементы должны быть в иерархичном порядке.|
|stateOrProvince|Строка|Состояние или область, в которую расположен принтер.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerLocation",
  "latitude": "Double",
  "longitude": "Double",
  "altitudeInMeters": "Integer",
  "streetAddress": "String",
  "subunit": [
    "String"
  ],
  "city": "String",
  "postalCode": "String",
  "countryOrRegion": "String",
  "site": "String",
  "building": "String",
  "floor": "String",
  "floorDescription": "String",
  "roomName": "String",
  "roomDescription": "String",
  "organization": [
    "String"
  ],
  "subdivision": [
    "String"
  ],
  "stateOrProvince": "String"
}
```

