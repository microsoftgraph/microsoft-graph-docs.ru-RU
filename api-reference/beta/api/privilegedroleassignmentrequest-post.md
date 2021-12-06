---
title: Создание privilegedRoleAssignmentRequest
description: Создание объекта privilegedroleassignmentrequest.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: 83ef3cb4ac08a9351d63625ec643ff3ed2ce9565
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60997051"
---
# <a name="create-privilegedroleassignmentrequest"></a>Создание privilegedRoleAssignmentRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v1AADRoles-deprecation](../../includes/pim-v1aadroles-deprecation.md)]

Создание [объекта privilegedroleassignmentrequest.](../resources/privilegedroleassignmentrequest.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [privilegedroleassignmentrequest.](../resources/privilegedroleassignmentrequest.md) 

| Свойство     | Тип    |  Описание|
|:---------------|:--------|:----------|
|roleId|Строка|ID роли. Обязательное.|
|type|Строка|Представляет тип операции при назначении ролей. Значение может `AdminAdd` быть: Администраторы добавляют пользователей в роли; `UserAdd` : Пользователи добавляют назначения ролей. Обязательный.|
|assignmentState|String|Состояние назначения. Это значение может быть для присвоения, если оно непосредственно назначено администраторами или активировано при назначении, назначенного `Eligible` `Active` `Active` пользователями. Возможные значения: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`. Обязательный.|
|reason|String|Причина должна быть предоставлена для запроса назначения ролей для целей аудита и проверки.|
|schedule|[governanceSchedule](../resources/governanceschedule.md)|Расписание запроса на назначение ролей.|

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код ответа и объект `201 Created` [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) в тексте ответа.

### <a name="error-codes"></a>Коды ошибок
Этот API возвращает стандартные коды ошибок HTTP. Кроме того, он может возвращать коды ошибок, перечисленные в следующей таблице.

|Код ошибки     | Сообщение об ошибке              | 
|:--------------------| :---------------------|
| 400 BadRequest | Свойство RoleAssignmentRequest было NULL |
| 400 BadRequest | Не удается deserialize roleAssignmentRequest Object. |
| 400 BadRequest | RoleId необходим. |
| 400 BadRequest | Дата начала расписания должна быть указана и должна быть больше, чем сейчас. |
| 400 BadRequest | Для этого пользователя, роли и типа расписания уже существует расписание. |
| 400 BadRequest | Ожидается утверждение уже существует для этого пользователя, роли и утверждения типа. |
| 400 BadRequest | Причина запроса отсутствует. |
| 400 BadRequest | Причина запроса должна быть менее 500 символов. |
| 400 BadRequest | Продолжительность высоты должна быть между 0,5 и {from setting}. |
| 400 BadRequest | Существует совпадение между запланированной активацией и запросом. |
| 400 BadRequest | Роль уже активирована. |
| 400 BadRequest | GenericElevateUserToRoleAssignments: сведения о тикинге необходимы и не поставляются в процессе активации. |
| 400 BadRequest | Существует совпадение между запланированной активацией и запросом. |
| 403 UnAuthorized | Высота требует многофакторной проверки подлинности. |
| 403 UnAuthorized | От имени высоты не допускается. |

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_privilegedroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
Content-type: application/json

{
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "schedule": {
        "startDateTime": "2018-02-08T02:35:17.903Z"
    },
    "type": "UserAdd",
    "assignmentState": "Active",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-privilegedroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-privilegedroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-privilegedroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-privilegedroleassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/post-privilegedroleassignmentrequest-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Отклик
Ниже представлен пример ответа. Примечание: показанный здесь объект ответа может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests/$entity",
    "schedule": {
        "type": "activation",
        "startDateTime": "2018-02-08T02:35:17.903Z",
        "endDateTime": null,
        "duration" : null
    },
    "id": "e13ef8a0-c1cb-4d03-aaae-9cd1c8ede2d1",
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "2018-02-08T02:35:42.9137335Z",
    "status": "NotStarted",
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "userId": "Self",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Post privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


