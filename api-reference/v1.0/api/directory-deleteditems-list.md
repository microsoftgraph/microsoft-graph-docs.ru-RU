---
title: Перечисление deletedItems (объекты каталога)
description: Получение списка недавно удаленных элементов.
author: keylimesoda
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 61d11d33871710267933fcf71e5932a33f71514d
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768163"
---
# <a name="list-deleteditems-directory-objects"></a>Перечисление deletedItems (объекты каталога)

Пространство имен: microsoft.graph

Получение списка недавно удаленных объектов каталога. В настоящее время эта функция поддерживается только для [ресурсов приложения](../resources/application.md), [группы](../resources/group.md) [и пользователей](../resources/user.md) .

>**Примечание:** Удаленные группы безопасности удаляются без возможности восстановления и не могут быть получены с помощью этого API.

## <a name="permissions"></a>Разрешения

[!INCLUDE [limited-info](../../includes/limited-info.md)]

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

### <a name="for-applications"></a>Для приложений:

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | Application.Read.All, Application.ReadWrite.All, Directory.Read.All |

### <a name="for-users"></a>Для пользователей:

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений | User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |

### <a name="for-groups"></a>Для групп:

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Group.Read.All, Group.ReadWrite.All, Directory.Read.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | Group.Read.All, Group.ReadWrite.All, Directory.Read.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.application
GET /directory/deletedItems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
GET /directory/deletedItems/microsoft.graph.device
```

В настоящее время этот API поддерживает извлечение типов объектов приложений (`microsoft.graph.application`), групп (`microsoft.graph.group`) или пользователей (`microsoft.graph.user`) из удаленных элементов. Тип приведения OData является обязательной частью URI, `GET /directory/deleteditems` и вызов без типа **не поддерживается** .

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает параметры запроса, поддерживаемые ресурсом, указанным приведения OData. То есть, `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, и `$select`параметры `$top` запроса. Некоторые запросы поддерживаются только при использовании заголовка **ConsistencyLevel** с присвоенным значением `eventual` и `$count`. Например:

```msgraph-interactive
https://graph.microsoft.com/beta/directory/deletedItems/microsoft.graph.group?&$count=true&$orderBy=deletedDateTime desc&$select=id,displayName,deletedDateTime
ConsistencyLevel: eventual
```

В этом примере требуется **заголовок ConsistencyLevel** `$orderBy` `$count` , так как в запросе используются параметры и параметры запроса.

### <a name="examples-using-the-orderby-odata-query-parameter"></a>Примеры использования параметра $orderBy OData

Параметр `$orderBy` запроса OData поддерживается в свойствах **deletedDateTime**, **displayName** и **userPrincipalName** удаленных типов объектов. В **свойстве deletedDateTime** запрос требует добавления дополнительных параметров запроса [(](/graph/aad-advanced-queries) заголовок **ConsistencyLevel** `true` задан и строка `$count=true` запроса).

| Приведение OData | Свойства, поддерживающие $orderBy | Пример |
| :--- | :--- | :--- |
| microsoft.graph.user | deletedDateTime, displayName, userPrincipalName | /directory/deletedItems/microsoft.graph.user?$orderBy=userPrincipalName |
| microsoft.graph.group | deletedDateTime, displayName | /directory/deletedItems/microsoft.graph.group?$orderBy=deletedDateTime asc&$count=true |
| microsoft.graph.application | deletedDateTime, displayName | /directory/deletedItems/microsoft.graph.application?$orderBy=displayName |
| microsoft.graph.device | deletedDateTime, displayName | /directory/deletedItems/microsoft.graph.device?$orderBy=deletedDateTime&$count=true |

## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Authorization  | Bearer &lt;code&gt; *Обязательный*.|
| Accept  | application/json |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.
## <a name="examples"></a>Примеры

### <a name="example-1-retrieve-deleted-groups"></a>Пример 1. Извлечение удаленных групп

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.group
```

#### <a name="response"></a>Отклик

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "value": [
    {
      "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
      "displayName":"SampleGroup",
      "groupTypes":["Unified"],
      "mail":"example@contoso.com",
      "mailEnabled":true,
      "mailNickname":"Example",
      "securityEnabled":false,
      "visibility":"Public"
    }
  ]
}
```

### <a name="example-2-retrieve-the-count-of-deleted-user-objects-and-order-the-results-by-the-deleteddatetime-property"></a>Пример 2. Получение количества удаленных объектов пользователя и упорядочивания результатов по свойству deletedDateTime

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_deleteditems_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.group?$count=true&$orderBy=deletedDateTime asc&$select=id,DisplayName,deletedDateTime
ConsistencyLevel: eventual
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-deleteditems-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-deleteditems-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-deleteditems-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-deleteditems-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-deleteditems-count-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-deleteditems-count-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups(id,displayName,deletedDateTime)",
    "@odata.count": 2,
    "value": [
        {
            "id": "c31799b8-0683-4d70-9e91-e032c89d3035",
            "displayName": "Role assignable group",
            "deletedDateTime": "2021-10-26T16:56:36Z"
        },
        {
            "id": "74e45ce0-a52a-4766-976c-7201b0f99370",
            "displayName": "Role assignable group",
            "deletedDateTime": "2021-10-26T16:58:37Z"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
