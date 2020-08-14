---
title: Обновление принтера
description: Обновление свойств объекта Printer.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 4040174e1f1ad0278dcdfcd1dd94dbe9b6d94b27
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/14/2020
ms.locfileid: "46674402"
---
# <a name="update-printer"></a>Обновление принтера

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [Printer](../resources/printer.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать. Пользователь, вошедшего в систему, должен быть [администратором принтера](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).

Только приложение, которое зарегистрировало принтер, может обновлять принтер с помощью разрешений приложения.

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:---------------|:--------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)| Printer. ReadWrite. ALL, Printer. FullControl. ALL |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений| Printer.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:-----------|:-----------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type  | `application/json` При использовании делегированных разрешений `application/ipp` при использовании разрешений приложения. Обязательный элемент.|

## <a name="request-body"></a>Текст запроса

### <a name="delegated-permissions-and-json-payload"></a>Делегированные разрешения и полезные данные JSON

Если в тексте запроса используется делегированные разрешения, укажите значения для соответствующих полей [принтера](../resources/printer.md) , которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|location|[принтерлокатион](../resources/printerlocation.md)|Физическое и/или организационное расположение принтера.|
|name|String|Имя принтера.|

### <a name="application-permissions-and-ipp-payload"></a>Разрешения приложений и полезные данные IPP

При использовании разрешений приложения текст запроса содержит двоичный поток, представляющий группу атрибутов принтера в [кодировке IPP](https://tools.ietf.org/html/rfc8010).

Клиент должен предоставить набор атрибутов принтера с одним или несколькими значениями (включая явно разрешенные значения из диапазона), как определено в [разделе RFC8011 section 4,2](https://tools.ietf.org/html/rfc8011#section-4.2) атрибуты шаблона задания ("XXX-Default", "XXX-supported" и "XXX-Ready"), [section 4,4](https://tools.ietf.org/html/rfc8011#section-4.4) атрибуты описания принтера и все расширения атрибутов, поддерживаемые принтером. Значения каждого из указанных атрибутов принтера заменяют значения соответствующего атрибута принтера для целевого объекта Printer. Для атрибутов, которые могут иметь несколько значений (1setOf), все значения, предоставляемые клиентом, заменяют все значения атрибута соответствующего объекта Printer.

## <a name="response"></a>Отклик

### <a name="delegated-permissions-and-json-payload"></a>Делегированные разрешения и полезные данные JSON

При успешном использовании делегированных разрешений этот метод возвращает `200 OK` код отклика и обновленный объект [Printer](../resources/printer.md) в тексте отклика.

### <a name="application-permissions-and-ipp-payload"></a>Разрешения приложений и полезные данные IPP

Если при успешном использовании разрешений приложения этот метод возвращает `204 No content` код отклика. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printer"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/printers/{id}
Content-type: application/json
Content-length: 124

{
  "name": "PrinterName",
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1313

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers/$entity",
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "name": "PrinterName",
  "manufacturer": "PrinterManufacturer",
  "model": "PrinterModel",
  "isShared": true,
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
  "acceptingJobs": true,
  "status": {
    "processingState": "idle",
    "processingStateReasons": [],
    "processingStateDescription": ""
  },
  "defaults": {
    "copiesPerJob":1,
    "documentMimeType": "application/oxps",
    "finishings": ["none"],
    "mediaType": "stationery"
  },
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3,
    "streetAddress": "One Microsoft Way",
    "subUnit": [
        "Main Plaza",
        "Unit 400"
    ],
    "city": "Redmond",
    "postalCode": "98052",
    "countryOrRegion": "USA",
    "site": "Puget Sound",
    "building": "Studio E",
    "floorNumber": 1,
    "floorDescription": "First Floor",
    "roomNumber": 1234,
    "roomDescription": "First floor copy room",
    "organization": [
        "C+AI",
        "Microsoft Graph"
    ],
    "subdivision": [
        "King County",
        "Red West"
    ],
    "stateOrProvince": "Washington"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update printer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
