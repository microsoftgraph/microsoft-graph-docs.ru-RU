---
title: Создание unifiedRoleAssignmentScheduleRequest
description: В PIM запросите активное и постоянное назначение ролей через объект unifiedRoleAssignmentScheduleRequest. Используйте этот API для активации допустимых ролей.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e8295babb10821b9949231bb27ebb20b8570662d
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134376"
---
# <a name="create-unifiedroleassignmentschedulerequest"></a>Создание unifiedRoleAssignmentScheduleRequest
Пространство имен: microsoft.graph

В PIM выполните следующие операции с помощью объекта [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) :
+ Запрашивать активные и постоянные назначения ролей для субъекта с датами окончания срока действия или без них.
+ Активация, деактивация, продление или продление допустимого назначения роли для субъекта.

Чтобы вызвать этот API для обновления, продления и расширения назначений для себя, необходимо применить многофакторную проверку подлинности (MFA) и выполнить запрос в сеансе, в котором они запрашивались для MFA. См[. раздел "Включение Azure AD многофакторной идентификации для защиты событий входа"](/azure/active-directory/authentication/howto-mfa-userstates).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|RoleAssignmentSchedule.ReadWrite.Directory|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|RoleAssignmentSchedule.ReadWrite.Directory|

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

При создании объекта **unifiedRoleAssignmentScheduleRequest** можно указать следующие свойства.

|Свойство|Тип|Описание|
|:---|:---|:---|
|action|unifiedRoleScheduleRequestActions|Представляет тип операции в запросе на назначение роли. Возможные значения: `adminAssign`, `adminUpdate`, `adminRemove`, `selfActivate`, `selfDeactivate`, `adminExtend`, `adminRenew`, `selfExtend`, `selfRenew`, `unknownFutureValue`. <br/><ul><li>`adminAssign`: администраторы могут назначать роли пользователям или группам.</li><li>`adminRemove`: администраторы могут удалять пользователей или группы из ролей.</li><li> `adminUpdate`: администраторы могут изменять существующие назначения ролей.</li><li>`adminExtend`: администраторы могут продлить назначения с истекающим сроком действия.</li><li>`adminRenew`: чтобы администраторы продлевали назначения с истекшим сроком действия.</li><li>`selfActivate`: для активации назначений пользователями.</li><li>`selfDeactivate`: для отключения активных назначений пользователями.</li><li>`selfExtend`: пользователи должны запрашивать продление назначений с истекающим сроком действия.</li><li>`selfRenew`: чтобы пользователи запрашивали продление назначений с истекшим сроком действия.</li></ul>|
|Customdata|String|Поле "Бесплатный текст" для определения любых пользовательских данных для запроса. Необязательное свойство.|
|principalId|String|Идентификатор участника, которым было предоставлено назначение. Обязательный.|
|roleDefinitionId|String|Идентификатор [назначаемого объекта unifiedRoleDefinition](../resources/unifiedroledefinition.md) . Обязательный.|
|directoryScopeId|String|Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области каталога — это общие области, хранящиеся в каталоге, которые распознаются несколькими приложениями. Используется `/` для области на уровне клиента. Используйте **appScopeId** , чтобы ограничить область только приложением. Требуется **directoryScopeId** **или appScopeId** .|
|appScopeId|String|Идентификатор области, относяшейся к конкретному приложению, если назначение предназначено для приложения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области приложения — это области, которые определяются и распознаются только этим приложением. Используется `/` для областей приложений на уровне клиента. Используйте **directoryScopeId** , чтобы ограничить область определенными объектами каталога, например административными единицами. Требуется **directoryScopeId** **или appScopeId** .|
|Обоснование|String|Сообщение, предоставляемое пользователями и администраторами при создании объекта **unifiedRoleAssignmentScheduleRequest** . Необязательное свойство.|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|Период запроса на назначение роли. В настоящее время повторяющиеся расписания не поддерживаются. Обязательный.|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|Сведения о билете, связанные с запросом на назначение роли, включая сведения о номере билета и системе билетов. Необязательный параметр.|



## <a name="response"></a>Отклик

В случае успешного выполнения `201 Created` этот метод возвращает код отклика и объект [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-admin-assigning-a-directory-role-to-a-principal"></a>Пример 1. Администратор назначает роль каталога субъекту

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentschedulerequest_from_"
}
-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignmentScheduleRequests
Content-Type: application/json

{
    "action": "adminAssign",
    "justification": "Assign Groups Admin to IT Helpdesk group",
    "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "directoryScopeId": "/",
    "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
    "scheduleInfo": {
        "startDateTime": "2022-04-10T00:00:00Z",
        "expiration": {
            "type": "NoExpiration"
        }
    }
}
```


#### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleRequest"
}
-->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleAssignmentScheduleRequests/$entity",
    "id": "95c690fb-3eb3-4942-a03f-4524aed6f31e",
    "status": "Provisioned",
    "createdDateTime": "2022-04-11T11:50:03.9014347Z",
    "completedDateTime": "2022-04-11T11:50:05.9999343Z",
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
```

### <a name="example-2-user-activating-their-eligible-role"></a>Пример 2. Активация допустимой роли пользователем

#### <a name="request"></a>Запрос

В следующем запросе пользователь, определяемый **principalId**`071cc716-8147-4397-a5ba-b2105951cc0b`, активирует собственную доступную роль для роли Azure AD, определяемой идентификатором. `8424c6f0-a189-499e-bbd0-26c1753c96d4` Областью их роли является все объекты каталога в клиенте, а назначение — в течение пяти часов. Чтобы выполнить этот запрос, вызывающему пользователю необходимо применить многофакторную проверку подлинности (MFA) и выполнить запрос в сеансе, в котором он был запрошен для MFA.

Чтобы получить сведения о своих запросах на участие и определить допустимость активации, пользователь будет вызывать API [unifiedRoleEligibilitySchedule: filterByCurrentUser](unifiedroleeligibilityschedule-filterbycurrentuser.md) .

<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentschedulerequest_from_unifiedroleassignmentschedulerequests_selfActivate"
}
-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignmentScheduleRequests/
Content-Type: application/json

{
    "action": "selfActivate",
    "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
    "roleDefinitionId": "8424c6f0-a189-499e-bbd0-26c1753c96d4",
    "directoryScopeId": "/",
    "justification": "I need access to the Attribute Administrator role to manage attributes to be assigned to restricted AUs",
    "scheduleInfo": {
        "startDateTime": "2022-04-14T00:00:00.000Z",
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleAssignmentScheduleRequests/$entity",
    "id": "911bab8a-6912-4de2-9dc0-2648ede7dd6d",
    "status": "Granted",
    "createdDateTime": "2022-04-13T08:52:32.6485851Z",
    "completedDateTime": "2022-04-14T00:00:00Z",
    "approvalId": null,
    "customData": null,
    "action": "selfActivate",
    "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
    "roleDefinitionId": "8424c6f0-a189-499e-bbd0-26c1753c96d4",
    "directoryScopeId": "/",
    "appScopeId": null,
    "isValidationOnly": false,
    "targetScheduleId": "911bab8a-6912-4de2-9dc0-2648ede7dd6d",
    "justification": "I need access to the Attribute Administrator role to manage attributes to be assigned to restricted AUs",
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "displayName": null,
            "id": "071cc716-8147-4397-a5ba-b2105951cc0b"
        }
    },
    "scheduleInfo": {
        "startDateTime": "2022-04-14T00:00:00Z",
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