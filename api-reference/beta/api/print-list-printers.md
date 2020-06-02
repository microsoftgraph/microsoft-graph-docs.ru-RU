---
title: Получение принтеров
description: Получение списка принтеров, зарегистрированных в клиенте.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 6625be6f12c3d2b430afa2d9099072955c68efdf
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44251109"
---
# <a name="list-printers"></a>Список принтеров

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка **принтеров** , зарегистрированных в клиенте.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:---------------|:--------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)| Users. Read. ALL |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Сервер приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает некоторые параметры запроса OData для настройки ответа. Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).

### <a name="exceptions"></a>Исключения
* `$expand`Операторы and `select` поддерживаются для `share` Свойства навигации, но не для `jobs` .
* Некоторые операторы не поддерживаются: `$count` , `$search` .

## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.
## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Printer](../resources/printer.md) в тексте отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1526

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "name": "PrinterName",
      "manufacturer": "PrinterManufacturer",
      "model": "PrinterModel",
      "isShared": true,
      "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
      "acceptingJobs": true,
      "status": {
        "processingState": "stopped",
        "processingStateReasons": ["disconnected"],
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List printers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
