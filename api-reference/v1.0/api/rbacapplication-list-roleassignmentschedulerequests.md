---
title: Перечисление roleAssignmentScheduleRequests
description: В PIM получите запросы на активные назначения ролей субъектам, выполненные с помощью объекта unifiedRoleAssignmentScheduleRequest.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 167fa54bcca28c3d9b362e3a44b6834aecab864d
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207271"
---
# <a name="list-roleassignmentschedulerequests"></a>Перечисление roleAssignmentScheduleRequests
Пространство имен: microsoft.graph

В PIM получите запросы на активные назначения ролей субъектам. Активные назначения включают назначения и запросы на активацию [, а](rbacapplication-post-roleassignmentschedulerequests.md) также [непосредственно через API назначений ролей](../resources/unifiedroleassignment.md). Назначения ролей могут быть безвозвратно активными с датой окончания срока действия или временно активными после активации пользователем соответствующих назначений.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается                               |
| Приложение                            | RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory               |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleRequests
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметры `$select``$filter`запроса OData `$expand` и , чтобы помочь настроить ответ. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного `200 OK` выполнения этот метод возвращает код отклика и коллекцию объектов [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-retrieve-role-assignment-requests"></a>Пример 1. Получение запросов на назначение ролей

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentschedulerequest"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignmentScheduleRequests
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedroleassignmentschedulerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedroleassignmentschedulerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedroleassignmentschedulerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedroleassignmentschedulerequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-unifiedroleassignmentschedulerequest-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleAssignmentScheduleRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleAssignmentScheduleRequests",
    "value": [
        {
            "id": "95c690fb-3eb3-4942-a03f-4524aed6f31e",
            "status": "Provisioned",
            "createdDateTime": "2022-04-11T11:50:05.95Z",
            "completedDateTime": "2022-04-11T11:50:06Z",
            "approvalId": null,
            "customData": null,
            "action": "adminAssign",
            "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
            "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
            "directoryScopeId": "/",
            "appScopeId": null,
            "isValidationOnly": false,
            "targetScheduleId": "95c690fb-3eb3-4942-a03f-4524aed6f31e",
            "justification": "Assign Groups Admin to IT Helpdesk group",
            "createdBy": {
                "application": null,
                "device": null,
                "user": {
                    "displayName": null,
                    "id": "3fbd929d-8c56-4462-851e-0eb9a7b3a2a5"
                }
            },
            "scheduleInfo": {
                "startDateTime": "2022-04-11T11:50:05.9999343Z",
                "recurrence": null,
                "expiration": {
                    "type": "noExpiration",
                    "endDateTime": null,
                    "duration": null
                }
            },
            "ticketInfo": {
                "ticketNumber": null,
                "ticketSystem": null
            }
        }
    ]
}
```


### <a name="example-2-retrieve-specified-properties-of-role-assignment-requests-and-expand-the-relationships"></a>Пример 2. Получение указанных свойств запросов на назначение ролей и расширение связей

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentschedulerequest_expand_relationships"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignmentScheduleRequests?$select=principalId,action,roleDefinitionId&$expand=roleDefinition,activatedUsing,principal,targetSchedule
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedroleassignmentschedulerequest-expand-relationships-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedroleassignmentschedulerequest-expand-relationships-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedroleassignmentschedulerequest-expand-relationships-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedroleassignmentschedulerequest-expand-relationships-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-unifiedroleassignmentschedulerequest-expand-relationships-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleAssignmentScheduleRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleAssignmentScheduleRequests(principalId,action,roleDefinitionId,roleDefinition(),activatedUsing(),principal(),targetSchedule())",
    "value": [
        {
            "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
            "action": "adminAssign",
            "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
            "roleDefinition": {
                "id": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
                "description": "",
                "displayName": "Groups Administrator",
                "isBuiltIn": true,
                "isEnabled": true,
                "templateId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
                "version": null,
                "resourceScopes": [],
                "rolePermissions": []
            },
            "activatedUsing": null,
            "principal": {
                "@odata.type": "#microsoft.graph.user",
                "id": "071cc716-8147-4397-a5ba-b2105951cc0b",
                "displayName": "Conf Room Adams",
                "userPrincipalName": "Adams@Contoso.com",
                "mail": "Adams@Contoso.com",
                "businessPhones": [],
                "givenName": null,
                "jobTitle": null,
                "mobilePhone": null,
                "officeLocation": null,
                "preferredLanguage": null,
                "surname": null
            },
            "targetSchedule": {
                "id": "95c690fb-3eb3-4942-a03f-4524aed6f31e",
                "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
                "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
                "directoryScopeId": "/",
                "appScopeId": null,
                "createdUsing": "95c690fb-3eb3-4942-a03f-4524aed6f31e",
                "createdDateTime": "2022-04-11T11:50:05.95Z",
                "modifiedDateTime": "2022-04-11T11:50:05.95Z",
                "status": "Provisioned",
                "assignmentType": "Assigned",
                "memberType": "Direct",
                "scheduleInfo": {
                    "startDateTime": "2022-04-11T11:50:05.9999343Z",
                    "recurrence": null,
                    "expiration": {
                        "type": "noExpiration",
                        "endDateTime": null,
                        "duration": null
                    }
                }
            }
        }
    ]
}
```
