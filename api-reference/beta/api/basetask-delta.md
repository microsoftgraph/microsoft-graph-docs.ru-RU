---
title: 'baseTask: дельта'
description: Получите набор ресурсов baseTask, которые были добавлены, удалены или обновлены в определенной базеTaskList.
author: devindrajit
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a662af2401b7cb0e56aa1616c04b195aa0bf6cf7
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341791"
---
# <a name="basetask-delta"></a>baseTask: дельта
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите набор ресурсов [baseTask](../resources/basetask.md) , которые были добавлены, удалены или обновлены в определенной [базеTaskList](../resources/basetasklist.md).

Вызов  функции delta для ресурсов **baseTask** в **baseTaskList** похож на запрос GET, за исключением того, что при надлежащем применении [](/graph/delta-query-overview) маркеров состояния в одном или более из этих вызовов можно запрашивать дополнительные изменения в **baseTask** в этой **baseTaskList**. Это позволяет поддерживать и синхронизировать локальный магазин ресурсов **baseTask** пользователя без необходимости каждый раз получать весь набор с сервера.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Tasks.Read, Tasks.ReadWrite|
|Делегированные (личная учетная запись Майкрософт)|Tasks.Read, Tasks.ReadWrite|
|Для приложений|Не поддерживается|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/tasks/lists/{baseTaskListId}/tasks/delta
GET /users/{userId|userPrincipalName}/tasks/lists/{baseTaskListId}/tasks/delta
```

## <a name="query-parameters"></a>Параметры запроса

Отслеживание изменений **в коллекции baseTask** вызывает один или несколько вызовов функций **дельты** . Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик. Параметры запроса нужно указать только один раз в первом запросе. В последующих запросах `nextLink` `deltaLink` просто скопируйте и примените URL-адрес из предыдущего ответа, так как этот URL-адрес уже содержит закодированные и нужные параметры.

| Параметр запроса    | Тип |Описание|
|:---------------|:--------|:----------|
| $deltatoken | string | Маркер [состояния,](/graph/delta-query-overview) возвращенный в `deltaLink` URL-адрес предыдущей  функции дельты, для той же коллекции baseTask, что указывает на завершение этого раунда отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.|
| $skiptoken | string | Маркер [состояния,](/graph/delta-query-overview) возвращенный в `nextLink` URL-адрес предыдущего  вызова функции дельты, указывает на то, что в той же коллекции baseTask необходимо отслеживать дальнейшие изменения. |

### <a name="odata-query-parameters"></a>Параметры запросов OData

- Поддержка запросов Delta `$filter` `$top`и параметры `$expand` запросов **для baseTask**. 
- Параметр `$search` не поддерживается.

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание |
|:---------------|:----------|:----------|
| Authorization  | string  | Bearer {token}. Обязательный. |
| Prefer | string  | odata.maxpagesize={x}. Необязательный параметр. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы эта функция возвращает код `200 OK` ответа и [коллекцию baseTask](../resources/basetask.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "basetask_delta"
}
-->
``` http
GET /me/tasks/lists/AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQpLAt-6oC2JgAQCQ47jE5P--SoVECqTdM17RAAAB4mDIAAA=/tasks/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/basetask-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/basetask-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/basetask-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/basetask-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/basetask-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/basetask-delta-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.baseTask)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(baseTask)",
    "@odata.deltaLink": "https://graph.microsoft.com/beta/me/tasks/lists/AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQpLAt-6oC2JgAQCQ47jE5P--SoVECqTdM17RAAAB4mDIAAA=/tasks/delta?$deltatoken=AVCnFFj2r7PtnjtkD-g_6dgDSPbEboZhaMYEytpd57pcJMrR9oGkCIjK_dyVkhNB1EQn1zcQt7YZTwCS0V5MNQo6Iy0-T0csAkLZTMlbiII.lVEHqD5xdDrH30csYKP6tEvoYa3WtFhmYLtKBSxCPpQ",
    "value": [
        {
            "@odata.type": "#microsoft.graph.task",
            "@odata.etag": "W/\"kOO4xOT//0qFRAqk3TNe0QAAAymRBQ==\"",
            "importance": "normal",
            "status": "notStarted",
            "displayName": "Read documentation",
            "createdDateTime": "2021-11-15T13:16:53.0831814Z",
            "lastModifiedDateTime": "2021-11-15T13:17:08.8273666Z",
            "id": "AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AkOO4xOT--0qFRAqk3TNe0QAAAy35RwAA",
            "body": {
                "content": "",
                "contentType": "text"
            },
            "parentList": {
                "id": "AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQpLAt-6oC2JgAQCQ47jE5P--SoVECqTdM17RAAAB4mDIAAA="
            }
        }
    ]
}
```

