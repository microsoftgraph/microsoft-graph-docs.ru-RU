---
title: Обновление governanceRoleAssignmentRequests
description: Администраторы могли обновлять свои решения (`AdminApproved` или `AdminDenied`) на governanceRoleAssignmentRequests, находятся в состоянии `PendingAdminDecision`.
ms.openlocfilehash: 0f52b810b861e18a679ae8aea4ffdf7fd2d67abd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082292"
---
# <a name="update-governanceroleassignmentrequests"></a>Обновление governanceRoleAssignmentRequests

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Администраторы могли обновлять свои решения (`AdminApproved` или `AdminDenied`) на [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) , находятся в состоянии `PendingAdminDecision`.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Permissions              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureResources  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложения | PrivilegedAccess.ReadWrite.AzureResources |

Помимо области разрешений этот интерфейс API требует инициатор запроса может иметь по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) на ресурс, который принадлежит [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) . 

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

### <a name="request-headers"></a>Заголовки запросов
| Имя           | Описание|
|:---------------|:----------|
| Authorization  | Bearer {code}|
| Content-Type  | application/json|

### <a name="request-body"></a>Текст запроса
|Parameters      |Тип                   |Обязательный |Описание|
|:-------------|:----------------------|:--------|:----------|
|Причина        |String                 |✓        |Причины, предоставленный администратором для его решение.|
|решение        |String                 |✓        |Администратор решение для запроса назначений ролей. Значение должно быть обновлено как `AdminApproved` или `AdminDenied`.|
|расписание      |[governanceSchedule](../resources/governanceschedule.md)|        | Расписание для запроса назначений ролей. Состояние `AdminApproved`, это необходимо.|
|assignmentState      |String|         | Состояние назначения и значения, может быть `Eligible` или `Active`. Для принятия решений о `AdminApproved`, это необходимо. |
### <a name="response"></a>Ответ
Этот метод может применяться только к запросам, которые находятся в состоянии `PendingAdminDecision`.

В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.

### <a name="example"></a>Пример
##### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
##### <a name="request-body"></a>Текст запроса
```json
{
  "reason":"approve the request to extend role assignment",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-02-20T07:31:13.451Z",
    "stopDateTime":"2018-05-21T07:31:13.451Z",
    },
  "decision":"AdminApproved",
  "assignmentState": "Eligible"
}
```

##### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UpdateRequest governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
