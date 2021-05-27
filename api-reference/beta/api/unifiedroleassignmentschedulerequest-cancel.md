---
title: 'unifiedRoleAssignmentScheduleRequest: отмена'
description: Отмена единой системыRoleAssignmentScheduleRequest.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: db696f4a7841557f743d2cea807f273b5d538230
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680453"
---
# <a name="unifiedroleassignmentschedulerequest-cancel"></a>unifiedRoleAssignmentScheduleRequest: отмена
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Немедленно [отмените унифицированныйRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) и задайте системе автоматическое удаление отмененного запроса через 30 дней.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|PrivilegedAccess.ReadWrite.AzureAD|
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
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения это действие возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "unifiedroleassignmentschedulerequest_cancel"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}/cancel
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

---



### <a name="response"></a>Отклик
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

