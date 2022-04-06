---
title: Список унифицированныхRoleManagementPolicies
description: Получите список объектов unifiedRoleManagementPolicy и их свойств.
author: japere
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 0ee14bcd9dd97689c1260b1f681be7a13ed8d0e1
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510374"
---
# <a name="list-unifiedrolemanagementpolicies"></a>Список унифицированныхRoleManagementPolicies
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список объектов [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) и их свойств. Этот API применяется только к ролям Azure AD. Чтобы получить политики, применимые к Azure RBAC, используйте [API PIM REST Azure для политик управления ролью](/rest/api/authorization/role-management-policies/list-for-scope).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|RoleManagementPolicy.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagementPolicy.ReadWrite.Directory, RoleManagement.ReadWrite.Directory|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies?$filter=scopeId eq 'scopeId' and scopeType eq 'scopeType'
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает все параметры запроса OData, чтобы помочь настроить ответ. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного `200 OK` выполнения этот метод возвращает код ответа и коллекцию объектов [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

В следующем примере извлекаются политики, масштабные для клиента, и применяются к ролям каталогов.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicies?$filter=scopeId eq '/' and scopeType eq 'DirectoryRole'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedrolemanagementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedrolemanagementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedrolemanagementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedrolemanagementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-unifiedrolemanagementpolicy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-unifiedrolemanagementpolicy-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleManagementPolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/roleManagementPolicies",
    "value": [
        {
            "id": "DirectoryRole_84841066-274d-4ec0-a5c1-276be684bdd3_200ec19a-09e7-4e7a-9515-cf1ee64b96f9",
            "displayName": "DirectoryRole",
            "description": "DirectoryRole",
            "isOrganizationDefault": false,
            "scopeId": "/",
            "scopeType": "DirectoryRole",
            "lastModifiedDateTime": null,
            "lastModifiedBy": {
                "displayName": null,
                "id": null
            }
        },
        {
            "id": "DirectoryRole_84841066-274d-4ec0-a5c1-276be684bdd3_da83a66c-eb51-44ae-98d8-3da5f924f90a",
            "displayName": "DirectoryRole",
            "description": "DirectoryRole",
            "isOrganizationDefault": false,
            "scopeId": "/",
            "scopeType": "DirectoryRole",
            "lastModifiedDateTime": null,
            "lastModifiedBy": {
                "displayName": null,
                "id": null
            }
        }
    ]
}
```

