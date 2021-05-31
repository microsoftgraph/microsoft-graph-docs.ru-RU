---
title: Создание unifiedRoleDefinition
description: Создайте новый объект unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: e5512205b346d1005b8ce51f3ab11afa4f95a9a2
ms.sourcegitcommit: 30903b12daf4cf2841524c57743889e23d11f85a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2021
ms.locfileid: "52709509"
---
# <a name="create-unifiedroledefinition"></a>Создание unifiedRoleDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового [единого объектаRoleDefinition](../resources/unifiedroledefinition.md) для поставщика RBAC.

В настоящее время поддерживаются следующие поставщики RBAC:
- управление устройствами (Intune)
- каталог (Azure AD) 

> [!NOTE]
> Поставщик облачных ПК RBAC в настоящее время поддерживает только [список и](rbacapplication-list-roledefinitions.md) [получать](unifiedroledefinition-get.md) операции.

## <a name="permissions"></a>Разрешения

В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API. Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference). 

|Поддерживаемый поставщик      | Делегированные (рабочая или учебная учетная запись)  | Делегированное (личная учетная запись Майкрософт) | Для приложений |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| Управление устройствами | DeviceManagementRBAC.ReadWrite.All | Не поддерживается. | DeviceManagementRBAC.ReadWrite.All |
| Каталог | RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All | Не поддерживается.| RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

Чтобы создать определение роли для поставщика управления устройствами:
<!-- { "blockType": "ignored" } -->
```http
POST /roleManagement/deviceManagement/roleDefinitions
```

Чтобы создать определение роли для поставщика каталогов:
<!-- { "blockType": "ignored" } -->
```http
POST /roleManagement/directory/roleDefinitions
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {token} |

## <a name="request-body"></a>Тело запроса

В теле запроса поставляем представление JSON объекта [unifiedRoleDefinition.](../resources/unifiedroledefinition.md)

В следующей таблице показаны свойства, необходимые при создании roleDefinition.

| Параметр | Тип | Описание|
|:---------------|:--------|:----------|
|displayName |string |Имя отображения для определения роли.|
|isEnabled |Boolean |Флаг, указывающий, включена ли роль для назначения. Если значение false, роль недоступна для назначения.|
|rolePermissions |[коллекция unifiedRolePermission](../resources/unifiedrolepermission.md) |Список разрешений, включенных в роль.|

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика и новый `201 Created` [объект unifiedRoleDefinition](../resources/unifiedroledefinition.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приводится пример создания настраиваемой роли поставщика каталогов.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroledefinition_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions
Content-type: application/json

{
  "description": "Update basic properties of application registrations",
  "displayName": "Application Registration Support Administrator",
  "rolePermissions":
    [
        {
            "allowedResourceActions": 
            [
                "microsoft.directory/applications/basic/read"
            ]
        }
    ],
    "isEnabled" : "true"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroledefinition-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroledefinition-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroledefinition-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroledefinition-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.
> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions/$entity",
    "id": "d5eec5e0-6992-4c6b-b430-0f833f1a815a",
    "description": "Update basic properties of application registrations",
    "displayName": "Application Registration Support Administrator",
    "isBuiltIn": false,
    "isEnabled": true,
    "templateId": "c2cb59a3-2d01-4176-a458-95b0e674966f",
    "version": null,
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/standard/read",
                "microsoft.directory/applications/basic/update"
            ],
            "condition": null
        }
    ],
    "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('c2cb59a3-2d01-4176-a458-95b0e674966f')/inheritsPermissionsFrom",
    "inheritsPermissionsFrom": []
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


