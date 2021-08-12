---
title: тип ресурса комнаты
description: Указывает свойства комнаты в клиенте.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 051fcfc0f9a5211ae2210eee6c7942d9b7d9efd6b334ea6491a406982e9224a1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54246600"
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
| audioDeviceName        | String                                            | Указывает имя звукового устройства в комнате. |
| bookingType            | [bookingType](#bookingtype-values)                | Тип комнаты. Возможные значения , `standard` и `reserved` . |
| здание               | String                                            | Указывает имя здания или номер здания, в который находится комната. |
| емкость               | Int32                                             | Указывает емкость комнаты. |
| displayName            | String                                            | Имя, связанное с комнатой. |
| displayDeviceName      | String                                            | Указывает имя отображаемого устройства в комнате. |
| emailAddress           | String                                            | Адрес электронной почты комнаты. |
| floorLabel             | String                                            | Указывает описательный метку для пола, например P. |
| floorNumber            | Int32                                             | Указывает номер пола, на который находится номер. |
| geoCoordinates         | [outlookGeoCoordinates](outlookgeocoordinates.md) | Указывает расположение комнаты в широте, долготе и необязательных координатах высоты. |
| id                     | String                                            | Уникальный идентификатор для комнаты. Только для чтения. |
| isWheelChairAccessible | Логический                                           | Указывает, доступна ли комната для инвалидных колясок. |
| label                  | String                                            | Указывает описательный метку для комнаты, например номер или имя. |
| nickname               | String                                            | Указывает псевдоним для комнаты, например " conf room". |
| phone                  | String                                            | Номер телефона комнаты. |
| tags                   | Коллекция String                                 | Указывает дополнительные функции комнаты, например, такие сведения, как тип представления или тип мебели. |
| videoDeviceName        | String                                            | Указывает имя видео устройства в комнате. |

### <a name="bookingtype-values"></a>Значения bookingType

| Значение    | Описание                                               |
|:---------|:----------------------------------------------------------|
| стандартный | Комната доступна и может быть зарезервирована. Это значение используется по умолчанию. |
| зарезервировано | Номер доступен только с первого прибытого, сначала обслуживаемого. Его нельзя зарезервировать.|

## <a name="relationships"></a>Связи

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

