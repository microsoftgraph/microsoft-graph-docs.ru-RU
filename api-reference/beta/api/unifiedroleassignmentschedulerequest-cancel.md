---
title: 'unifiedRoleAssignmentScheduleRequest: отмена'
description: Отмена единой системыRoleAssignmentScheduleRequest.
author: carolinetempleton
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2314bd9284a5f801e64b2ddf38d5f0ff9b8e9914
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348192"
---
# <a name="unifiedroleassignmentschedulerequest-cancel"></a>unifiedRoleAssignmentScheduleRequest: отмена
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Немедленно отмените [объект unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)`Granted`, который находится в состоянии, и через 30 дней система автоматически удалит отмененный запрос. После вызова этого действия **состояние** отмененного unifiedRoleAssignmentScheduleRequest изменяется на `Canceled`.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|Не поддерживается|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}/cancel
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения это действие возвращает код отклика `204 No Content`.  Попытка отменить запрос, который не отменяется, например, объект unifiedRoleAssignmentScheduleRequest `Provisioned` `Failed``400 Bad Request`, состояние которого или , возвращает код ошибки.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "unifiedroleassignmentschedulerequest_cancel"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests/15fec3d4-64b1-4b03-beb7-f1ba6dddf6cc/cancel
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unifiedroleassignmentschedulerequest-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unifiedroleassignmentschedulerequest-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unifiedroleassignmentschedulerequest-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unifiedroleassignmentschedulerequest-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/unifiedroleassignmentschedulerequest-cancel-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/unifiedroleassignmentschedulerequest-cancel-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

