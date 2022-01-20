---
title: Создание unifiedRoleAssignmentScheduleRequest
description: Создайте новый объект unifiedRoleAssignmentScheduleRequest.
author: carolinetempleton
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3caaa5a39542555f6cc89d2385fd56721bb55beb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62098421"
---
# <a name="create-unifiedroleassignmentschedulerequest"></a>Создание unifiedRoleAssignmentScheduleRequest
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новый [объект unifiedRoleAssignmentScheduleRequest.](../resources/unifiedroleassignmentschedulerequest.md) Эта операция позволяет администраторам и пользователям добавлять, удалять, расширять или продлевать назначения. Чтобы выполнить этот запрос, вызываемого пользователя необходимо применять многофакторную проверку подлинности (MFA) и запускать запрос в сеансе, в котором он был опровержение для MFA. См. в документе Включить многофакторную проверку подлинности Azure AD для обеспечения безопасности событий [регистрации.](/azure/active-directory/authentication/howto-mfa-userstates)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|RoleAssignmentSchedule.ReadWrite.Directory|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|Не поддерживается|

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
В теле запроса поставляем представление JSON объекта [unifiedRoleAssignmentScheduleRequest.](../resources/unifiedroleassignmentschedulerequest.md)

В следующей таблице показаны свойства, необходимые при создании [единой системыRoleAssignmentScheduleRequest.](../resources/unifiedroleassignmentschedulerequest.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для unifiedRoleAssignmentScheduleRequest. Key, not nullable, Read-only.|
|action|Строка|Представляет тип операции при назначении ролей. Возможные значения: <ul><li>`AdminAssign`: Чтобы администраторы назначали роли пользователям или группам.</li><li>`AdminRemove`: Чтобы администраторы удаляли пользователей или группы из ролей.</li><li> `AdminUpdate`: Чтобы администраторы изменили существующие назначения ролей.</li><li>`AdminExtend`: Чтобы администраторы продлили назначения по истечении срока действия.</li><li>`AdminRenew`. Чтобы администраторы возобновляли истекаемы назначения.</li><li>`SelfActivate`: Чтобы пользователи активировали свои назначения.</li><li>`SelfDeactivate`: Чтобы пользователи отключались от активных назначений.</li><li>`SelfExtend`. Чтобы пользователи просили продлить срок действия назначений.</li><li>`SelfRenew`: Чтобы пользователи запрашивали продление истеканий назначений.</li></ul>
|principalId|Строка|Идентификатор основного, которому предоставляется назначение.|
|roleDefinitionId|Строка|Идентификатор унифицированногоRoleDefinition для назначения. Только для чтения.|
|directoryScopeId|String|Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте `/` для области для клиента. Используйте **appScopeId,** чтобы ограничить область только приложения. |
|appScopeId|Строка|Идентификатор области, определенной для приложения, когда область назначения является конкретной для приложения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области приложений — это области, которые определяются и понимаются только этим приложением. Используйте `/` для областей приложений для всех клиентов. Используйте **directoryScopeId,** чтобы ограничить область для определенных объектов каталогов, например административных единиц.|
|isValidationOnly|Логический|Указывает, является ли вызов проверкой или фактическим вызовом. Только задайте это свойство, если необходимо проверить, подчиняется ли активация дополнительным правилам, таким как MFA, перед отправкой запроса.|
|targetScheduleId|Строка|ID объекта расписания, прикрепленного к назначению.|
|обоснование|Строка|Сообщение, предоставленное пользователями и администраторами при создании запроса о необходимости.|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|Объект расписания запроса назначения ролей.|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|Объект ticketInfo, присоединенный к запросу назначения ролей, который включает сведения о номере билета и системе билетов.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код ответа и `201 Created` объект [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) в тексте ответа.

Когда вызываемого пользователя не вызывалось для многофакторной проверки подлинности во время записи в сеансе, запрос с действием SelfActivate сбой и возвращает код `400 Bad request` ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-admin-assigning-a-directory-role-to-a-principal"></a>Пример 1. Назначение администратором роли каталога директору

#### <a name="request"></a>Запрос

В следующем запросе администратор создает запрос, чтобы назначить роль, определенную главной, `fdd7a751-b60b-444a-984c-02652fe8fa1c` идентифицированной **по id.** `07706ff1-46c7-4847-ae33-3003830675a1` Область их роли — это все объекты каталога в клиенте, а назначение является постоянным, то есть не истекает.

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

### <a name="example-2-user-activating-their-eligible-role"></a>Пример 2. Активация пользователем допустимой роли

#### <a name="request"></a>Запрос

В следующем запросе пользователь, идентифицированный **principalId,** активирует `c6ad1942-4afa-47f8-8d48-afb5d8d69d2f` свою собственную роль, определенную `9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3` . Область их роли — все объекты каталога в клиенте, а назначение — пять часов. Чтобы выполнить этот запрос, вызываемого пользователя необходимо применять многофакторную проверку подлинности (MFA) и запускать запрос в сеансе, в котором он был опровержение для MFA.


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
