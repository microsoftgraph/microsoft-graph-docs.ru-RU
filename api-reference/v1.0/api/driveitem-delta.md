---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Синхронизация содержимого ресурса drive
localization_priority: Priority
ms.prod: sharepoint
description: С помощью этого метода приложение может отслеживать изменения drive и соответствующих дочерних элементов.
doc_type: apiPageType
ms.openlocfilehash: d86a02efc98d604bb970faea07c058e3a8651bfa
ms.sourcegitcommit: 41a5bd5868685c10181f6285d5ac91c6dad556e2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2020
ms.locfileid: "45038690"
---
# <a name="track-changes-for-a-drive"></a>Отслеживание изменений для Drive

Пространство имен: microsoft.graph

С помощью этого метода приложение может отслеживать изменения drive и соответствующих дочерних элементов.

Your app begins by calling `delta` without any parameters. The service starts enumerating the drive's hierarchy, returning pages of items and either an `@odata.nextLink` or an `@odata.deltaLink`, as described below.
Your app should continue calling with the `@odata.nextLink` until you no longer see an `@odata.nextLink` returned, or you see a response with an empty set of changes.

After you have finished receiving all the changes, you may apply them to your local state.
To check for changes in the future, call `delta` again with the `@odata.deltaLink` from the previous response.

Deleted items are returned with the [`deleted` facet](../resources/deleted.md). Items with this property set should be removed from your local state. 

>**Примечание.** Локально удалять папку следует, только если после синхронизации всех изменений она пуста.

## <a name="permissions"></a>Разрешения

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Для приложений | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/delta
GET /groups/{groupId}/drive/root/delta
GET /me/drive/root/delta
GET /sites/{siteId}/drive/root/delta
GET /users/{userId}/drive/root/delta
```

## <a name="function-parameters"></a>Параметры функции

| Параметр   | Тип  | Описание                                                                                                                          |
|:-------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| token  | string | Необязательный параметр. Если не указан, перечисляет текущее состояние иерархии. Если используется значение `latest`, возвращает пустой ответ с последним разностным маркером. Если используется предыдущий разностный маркер, возвращает новое состояние с момента того маркера.

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$select`, `$expand` и `$top` для настройки ответа.

## <a name="response"></a>Ответ

В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию ресурсов [DriveItem](../resources/driveitem.md) в теле отклика.

Помимо коллекции ресурсов DriveItem, отклик также включает одно из указанных ниже свойств.

| Имя                 | Значение  | Описание                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| **\@odata.nextLink**  | url    | URL-адрес для получения следующей доступной страницы изменений, если в текущем наборе есть дополнительные изменения.                                        |
| **\@odata.deltaLink** | url    | URL-адрес, возвращаемый вместо **\@odata.nextLink** после возврата всех текущих изменений. Используется для считывания следующего набора изменений в будущем.  |

## <a name="example-initial-request"></a>Пример (первоначальный запрос)

Ниже приведен пример вызова этого API для определения локального состояния.

### <a name="request"></a>Запрос

Ниже приведен пример первоначального запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get_item_delta_first", "tags": "service.graph" } -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-delta-first-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-delta-first-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-delta-first-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-delta-first-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true, "scope": "file.read" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "0123456789abc",
            "name": "folder2",
            "folder": { }
        },
        {
            "id": "123010204abac",
            "name": "file.txt",
            "file": { }
        },
        {
            "id": "2353010204ddgg",
            "name": "file5.txt",
            "deleted": { }
        }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/delta(token=1230919asd190410jlka)"
}
```

Этот отклик включает первую страницу изменений, а свойство **\@odata.nextLink** указывает, что в текущем наборе доступны дополнительные элементы.
Ваше приложение должно запрашивать значение URL-адреса, указанного в свойстве **\@odata.nextLink**, пока не будут восстановлены все страницы элементов.

## <a name="example-last-page-in-a-set"></a>Пример (последняя страница в наборе)

Ниже приведен пример вызова этого API для обновления локального состояния.

### <a name="request"></a>Запрос

Ниже приведен пример запроса, выполненного после первоначального.


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get-item-delta-last", "tags": "service.graph" }-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/delta(token='1230919asd190410jlka')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-delta-last-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-delta-last-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-delta-last-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-delta-last-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- { "blockType": "response", "truncated": true, "@odata.type": "Collection(microsoft.graph.driveItem)", "scope": "file.read" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "0123456789abc",
            "name": "folder2",
            "folder": { },
            "deleted": { }
        },
        {
            "id": "123010204abac",
            "name": "file.txt",
            "file": { }
        }
    ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?(token='1230919asd190410jlka')"
}
```

Такой отклик означает, что между отправками первоначального запроса и данного запроса (на обновление локального состояния) был удален элемент `folder2`, а элемент `file.txt` был добавлен или изменен.

Последняя страница элементов включает свойство **\@odata.deltaLink**, содержащее URL-адрес, с помощью которого можно в дальнейшем восстановить изменения относительно текущего набора элементов.

There may be cases when the service can't provide a list of changes for a given token (for example, if a client tries to reuse an old token after being disconnected for a long time, or if server state has changed and a new token is required).
In these cases the service will return an `HTTP 410 Gone` error with an error response containing one of the error codes below, and a `Location` header containing a new nextLink that starts a fresh delta enumeration from scratch.
After finishing the full enumeration, compare the returned items with your local state and follow these instructions.

| Тип ошибки                       | Инструкции                                                                                                                                                                                                                    |
|:---------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | Replace any local items with the server's version (including deletes) if you're sure that the service was up to date with your local changes when you last sync'd. Upload any local changes that the server doesn't know about. |
| `resyncChangesUploadDifferences` | Отправьте все локальные элементы, не возвращенные службой, и все файлы, отличающиеся от соответствующих файлов на сервере (сохраняйте обе копии, если вы не знаете, какая из них более актуальна).                                       |

## <a name="retrieving-the-current-deltalink"></a>Получение текущего значения deltaLink

В некоторых случаях может быть удобно запросить текущее значение deltaLink, не перечисляя перед этим все элементы, уже хранящиеся в объекте drive.

Это может быть полезно, если приложению достаточно узнать об изменениях и ему не нужны сведения о существующих элементах.
Чтобы получить последнее значение deltaLink, вызовите функцию `delta` с параметром `?token=latest` в строке запроса.

**Примечание. Если вы пытаетесь поддерживать полное локальное представление элементов в папке или на диске, необходимо использовать `delta` для исходного перечисления. Другие подходы, например постраничный просмотр коллекции `children` для папки, не гарантируют возврата всех элементов, если во время перечисления выполняются операции записи. Только с помощью функции `delta` можно гарантировать, что считываются все необходимые данные.**

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get-delta-latest", "scopes": "files.read", "tags": "service.graph", "target": "action" } -->

```msgraph-interactive
GET /me/drive/root/delta?token=latest
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-delta-latest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-delta-latest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-delta-latest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-delta-latest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

<!-- { "blockType": "response", "isEmpty": true, "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [ ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?token=1230919asd190410jlka"
}
```

## <a name="remarks"></a>Примечания

* The delta feed shows the latest state for each item, not each change. If an item were renamed twice, it would only show up once, with its latest name.
* The same item may appear more than once in a delta feed, for various reasons. You should use the last occurrence you see.
* The `parentReference` property on items will not include a value for **path**. This occurs because renaming a folder does not result in any descendants of the folder being returned from **delta**. **When using delta you should always track items by id**.
* В OneDrive для бизнеса и SharePoint функция `delta` поддерживается только для папки `root`.

* Запрос изменений не возвращает некоторые свойства DriveItem, в зависимости от типа операции и службы, как показано в таблицах ниже.

    **OneDrive для бизнеса**
    
    | Тип операции | Свойства, опущенные запросом изменений |
    |---------|----------|
    | Создание или изменение | `ctag`, `lastModifiedBy` |
    | Удаление | `ctag`, `lastModifiedBy`, `name` |


    **OneDrive (для потребителей)**
    
    | Тип операции | Свойства, опущенные запросом изменений |
    |---------|----------|
    | Создание или изменение | н/д |
    | Удаление | `ctag`, `size` |

## <a name="scanning-permissions-hierarchies"></a>Сканирование иерархии разрешений
По умолчанию ответ на запрос изменений включает информацию об общем доступе для всех изменившихся элементов в запросе, даже если они наследуют разрешения от родительского элемента и сами непосредственно не имеют изменений общего доступа. Обычно за этим следует дополнительный запрос на получение сведений о разрешениях для каждого элемента, а не только для тех, которые имеют изменения общего доступа. Чтобы получить более детальные сведения о произошедших изменениях разрешений, добавьте в запрос заголовок `Prefer: hierarchicalsharing`.

При наличии заголовка `Prefer: hierarchicalsharing` возвращается информация об общем доступе для корневого элемента иерархии разрешений, а также для элементов с изменениями общего доступа. В случае когда изменения состоят в отмене общего доступа для элемента, отображается пустой аспект общего доступа, что позволяет отличать элементы, наследующие разрешения от родителя, и уникальные элементы, не имеющие ссылок для общего доступа. Пустой аспект общего доступа также отображается для корневого элемента иерархии разрешений, который не имеет общего доступа.

Во многих сценариях сканирования интерес представляют именно изменения разрешений. Чтобы получить сведения о том, какие изменения являются следствием изменений разрешений, можно использовать в запросе заголовок `Prefer: deltashowsharingchanges`. В этом случае для всех элементов, включенных в ответ на запрос в связи с изменениями разрешений, будет отображаться примечание OData `@microsoft.graph.sharedChanged":"True"`. Эта функция применима к SharePoint и OneDrive для бизнеса, но не к личным учетным записям OneDrive.

> **Примечание.** При включении в запрос заголовка `Prefer: deltashowsharingchanges` требуется использовать `Prefer: deltashowremovedasdeleted` и `Prefer: deltatraversepermissiongaps`. Эти значения заголовка можно объединить в один общий заголовок: `Prefer: deltashowremovedasdeleted; deltatraversepermissiongaps; deltashowsharingchanges;`.

## <a name="error-responses"></a>Ответы с ошибками

Помимо вышеописанных ошибок повторной синхронизации, в статье [Ответы с ошибками][error-response] представлены сведения о том, как возвращаются ошибки.

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Sync changes from the service to your client state.",
  "keywords": "sync,delta,changes,$delta",
  "section": "documentation",
  "tocPath": "Items/Sync changes",
  "suppressions": [
  ]
} -->
