---
title: тип ресурса printerLocation
description: Представляет физическое и иерархическое расположение принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: c642c60cd148d7826432672d1bdef198c230e2a82f483299cbb7773bc2583d6d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54149718"
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
|subUnit|Коллекция String|Иерархия подразделения, в которой расположен принтер. Элементы должны быть в иерархичном порядке. Например, если кампус разделен на разные разделы, иерархия может выглядеть так: `["East Wing", "Block A"]`|
|city|String|Город, в который расположен принтер.|
|postalCode|String|Почтовый код, в который находится принтер.|
|countryOrRegion|String|Страна или область, в которую расположен принтер.|
|site|String|Сайт, на который расположен принтер.|
|здание|String|Здание, в которое расположен принтер.|
|floor|String|Пол, на который расположен принтер. Сейчас поддерживаются только численное значение.|
|floorDescription|String|Описание пола, на который расположен принтер.|
|имя roomName|String|Комната, в которую расположен принтер. Сейчас поддерживаются только численное значение.|
|roomDescription|String|Описание комнаты, в которую расположен принтер.|
|organization;|Коллекция String|Иерархия организации, к которой принадлежит принтер. Элементы должны быть в иерархичном порядке.|
|подразделение|Коллекция строк|Подразделение, в которое расположен принтер. Элементы должны быть в иерархичном порядке.|
|stateOrProvince|String|Состояние или область, в которую расположен принтер.|

## <a name="relationships"></a>Связи
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

