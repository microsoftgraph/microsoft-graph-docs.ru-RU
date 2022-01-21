---
title: Перечисление объектов unifiedRoleAssignmentMultiple
description: Извлечение свойств и связей объекта unifiedRoleAssignmentMultiple.
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 3d9a05d9f9e6acd69b28a39c4325a6d170ab76ff
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123056"
---
# <a name="list-unifiedroleassignmentmultiple"></a>Перечисление объектов unifiedRoleAssignmentMultiple

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список объектов [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) для поставщика RBAC.

В настоящее время поддерживаются следующие поставщики RBAC:
- Облачный КОМПЬЮТЕР 
- управление устройствами (Intune)

Для других Microsoft 365 приложений (например, Azure AD) используйте [унифицированную системуRoleAssignment.](../resources/unifiedroleassignment.md)

## <a name="permissions"></a>Разрешения

В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API. Дополнительные новости, в том числе осторожность [перед](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) выбором более привилегированных разрешений, см. [в см. в руб. Permissions.](/graph/permissions-reference) 

### <a name="for-cloud-pc-provider"></a>Поставщик облачных ПК

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  CloudPC.Read.All, CloudPC.ReadWrite.All   |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | CloudPC.Read.All, CloudPC.ReadWrite.All  |

### <a name="for-device-management-intune-provider"></a>Для поставщика управления устройствами (Intune)

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All   |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All |


## <a name="http-request"></a>HTTP-запрос

Список назначений ролей для поставщика облачных ПК:

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/cloudPc/roleAssignments
```

Список назначений ролей для поставщика Intune:

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/deviceManagement/roleAssignments
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Вы можете фильтровать свойства `roleDefinitionId` или `principalId` свойства. Свойство `roleDefinitionId` может быть как ИД объекта роли, так и объектом шаблона ролей. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов

| Имя | Описание |
|:---- |:----------- |
| Авторизация | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) в теле ответа.

## <a name="example"></a>Пример

### <a name="example-1-list-the-role-assignments-for-a-specific-principal-for-an-intune-provider"></a>Пример 1. Список назначений ролей для определенного основного поставщика Intune

### <a name="request"></a>Запрос

Ниже приводится пример запроса:

<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentmultiple"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/$filter=principalId eq '9e47fc6f-2d7a-464c-944e-d3dd0de522e4'
```

### <a name="response"></a>Отклик

Ниже приводится пример ответа:
> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
    "value": [ 
       {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
            "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalIds[]": ["9e47fc6f-2d7a-464c-944e-d3dd0de522e4", "f8ca5a85-489a-49a0-b555-0a6d81e56f0d"],
            "directoryScopeIds[]": ["28ca5a85-489a-49a0-b555-0a6d81e56f0", "8152656a-cf9a-4928-a457-1512d4cae295"]
       },
       {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
            "id": "2BNpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SWRD-2",
            "roleDefinitionId": "9e47fc6f-2d7a-464c-944e-d3dd0de522e4",
            "principalIds[]": ["9e47fc6f-2d7a-464c-944e-d3dd0de522e4", "53a6c08d-0227-41bd-8bc6-2728df6be749", "a4991fe1-6d7c-427c-969b-bda6df78c458"],
            "appScopeIds[]": ["28ca5a85-489a-49a0-b555-0a6d81e56f0"]
       }
    ]
}
```
### <a name="example-2-list-role-assignments-for-a-cloud-pc-provider"></a>Пример 2. Список назначений ролей для поставщика облачных ПК

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcunifiedroleassignmentmultiple_1"
}-->

```msgraph-interactive
GET  https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcunifiedroleassignmentmultiple-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcunifiedroleassignmentmultiple-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcunifiedroleassignmentmultiple-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcunifiedroleassignmentmultiple-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-cloudpcunifiedroleassignmentmultiple-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-cloudpcunifiedroleassignmentmultiple-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleAssignments/$entity",
    "value": [
        {
            "id": "dbe9d288-fd87-41f4-b33d-b498ed207096",
            "description": null,
            "displayName": "My test role assignment 1",
            "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
            "principalIds": [
                "8e811502-ebda-4782-8f81-071d17f0f892",
                "30e3492f-964c-4d73-88c6-986a53c6e2a0"
            ],
            "directoryScopeIds": [
                "/"
            ],
            "appScopeIds": []
        },
        {
            "id": "fad74173-3fe3-4e64-9a80-297bdad2b36e",
            "description": null,
            "displayName": "My test role assignment 2",
            "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
            "principalIds": [
                "8e811502-ebda-4782-8f81-071d17f0f892",
            ],
            "directoryScopeIds": [
                "/"
            ],
            "appScopeIds": []
        }
    ]
}
```

### <a name="example-3-list-role-assignments-for-specific-role-of-a-cloud-pc-provider"></a>Пример 3. Список назначений ролей для определенной роли поставщика облачных ПК

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcunifiedroleassignmentmultiple_2"
}-->

```msgraph-interactive
GET  https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments?$filter=roleDefinitionId eq 'b5c08161-a7af-481c-ace2-a20a69a48fb1'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcunifiedroleassignmentmultiple-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcunifiedroleassignmentmultiple-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcunifiedroleassignmentmultiple-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcunifiedroleassignmentmultiple-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-cloudpcunifiedroleassignmentmultiple-2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-cloudpcunifiedroleassignmentmultiple-2-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleAssignments",
    "value": [{
        "id": "ed9e247f-f23b-4d72-9e8c-97fa6f385246",
        "description": "",
        "displayName": "test",
        "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
        "principalIds": ["689c9051-77ff-4f14-9b39-3d22de07321a"],
        "directoryScopeIds": ["/"],
        "appScopeIds": []
    }, {
        "id": "3d8e564b-761a-4b32-8f50-63d555f7bc00",
        "description": "test1",
        "displayName": "AssignmentTest",
        "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
        "principalIds": ["0ec7855b-4057-4b7c-9217-09ee9bf4dfd7"],
        "directoryScopeIds": ["/"],
        "appScopeIds": []
    }, {
        "id": "f36a3269-d03d-4d33-81e7-190bded40ad2",
        "description": "",
        "displayName": "test3",
        "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
        "principalIds": ["e4ea53cf-cdd6-46b5-bf38-570033a0fba3"],
        "directoryScopeIds": ["/"],
        "appScopeIds": []
    }]
}
```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List roleAssignmentsMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


