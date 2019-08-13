---
title: Создание Привилежедролеассигнментрекуест
description: Создание объекта привилежедролеассигнментрекуест.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 6b98c5421f2007ede2f4cdd60b1602fe6f3b42db
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361018"
---
# <a name="create-privilegedroleassignmentrequest"></a>Создание Привилежедролеассигнментрекуест

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание объекта [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Привилежедакцесс. ReadWrite. AzureAD, Directory. AccessAsUser. ALL    |
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

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md) в формате JSON. 

| Свойство     | Тип    |  Описание|
|:---------------|:--------|:----------|
|roleId|String|Идентификатор роли. Обязательное.|
|type|String|Представляет тип операции для назначения роли. Возможные значения `AdminAdd`: администраторы добавляют пользователей к ролям; `UserAdd`: Пользователи добавляют назначения ролей. Обязательно.|
|ассигнментстате|String|Состояние назначения. Значение может быть `Eligible` для правого назначения `Active` , если оно напрямую назначено `Active` администраторами или активировано в соответствии с подходящими пользователями. Возможные значения: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`. Обязательно.|
|причиной|String|Необходимо указать причину для запроса на назначение роли для аудита и проверки.|
|schedule|[governanceSchedule](../resources/governanceschedule.md)|Расписание запроса на назначение роли.|

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md) в тексте отклика.

### <a name="error-codes"></a>Коды ошибок
Этот API возвращает стандартные коды ошибок HTTP. Кроме того, он может возвращать коды ошибок, приведенные в следующей таблице.

|Код ошибки     | Сообщение об ошибке              | 
|:--------------------| :---------------------|
| 400 Бадрекуест | Свойство Ролеассигнментрекуест имеет значение NULL |
| 400 Бадрекуест | Не удается десериализовать объект Ролеассигнментрекуест. |
| 400 Бадрекуест | RoleId является обязательным. |
| 400 Бадрекуест | Дата начала расписания должна быть указана и должна быть больше, чем сейчас. |
| 400 Бадрекуест | Расписание для этого пользователя, роли и типа расписания уже существует. |
| 400 Бадрекуест | Для этого пользователя, роли и типа утверждения уже существует ожидающее утверждение. |
| 400 Бадрекуест | Не указана причина запрашивающей стороны. |
| 400 Бадрекуест | Срок запрашивающего не должен быть меньше 500 символов. |
| 400 Бадрекуест | Длительность возвышения должна быть между 0,5 и {from Setting}. |
| 400 Бадрекуест | Между запланированной активацией и запросом существует перекрытие. |
| 400 Бадрекуест | Роль уже активирована. |
| 400 Бадрекуест | Женерицелеватеусерторолеассигнментс: Тикктинг сведения являются обязательными и не предоставляются в процессе активации. |
| 400 Бадрекуест | Между запланированной активацией и запросом существует перекрытие. |
| 403 авторизация | Для повышения требуется многофакторная проверка подлинности. |
| 403 авторизация | От имени повышения прав не разрешено. |

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
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
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-privilegedroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-privilegedroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Цель — C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-privilegedroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
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
    "evaluateOnly": false,
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
