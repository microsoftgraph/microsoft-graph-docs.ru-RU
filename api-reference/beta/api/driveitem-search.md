---
author: JeremyKelley
description: Поиск элементов, соответствующих запросу, в иерархии элементов.
ms.date: 09/10/2017
title: Поиск файлов
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 6869940c6c4e8a22061343f5152f424b5d27adaf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42432343"
---
# <a name="search-for-a-driveitems-within-a-drive"></a>Поиск элементов DriveItem на диске

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Поиск элементов, соответствующих запросу, в иерархии элементов.
Вы можете выполнить поиск в иерархии папок, на всем диске или среди файлов, к которым предоставлен доступ текущему пользователю.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Для приложений | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/search(q='{search-text}')
GET /groups/{group-id}/drive/root/search(q='{search-text}')
GET /me/drive/root/search(q='{search-text}')
GET /sites/{site-id}/drive/root/search(q='{search-text}')
GET /users/{user-id}/drive/root/search(q='{search-text}')
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$expand`, `$select`, `$skipToken`, `$top` и `$orderby` для настройки ответа.

## <a name="function-parameters"></a>Параметры функции

| Параметр | Тип  | Описание                                                                                                                          |
|:-----|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| q  | string | Текст запроса, используемый для поиска элементов. Для поиска можно использовать несколько полей, включая поля имени файла, метаданных и содержимого файла. |

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Вот пример запроса, выполняющего поиск в хранилище OneDrive текущего пользователя.


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "item_search" }-->

```msgraph-interactive
GET /me/drive/root/search(q='{search-query}')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/item-search-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/item-search-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/item-search-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Этот метод возвращает объект, который содержит коллекцию элементов [DriveItem](../resources/driveitem.md), соответствующих условиям поиска. Если не будет найдено ни одного элемента, то будет возвращена пустая коллекция.

Если будет найдено слишком много совпадений, отклик будет разбит на страницы, а свойство **@odata.nextLink** будет содержать URL-адрес на следующую страницу с результатами. Чтобы указать количество элементов на странице, вы можете использовать параметр запроса `$top`.

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```

## <a name="searching-for-items-a-user-can-access"></a>Поиск элементов, к которым пользователь может получить доступ

Помимо поиска элементов на диске ваше приложение может выполнять более широкий поиск и включать элементы, к которым текущему пользователю предоставлен доступ. Чтобы расширить область поиска, используйте метод **search** в ресурсе [Drive](../resources/drive.md).

### <a name="example"></a>Пример


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "item_search_all" }-->

```msgraph-interactive
GET /me/drive/search(q='{search-query}')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/item-search-all-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/item-search-all-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/item-search-all-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Отклики при поиске на ресурсе **Drive** могут включать элементы, расположенные за пределами диска (элементы, к которым текущему пользователю предоставлен доступ). Эти элементы будут содержать аспект [**remoteItem**](../resources/remoteitem.md), который указывает, что они хранятся не на целевом диске. 

<!-- { "blockType": "response", "truncated": true, "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" },
        "remoteItem": { "id": "!23141901", "driveId": "s!1020101jlkjl12lx" }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```

## <a name="error-responses"></a>Ответы с ошибками

Дополнительные сведения о возвращении ошибок см. в статье [Ответы с ошибками][error-response].

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md
[odata-query-parameters]: /graph/query-parameters

<!--
{
  "type": "#page.annotation",
  "description": "Search for a file across a OneDrive.",
  "keywords": "search,query,bing,filename,content",
  "section": "documentation",
  "tocPath": "Items/Search",
  "suppressions": [
  ]
}
-->
