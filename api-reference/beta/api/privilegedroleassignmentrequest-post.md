---
title: Создание privilegedRoleAssignmentRequest
description: Создайте объект privilegedroleassignmentrequest.
ms.openlocfilehash: e262682b5a5e8bffa7fb089ae783f3bb7e67803c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078737"
---
# <a name="create-privilegedroleassignmentrequest"></a>Создание privilegedRoleAssignmentRequest

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Создайте объект [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All    |
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
В тексте запроса укажите представление JSON объекта [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) . 

| Свойство     | Тип    |  Description|
|:---------------|:--------|:----------|
|roleId|String|Идентификатор роли. Обязательное.|
|type|String|Представляет тип операции в назначении ролей. Значение может быть `AdminAdd`: администраторам Добавление пользователей в роли. `UserAdd`: Добавление назначений ролей пользователей. Обязательный атрибут.|
|assignmentState|String|Состояние назначения. Значение может быть `Eligible` подходящими назначения `Active` - если она назначена непосредственно `Active` администраторами, или активируемого на допустимость назначения для пользователей. Возможные значения: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`. Обязательный атрибут.|
|Причина|String|Причину должно предоставляться для запроса назначений ролей для аудита и предварительный просмотр цели.|
|расписание|[governanceSchedule](../resources/governanceschedule.md)|Расписание для запроса назначений ролей.|

## <a name="response"></a>Ответ
Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) в теле ответа.

### <a name="error-codes"></a>Коды ошибок
Этот интерфейс API возвращает этому стандарту коды ошибок HTTP. Кроме того он может вернуть коды ошибок, перечисленных в следующей таблице.

|Код ошибки     | Сообщение об ошибке              | 
|:--------------------| :---------------------|
| 400 BadRequest | Свойство RoleAssignmentRequest был равен NULL |
| 400 BadRequest | Не удается десериализации roleAssignmentRequest объекта. |
| 400 BadRequest | RoleId является обязательным. |
| 400 BadRequest | Дата начала расписания должен быть указан и должен быть больше, чем сейчас. |
| 400 BadRequest | Расписание для этого типа пользователей, ролей и расписание уже существует. |
| 400 BadRequest | Обновление, ожидающее утверждения уже существует для этого типа пользователей, ролей и утверждения. |
| 400 BadRequest | Запросившая сторона причину, отсутствует. |
| 400 BadRequest | Запросившая сторона причина должна быть не более 500 символов. |
| 400 BadRequest | Несанкционированное получение длительность должна быть между 0,5 и {из параметра}. |
| 400 BadRequest | Существует перекрытия запланированного активации и запрос. |
| 400 BadRequest | Роль уже активировано. |
| 400 BadRequest | GenericElevateUserToRoleAssignments: Tickting сведения необходимо и не указано в процессе активации. |
| 400 BadRequest | Существует перекрытия запланированного активации и запрос. |
| 403 доступ запрещен | Несанкционированное получение требуется многофакторная проверка подлинности. |
| 403 доступ запрещен | От имени повышения прав не допускается. |

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
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
    "evaluateOnly": false,
    "type": "UserAdd",
    "assignmentState": "Active",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```
##### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
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
    "evaluateOnly": false,
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "2018-02-08T02:35:42.9137335Z",
    "status": "NotStarted",
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "userId": "Self"，
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Post privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
