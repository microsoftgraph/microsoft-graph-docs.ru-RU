---
author: learafa
description: Получение только что созданных, обновленных или удаленных элементов списка без необходимости выполнять полное чтение всей коллекции элементов.
title: 'lisItem: delta'
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: def214ca5ba9d633ba9835d3678350fd9cf6e04a
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549636"
---
# <a name="listitem-delta"></a>listItem: delta

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение только что созданных, обновленных или удаленных элементов списка без необходимости выполнять полное чтение всей коллекции элементов.[](../resources/listitem.md)

Для начала приложение вызывает `delta` без параметров.
Служба начинает перечисление иерархии списка, возвращая страницы элементов и **либо @odata.nextLink** , либо **@odata.deltaLink**.
Ваше приложение должно продолжать вызывать **@odata.nextLink** , пока не отобразится **@odata.deltaLink** .

После получения всех изменений их можно применить к локальному состоянию.
Чтобы проверить наличие изменений в будущем, `delta` снова вызовите метод **@odata.deltaLink** из предыдущего ответа.

В разностном канале показано последнее состояние каждого элемента, а не каждое изменение. Если элемент был переименован дважды, он будет отображаться только один раз с его последним именем.
Один и тот же элемент может отображаться несколько раз в разностной ленте по различным причинам. Следует использовать последний представленный вариант.

Удаленные элементы возвращаются с [удаленным аспектом](../resources/deleted.md). Удаление означает, что элемент удален и не может быть восстановлен.
Элементы с этим свойством должны быть удалены из локального состояния.

> **Примечание:** Папку следует удалять только локально, если она пуста после синхронизации всех изменений.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Sites.Read.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.   |
|Для приложений | Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{siteId}/lists/{listId}/items/delta
```

## <a name="query-parameters"></a>Параметры запроса

В URL-адрес запроса можно включить следующий необязательный параметр запроса.

| Параметр    | Тип   | Описание                                                                                                                          |
|:-------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| token        | string | Необязательно. Если значение не указано, перечисляет текущее состояние иерархии. Если `latest`, возвращает пустой ответ с последним разностным токеном. Если предыдущий разностный токен, возвращает новое состояние после этого маркера.|

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$select`, `$expand` и `$top` для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов

|Заголовок       |Значение                    |
|-------------|-------------------------|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и совокупность объектов [listItem](../resources/listitem.md) в тексте отклика.

Помимо коллекции объектов **listItem** , ответ также будет содержать одно из следующих свойств.

| Имя                 | Значение  | Описание                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| **@odata.nextLink**  | URL    | URL-адрес для получения следующей доступной страницы изменений, если в текущем наборе есть дополнительные изменения.                                        |
| **@odata.deltaLink** | URL-адрес    | URL-адрес, возвращаемый вместо **@odata.nextLink** после возврата всех текущих изменений. Используется для считывания следующего набора изменений в будущем.  |

В некоторых случаях `410 Gone` служба возвращает код ответа с ответом об ошибке, который содержит один из следующих кодов ошибок, и заголовок, `Location` `nextLink` содержащий новый, который запускает новое разностное перечисление. Это происходит, когда служба не может предоставить список изменений для заданного маркера (например, если клиент пытается повторно использовать старый маркер после длительного отключения или если состояние сервера изменилось и требуется новый маркер).

После завершения полного перечисления сравните возвращенные элементы с локальным состоянием и следуйте инструкциям в зависимости от типа ошибки.

| Тип "ошибка"                       | Инструкции                                                                                                                               |
|:---------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | Замените все локальные элементы версиями с сервера (включая удаления), если вы уверены, что служба была в курсе локальных изменений при последней синхронизации. Отправьте все локальные изменения, не загруженные на сервер. |
| `resyncChangesUploadDifferences` | Отправьте все локальные элементы, которые служба не вернула, и отправьте элементы, которые отличаются от версий сервера (сохраните обе копии, если вы не знаете, какая из них более последняя).                                       |

В дополнение к ошибкам повторной синхронизации и дополнительным сведениям о том, как возвращаются ошибки, см. Graph microsoft Graph и [типы ресурсов][error-response].

## <a name="examples"></a>Примеры

### <a name="example-1-initial-request"></a>Пример 1. Исходный запрос

Ниже приведен пример исходного запроса, в котором показано, как вызвать этот API для установления локального состояния.

#### <a name="request"></a>Запрос

Ниже приведен пример исходного запроса.

<!-- { "blockType": "request", "name": "get_listItem_delta_first" } -->

```http
GET https://graph.microsoft.com/beta/sites/contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE/lists/22e03ef3-6ef4-424d-a1d3-92a337807c30/items/delta
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа, который включает первую страницу изменений и свойство **@odata.nextLink** , указывающее, что в текущем наборе элементов больше нет доступных элементов. Ваше приложение должно запрашивать значение URL-адреса, указанного в свойстве **@odata.nextLink**, пока не будут получены все страницы элементов.

<!-- { "blockType": "response", "name": "get_listItem_delta_first", "@odata.type": "microsoft.graph.listItem", "isCollection": true, "truncated": true, "scope": "site.read" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "createdDateTime": "2020-06-02T22:46:58Z",
            "eTag": "\"{12AD05BB-59B8-43AA-9456-77C44E9BC066},756\"",
            "id": "1",
            "lastModifiedDateTime": "2021-10-14T23:27:27Z",
            "webUrl": "http://contoso.sharepoint.com/Shared%20Documents/TestFolder",
            "createdBy": {
                "user": {
                    "displayName": "John doe",
                }
            },
            "parentReference": {
                "id": "1",
                "path": "Shared%20Documents",
                "siteId": "12AD05BB-59B8-43AA-9456-77C44E9BC066"
            },
            "contentType": {
                "id": "0x00123456789abc",
                "name": "Folder"
            }
        },
        {
            "createdDateTime": "2020-06-02T22:46:58Z",
            "eTag": "\"{12AD05BB-59B8-43AA-9456-77C44E9BC067},756\"",
            "id": "2",
            "lastModifiedDateTime": "2021-10-14T23:27:27Z",
            "webUrl": "http://contoso.sharepoint.com/Shared%20Documents/TestItemA.txt",
            "createdBy": {
                "user": {
                    "displayName": "John doe",
                }
            },
            "parentReference": {
                "id": "2",
                "path": "Shared%20Documents",
                "siteId": "12AD05BB-59B8-43AA-9456-77C44E9BC066"
            },
            "contentType": {
                "id": "0x00123456789abc",
                "name": "Document"
            }
        },
        {
            "createdDateTime": "2020-06-02T22:46:58Z",
            "eTag": "\"{12AD05BB-59B8-43AA-9456-77C44E9BC068},756\"",
            "id": "3",
            "lastModifiedDateTime": "2021-10-14T23:27:27Z",
            "webUrl": "http://contoso.sharepoint.com/Shared%20Documents/TestItemB.txt",
            "createdBy": {
                "user": {
                    "displayName": "John doe",
                }
            },
            "parentReference": {
                "id": "3",
                "path": "Shared%20Documents",
                "siteId": "12AD05BB-59B8-43AA-9456-77C44E9BC066"
            },
            "contentType": {
                "id": "0x00123456789abc",
                "name": "Document"
            }
        }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/beta/sites/contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE/lists/22e03ef3-6ef4-424d-a1d3-92a337807c30/items/delta?token=1230919asd190410jlka"
}
```

### <a name="example-2-last-page-request"></a>Пример 2. Запрос последней страницы

Ниже приведен пример запроса, в котором показана последняя страница в наборе и как вызвать этот API для обновления локального состояния.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса после первоначального запроса.

<!-- { "blockType": "request", "name": "get-listItem-delta-last" }-->

```http
GET https://graph.microsoft.com/beta/sites/contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE/lists/22e03ef3-6ef4-424d-a1d3-92a337807c30/items/delta?token=1230919asd190410jlka
```

#### <a name="response"></a>Отклик

Ниже приведен пример `TestItemB.txt` `TestFolder` ответа, указывающий, что элемент с именем был удален и элемент был добавлен или изменен между исходным запросом и этим запросом для обновления локального состояния.

На последней странице элементов указано свойство **@odata.deltaLink**, содержащее URL-адрес, с помощью которого можно будет получить изменения относительно текущего набора элементов.


<!-- { "blockType": "response", "name": "get-listItem-delta-last", "truncated": true, "@odata.type": "microsoft.graph.listItem", "isCollection": true,  "scope": "site.read" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
       {
            "createdDateTime": "2020-06-02T22:46:58Z",
            "eTag": "\"{12AD05BB-59B8-43AA-9456-77C44E9BC066},756\"",
            "id": "1",
            "lastModifiedDateTime": "2016-03-21T20:01:37Z",
            "webUrl": "http://contoso.sharepoint.com/Shared%20Documents/TestFolder",
            "createdBy": {
                "user": {
                    "displayName": "John doe",
                }
            },
            "parentReference": {
                "id": "1",
                "path": "Shared%20Documents",
                "siteId": "12AD05BB-59B8-43AA-9456-77C44E9BC066"
            },
            "contentType": {
                "id": "0x00123456789abc",
                "name": "Folder"
            }
        },
        {
            "id": "3",
            "parentReference": {
                "siteId": "12AD05BB-59B8-43AA-9456-77C44E9BC066"
            },
            "contentType": {
                "id": "0x00123456789abc",
                "name": "Document"
            },
            "deleted": {"state": "deleted"}
        }
    ],
    "@odata.deltaLink": "https://graph.microsoft.com/beta/sites/contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE/lists/22e03ef3-6ef4-424d-a1d3-92a337807c30/items/delta?token=1230919asd190410jlka"
}
```

### <a name="example-3-delta-link-request"></a>Пример 3. Запрос на разностную ссылку

В некоторых сценариях может быть `deltaLink` полезно запросить текущее значение без предварительного перечисления всех элементов в списке. Это может быть полезно, если приложению нужно знать только об изменениях и не нужно знать о существующих элементах.
Чтобы получить последнюю версию `deltaLink`, вызовите его `delta` с параметром строки запроса `?token=latest`.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- { "blockType": "request", "name": "get-delta-latest", "scope": "sites.read", "target": "action" } -->

```http
GET /sites/contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE/lists/22e03ef3-6ef4-424d-a1d3-92a337807c30/items/delta?token=latest
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- { "blockType": "response", "name": "get-delta-latest", "isEmpty": true, "@odata.type": "microsoft.graph.listItem", "isCollection": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [ ],
    "@odata.deltaLink": "https://graph.microsoft.com/beta/sites/contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE/lists/22e03ef3-6ef4-424d-a1d3-92a337807c30/items/delta?token=1230919asd190410jlka"
}
```

## <a name="see-also"></a>См. также
[Отслеживание изменений данных Microsoft Graph с помощью запроса изменений](/graph/delta-query-overview)

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Sync changes from the service to your client state.",
  "keywords": "sync,delta,changes,$delta",
  "section": "documentation",
  "tocPath&quot;: &quot;ListItem/Get delta"
} -->
