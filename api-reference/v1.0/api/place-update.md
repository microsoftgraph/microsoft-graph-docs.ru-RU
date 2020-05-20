---
title: Обновление места
description: Обновление свойств объекта Place.
localization_priority: Normal
author: vrod9429
ms.prod: Outlook
doc_type: apiPageType
ms.openlocfilehash: 3caf019dd8966ca6bbeba9f3a150b2bdbc552925
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288889"
---
# <a name="update-place"></a>Обновление места

Пространство имен: microsoft.graph


Обновление свойств объекта [Place](../resources/place.md) , который может быть [комнатой](../resources/room.md) или [RoomList принимают одиночные](../resources/roomlist.md). Можно определить **комнату** или **RoomList принимают одиночные** , указав свойство **ID** или **EmailAddress** .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Поместите. ReadWrite. ALL. |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /places/{id | emailAddress}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Значение|
|:-----------|:------|
| Авторизация  | Bearer {токен}. Обязательный. |
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. За один раз можно обновить только один экземпляр ресурса "помещение" (**комната** или **RoomList принимают одиночные**). В тексте запроса `@odata.type` Укажите тип размещения и включите свойства этого типа для обновления. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство               | Тип                                              | Описание |
|:-----------------------|:--------------------------------------------------|:--|
| address                | [physicalAddress](../resources/physicaladdress.md)             | Почтовый адрес комнаты или RoomList принимают одиночные. |
| аудиодевиценаме        | String                                            | Указывает имя звукового устройства в комнате. |
| букингтипе            | [букингтипе](../resources/room.md)                            | Тип комнаты. Возможные значения: `Standard` и `Reserved`. |
| создания               | String                                            | Задает имя здания или номер здания, в котором находится комната. |
| мощности               | String                                            | Указывает емкость комнаты. |
| дисплайдевиценаме      | String                                            | Задает имя устройства отображения в комнате. |
| флурлабел             | String                                            | Указывает этаж, в котором находится комната. |
| флурнумбер            | Int32                                             | Указывает номер этажа, в котором находится комната. |
| geoCoordinates         | [outlookGeoCoordinates](../resources/outlookgeocoordinates.md) | Указывает место в комнате или RoomList принимают одиночные в широте, долготе и дополнительном координатах высоты. |
| исвхилчаиракцессибле | Логический                                           | Указывает, является ли комната вхилчаир доступным. |
| label                  | String                                            | Задает описательную метку для комнаты, например номер или имя. |
| прозвищ               | String                                            | Задает псевдоним для комнаты, например "назначение комнаты". |
| phone                  | String                                            | Номер телефона комнаты или RoomList принимают одиночные. |
| tags                   | Коллекция String                                 | Задает дополнительные функции комнаты, например, сведения, например тип представления или тип мебели. |
| видеодевиценаме        | String                                            | Задает имя видеоустройства в комнате. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [Place](../resources/place.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-update-a-room"></a>Пример 1: обновление комнаты

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


<!-- {
  "blockType": "request",
  "name": "update_room"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/places/cf100@contoso.com
Content-type: application/json
Content-length: 285

{
  "@odata.type": "microsoft.graph.room",
  "nickname": "Conf Room",
  "building": "1",
  "label": "100",
  "capacity": "50",
  "isWheelchairAccessible": false
}
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> [!NOTE]
> Объект Response, показанный здесь, может быть укорочен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.room"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#places/$entity",
    "@odata.type": "#microsoft.graph.room",
    "id": "3162F1E1-C4C0-604B-51D8-91DA78989EB1",
    "emailAddress": "cf100@contoso.com",
    "displayName": "Conf Room 100",
    "address": {
      "street": "4567 Main Street",
      "city": "Buffalo",
      "state": "NY",
      "postalCode": "98052",
      "countryOrRegion": "USA"
    },
    "geoCoordinates": {
      "latitude": 47.0,
      "longitude": -122.0
    },
    "phone": "555-555-0100",
    "nickname": "Conf Room",
    "label": "100",
    "capacity": "50",
    "building": "1",
    "floorLabel": "1P",
    "floorNumber": 1,
    "isManaged": true,
    "isWheelchairAccessible": false,
    "bookingType": "standard",
    "tags": [
      "bean bags"
    ],
    "audioDeviceName": null,
    "videoDeviceName": null,
    "displayDevice": "surface hub"
}
```

### <a name="example-2-update-a-roomlist"></a>Пример 2: обновление объекта RoomList принимают одиночные

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "update_roomlist"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/places/Building1RroomList@contoso.onmicrosoft.com
Content-type: application/json

{
  "@odata.type": "microsoft.graph.roomlist",
  "displayName": "Building 1",
  "phone":"555-555-0100",
  "address": {
    "street": "4567 Main Street",
    "city": "Buffalo",
    "state": "NY",
    "postalCode": "98052",
    "countryOrRegion": "USA"
  },
  "geoCoordinates": {
    "altitude": null,
    "latitude": 47.0,
    "longitude": -122.0,
    "accuracy": null,
    "altitudeAccuracy": null
 }
}
```


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> [!NOTE]
> Объект Response, показанный здесь, может быть укорочен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.roomList"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#places/$entity",
  "@odata.type": "#microsoft.graph.roomList",
  "id": "DC404124-302A-92AA-F98D-7B4DEB0C1705",
  "displayName": "Building 1",
  "address": {
    "street": "4567 Main Street",
    "city": "Buffalo",
    "state": "NY",
    "postalCode": "98052",
    "countryOrRegion": "USA"
  },
  "geoCoordinates": {
    "altitude": null,
    "latitude": 47.0,
    "longitude": -122.0,
    "accuracy": null,
    "altitudeAccuracy": null
 },
  "phone": "555-555-0100",
  "emailAddress": "bldg1@contoso.com"
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update place",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
