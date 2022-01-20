---
title: 'baseTaskList: дельта'
description: Получите набор ресурсов baseTaskList, которые были добавлены, удалены или удалены в Microsoft To Do.
author: devindrajit
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c8c321bf4b3f09e38fe1d53318d6ff9e89b5e7c6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094896"
---
# <a name="basetasklist-delta"></a>baseTaskList: дельта
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите набор ресурсов [baseTaskList,](../resources/basetasklist.md) которые были добавлены, удалены или удалены в Microsoft To Do.

Вызов  функции дельты для **baseTaskList** похож на запрос GET, [](/graph/delta-query-overview) за исключением того, что при надлежащем применении маркеров состояния в одном или более из этих вызовов можно запрашивать дополнительные изменения **в baseTaskList**. Это позволяет поддерживать и синхронизировать локальный магазин **базыTaskList** пользователя без необходимости получать все **baseTaskList** с сервера каждый раз.

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
GET /me/tasks/lists/delta
GET /users/{userId|userPrincipalName}/tasks/lists/delta
```

## <a name="query-parameters"></a>Параметры запроса

Отслеживание изменений **в ресурсах baseTaskList** вызывает один или несколько вызовов функции **дельты.** Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик. Параметры запроса нужно указать только один раз в первом запросе. В последующих запросах просто скопируйте и примените URL-адрес из предыдущего ответа, так как этот URL-адрес уже содержит закодированные `nextLink` `deltaLink` и нужные параметры.

| Параметр запроса    | Тип |Описание|
|:---------------|:--------|:----------|
| $deltatoken | string | В [URL-адрес](/graph/delta-query-overview) предыдущей функции дельты возвращается маркер состояния для той же коллекции `deltaLink` **baseTaskList,** что указывает на завершение этого раунда отслеживания изменений.  Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.|
| $skiptoken | string | Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адрес предыдущего вызова функции дельты, указывает на то, что в том же `nextLink` базовом  **собранииTaskList** необходимо отслеживать дальнейшие изменения. |

### <a name="odata-query-parameters"></a>Параметры запросов OData

- Поддержка запросов Delta `$filter` `$top` и `$expand` параметры запросов **для baseTaskList.** 
- Параметр `$search` не поддерживается. 

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание |
|:---------------|:----------|:----------|
| Authorization  | string  | Bearer {token}. Обязательный. |
| Prefer | string  | odata.maxpagesize={x}. Необязательный параметр. |

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы эта функция возвращает код отклика и `200 OK` [коллекцию baseTaskList](../resources/basetasklist.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "basetasklist_delta"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/tasks/lists/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/basetasklist-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/basetasklist-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/basetasklist-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/basetasklist-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/basetasklist-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.baseTaskList)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(baseTaskList)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/tasks/lists/delta?$skiptoken=AVCnFFj2r7PtnjtkD-g_6Y5Ntek1m4V",
    "value": [
        {
            "@odata.type": "#microsoft.graph.wellKnownTaskList",
            "@odata.etag": "W/\"kOO4xOT//0qFRAqk3TNe0QAAAAAAkw==\"",
            "wellKnownListName": "defaultList",
            "displayName": "Tasks",
            "id": "AQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNm"
        }
    ]
}
```

