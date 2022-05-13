---
title: Создание privilegedRoleAssignmentRequest
description: Создайте объект privilegedroleassignmentrequest.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: b54785f4c857b3c7c45ffbba3c81e2d64f2a427a
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399515"
---
# <a name="create-privilegedroleassignmentrequest"></a>Создание privilegedRoleAssignmentRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2AADRoles-deprecation](../../includes/pim-v2AADRoles-deprecation.md)]

Создайте [объект privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированное (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureAD    |
|Делегированное (личная учетная запись Майкрософт) | Не поддерживается. |
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
В тексте запроса добавьте представление объекта [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) в формате JSON. 

| Свойство     | Тип    |  Описание|
|:---------------|:--------|:----------|
|roleId|String|Идентификатор роли. Обязательное.|
|type|String|Представляет тип операции назначения роли. Значение может быть: `AdminAdd`администраторы добавляют пользователей к ролям;`UserAdd` пользователи добавляют назначения ролей. Обязательно.|
|assignmentState|String|Состояние назначения. Значение может быть задано `Eligible` для `Active` допустимого назначения , `Active` если оно напрямую назначено администраторами или активировано для допустимого назначения пользователями. Возможные значения: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`. Обязательно.|
|reason|String|Причина должна быть указана для запроса на назначение роли для аудита и проверки.|
|schedule|[governanceSchedule](../resources/governanceschedule.md)|Расписание запроса на назначение ролей.|

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код `201 Created` отклика и объект [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) в тексте отклика.

### <a name="error-codes"></a>Коды ошибок
Этот API возвращает стандартные коды ошибок HTTP. Кроме того, он может возвращать коды ошибок, перечисленные в следующей таблице.

|Код ошибки     | Сообщение об ошибке              | 
|:--------------------| :---------------------|
| 400 BadRequest | Свойство RoleAssignmentRequest было NULL |
| 400 BadRequest | Не удалось десериализировать объект roleAssignmentRequest. |
| 400 BadRequest | Требуется RoleId. |
| 400 BadRequest | Дата начала расписания должна быть указана и больше, чем сейчас. |
| 400 BadRequest | Для этого пользователя, роли и типа расписания уже существует расписание. |
| 400 BadRequest | Для этого пользователя, роли и типа утверждения уже существует ожидающее утверждения. |
| 400 BadRequest | Отсутствует причина запроса. |
| 400 BadRequest | Причина запроса не должна превышать 500 символов. |
| 400 BadRequest | Длительность повышения прав должна находиться в диапазоне от 0,5 до {с параметра}. |
| 400 BadRequest | Между запланированной активацией и запросом существует перекрытие. |
| 400 BadRequest | Роль уже активирована. |
| 400 BadRequest | GenericElevateUserToRoleAssignments: сведения о делениях являются обязательными и не предоставляются в процессе активации. |
| 400 BadRequest | Между запланированной активацией и запросом существует перекрытие. |
| 403 Без проверки подлинности | Повышение прав требует многофакторной проверки подлинности. |
| 403 Без проверки подлинности | От имени повышения прав не допускается. |

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

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/post-privilegedroleassignmentrequest-powershell-snippets.md)]
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


