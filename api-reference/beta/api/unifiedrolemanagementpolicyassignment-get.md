---
title: Get unifiedRoleManagementPolicyAssignment
description: Ознакомьтесь с свойствами и отношениями единого объектаRoleManagementPolicyAssignment.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c5efdf8e2890651c8629efb27837ffb1953c1376
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682322"
---
# <a name="get-unifiedrolemanagementpolicyassignment"></a>Get unifiedRoleManagementPolicyAssignment
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ознакомьтесь с свойствами и отношениями единого [объектаRoleManagementPolicyAssignment.](../resources/unifiedrolemanagementpolicyassignment.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|PrivilegedAccess.ReadWrite.AzureAD|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|PrivilegedAccess.Read.AzureAD|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicyAssignments/{unifiedRoleManagementPolicyAssignmentId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает все параметры запроса OData, чтобы помочь настроить ответ. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код ответа и `200 OK` [унифицированный объектRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedrolemanagementpolicyassignment"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicyAssignments/d6e4112f-112f-d6e4-2f11-e4d62f11e4d6
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedrolemanagementpolicyassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedrolemanagementpolicyassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedrolemanagementpolicyassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedrolemanagementpolicyassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyAssignment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6",
    "policyId": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6",
    "scopeId": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6",
    "scopeType": "subscription",
    "roleDefinitionId": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6"
  }
}
```

