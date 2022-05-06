---
title: 'baseTaskList: delta'
description: Получение набора ресурсов baseTaskList, которые были добавлены, удалены или удалены в Список дел Microsoft.
author: devindrajit
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f5427f68c14faf5e1205cebee608a37e8eda87e0
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247177"
---
# <a name="basetasklist-delta"></a>baseTaskList: delta
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение набора ресурсов [baseTaskList](../resources/basetasklist.md), которые были добавлены, удалены или удалены в Список дел Microsoft.

Вызов **разностной** функции **для baseTaskList** аналогичен запросу GET, за исключением того, [](/graph/delta-query-overview) что при соответствующем применении маркеров состояния в одном или нескольких из этих вызовов можно запросить добавочные изменения **в baseTaskList**. Это позволяет поддерживать и синхронизировать локальное хранилище **baseTaskList** пользователя без необходимости каждый раз получать **все данные baseTaskList** с сервера.

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

Отслеживание изменений **в ресурсах baseTaskList** вызывает один или несколько вызовов **разностных** функций. Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `@odata.nextLink` или `@odata.deltaLink`, включенного в отклик. Параметры запроса нужно указать только один раз в первом запросе. В последующих запросах `@odata.nextLink` `@odata.deltaLink` просто скопируйте и примените URL-адрес из предыдущего ответа, так как этот URL-адрес уже содержит закодированные требуемые параметры.

| Параметр запроса    | Тип |Описание|
|:---------------|:--------|:----------|
| $deltatoken | string | Маркер [состояния,](/graph/delta-query-overview) возвращенный `@odata.deltaLink` в URL-адресе предыдущего вызова разностной функции для той же коллекции **baseTaskList**, что указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `@odata.deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.|
| $skiptoken | string | Маркер [состояния,](/graph/delta-query-overview) возвращенный `@odata.nextLink` в URL-адресе предыдущего вызова функции delta, указывающий на то, что в той же коллекции **baseTaskList** будут отслеживаться дальнейшие изменения. |

### <a name="odata-query-parameters"></a>Параметры запросов OData

- Поддержка разностных `$filter` `$top`запросов и `$expand` параметры запроса **для baseTaskList**. 
- Параметр `$search` не поддерживается. 

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание |
|:---------------|:----------|:----------|
| Authorization  | string  | Bearer {token}. Обязательный. |
| Prefer | string  | odata.maxpagesize={x}. Необязательный параметр. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения эта функция возвращает код `200 OK` отклика и [коллекцию baseTaskList](../resources/basetasklist.md) в тексте отклика.

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

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/basetasklist-delta-powershell-snippets.md)]
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

