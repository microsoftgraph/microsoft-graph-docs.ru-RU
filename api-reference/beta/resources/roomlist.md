---
title: Тип ресурса RoomList принимают одиночные
description: Представляет группу комнат, созданных компанией.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3aa89075b93f34ad565d210bee3dff2bfd1ffe81
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521035"
---
# <a name="roomlist-resource-type"></a>Тип ресурса RoomList принимают одиночные

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет группу объектов [комнаты](room.md) , определенных в клиенте.

Производный от [позиции](place.md).

## <a name="methods"></a>Методы

| Метод                              | Возвращаемый тип                  | Описание |
|:------------------------------------|:-----------------------------|:--------|
| [Список мест](../api/place-list.md) | Коллекция запрошенного, производного типа [места](place.md) | Получение коллекции указанного типа объекта **Place** , определенного в клиенте. Например, вы можете получить все комнаты, все списки помещений или комнаты в определенном списке помещений в клиенте.|
| [Получение](../api/place-get.md)    | Запрошенный, производный тип [места](place.md)            | Получение свойств и связей указанного объекта **Place** , например списка помещений. |

## <a name="properties"></a>Свойства

| Свойство       | Тип                                              | Описание |
|:---------------|:--------------------------------------------------|:--------|
| address        | [physicalAddress](physicaladdress.md)             | Почтовый адрес списка помещений. |
| displayName    | Строка                                            | Имя, связанное со списком помещений. |
| emailAddress   | String                                            | Адрес электронной почты списка помещений. |
| geoCoordinates | [outlookGeoCoordinates](outlookgeocoordinates.md) | Указывает расположение RoomList принимают одиночные в широте, долготе и (дополнительно) координатах высоты. |
| id             | String                                            | Уникальный идентификатор для списка помещений. Только для чтения. |
| phone          | String                                            | Номер телефона списка помещений. |

## <a name="relationships"></a>Связи

| Связь | Тип                         | Описание          |
|:-------------|:-----------------------------|:---------------------|
| комната        | [помещение](place.md) коллекции | Только для чтения. Допускается значение null. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.roomList"
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "String",
  "emailAddress": "String",
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "id": "String (identifier)",
  "phone": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roomList resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
