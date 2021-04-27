---
author: JeremyKelley
title: Получить пакет
description: Получить пакет driveItems
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b6f1619bbb169a92841d3999c43603860c0038fd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047793"
---
# <a name="get-bundle"></a>Получить пакет

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Извлечение метаданных для [пакета][] на основе уникального ID пакета.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Не поддерживается.                             |
|Делегированные (личная учетная запись Майкрософт) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Для приложений          | Не поддерживается.                                           |

## <a name="http-request"></a>HTTP-запрос

```http
GET /drive/bundles/{bundle-id}
GET /drive/items/{bundle-id}
```

Так как пакеты являются элементами, можно использовать **коллекцию** элементов для возврата метаданных о пакете.
Вы также можете использовать коллекцию **пакетов** в качестве удобства, чтобы убедиться, что вы получаете пакет в ответ.

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Чтобы ограничить форму объектов, возвращаемых в результате вызова, вы можете использовать [параметры запросов OData][odata-parameters].

## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание  |
|:------------- |:------------ |
| Авторизация | Носитель \{токен\}. Обязательный. |
| if-none-match | eTag. Необязательное. Если указан заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то возвращается отклик `HTTP 304 Not Modified`.

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает [driveItem][driveItem] resource with the [bundle][bundle] в теле отклика.

Дополнительные сведения о возвращении ошибок см. в статье [Отклики с ошибками][error-response].

## <a name="examples"></a>Примеры

### <a name="example-1-get-a-bundle"></a>Пример 1. Получить пакет

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get-bundle-metadata" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/bundles/{bundle-id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bundle-metadata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bundle-metadata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bundle-metadata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bundle-metadata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0123456789abc",
  "name": "My Photo Album Bundle",
  "eTag": "etag",
  "cTag": "etag",
  "createdBy": { "user": { "id": "1234", "displayName": "Ryan Gregg" } },
  "createdDateTime": "datetime",
  "lastModifiedBy": { "user": { "id": "1234", "displayName": "Ryan Gregg" } },
  "lastModifiedDateTime": "datetime",
  "size": 1234,
  "webUrl": "http://onedrive.com/...",
  "bundle": {
    "childCount": 4,
     "album": { }
  }
}
```

Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.

### <a name="example-2-get-a-bundle-and-its-children-in-a-single-call"></a>Пример 2. Получить пакет и его детей в одном вызове

Параметр строки запроса можно использовать для включения детей пакета в тот же вызов, что и для запроса метаданных [`expand`](/graph/query-parameters) пакета.

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get-bundle-and-children" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/items/{bundle-id}?expand=children
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bundle-and-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bundle-and-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bundle-and-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bundle-and-children-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Этот вызов возвращает метаданные пакета и список детей пакета.
Если в пакете нет детей, он возвращает пустую коллекцию.

Если количество детей в пакете больше размера страницы по умолчанию, **свойство children@odata.nextLink** возвращается с URL-адресом, который можно использовать для запроса следующей страницы детей в пакете.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "101230100alkc",
  "name": "My Cool Day at the Beach",
  "children": [
    { "id": "120100abab", "name": "image1.jpg", "file": {} },
    { "id": "120100abo1", "name": "image2.jpg", "file": {} }
  ],
  "children@odata.nextLink": "https://api.onedrive.com/v1.0/..."
}
```

Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.


[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md
[error-response]: /graph/errors
[odata-parameters]: /graph/query-parameters


<!-- {
  "type": "#page.annotation",
  "description": "Retrieve metadata about a bundle and its children in OneDrive",
  "keywords": "retrieve,item,bundle,metadata",
  "section": "documentation",
  "tocPath&quot;: &quot;Bundles/Get Bundle Metadata"
} -->


