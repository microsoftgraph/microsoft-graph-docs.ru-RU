---
title: 'unifiedRoleAssignmentScheduleRequest: filterByCurrentUser'
description: В PIM получите запросы на активные назначения ролей для определенного субъекта. Субъект может быть создателем или утверждающим объектом unifiedRoleAssignmentScheduleRequest или целевым объектом назначения.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 5a65b32cef4376fbddff43d10c15ed933a28c966
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439830"
---
# <a name="unifiedroleassignmentschedulerequest-filterbycurrentuser"></a>unifiedRoleAssignmentScheduleRequest: filterByCurrentUser
Пространство имен: microsoft.graph

В PIM получите запросы на активные назначения ролей для определенного субъекта. Субъект может быть создателем или утверждающим **объектом unifiedRoleAssignmentScheduleRequest** или целевым объектом назначения.

> [!NOTE]
> Этот API не возвращает активные назначения ролей через членство в группах.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleRequests/filterByCurrentUser(on='parameterValue')
```

## <a name="function-parameters"></a>Параметры функции
В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.
В следующей таблице показаны параметры, необходимые для этой функции.

|Параметр|Тип|Описание|
|:---|:---|:---|
|on|roleAssignmentScheduleRequestFilterByCurrentUserOptions| Возможные значения: `principal`, `createdBy`, `approver`, `unknownFutureValue`. Только и `principal` `approver` в настоящее время поддерживаются.|

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает параметры `$select``$filter`запроса OData `$expand` и , чтобы помочь настроить ответ. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).


## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения `200 OK` эта функция возвращает код отклика и коллекцию [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "unifiedroleassignmentschedulerequestthis.filterbycurrentuser"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignmentScheduleRequests/filterByCurrentUser(on='principal')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unifiedroleassignmentschedulerequestthisfilterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unifiedroleassignmentschedulerequestthisfilterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unifiedroleassignmentschedulerequestthisfilterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unifiedroleassignmentschedulerequestthisfilterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/unifiedroleassignmentschedulerequestthisfilterbycurrentuser-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/unifiedroleassignmentschedulerequestthisfilterbycurrentuser-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
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

