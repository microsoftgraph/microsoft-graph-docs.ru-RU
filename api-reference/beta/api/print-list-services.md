---
title: Список Принтсервицес
description: Получение списка объектов Принтсервице, представляющих службы, доступные в клиенте.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: b72a2e2a59cfc718832a9082428878c0258d3321
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967073"
---
# <a name="list-printservices"></a>Список Принтсервицес

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка объектов [принтсервице](../resources/printservice.md) , представляющих **службы** , доступные в клиенте.

## <a name="permissions"></a>Разрешения
Для вызова этого API не требуется никаких разрешений, но чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать.

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:---------------|:--------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|Нет.|
|Делегированные (личная учетная запись Майкрософт)|Нет.|
|Приложение|Нет.|

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /print/services
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает некоторые параметры запросов OData для настройки отклика. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.
## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [принтсервице](../resources/printservice.md) в тексте отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_services"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/services
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-services-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-services-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-services-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-services-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printService",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 389

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/services",
  "value": [
    {
      "id": "f4cfee8b-4117-4773-a2f0-3807beb282b9",
      "endpoints": [
        {
          "id": "mpsdiscovery",
          "displayName": "Microsoft Universal Print Discovery Service",
          "uri": "https://discovery.print.microsoft.com"
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List services",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


