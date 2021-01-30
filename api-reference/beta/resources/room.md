---
title: Тип ресурса room
description: Указывает свойства комнаты в клиенте.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 39e1bf097519f143bc2eeb1a825fc963d49fd359
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059562"
---
# <a name="room-resource-type"></a>Тип ресурса room

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет комнату в клиенте. 

В Exchange Online каждая комната связана с почтовым ящиком помещения. Является производным от [места.](place.md)

## <a name="methods"></a>Методы

| Метод                              | Возвращаемый тип                  | Описание |
|:------------------------------------|:-----------------------------|:--------|
| [Места списка](../api/place-list.md) | Коллекция запрашиваемого производного типа [места](place.md) | Получите коллекцию указанного типа объекта **place,** определенного в клиенте. Например, можно получить все комнаты, все списки помещений или комнаты в определенном списке помещений в клиенте. |
| [Получить место](../api/place-get.md)    | Запрашиваемая производная тип [места](place.md)            | Получите свойства и связи объекта указанного **места,** например помещения. |

## <a name="properties"></a>Свойства

| Свойство               | Тип                                              | Описание |
|:-----------------------|:--------------------------------------------------|:--|
| address                | [physicalAddress](physicaladdress.md)             | Адрес улицы помещения. |
| audioDeviceName        | String                                            | Указывает имя звукового устройства в комнате. |
| bookingType            | [bookingType](#bookingtype-values)                | Тип комнаты. Возможные значения: `standard` и `reserved` . |
| building               | String                                            | Указывает имя здания или номер здания, в который находится помещение. |
| capacity               | Int32                                             | Указывает емкость комнаты. |
| displayName            | String                                            | Имя, связанное с комнатой. |
| displayDeviceName      | String                                            | Указывает имя устройства отображения в комнате. |
| emailAddress           | String                                            | Адрес электронной почты помещения. |
| floorLabel             | String                                            | Указывает описательную метку для полу, например P. |
| floorNumber            | Int32                                             | Указывает номер этажа, на который находится комната. |
| geoCoordinates         | [outlookGeoCoordinates](outlookgeocoordinates.md) | Указывает расположение помещения в широте, долготе и при желании в координатах высоты. |
| id                     | String                                            | Уникальный идентификатор комнаты. Только для чтения. |
| isWheelChairAccessible | Boolean                                           | Указывает, доступна ли комната. |
| label                  | String                                            | Указывает описательную метку для комнаты, например номер или имя. |
| nickname               | String                                            | Указывает псевдоним для комнаты, например "conf room". |
| phone                  | String                                            | Номер телефона комнаты. |
| tags                   | Коллекция объектов string                                 | Указывает дополнительные функции комнаты, например сведения о типе представления или типе ветвя. |
| videoDeviceName        | String                                            | Указывает имя видео устройства в комнате. |

### <a name="bookingtype-values"></a>Значения bookingType

| Значение    | Описание                                               |
|:---------|:----------------------------------------------------------|
| standard | Комната может быть зарезервирована в зависимости от других параметров этого cmdlet. Это значение используется по умолчанию. |
| reserved | Комната доступна только при первом веданном помещении. Его нельзя зарезервировать.|

## <a name="relationships"></a>Связи

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
  "capacity": 1024,
  "displayName": "String",
  "displayDeviceName": "String",
  "emailAddress": "String",
  "floorLabel": "String",
  "floorNumber": 1024,
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "id": "String (identifier)",
  "isWheelChairAccessible": true,
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


