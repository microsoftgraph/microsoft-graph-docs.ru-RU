---
title: Создание unifiedRoleEligibilityScheduleRequest
description: Создайте новый объект unifiedRoleEligibilityScheduleRequest.
author: japere
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b3b4c741c445de9a53bccd366c28abb0c98a5a8d
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510522"
---
# <a name="create-unifiedroleeligibilityschedulerequest"></a>Создание unifiedRoleEligibilityScheduleRequest
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новый [объект unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) . Эта операция позволяет администраторам и подходящим пользователям добавлять, отоперить или продлевать допустимые назначения.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|RoleEligibilitySchedule.ReadWrite.Directory|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|Не поддерживается|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /roleManagement/directory/roleEligibilityScheduleRequests
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) .

В следующей таблице показаны необязательные и необходимые свойства при создании [единойRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|action|Строка|Представляет тип операции по назначению права на роль. Возможные значения: <ul><li>`AdminAssign`. Чтобы администраторы назначали права на роль пользователям или группам в роли.</li><li>`AdminExtend`: Чтобы администраторы продлили назначения по истечении срока действия.</li><li>`AdminUpdate`: Чтобы администраторы изменили существующие назначения ролей.</li><li>`AdminRenew`. Чтобы администраторы возобновляли истекаемы назначения.</li><li>`AdminRemove`: Чтобы администраторы удаляли пользователей или группы из подходящих ролей.</li><li>`UserAdd`: Чтобы пользователи активировали соответствующие назначения.</li><li>`UserExtend`: Чтобы пользователи просили продлить срок действия соответствующих назначений.</li><li>`UserRemove`. Чтобы пользователи отключались от активных назначений.</li><li>`UserRenew`. Чтобы пользователи просили продлить срок действия своих назначений, имеющих право на срок действия.</li></ul>|
|appScopeId|String|Идентификатор области, определенной для приложения, когда область назначения является конкретной для приложения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области приложений — это области, которые определяются и понимаются только этим приложением. Используйте `/` для областей приложений для всех клиентов. Используйте **directoryScopeId** , чтобы ограничить область действия определенными объектами каталогов, например административными единицами или всеми пользователями.|
|directoryScopeId|Строка|Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте `/` для области для клиента. Используйте **appScopeId,** чтобы ограничить область только приложения.|
|isValidationOnly|Boolean|Boolean, определяющая, является ли вызов проверкой или фактическим вызовом. Только задайте это свойство, если необходимо проверить, подчиняется ли активация дополнительным правилам, таким как MFA, перед отправкой запроса.|
|обоснование|String|Сообщение, предоставленное пользователями и администраторами при создании запроса о необходимости. Необязательный **при действии** `AdminRemove`.|
|principalId|String|Идентификатор основного, которому предоставляется назначение. Например, пользователь или группа. Для групп они должны назначаться ролям, то есть **isAssignableToRole** свойства группы, задаваемого .`true`|
|roleDefinitionId|Строка|Идентификатор унифицированногоRoleDefinition для назначения. Обязательный аргумент. Только для чтения.|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|Объект расписания запроса назначения ролей. Это свойство не требуется при **действии** `AdminRemove`.|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|Объект ticketInfo, присоединенный к запросу назначения ролей, который включает сведения о номере билета и системе билетов. Необязательный параметр.|



## <a name="response"></a>Отклик

В случае успешной `201 Created` работы этот метод возвращает код ответа и объект [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-admin-to-assign-a-role-eligibility-schedule-request"></a>Пример 1. Администратор назначит запрос на расписание прав на роль

В следующем запросе `fdd7a751-b60b-444a-984c-02652fe8fa1c` администратор создает запрос на назначение права на роль, определяемую главным идентифицированным **по id** `07706ff1-46c7-4847-ae33-3003830675a1`. Область права — это все объекты каталога в клиенте до 30 июня 2022 г. в полночь по времени UTC.

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleeligibilityschedulerequest_from_unifiedroleeligibilityschedulerequests"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests
Content-Type: application/json

{
  "action": "AdminAssign",
  "justification": "Assign User Admin eligibility to IT Helpdesk (User) group",
  "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
  "directoryScopeId": "/",
  "principalId": "07706ff1-46c7-4847-ae33-3003830675a1",
  "scheduleInfo": {
    "startDateTime": "2021-07-01T00:00:00Z",
    "expiration": {
      "endDateTime": "2022-06-30T00:00:00Z",
      "type": "AfterDateTime"
    }
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик

Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleRequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleEligibilityScheduleRequests/$entity",
    "id": "672c03bf-226a-42ec-a8b7-3bfab96064a1",
    "status": "Provisioned",
    "createdDateTime": "2021-07-26T18:08:03.1299669Z",
    "completedDateTime": "2021-07-26T18:08:06.2081758Z",
    "approvalId": null,
    "customData": null,
    "action": "AdminAssign",
    "principalId": "07706ff1-46c7-4847-ae33-3003830675a1",
    "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "directoryScopeId": "/",
    "appScopeId": null,
    "isValidationOnly": false,
    "targetScheduleId": "672c03bf-226a-42ec-a8b7-3bfab96064a1",
    "justification": "Assign User Admin eligibility to IT Helpdesk (User) group",
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "displayName": null,
            "id": "fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f"
        }
    },
    "scheduleInfo": {
        "startDateTime": "2021-07-26T18:08:06.2081758Z",
        "recurrence": null,
        "expiration": {
            "type": "afterDateTime",
            "endDateTime": "2022-06-30T00:00:00Z",
            "duration": null
        }
    },
    "ticketInfo": {
        "ticketNumber": null,
        "ticketSystem": null
    }
}
```

### <a name="example-2-admin-to-remove-an-existing-role-eligibility-schedule-request"></a>Пример 2. Администратор для удаления существующего запроса на получение права на роль

В следующем запросе `fdd7a751-b60b-444a-984c-02652fe8fa1c` администратор создает запрос об отводе права на роль, определяемую главным идентифицированным **id**`07706ff1-46c7-4847-ae33-3003830675a1`.

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleeligibilityschedulerequest_from_unifiedroleeligibilityschedulerequests_AdminRemove"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests
Content-Type: application/json

{
    "action": "AdminRemove",
    "justification": "Assign User Admin eligibility to IT Helpdesk (User) group",
    "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "directoryScopeId": "/",
    "principalId": "07706ff1-46c7-4847-ae33-3003830675a1",
    "scheduleInfo": {
        "startDateTime": "2021-07-26T18:08:06.2081758Z",
        "expiration": {
            "endDateTime": "2022-06-30T00:00:00Z",
            "type": "AfterDateTime"
        }
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-adminremove-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-adminremove-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-adminremove-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-adminremove-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-adminremove-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-adminremove-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




#### <a name="response"></a>Отклик

Ниже приведен пример ответа. Запрос возвращает объект ответа, который отображает состояние ранее подходящих изменений назначения как `Revoked`. Директор больше не будет видеть свою ранее подходящую роль.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleRequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleEligibilityScheduleRequests/$entity",
    "id": "7f88a144-f9a9-4f8c-9623-39c321ae93c2",
    "status": "Revoked",
    "createdDateTime": "2021-08-06T17:59:12.4263499Z",
    "completedDateTime": null,
    "approvalId": null,
    "customData": null,
    "action": "AdminRemove",
    "principalId": "07706ff1-46c7-4847-ae33-3003830675a1",
    "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "directoryScopeId": "/",
    "appScopeId": null,
    "isValidationOnly": false,
    "targetScheduleId": null,
    "justification": "Assign User Admin eligibility to IT Helpdesk (User) group",
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "displayName": null,
            "id": "fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f"
        }
    },
    "scheduleInfo": {
        "startDateTime": "2021-07-26T18:08:06.2081758Z",
        "recurrence": null,
        "expiration": {
            "type": "afterDateTime",
            "endDateTime": "2022-06-30T00:00:00Z",
            "duration": null
        }
    },
    "ticketInfo": {
        "ticketNumber": null,
        "ticketSystem": null
    }
}
```
