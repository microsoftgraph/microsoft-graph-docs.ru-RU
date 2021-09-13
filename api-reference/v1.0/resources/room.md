---
title: тип ресурса комнаты
description: Указывает свойства комнаты в клиенте.
ms.localizationpriority: medium
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d676dbcd36760bc14edb38b35f6f93573f03b9b5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117776"
---
# <a name="room-resource-type"></a>тип ресурса комнаты

Пространство имен: microsoft.graph

Представляет комнату в клиенте. 

В Exchange Online каждый номер связан с почтовым ящиком комнаты. Производные от [места](place.md).

## <a name="methods"></a>Методы

| Метод                              | Возвращаемый тип                  | Описание |
|:------------------------------------|:-----------------------------|:--------|
| [Места списка](../api/place-list.md) | Коллекция запрашиваемого, производный тип [места](place.md) | Получите коллекцию указанного типа объекта **места,** определенного в клиенте. Например, вы можете получить все комнаты, все списки комнат или комнаты в определенном списке комнат в клиенте. |
| [Получить место](../api/place-get.md)    | Запрашиваемое, производный тип [места](place.md)            | Получите свойства и связи указанного **объекта,** например комнаты. |

## <a name="properties"></a>Свойства

| Свойство               | Тип                                              | Описание |
|:-----------------------|:--------------------------------------------------|:--|
| address                | [physicalAddress](physicaladdress.md)             | Адрес улицы комнаты. |
| audioDeviceName        | Строка                                            | Указывает имя звукового устройства в комнате. |
| bookingType            | [bookingType](#bookingtype-values)                | Тип комнаты. Возможные значения , `standard` и `reserved` . |
| здание               | String                                            | Указывает имя здания или номер здания, в который находится комната. |
| емкость               | Int32                                             | Указывает емкость комнаты. |
| displayName            | String                                            | Имя, связанное с комнатой. |
| displayDeviceName      | Строка                                            | Указывает имя отображаемого устройства в комнате. |
| emailAddress           | String                                            | Адрес электронной почты комнаты. |
| floorLabel             | String                                            | Указывает описательный метку для пола, например P. |
| floorNumber            | Int32                                             | Указывает номер пола, на который находится номер. |
| geoCoordinates         | [outlookGeoCoordinates](outlookgeocoordinates.md) | Указывает расположение комнаты в широте, долготе и необязательных координатах высоты. |
| id                     | Строка                                            | Уникальный идентификатор для комнаты. Только для чтения. |
| isWheelChairAccessible | Логический                                           | Указывает, доступна ли комната для инвалидных колясок. |
| подпись                  | String                                            | Указывает описательный метку для комнаты, например номер или имя. |
| nickname               | String                                            | Указывает псевдоним для комнаты, например " conf room". |
| phone                  | String                                            | Номер телефона комнаты. |
| tags                   | Коллекция String                                 | Указывает дополнительные функции комнаты, например, такие сведения, как тип представления или тип мебели. |
| videoDeviceName        | String                                            | Указывает имя видео устройства в комнате. |

### <a name="bookingtype-values"></a>Значения bookingType

| Значение    | Описание                                               |
|:---------|:----------------------------------------------------------|
| стандартный | Комната доступна и может быть зарезервирована. Это значение используется по умолчанию. |
| зарезервировано | Номер доступен только с первого прибытого, сначала обслуживаемого. Его нельзя зарезервировать.|

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.room"
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

