---
title: 'unifiedRoleAssignmentScheduleRequest: filterByCurrentUser'
description: Получить список объектов unifiedRoleAssignmentScheduleRequest и их свойств, отфильтрованных определенным пользователем
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 182ffc04a0c86838eea976c3c77496cba8a92f86
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53333977"
---
# <a name="unifiedroleassignmentschedulerequest-filterbycurrentuser"></a>unifiedRoleAssignmentScheduleRequest: filterByCurrentUser
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


Получите список объектов [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) и их свойств, связанных с определенным основным объектом.

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
GET /roleManagement/directory/roleAssignmentScheduleRequests/filterByCurrentUser
```

## <a name="query-parameters"></a>Параметры запроса
В следующей таблице показаны параметры запроса, которые можно использовать с помощью этого метода.

|Параметр|Тип|Описание|
|:---|:---|:---|
|on|RoleAssignmentScheduleRequestFilterByCurrentUserOptions|Id основного объекта.|


## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код ответа и `200 OK` [унифицированную коллекциюRoleAssignmentScheduleRequest](../resources/unifiedRoleAssignmentScheduleRequest.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "unifiedroleassignmentschedulerequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/RoleAssignmentScheduleRequests/filterByCurrentUser(on='d6e4112f-112f-d6e4-2f11-e4d62f11e4d6')
```


### <a name="response"></a>Отклик
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
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
  "value": [
    {
      "id": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "action": "AdminAssign",
      "principalId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "roleDefinitionId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "directoryScopeId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "appScopeId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "isValidationOnly": false,
      "targetScheduleId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "justification": "this is a justification",
      "scheduleInfo": {
        "@odata.type": "microsoft.graph.requestSchedule"
      },
      "ticketInfo": {
        "@odata.type": "microsoft.graph.ticketInfo"
      }
    }
  ]
}
```

