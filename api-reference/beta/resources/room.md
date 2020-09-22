---
title: Тип ресурса "комната"
description: Задает свойства комнаты в клиенте.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ff64a11b9a4e0e036824df1629f1ae055ade3f9d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016137"
---
# <a name="room-resource-type"></a>Тип ресурса "комната"

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет комнату в клиенте. 

В Exchange Online каждая комната связана с почтовым ящиком комнаты. Производный от [позиции](place.md).

## <a name="methods"></a>Методы

| Метод                              | Возвращаемый тип                  | Описание |
|:------------------------------------|:-----------------------------|:--------|
| [Список мест](../api/place-list.md) | Коллекция запрошенного, производного типа [места](place.md) | Получение коллекции указанного типа объекта **Place** , определенного в клиенте. Например, вы можете получить все комнаты, все списки помещений или комнаты в определенном списке помещений в клиенте. |
| [Получение](../api/place-get.md)    | Запрошенный, производный тип [места](place.md)            | Получение свойств и связей указанного объекта **Place** , например комнаты. |

## <a name="properties"></a>Свойства

| Свойство               | Тип                                              | Описание |
|:-----------------------|:--------------------------------------------------|:--|
| address                | [physicalAddress](physicaladdress.md)             | Почтовый адрес комнаты. |
| аудиодевиценаме        | String                                            | Указывает имя звукового устройства в комнате. |
| букингтипе            | [букингтипе](#bookingtype-values)                | Тип комнаты. Возможные значения: `standard` и `reserved` . |
| создания               | String                                            | Задает имя здания или номер здания, в котором находится комната. |
| мощности               | String                                            | Указывает емкость комнаты. |
| displayName            | String                                            | Имя, связанное с комнатой. |
| дисплайдевиценаме      | String                                            | Задает имя устройства отображения в комнате. |
| emailAddress           | String                                            | Адрес электронной почты комнаты. |
| флурлабел             | String                                            | Задает описательную метку для пола, например P. |
| флурнумбер            | Int32                                             | Указывает номер этажа, в котором находится комната. |
| geoCoordinates         | [outlookGeoCoordinates](outlookgeocoordinates.md) | Указывает расположение комнаты в широте, долготе и дополнительном координатах высоты. |
| id                     | String                                            | Уникальный идентификатор комнаты. Только для чтения. |
| исвхилчаиракцессибле | Boolean                                           | Указывает, является ли комната вхилчаир доступным. |
| label                  | String                                            | Задает описательную метку для комнаты, например номер или имя. |
| прозвищ               | String                                            | Задает псевдоним для комнаты, например "назначение комнаты". |
| phone                  | String                                            | Номер телефона комнаты. |
| tags                   | Коллекция String                                 | Задает дополнительные функции комнаты, например, сведения, например тип представления или тип мебели. |
| видеодевиценаме        | String                                            | Задает имя видеоустройства в комнате. |

### <a name="bookingtype-values"></a>значения Букингтипе

| Значение    | Описание                                               |
|:---------|:----------------------------------------------------------|
| Стандартный | Комнату можно зарезервировать в соответствии с другими параметрами в этом командлете. Это значение используется по умолчанию. |
| резервирования | Комната доступна только в первый поступающий, первый обслуживаемый. Оно не может быть зарезервировано.|

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.room",
  "baseType": ""
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "audioDeviceName": "String",
  "bookingType": "String",
  "building": "String",
  "capacity": "String",
  "displayName": "String",
  "displayDeviceName": "String",
  "emailAddress": "String",
  "floorLabel": "String",
  "floorNumber": 1024,
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "id": "String (identifier)",
  "isWheelchairAccessible": true,
  "label": "String",
  "nickname": "String",
  "phone": "String",
  "tags": ["String"],
  "videoDeviceName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "room resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


