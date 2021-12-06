---
title: Обновление принтера
description: Обновление свойств объекта принтера.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 85644248015ee4a55591ddee23231f04a82d7a52
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60980418"
---
# <a name="update-printer"></a>Обновление принтера

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [принтера.](../resources/printer.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать. Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)

Только приложение, которое зарегистрировал принтер, может обновлять принтер с помощью разрешений приложений.

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:---------------|:--------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)| Printer.ReadWrite.All, Printer.FullControl.All |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений| Printer.ReadWrite.All |

>**Примечание:** В настоящее время только принтеры, не оснащенные физическим устройством, могут обновляться с помощью разрешений приложений.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:-----------|:-----------|
| Авторизация | Bearer {token}. Обязательный. |
| Content-Type  | `application/json` при использовании делегирования разрешений или `application/ipp` `application/json` при использовании разрешений приложений. Обязательно.|

## <a name="request-body"></a>Текст запроса

### <a name="delegated-permissions-and-json-payload"></a>Делегирование разрешений и полезной нагрузки JSON

При использовании делегирования разрешений в теле запроса поставляют значения для соответствующих полей принтера, которые необходимо обновить. [](../resources/printer.md) Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились. 

Следующие свойства можно обновить с помощью делегирования разрешений.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|defaults|[printerDefaults](../resources/printerdefaults.md)|Параметры печати принтера по умолчанию.|
|расположение|[printerLocation](../resources/printerlocation.md)|Физическое и/или организационное расположение принтера.|
|displayName|Строка|Имя принтера.|

### <a name="application-permissions-and-json-payload"></a>Разрешения приложения и полезной нагрузки JSON
В теле запроса укажи значения [](../resources/printer.md) для соответствующих полей принтера, которые должны быть обновлены. Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились. 

Следующие свойства можно обновить с помощью разрешений приложений.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|defaults|[printerDefaults](../resources/printerdefaults.md)|Параметры печати принтера по умолчанию.|
|capabilities|[printerCapabilities](../resources/printerCapabilities.md)|Возможности принтера, связанного с этим разделом принтера.|
|displayName|Строка|Имя принтера.|
|manufacturer|String|Производитель принтера.|
|model|String|Имя модели принтера.|
|status|[printerStatus](../resources/printerstatus.md)|Состояние обработки принтера, включая ошибки.|
|isAcceptingJobs|Boolean|Принимает ли принтер новые задания печати.|

### <a name="application-permissions-and-ipp-payload"></a>Разрешения приложений и полезной нагрузки IPP

С разрешениями приложений принтер также может обновляться с помощью полезной нагрузки протокола интернет-печати (IPP). В этом случае тело запроса содержит двоичный поток, представляюющий группу атрибутов принтера в [кодовом коде IPP.](https://tools.ietf.org/html/rfc8010)

Клиент должен предоставить набор атрибутов принтера с одним или более значениями (включая явно разрешенные вне диапазона значения), как это определено в разделе [RFC8011 раздела 5.2](https://tools.ietf.org/html/rfc8011#section-5.2) Атрибуты шаблона работы ("xxx-default", "xxx-supported" и "xxx-ready"), Атрибуты описания принтера [5.4](https://tools.ietf.org/html/rfc8011#section-5.4) и все расширения атрибутов, поддерживаемые принтером. Значение (ы) каждого предоставленного атрибута принтера заменяет значение (ы) соответствующего атрибута принтера на объекте целевого принтера. Для атрибутов, которые могут иметь несколько значений (1setOf), все значения, предоставленные клиентом, заменяют все значения соответствующего атрибута объекта Printer.

> **Примечание:** Не пропускать атрибуты операции в теле запроса. Тело запроса должно содержать только атрибуты принтера.


> **Примечание:** Чтобы принтеры работали с определенной платформой, она должна соответствовать требованиям этой платформы. Например, на клиенте Windows ожидается, что принтер указывает все атрибуты, которые считаются обязательными в спецификациях [MOPRIA.](https://mopria.org) Обратите внимание, что спецификации MOPRIA доступны только платным членам MOPRIA.

## <a name="response"></a>Отклик

### <a name="delegated-permissions-and-json-payload"></a>Делегирование разрешений и полезной нагрузки JSON

При использовании делегирования разрешений при успешном использовании этот метод возвращает код отклика и обновленный объект принтера `200 OK` в тексте [](../resources/printer.md) ответа.

### <a name="application-permissions-and-json-payload"></a>Разрешения приложения и полезной нагрузки JSON

При использовании делегирования разрешений при успешном использовании этот метод возвращает код отклика и обновленный объект принтера `200 OK` в тексте [](../resources/printer.md) ответа.

### <a name="application-permissions-and-ipp-payload"></a>Разрешения приложений и полезной нагрузки IPP

При использовании разрешений приложений при успешном использовании этот метод возвращает `204 No content` код ответа. Метод не возвращает данные в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printer"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/printers/{id}
Content-type: application/json

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

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-printer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-printer-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a>Отклик
Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers/$entity",
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "displayName": "PrinterName",
  "manufacturer": "PrinterManufacturer",
  "model": "PrinterModel",
  "isShared": true,
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
  "isAcceptingJobs": true,
  "status": {
    "state": "idle",
    "details": [],
    "description": ""
  },
  "defaults": {
    "copiesPerJob":1,
    "contentType": "application/oxps",
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
    "floor": "1",
    "floorDescription": "First Floor",
    "roomName": "1234",
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
