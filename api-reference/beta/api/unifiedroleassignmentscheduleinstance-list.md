---
title: Перечисление объектов unifiedRoleAssignmentScheduleInstance
description: Получение списка объектов unifiedRoleAssignmentScheduleInstance и их свойств.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ce3c9e9706e28b5afe9dfa51e41fb1eb7cd8c472
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399252"
---
# <a name="list-unifiedroleassignmentscheduleinstances"></a>Перечисление объектов unifiedRoleAssignmentScheduleInstance
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка объектов [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) и их свойств.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Для приложения|RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleInstances
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметры `$select` запроса `$filter` oData и для настройки ответа. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного `200 OK` выполнения этот метод возвращает код отклика и коллекцию объектов [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentscheduleinstance"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleInstances
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedroleassignmentscheduleinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedroleassignmentscheduleinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedroleassignmentscheduleinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedroleassignmentscheduleinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-unifiedroleassignmentscheduleinstance-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-unifiedroleassignmentscheduleinstance-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик

Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleAssignmentScheduleInstance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignmentScheduleInstances",
  "value": [
    {
      "id": "4-PYiFWPHkqVOpuYmLiHa_8KmpPnrkhHmG41_UYRbUY-1",
      "principalId": "939a0aff-aee7-4748-986e-35fd46116d46",
      "roleDefinitionId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
      "directoryScopeId": "/",
      "appScopeId": null,
      "startDateTime": null,
      "endDateTime": null,
      "assignmentType": "Assigned",
      "memberType": "Direct",
      "roleAssignmentOriginId": "4-PYiFWPHkqVOpuYmLiHa_8KmpPnrkhHmG41_UYRbUY-1",
      "roleAssignmentScheduleId": "4-PYiFWPHkqVOpuYmLiHa_8KmpPnrkhHmG41_UYRbUY-1"
    },
    {
      "id": "4-PYiFWPHkqVOpuYmLiHa0VbFrscFfZMmRHNcYiRKEg-1",
      "principalId": "bb165b45-151c-4cf6-9911-cd7188912848",
      "roleDefinitionId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
      "directoryScopeId": "/",
      "appScopeId": null,
      "startDateTime": null,
      "endDateTime": null,
      "assignmentType": "Assigned",
      "memberType": "Direct",
      "roleAssignmentOriginId": "4-PYiFWPHkqVOpuYmLiHa0VbFrscFfZMmRHNcYiRKEg-1",
      "roleAssignmentScheduleId": "4-PYiFWPHkqVOpuYmLiHa0VbFrscFfZMmRHNcYiRKEg-1"
    }
  ]
}
```

