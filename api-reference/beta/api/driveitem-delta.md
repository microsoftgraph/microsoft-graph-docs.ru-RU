---
author: JeremyKelley
description: С помощью этого метода приложение может отслеживать изменения drive и соответствующих дочерних элементов.
ms.date: 09/10/2017
title: Синхронизация содержимого ресурса drive
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 483bfdcdd08c5d01f69d1b12455e64b903d9fac8
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912077"
---
# <a name="track-changes-for-a-drive"></a>Отслеживание изменений для диска

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

С помощью этого метода приложение может отслеживать изменения drive и соответствующих дочерних элементов.

Для начала приложение вызывает `delta` без параметров. Служба начинает перечислять иерархию диска, возвращая страницы элементов и `@odata.nextLink` или `@odata.deltaLink`, как показано ниже. Приложению следует выполнять вызовы с использованием `@odata.nextLink`, пока не будет возвращен отклик без `@odata.nextLink` или с пустым набором изменений.

Завершив получать изменения, вы можете применить их к локальному состоянию. Для проверки наличия изменений в будущем снова вызовите `delta` с использованием `@odata.deltaLink` из предыдущего отклика.

Удаленные элементы возвращаются с [аспектом `deleted`](../resources/deleted.md). Элементы с этим набором свойств следует удалить из локального состояния. 

**Примечание.** Локально удалять папку следует, только если после синхронизации всех изменений она пуста.

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
| **@odata.nextLink**  | url    | URL-адрес для получения следующей доступной страницы изменений, если в текущем наборе есть дополнительные изменения.                                        |
| **@odata.deltaLink** | url    | URL-адрес, возвращаемый вместо **@odata.nextLink** после возврата всех текущих изменений. Используется для считывания следующего набора изменений в будущем.  |

## <a name="example-initial-request"></a>Пример (первоначальный запрос)

Ниже приведен пример вызова этого API для определения локального состояния.

### <a name="request"></a>Запрос

Ниже приведен пример первоначального запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get_item_delta_first" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/root/delta
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

Этот отклик включает первую страницу изменений, а свойство **@odata.nextLink** указывает, что в текущем наборе доступны дополнительные элементы. Ваше приложение должно запрашивать значение URL-адреса, указанного в свойстве **@odata.nextLink**, пока не будут получены все страницы элементов.

## <a name="example-last-page-in-a-set"></a>Пример (последняя страница в наборе)

Ниже приведен пример вызова этого API для обновления локального состояния.

### <a name="request"></a>Запрос

Ниже приведен пример запроса, выполненного после первоначального.


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get_item_delta_last" }-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/root/delta(token='1230919asd190410jlka')
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

На последней странице элементов указано свойство **@odata.deltaLink**, содержащее URL-адрес, с помощью которого можно будет получить изменения относительно текущего набора элементов.

В некоторых случаях службе не удается предоставить список изменений для определенного маркера (например, если клиент пытается повторно использовать старый маркер после долгого отключения, а также если из-за измененного состояния сервера требуется новый маркер). В таких случаях служба возвращает ошибку `HTTP 410 Gone` с откликом, содержащим один из представленных ниже кодов ошибок, и заголовком `Location`, содержащим новый аргумент nextLink, который начинает новое перечисление delta. По завершении полного перечисления сравните возвращенные элементы с локальным состоянием и выполните указанные ниже действия.

| Тип ошибки                       | Инструкции                                                                                                                                                                                                                    |
|:---------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | Замените все локальные элементы (в том числе удаленные) соответствующими элементами с сервера, если вы уверены, что при последней синхронизации в службу были внесены все локальные изменения. Отправьте все локальные изменения, не загруженные на сервер. |
| `resyncChangesUploadDifferences` | Отправьте все локальные элементы, не возвращенные службой, и все файлы, отличающиеся от соответствующих файлов на сервере (сохраняйте обе копии, если вы не знаете, какая из них более актуальна).                                       |

## <a name="retrieving-the-current-deltalink"></a>Получение текущего значения deltaLink

В некоторых случаях может быть удобно запросить текущее значение deltaLink, не перечисляя перед этим все элементы, уже хранящиеся в объекте drive.

Это может быть полезно, если приложению достаточно узнать об изменениях и ему не нужны сведения о существующих элементах.
Чтобы получить последнее значение deltaLink, вызовите функцию `delta` с параметром `?token=latest` в строке запроса.

>**Примечание:** Если вы пытаетесь сохранить полное локальное представление элементов в папке или диске, необходимо использовать для первоначального `delta` переозначения.
Другие подходы, такие как прокачив коллекцию папки, не гарантируют возвращение каждого элемента, если записи имеют место во время `children` переуступки. Использование — это единственный способ гарантировать, что вы считыли все `delta` необходимые данные.

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get-delta-latest", "scope": "files.read", "target": "action" } -->

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

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [ ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?token=1230919asd190410jlka"
}
```

## <a name="remarks"></a>Примечания

* В разностном канале показано последнее состояние каждого элемента, а не каждое изменение. Если элемент был переименован дважды, он будет указан только один раз, но с последним именем.
* По ряду причин один и тот же элемент может отображаться в разностном канале несколько раз. Следует использовать последний представленный вариант.
* Свойство `parentReference` элементов не включает значение **path**. Это вызвано тем, что при переименовании папки ее потомки не возвращаются с помощью **delta**. **При использовании delta следует всегда отслеживать элементы по идентификатору**.
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

По умолчанию ответ на запрос изменений включает информацию об общем доступе для всех изменившихся элементов в запросе, даже если они наследуют разрешения от родительского элемента и сами непосредственно не имеют изменений общего доступа. Обычно это приводит к последующему вызову для получения сведений о разрешении для каждого элемента, а не только для тех, чьи сведения о совместном использовании изменились. Чтобы получить более детальные сведения о произошедших изменениях разрешений, добавьте в запрос заголовок `Prefer: hierarchicalsharing`.

При наличии заголовка `Prefer: hierarchicalsharing` возвращается информация об общем доступе для корневого элемента иерархии разрешений, а также для элементов с изменениями общего доступа. В случае когда изменения состоят в отмене общего доступа для элемента, отображается пустой аспект общего доступа, что позволяет отличать элементы, наследующие разрешения от родителя, и уникальные элементы, не имеющие ссылок для общего доступа. Пустой аспект общего доступа также отображается для корневого элемента иерархии разрешений, который не имеет общего доступа.

Во многих сценариях сканирования интерес представляют именно изменения разрешений. Чтобы получить сведения о том, какие изменения являются следствием изменений разрешений, можно использовать в запросе заголовок `Prefer: deltashowsharingchanges`. В этом случае для всех элементов, включенных в ответ на запрос в связи с изменениями разрешений, будет отображаться примечание OData `@microsoft.graph.sharedChanged":"True"`. Эта функция применима к SharePoint и OneDrive для бизнеса, но не к личным учетным записям OneDrive.

> **Примечание.** При включении в запрос заголовка `Prefer: deltashowsharingchanges` требуется использовать `Prefer: deltashowremovedasdeleted` и `Prefer: deltatraversepermissiongaps`. Эти значения заголовка можно объединить в один общий заголовок: `Prefer: deltashowremovedasdeleted, deltatraversepermissiongaps, deltashowsharingchanges`.

## <a name="error-responses"></a>Ответы с ошибками

Помимо вышеописанных ошибок повторной синхронизации, в статье [Ответы с ошибками][error-response] представлены сведения о том, как возвращаются ошибки.

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Sync changes from the service to your client state.",
  "keywords": "sync,delta,changes,$delta",
  "section": "documentation",
  "tocPath": "Items/Sync changes",
  "suppressions": [
  ]
}
-->


