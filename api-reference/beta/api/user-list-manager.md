---
title: Получение руководителя
description: Получение руководителя пользователя. Возвращает пользователя или контакт, назначенный в качестве руководителя пользователя.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 1f04dc23b777906a3ee36bbcefea035e1e8d2422
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49524446"
---
# <a name="list-manager"></a>Получение руководителя

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Возвращает пользователя или контакт организации, назначенный в качестве руководителя пользователя. Кроме того, вы можете развернуть цепочку руководителя вплоть до корневого узла.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a>HTTP-запрос

Получение руководителя:
<!-- { "blockType": "ignored" } -->
```http
GET /me/manager
GET /users/{id | userPrincipalName}/manager
```
Получение цепочки управления:
<!-- { "blockType": "ignored" } -->
```http
GET /me?$expand=manager
GET /users?$expand=manager($levels=n)
GET /users/{id | userPrincipalName}/?$expand=manager($levels=n)
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.  

Если запрос содержит `$expand=manager($levels=n)` параметр для получения цепочки руководителя, необходимо также указать следующее:

- `$count=true` параметр строки запроса
- `ConsistencyLevel=eventual` заголовок запроса

>**Note:** `n` значение `$levels` может быть `max` (для возврата всех руководителей) или число от 1 до 1000.  
> Если `$level` параметр не указан, возвращается только диспетчер immediate.  
> Вы можете указать `$select` внутри `$expand` , чтобы выбрать свойства отдельного руководителя: `$expand=manager($levels=max;$select=id,displayName)`

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение|
|:-----------|:------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| ConsistencyLevel | необязательный. Является обязательным, если запрос содержит `$expand=manager($levels=max)` параметр. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-get-manager"></a>Пример 1: Get Manager

В приведенном ниже примере показан запрос на получение диспетчера.

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/manager
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manager-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manager-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manager-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-manager-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример отклика.
>**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "<user-id>",
  "displayName": "Sara Davis",
  "jobTitle": "Finance VP",
  "mail": "SaraD@contoso.onmicrosoft.com",
  "userPrincipalName": "SaraD@contoso.onmicrosoft.com"
}
```

### <a name="example-2-get-manager-chain-up-to-the-root-level"></a>Пример 2: получение цепочки диспетчера вплоть до корневого уровня

В приведенном ниже примере показан запрос на получение цепочки диспетчера до корневого уровня.

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "get_transitive_managers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me?$expand=manager($levels=max;$select=id,displayName)&$select=id,displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа. Транзитивные руководители отображаются в иерархическом порядке.

>**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "<user1-id>",
    "displayName": "Individual Contributor",
    "manager": {
        "id": "<manager1-id>",
        "displayName": "Manager 1",
        "manager": {
            "id": "<manager2-id>",
            "displayName": "Manager 2",
            "manager": {
                "id": "<manager3-id>",
                "displayName": "Manager 3"
            }
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
