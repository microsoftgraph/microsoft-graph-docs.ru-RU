---
title: Обновление governanceRoleAssignmentRequests
description: Администраторы могли обновлять свои решения (`AdminApproved` или `AdminDenied`) на governanceRoleAssignmentRequests, находятся в состоянии `PendingAdminDecision`.
ms.openlocfilehash: bd924acd8ddd3a79ad1fb97ac5f9bdc9baba17dd
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191153"
---
# <a name="update-governanceroleassignmentrequests"></a>Обновление governanceRoleAssignmentRequests

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Администраторы могли обновлять свои решения (`AdminApproved` или `AdminDenied`) на [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) , находятся в состоянии `PendingAdminDecision`.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

>**Примечание:** Этот интерфейс API также требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) на ресурс, к которой принадлежит [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) . 

|Тип разрешения      | Разрешения              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureResources  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | PrivilegedAccess.ReadWrite.AzureResources |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a>Заголовки запросов
| Имя           | Описание|
|:---------------|:----------|
| Authorization  | Bearer {code}|
| Content-Type  | application/json|

## <a name="request-body"></a>Текст запроса

|Параметры      |Тип                   |Обязательный |Описание|
|:-------------|:----------------------|:--------|:----------|
|Причина        |Строка                 |✓        |Причины, предоставленный администратором для его решение.|
|решение        |Строка                 |✓        |Администратор решение для запроса назначений ролей. Значение должно быть обновлено как `AdminApproved` или `AdminDenied`.|
|расписание      |[governanceSchedule](../resources/governanceschedule.md)|        | Расписание для запроса назначений ролей. Состояние `AdminApproved`, это необходимо.|
|assignmentState      |Строка|         | Состояние назначения и значения, может быть `Eligible` или `Active`. Для принятия решений о `AdminApproved`, это необходимо. |
### <a name="response"></a>Отклик
Этот метод может применяться только к запросам, которые находятся в состоянии `PendingAdminDecision`.

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="example"></a>Пример
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
