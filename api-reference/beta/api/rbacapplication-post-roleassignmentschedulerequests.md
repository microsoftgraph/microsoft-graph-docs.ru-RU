---
title: Создание roleAssignmentScheduleRequests
description: Создайте объект unifiedRoleAssignmentScheduleRequest.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c635af3e8e315ed11cb3096a7f97b2b93eddefbb
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461770"
---
# <a name="create-roleassignmentschedulerequests"></a>Создание roleAssignmentScheduleRequests
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте объект [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) . Эта операция позволяет администраторам и пользователям добавлять, удалять, расширять или продлевать назначения. Чтобы выполнить этот запрос, вызывающему пользователю необходимо применить многофакторную проверку подлинности (MFA) и выполнить запрос в сеансе, в котором он был запрошен для MFA. См[. раздел "Включение Azure AD многофакторной идентификации для защиты событий входа"](/azure/active-directory/authentication/howto-mfa-userstates).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|RoleAssignmentSchedule.ReadWrite.Directory|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Для приложений|Не поддерживается|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /roleManagement/directory/roleAssignmentScheduleRequests
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) в формате JSON.

В следующей таблице показаны свойства, необходимые при создании [объекта unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта unifiedRoleAssignmentScheduleRequest. Ключ, не допускающий значения NULL, только для чтения.|
|action|String|Представляет тип операции назначения роли. Возможные значения: <ul><li>`AdminAssign`: администраторы могут назначать роли пользователям или группам.</li><li>`AdminRemove`: администраторы могут удалять пользователей или группы из ролей.</li><li> `AdminUpdate`: администраторы могут изменять существующие назначения ролей.</li><li>`AdminExtend`: администраторы могут продлить назначения с истекающим сроком действия.</li><li>`AdminRenew`: чтобы администраторы продлевали назначения с истекшим сроком действия.</li><li>`SelfActivate`: для активации назначений пользователями.</li><li>`SelfDeactivate`: для отключения активных назначений пользователями.</li><li>`SelfExtend`: пользователи должны запрашивать продление назначений с истекающим сроком действия.</li><li>`SelfRenew`: чтобы пользователи запрашивали продление назначений с истекшим сроком действия.</li></ul>
|principalId|Строка|Идентификатор субъекта, которому предоставляется назначение.|
|roleDefinitionId|Строка|Идентификатор объекта unifiedRoleDefinition, для который предназначено назначение. Только для чтения.|
|directoryScopeId|Строка|Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области каталога — это общие области, хранящиеся в каталоге, которые распознаются несколькими приложениями. Используется `/` для области на уровне клиента. Используйте **appScopeId** , чтобы ограничить область только приложением. |
|appScopeId|Строка|Идентификатор области, относяшейся к приложению, если область назначения предназначена для конкретного приложения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области приложения — это области, которые определяются и распознаются только этим приложением. Используется `/` для областей приложений на уровне клиента. Используйте **directoryScopeId** , чтобы ограничить область определенными объектами каталога, например административными единицами.|
|isValidationOnly|Boolean|Указывает, является ли вызов проверкой или фактическим вызовом. Задайте это свойство только в том случае, если вы хотите проверить, применяется ли активация к дополнительным правилам, таким как MFA, перед фактической отправкой запроса.|
|targetScheduleId|Строка|Идентификатор объекта расписания, присоединенного к назначению.|
|Обоснование|String|Сообщение, предоставленное пользователями и администраторами при создании запроса о том, зачем он нужен.|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|Объект расписания запроса на назначение роли.|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|Объект ticketInfo, присоединенный к запросу на назначение роли, который содержит сведения о номере билета и системе билетов.|

## <a name="response"></a>Отклик

В случае успешного выполнения `201 Created` этот метод возвращает код отклика и объект [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) в теле отклика.

Если вызывающему пользователю не была запрошена многофакторная проверка подлинности во время сеанса входа, запрос с действием SelfActivate `400 Bad request` завершается сбоем и возвращает код ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-admin-assigning-a-directory-role-to-a-principal"></a>Пример 1. Администратор назначает роль каталога субъекту

#### <a name="request"></a>Запрос

В следующем запросе администратор создает `fdd7a751-b60b-444a-984c-02652fe8fa1c` запрос на назначение роли, определяемой субъектом, определяемого **идентификатором**`07706ff1-46c7-4847-ae33-3003830675a1`. Областью их роли является все объекты каталога в клиенте, а назначение является постоянным, то есть срок его действия не истекает.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentschedulerequest_from_unifiedroleassignmentschedulerequests"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests/
Content-Type: application/json

{
  "action": "AdminAssign",
  "justification": "Assign User Admin to IT Helpdesk (User) group",
  "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
  "directoryScopeId": "/",
  "principalId": "07706ff1-46c7-4847-ae33-3003830675a1",
  "scheduleInfo": {
    "startDateTime": "2021-07-01T00:00:00Z",
    "expiration": {
      "type": "NoExpiration"
    }
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик

Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleRequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignmentScheduleRequests/$entity",
  "id": "b5a22921-656a-4429-9c4e-59a5f576614d",
  "status": "Provisioned",
  "createdDateTime": "2021-07-27T09:18:40.2029365Z",
  "completedDateTime": "2021-07-27T09:18:42.7811184Z",
  "approvalId": null,
  "customData": null,
  "action": "AdminAssign",
  "principalId": "07706ff1-46c7-4847-ae33-3003830675a1",
  "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
  "directoryScopeId": "/",
  "appScopeId": null,
  "isValidationOnly": false,
  "targetScheduleId": "b5a22921-656a-4429-9c4e-59a5f576614d",
  "justification": "Assign User Admin to IT Helpdesk (User) group",
  "createdBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": null,
      "id": "fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f"
    }
  },
  "scheduleInfo": {
    "startDateTime": "2021-07-27T09:18:42.7811184Z",
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
```

### <a name="example-2-user-activating-their-eligible-role"></a>Пример 2. Активация допустимой роли пользователем

#### <a name="request"></a>Запрос

В следующем запросе пользователь, определяемый **principalId**`c6ad1942-4afa-47f8-8d48-afb5d8d69d2f`, активирует собственную допустимую роль, определенную по `9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3`. Областью их роли является все объекты каталога в клиенте, а назначение — в течение пяти часов. Чтобы выполнить этот запрос, вызывающему пользователю необходимо применить многофакторную проверку подлинности (MFA) и выполнить запрос в сеансе, в котором он был запрошен для MFA.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentschedulerequest_from_unifiedroleassignmentschedulerequests_SelfActivate"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests/
Content-Type: application/json

{
    "action": "SelfActivate",
    "principalId": "c6ad1942-4afa-47f8-8d48-afb5d8d69d2f",
    "roleDefinitionId": "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
    "directoryScopeId": "/",
    "justification": "Need to update app roles for selected apps.",
    "scheduleInfo": {
        "startDateTime": "2021-08-17T17:40:00.000Z",
        "expiration": {
            "type": "AfterDuration",
            "duration": "PT5H"
        }
    },
    "ticketInfo": {
        "ticketNumber": "CONTOSO:Normal-67890",
        "ticketSystem": "MS Project"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-selfactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-selfactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-selfactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-selfactivate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-selfactivate-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-selfactivate-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик

Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleRequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignmentScheduleRequests/$entity",
    "id": "163daf73-8746-4996-87de-ab71dc624bf9",
    "status": "Granted",
    "createdDateTime": "2021-08-17T17:39:36.7040696Z",
    "completedDateTime": "2021-08-17T17:40:00Z",
    "approvalId": null,
    "customData": null,
    "action": "SelfActivate",
    "principalId": "c6ad1942-4afa-47f8-8d48-afb5d8d69d2f",
    "roleDefinitionId": "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
    "directoryScopeId": "/",
    "appScopeId": null,
    "isValidationOnly": false,
    "targetScheduleId": "163daf73-8746-4996-87de-ab71dc624bf9",
    "justification": "Need to update app roles for selected apps.",
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "displayName": null,
            "id": "c6ad1942-4afa-47f8-8d48-afb5d8d69d2f"
        }
    },
    "scheduleInfo": {
        "startDateTime": "2021-08-17T17:40:00Z",
        "recurrence": null,
        "expiration": {
            "type": "afterDuration",
            "endDateTime": null,
            "duration": "PT5H"
        }
    },
    "ticketInfo": {
        "ticketNumber": "CONTOSO:Normal-67890",
        "ticketSystem": "MS Project"
    }
}
```
