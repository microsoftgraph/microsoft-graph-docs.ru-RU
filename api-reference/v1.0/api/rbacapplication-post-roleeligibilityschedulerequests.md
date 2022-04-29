---
title: Создание unifiedRoleEligibilityScheduleRequest
description: В PIM запросите право на роль для субъекта через объект unifiedRoleEligibilityScheduleRequest.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 871755979904dfa05156c814911a40b43a177914
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134373"
---
# <a name="create-unifiedroleeligibilityschedulerequest"></a>Создание unifiedRoleEligibilityScheduleRequest
Пространство имен: microsoft.graph

В PIM запросите право на роль для субъекта через объект [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) . Эта операция позволяет администраторам и соответствующим пользователям добавлять, отзывать или расширять допустимые назначения.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|RoleEligibilitySchedule.ReadWrite.Directory|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|RoleAssignmentSchedule.ReadWrite.Directory|

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
В тексте запроса добавьте представление объекта [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) в формате JSON.

При создании объекта **unifiedRoleEligibilityScheduleRequest** можно указать следующие свойства.

|Свойство|Тип|Описание|
|:---|:---|:---|
|action|unifiedRoleScheduleRequestActions|Представляет тип операции в запросе на получение прав на роль. Возможные значения: `adminAssign`, , `adminUpdate`, `adminRemove`, `selfActivate`, `selfDeactivate`, `adminExtend``adminRenew`, `selfExtend``selfRenew``unknownFutureValue`. <br/><ul><li>`adminAssign`: администраторы могут назначать субъектам допустимые роли.</li><li>`adminRemove`: чтобы администраторы удаляли допустимые роли из субъектов.</li><li> `adminUpdate`: чтобы администраторы меняли существующие права на роль.</li><li>`adminExtend`: чтобы администраторы расширяли права на роль с истекающим сроком действия.</li><li>`adminRenew`: чтобы администраторы продлевали просроченные права доступа.</li><li>`selfActivate`: для активации назначений пользователями.</li><li>`selfDeactivate`: для отключения активных назначений пользователями.</li><li>`selfExtend`: пользователи должны запрашивать продление назначений с истекающим сроком действия.</li><li>`SelfRenew`: чтобы пользователи запрашивали продление назначений с истекшим сроком действия.</li></ul>|
|appScopeId|String|Идентификатор области, относяшейся к приложению, если доступ к роли определяется приложением. Область действия роли определяет набор ресурсов, к которым субъект имеет право доступа. Области приложения — это области, которые определяются и распознаются только этим приложением. Используется `/` для областей приложений на уровне клиента. Используйте **directoryScopeId** , чтобы ограничить область определенными объектами каталога, например административными единицами. Требуется **directoryScopeId** **или appScopeId** .|
|directoryScopeId|String|Идентификатор объекта каталога, представляющего область допустимости роли. Область действия роли определяет набор ресурсов, к которым участнику был предоставлен доступ. Области каталога — это общие области, хранящиеся в каталоге, которые распознаются несколькими приложениями. Используется `/` для области на уровне клиента. Используйте **appScopeId** , чтобы ограничить область только приложением. Требуется **directoryScopeId** **или appScopeId** .|
|isValidationOnly|Boolean|Определяет, является ли вызов проверкой или фактическим вызовом. Задайте это свойство только в том случае, если вы хотите проверить, применяется ли активация к дополнительным правилам, таким как MFA, перед фактической отправкой запроса. Необязательное свойство.|
|Обоснование|String|Сообщение, предоставляемое пользователями и администраторами при создании объекта **unifiedRoleEligibilityScheduleRequest** . Необязательный, **если действие** имеет значение `adminRemove`.|
|principalId|String|Идентификатор участника, которой предоставлено право на роль. Обязательный.|
|roleDefinitionId|String|Идентификатор объекта [unifiedRoleDefinition](../resources/unifiedroledefinition.md) , назначаемого субъекту. Обязательный.|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|Период допустимости роли. В настоящее время повторяющиеся расписания не поддерживаются. Необязательный, **если действие** имеет значение `adminRemove`.|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|Сведения о билете, связанные с запросом на участие в роли, включая сведения о номере билета и системе билетов. Необязательна|


## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `201 Created` отклика и объект [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-admin-to-assign-a-role-eligibility-schedule-request"></a>Пример 1. Назначение администратором запроса на расписание соответствия роли

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleeligibilityschedulerequest_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/roleManagement/directory/roleEligibilityScheduleRequests
Content-Type: application/json

{
    "action": "adminAssign",
    "justification": "Assign Attribute Assignment Admin eligibility to restricted user",
    "roleDefinitionId": "8424c6f0-a189-499e-bbd0-26c1753c96d4",
    "directoryScopeId": "/",
    "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
    "scheduleInfo": {
        "startDateTime": "2022-04-10T00:00:00Z",
        "expiration": {
            "type": "afterDateTime",
            "endDateTime": "2024-04-10T00:00:00Z"
        }
    }
}
```


### <a name="response"></a>Отклик
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleEligibilityScheduleRequests/$entity",
    "id": "50877283-9d40-433c-bab8-7986dc10458a",
    "status": "Provisioned",
    "createdDateTime": "2022-04-12T09:05:39.7594064Z",
    "completedDateTime": "2022-04-12T09:05:41.8532931Z",
    "approvalId": null,
    "customData": null,
    "action": "adminAssign",
    "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
    "roleDefinitionId": "8424c6f0-a189-499e-bbd0-26c1753c96d4",
    "directoryScopeId": "/",
    "appScopeId": null,
    "isValidationOnly": false,
    "targetScheduleId": "50877283-9d40-433c-bab8-7986dc10458a",
    "justification": "Assign Attribute Assignment Admin eligibility to restricted user",
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "displayName": null,
            "id": "3fbd929d-8c56-4462-851e-0eb9a7b3a2a5"
        }
    },
    "scheduleInfo": {
        "startDateTime": "2022-04-12T09:05:41.8532931Z",
        "recurrence": null,
        "expiration": {
            "type": "afterDateTime",
            "endDateTime": "2024-04-10T00:00:00Z",
            "duration": null
        }
    },
    "ticketInfo": {
        "ticketNumber": null,
        "ticketSystem": null
    }
}
```

### <a name="example-2-admin-to-remove-an-existing-role-eligibility-schedule-request"></a>Пример 2. Удаление существующего запроса на расписание соответствия роли администратору

В следующем запросе `071cc716-8147-4397-a5ba-b2105951cc0b` администратор создает запрос на отмену права субъекта с идентификатором на роль с идентификатором `8424c6f0-a189-499e-bbd0-26c1753c96d4`.

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleeligibilityschedulerequest_from_unifiedroleeligibilityschedulerequests_adminRemove"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests
Content-Type: application/json

{
    "action": "adminRemove",
    "roleDefinitionId": "8424c6f0-a189-499e-bbd0-26c1753c96d4",
    "directoryScopeId": "/",
    "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b"
}
```


#### <a name="response"></a>Отклик

Ниже приведен пример отклика. Объект ответа показывает, что предыдущая роль для субъекта имеет значение `Revoked`. Субъект больше не будет видеть свою ранее допустимую роль.

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleEligibilityScheduleRequests/$entity",
    "id": "f341269e-c926-41fa-a905-cef3b01b2a67",
    "status": "Revoked",
    "createdDateTime": "2022-04-12T09:12:15.6859992Z",
    "completedDateTime": null,
    "approvalId": null,
    "customData": null,
    "action": "adminRemove",
    "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
    "roleDefinitionId": "8424c6f0-a189-499e-bbd0-26c1753c96d4",
    "directoryScopeId": "/",
    "appScopeId": null,
    "isValidationOnly": false,
    "targetScheduleId": null,
    "justification": null,
    "scheduleInfo": null,
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "displayName": null,
            "id": "3fbd929d-8c56-4462-851e-0eb9a7b3a2a5"
        }
    },
    "ticketInfo": {
        "ticketNumber": null,
        "ticketSystem": null
    }
}
```