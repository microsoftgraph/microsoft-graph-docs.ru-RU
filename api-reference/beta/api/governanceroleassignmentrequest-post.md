---
title: Создание governanceRoleAssignmentRequest
description: Создание роли назначения запроса для представления операции, требуется на назначения ролей. В следующей таблице перечислены операции.
localization_priority: Normal
ms.openlocfilehash: 0fc8d96585daf63f53bc6b33985a289e8f810d6b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572369"
---
# <a name="create-governanceroleassignmentrequest"></a>Создание governanceRoleAssignmentRequest

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание роли назначения запроса для представления операции, требуется на назначения ролей. В следующей таблице перечислены операции.

| Operation       | Тип | 
|:---------------|:----------|
| Назначение назначения ролей| AdminAdd |
| Активация назначение подходящими роли| UserAdd | 
| Деактивация назначение активированные роли| UserRemove | 
| Удаление назначения ролей| AdminRemove |
| Обновление назначения ролей| AdminUpdate |
| Запрос на расширение my назначения роли| UserExtend | 
| Расширение назначения ролей| AdminExtend | 
| Запрос на обновление назначения ролей с истекшим сроком действия| UserRenew | 
| Обновление назначения ролей с истекшим сроком действия| AdminRenew | 

 
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureResources  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | PrivilegedAccess.ReadWrite.AzureResources |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Authorization  | Bearer {code}|
| Content-Type  | application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите представление JSON объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) . 

| Свойство     | Тип    |Обязательный|  Описание|
|:---------------|:--------|:----------|:----------|
|resourceId|Строка|Да|Идентификатор ресурса.|
|roleDefinitionId|Строка|Да|Идентификатор определения роли.|
|subjectId|Строка|Да|Идентификатор субъекта.|
|assignmentState|Строка|Да|Состояние назначения. Значение может быть ``Eligible`` и ``Active``.|
|type|Строка|Да|Тип запроса. Значение может быть `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`и `AdminExtend`.|
|Причина|Строка| |Причину должно предоставляться для запроса назначений ролей для аудита и предварительный просмотр цели.|
|расписание|[microsoft.graph.governanceSchedule](../resources/governanceschedule.md)| | Расписание для запроса назначений ролей. Для запроса типа `UserAdd`, `AdminAdd`, `AdminUpdate`, и `AdminExtend`, это необходимо.|

## <a name="response"></a>Отклик
Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в теле ответа.

### <a name="error-codes"></a>Коды ошибок
Этот интерфейс API возвращает стандартные коды ошибок HTTP. Кроме того он возвращает коды ошибок, перечисленных в следующей таблице.

|Код ошибки     | Сообщение об ошибке              | Сведения |
|:--------------------| :---------------------|:--------------------|
| 400 BadRequest | RoleNotFound    | `roleDefinitionId` Условии, что в запросе не удается найти текст.
| 400 BadRequest | ResourceIsLocked    | Ресурс, представленные в тексте запроса находится в состоянии из `Locked` и не могут создавать запросы назначений ролей.
| 400 BadRequest | SubjectNotFound    | `subjectId` Условии, что в запросе не удается найти текст.
| 400 BadRequest | PendingRoleAssignmentRequest    | Уже существует ожидающие [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в системе.
| 400 BadRequest | RoleAssignmentExists    | [GovernanceRoleAssignment](../resources/governanceroleassignment.md) запрошено будет создан уже существует в системе.
| 400 BadRequest | RoleAssignmentDoesNotExist    | [GovernanceRoleAssignment](../resources/governanceroleassignment.md) запрос на обновление/расширить не существует в системе.
| 400 BadRequest | RoleAssignmentRequestPolicyValidationFailed | [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) не соответствует внутренней политик и не может быть создан.

## <a name="examples"></a>Примеры
В приведенных ниже примерах показано, как использовать этот интерфейс API.

### <a name="example-1"></a>Пример 1
В этом примере администраторам назначение роли выставления счетов читатель nawu@fimdev.net пользователя.

 >**Примечание:** В дополнение к разрешение, в этом примере требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса. 

| Свойство     | Тип    |Обязательный|  Значение |
|:---------------|:--------|:----------|:----------|
|resourceId|Строка|Да|\<Ид_ресурса\>|
|roleDefinitionId|Строка|Да|\<roleDefinitionId\>|
|subjectId|Строка|Да|\<subjectId\>|
|assignmentState|Строка|Да| Допустимость / Active|
|type|Строка|Да| AdminAdd|
|Причина|Строка| зависит от роли параметров||
|расписание|[microsoft.graph.governanceSchedule](../resources/governanceschedule.md)|Да|        |
##### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
"resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Eligible",
"type":"AdminAdd",
"reason":"Assign an eligible role",
"schedule":{
  "startDateTime":"2018-05-12T23:37:43.356Z",
  "endDateTime":"2018-11-08T23:37:43.356Z",
  "type":"Once"
  }
}
```
##### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
    "id": "1232e4ea-741a-4be5-8044-5edabdd61672",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
    "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
    "linkedEligibleRoleAssignmentId": "",
    "type": "AdminAdd",
    "assignmentState": "Eligible",
    "requestedDateTime": "0001-01-01T00:00:00Z",
    "reason": "Evaluate Only",
    "status": {
        "status": "InProgress",
        "subStatus": "Granted",
        "statusDetails": [
            {
                "key": "AdminRequestRule",
                "value": "Grant"
            },
            {
                "key": "ExpirationRule",
                "value": "Grant"
            },
            {
                "key": "MfaRule",
                "value": "Grant"
            }
        ]
    },
    "schedule": {
        "type": "Once",
        "startDateTime": "2018-05-12T23:37:43.356Z",
        "endDateTime": "2018-11-08T23:37:43.356Z",
        "duration": "PT0S"
    }
}
```

### <a name="example-2"></a>Пример 2
В этом примере nawu@fimdev.net пользователь активирует право чтения выставления счетов роли.

| Свойство     | Тип    |Обязательный|  Значение |
|:---------------|:--------|:----------|:----------|
|resourceId|Строка|Да|\<Ид_ресурса\>|
|roleDefinitionId|Строка|Да|\<roleDefinitionId\>|
|subjectId|Строка|Да|\<subjectId\>|
|assignmentState|Строка|Да| Активное|
|type|Строка|Да| UserAdd|
|Причина|Строка| зависит от роли параметров||
|расписание|[microsoft.graph.governanceSchedule](../resources/governanceschedule.md)|Да|        |
##### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"8b4d1d51-08e9-4254-b0a6-b16177aae376",
"resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Active",
"type":"UserAdd",
"reason": "Activate the owner role",
"schedule":{
  "type":"Once",
  "startDateTime":"2018-05-12T23:28:43.537Z",
  "duration":"PT9H"
  },
"linkedEligibleRoleAssignmentId":"e327f4be-42a0-47a2-8579-0a39b025b394"
}
```
##### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
    "id": "3ad49a7c-918e-4d86-9f84-fab28f8658c0",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
    "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
    "linkedEligibleRoleAssignmentId": "e327f4be-42a0-47a2-8579-0a39b025b394",
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "0001-01-01T00:00:00Z",
    "reason": "Activate the owner role",
    "status": {
        "status": "InProgress",
        "subStatus": "Granted",
        "statusDetails": [
            {
                "key": "EligibilityRule",
                "value": "Grant"
            },
            {
                "key": "ExpirationRule",
                "value": "Grant"
            },
            {
                "key": "MfaRule",
                "value": "Grant"
            },
            {
                "key": "JustificationRule",
                "value": "Grant"
            },
            {
                "key": "ActivationDayRule",
                "value": "Grant"
            },
            {
                "key": "ApprovalRule",
                "value": "Grant"
            }
        ]
    },
    "schedule": {
        "type": "Once",
        "startDateTime": "2018-05-12T23:28:43.537Z",
        "endDateTime": "0001-01-01T00:00:00Z",
        "duration": "PT9H"
    }
}
```

### <a name="example-3"></a>Пример 3
В этом примере пользователь nawu@fimdev.net деактивирует активная роль чтения выставления счетов.

| Свойство     | Тип    |Обязательный|  Значение |
|:---------------|:--------|:----------|:----------|
|resourceId|Строка|Да|\<Ид_ресурса\>|
|roleDefinitionId|Строка|Да|\<roleDefinitionId\>|
|subjectId|Строка|Да|\<subjectId\>|
|assignmentState|Строка|Да| Активное|
|type|Строка|Да| UserRemove|
|Причина|Строка| Нет||
|расписание|[microsoft.graph.governanceSchedule](../resources/governanceschedule.md)|Нет|        |
##### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"bc75b4e6-7403-4243-bf2f-d1f6990be122",
"resourceId":"fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Active",
"type":"UserRemove",
"reason":"Deactivate the role",
"linkedEligibleRoleAssignmentId":"cb8a533e-02d5-42ad-8499-916b1e4822ec"
}
```
##### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
    "id": "abfcdb57-8e5d-42a0-ae67-7598b96fddb1",
    "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
    "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
    "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
    "linkedEligibleRoleAssignmentId": "cb8a533e-02d5-42ad-8499-916b1e4822ec",
    "type": "UserRemove",
    "assignmentState": "Active",
    "requestedDateTime": "0001-01-01T00:00:00Z",
    "reason": "Evaluate only",
    "schedule": null,
    "status": {
        "status": "Closed",
        "subStatus": "Revoked",
        "statusDetails": []
    }
}
```

### <a name="example-4"></a>Пример 4
В этом примере администраторам удалить nawu@fimdev.net пользователя из роли выставления счетов чтения.

 >**Примечание:** В дополнение к разрешение, в этом примере требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.
 
| Свойство     | Тип    |Обязательный|  Значение |
|:---------------|:--------|:----------|:----------|
|resourceId|Строка|Да|\<Ид_ресурса\>|
|roleDefinitionId|Строка|Да|\<roleDefinitionId\>|
|subjectId|Строка|Да|\<subjectId\>|
|assignmentState|Строка|Да| Допустимость / Active|
|type|Строка|Да| AdminRemove|
|Причина|Строка| Нет||
|расписание|[microsoft.graph.governanceSchedule](../resources/governanceschedule.md)|Нет|        |
##### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState":"Eligible",
  "type":"AdminRemove"
}
```
##### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"c934fcb9-cf53-42ac-a8b4-6246f6726299",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminRemove",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "reason":null,
  "status":{
    "status":"Closed",
    "subStatus":"Revoked",
    "statusDetails":[]
  },
  "schedule":null
}
```

### <a name="example-5"></a>Пример 5
В этом примере Администраторы обновление назначения ролей для пользователя nawu@fimdev.net владельцу.

 >**Примечание:** В дополнение к разрешение, в этом примере требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса. 

| Свойство     | Тип    |Обязательный|  Значение |
|:---------------|:--------|:----------|:----------|
|resourceId|Строка|Да|\<Ид_ресурса\>|
|roleDefinitionId|Строка|Да|\<roleDefinitionId\>|
|subjectId|Строка|Да|\<subjectId\>|
|assignmentState|Строка|Да| Допустимость / Active|
|type|Строка|Да| AdminUpdate|
|Причина|Строка| зависит от roleSettings||
|расписание|[microsoft.graph.governanceSchedule](../resources/governanceschedule.md)|Да|        |
##### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"1566d11d-d2b6-444a-a8de-28698682c445",
  "assignmentState":"Eligible",
  "type":"AdminUpdate",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-03-08T05:42:45.317Z",
    "endDateTime":"2018-06-05T05:42:31.000Z"
  }
}
```
##### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"4f6d4802-b3ac-4f5a-86d7-a6a4edd7d383",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "subjectId":"1566d11d-d2b6-444a-a8de-28698682c445",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminUpdate",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "reason":null,
  "status":{
    "status":"InProgress",
    "subStatus":"Granted",
    "statusDetails":[
      {
        "key":"AdminRequestRule","value":"Grant"
      },{
        "key":"ExpirationRule","value":"Grant"
      },{
        "key":"MfaRule","value":"Grant"
      }
    ]
  },
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-03-08T05:42:45.317Z",
    "endDateTime":"2018-06-05T05:42:31Z",
    "duration":"PT0S"
  }
}
```

### <a name="example-6"></a>В примере 6
В этом примере расширяет истекающим сроком действия назначения ролей для пользователя ANUJCUSER для участника службы управления API.

 >**Примечание:** В additon разрешение, в этом примере требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.
 
| Свойство     | Тип    |Обязательный|  Значение |
|:---------------|:--------|:----------|:----------|
|resourceId|Строка|Да|\<Ид_ресурса\>|
|roleDefinitionId|Строка|Да|\<roleDefinitionId\>|
|subjectId|Строка|Да|\<subjectId\>|
|assignmentState|Строка|Да| Допустимость / Active |
|type|Строка|Да| AdminExtend|
|Причина|Строка| зависит от roleSettings||
|расписание|[microsoft.graph.governanceSchedule](../resources/governanceschedule.md)|Да|        |
##### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState":"Eligible",
  "type":"AdminExtend",
  "reason":"extend role assignment",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-05-12T23:53:55.327Z",
    "endDateTime":"2018-08-10T23:53:55.327Z"
  }
}
```
##### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"486f0c05-47c8-4498-9c06-086a78c83004",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminExtend",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "reason":"extend role assignment",
  "status":{
    "status":"InProgress",
    "subStatus":"Granted",
    "statusDetails":[
      {
        "key":"AdminRequestRule","value":"Grant"
      },{
        "key":"ExpirationRule","value":"Grant"
      },{
        "key":"MfaRule","value":"Grant"
      }
    ]
  },
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-05-12T23:53:55.327Z",
    "endDateTime":"2018-08-10T23:53:55.327Z",
    "duration":"PT0S"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Post roleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
