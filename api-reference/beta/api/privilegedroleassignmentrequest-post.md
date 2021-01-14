---
title: Создание privilegedRoleAssignmentRequest
description: Создание объекта privilegedroleassignmentrequest.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 771edf9d102a890214156df43791be42a47b14dd
ms.sourcegitcommit: dbbf77c732ae8d982e59865432b9b6147002a30a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/14/2021
ms.locfileid: "49866175"
---
# <a name="create-privilegedroleassignmentrequest"></a>Создание privilegedRoleAssignmentRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание объекта [privilegedroleassignmentrequest.](../resources/privilegedroleassignmentrequest.md)

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
| Авторизация  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
В теле запроса укажу представление объекта [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) в JSON. 

| Свойство     | Тип    |  Описание|
|:---------------|:--------|:----------|
|roleId|String|ИД роли. Обязательное.|
|type|String|Представляет тип операции для назначения роли. Значением может `AdminAdd` быть: Администраторы добавляют пользователей к ролям; `UserAdd` : пользователи добавляют назначения ролей. Обязательный.|
|assignmentState|String|Состояние назначения. Это значение может быть присвоено в случае, если оно напрямую назначено администраторами или активировано для соответствующих назначений `Eligible` `Active` `Active` пользователями. Возможные значения: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`. Обязательный.|
|reason|String|Причина должна быть предоставлена для запроса на назначение роли для целей аудита и проверки.|
|schedule|[governanceSchedule](../resources/governanceschedule.md)|Расписание запроса на назначение роли.|

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика и объект `201 Created` [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) в тексте отклика.

### <a name="error-codes"></a>Коды ошибок
Этот API возвращает стандартные коды ошибок HTTP. Кроме того, он может возвращать коды ошибок, перечисленные в следующей таблице.

|Код ошибки     | Сообщение об ошибке              | 
|:--------------------| :---------------------|
| 400 BadRequest | Свойство RoleAssignmentRequest было NULL |
| 400 BadRequest | Не удается десериализировать объект roleAssignmentRequest. |
| 400 BadRequest | Требуется RoleId. |
| 400 BadRequest | Дата начала расписания должна быть указана и должна быть больше, чем сейчас. |
| 400 BadRequest | Для этого пользователя, роли и типа расписания уже существует расписание. |
| 400 BadRequest | Для этого пользователя, роли и типа утверждения уже существует ожидающих утверждения. |
| 400 BadRequest | Отсутствует причина запросителя. |
| 400 BadRequest | Причина запросителя не должна быть меньше 500 символов. |
| 400 BadRequest | Длительность повышения прав должна быть от 0,5 до {from setting}. |
| 400 BadRequest | Между запланированной активацией и запросом существует перекрытие. |
| 400 BadRequest | Роль уже активирована. |
| 400 BadRequest | GenericElevateUserToRoleAssignments: сведения о тактах являются обязательной и не дается в процессе активации. |
| 400 BadRequest | Между запланированной активацией и запросом существует перекрытие. |
| 403 UnAuthorized | Повышение прав требует многофакторной проверки подлинности. |
| 403 UnAuthorized | От имени не допускается повышение прав. |

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

---

##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304


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


