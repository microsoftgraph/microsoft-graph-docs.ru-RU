---
title: Создание calendarPermission
description: Создание объекта calendarpermission.
ms.localizationpriority: medium
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 82a12d3d82951accb7ae998229d9cbb8e460ff7d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61000999"
---
# <a name="create-calendarpermission"></a>Создание calendarPermission

Пространство имен: microsoft.graph

Создайте [ресурс calendarPermission,](../resources/calendarpermission.md) чтобы указать удостоверение и роль пользователя, с которым указанный календарь является общим или делегированным.

## <a name="permissions"></a>Разрешения

В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Календарь | Делегированные (рабочая или учебная учетная запись) | Делегированное (личная учетная запись Майкрософт) | Приложение |
|:-----|:-----|:-----|:-----|
| календарь пользователя | Calendars.Read, Calendars.ReadWrite | Calendars.Read, Calendars.ReadWrite | Calendars.Read, Calendars.ReadWrite |
| календарь группы | Group.Read.All, Group.ReadWrite.All | Не поддерживается. | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

Создание указанных разрешений основного календаря пользователя:
<!-- { 
  "blockType": "ignored",
}-->

```http
POST /users/{id}/calendar/calendarPermissions
```

Создайте указанные разрешения группового календаря:
<!-- { 
  "blockType": "ignored",
}-->
```http
POST /groups/{id}/calendar/calendarPermissions
```

Создайте указанные разрешения пользовательского календаря, который содержит указанное событие:
<!-- { 
  "blockType": "ignored",
}-->
```http
POST /users/{id}/events/{id}/calendar/calendarPermissions
```

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Bearer {token}. Обязательный. |
| Content-Type  | application/json. Обязательный.  |

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON объекта [calendarPermission.](../resources/calendarpermission.md)

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` calendarPermission в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- { 
  "blockType": "request",
  "sampleKeys": ["458d4c95-124e-49da-ba9d-1dd0387e682e"],
  "name": "create_calendarpermissions"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/calendar/calendarPermissions

{
    "emailAddress": {
        "name": "Samantha Booth",
        "address": "samanthab@adatum.onmicrosoft.com"
    },
    "isInsideOrganization": true,
    "isRemovable": true,
    "role": "read"
}

```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-calendarpermissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendarpermissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-calendarpermissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-calendarpermissions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-calendarpermissions-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('458d4c95-124e-49da-ba9d-1dd0387e682e')/calendar/calendarPermissions/$entity",
    "id": "RXhjaGFuZ2VQdWJsaXNoZWRVc2VyLnNhbWFudGhhYkBhZGF0dW0ub25taWNyb3NvZnQuY29t",
    "isRemovable": true,
    "isInsideOrganization": true,
    "role": "read",
    "allowedRoles": [
        "freeBusyRead",
        "limitedRead",
        "read"
    ],
    "emailAddress": {
        "name": "Samantha Booth",
        "address": "samanthab@adatum.onmicrosoft.com"
    }
}
```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed99
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create calendarPermission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
  } -->
