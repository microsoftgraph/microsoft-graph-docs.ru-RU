---
title: Обновление unifiedRoleDefinition
description: Обновление свойств объекта unifiedRoleDefinition.
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: f35421b8f922c14e16930706cff10400520a0a85
ms.sourcegitcommit: 0fa7148e0b776663eaca3e79e72b85046d4b8b1a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/15/2022
ms.locfileid: "63500954"
---
# <a name="update-unifiedroledefinition"></a>Обновление unifiedRoleDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [unifiedRoleDefinition](../resources/unifiedroledefinition.md) для поставщика RBAC.


В настоящее время поддерживаются следующие поставщики RBAC:
- Облачный КОМПЬЮТЕР
- управление устройствами (Intune)
- каталог (Azure AD) 


## <a name="permissions"></a>Разрешения

В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующих таблиц наименее привилегированное разрешение, необходимое для вызова этого API. Дополнительные данные, в том [](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) числе осторожность перед выбором более привилегированных разрешений, поиск следующих разрешений в ссылке [Permissions](/graph/permissions-reference). 

### <a name="for-a-cloud-pc-provider"></a>Поставщик облачных ПК

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | RoleManagement.ReadWrite.CloudPC, CloudPC.ReadWrite.All   |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | RoleManagement.ReadWrite.CloudPC, CloudPC.ReadWrite.All  |

### <a name="for-a-device-management-intune-provider"></a>Для поставщика управления устройствами (Intune)

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  DeviceManagementRBAC.ReadWrite.All   |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | DeviceManagementRBAC.ReadWrite.All |

### <a name="for-a-directory-azure-ad-provider"></a>Поставщик каталогов (Azure AD)

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All   |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

Обновление определения ролей для поставщика управления устройствами:
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/deviceManagement/roleDefinitions/{id}
```

Обновление определения ролей для поставщика каталогов:
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

Обновление определения ролей для поставщика облачных ПК:
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/cloudPc/roleDefinitions/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:-----------|
| Авторизация | Bearer {token} |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|String| Описание определения роли. Только для чтения, когда isBuiltIn является правдой. |
|displayName|String| Имя отображения для определения роли. Только для чтения, когда isBuiltIn является правдой. Обязательный.|
|id|String| Уникальный идентификатор определения роли. Key, not nullable, Read-only. |
|isBuiltIn|Boolean| Флаг, указывающий, является ли определение роли частью набора по умолчанию, включенного в продукт или настраиваемый. Только для чтения. |
|isEnabled|Boolean| Флаг, указывающий, включена ли роль для назначения. Если значение false, роль недоступна для назначения. Только для чтения, когда isBuiltIn является правдой. |
|resourceScopes|Коллекция String| К списку областей применяются разрешения, предоставленные определением ролей. В настоящее время поддерживается только "/". Только для чтения, когда isBuiltIn является правдой. **НЕ ИСПОЛЬЗУЙТЕ. В ближайшее время это свойство будет обесценилось. Прикрепить область к назначению ролей.**|
|rolePermissions|[коллекция unifiedRolePermission](../resources/unifiedrolepermission.md)| Список разрешений, включенных в роль. Только для чтения, когда isBuiltIn является правдой. Обязательный. |
|templateId|String| Настраиваемый идентификатор шаблона, который можно установить, когда isBuiltIn является ложным. Этот идентификатор обычно используется, если требуется, чтобы идентификатор был одинаковым в разных каталогах. Только для чтения, когда isBuiltIn является правдой. |
|inheritsPermissionsFrom| [коллекция unifiedRoleDefinition](../resources/unifiedroledefinition.md)| Только для чтения набор определений ролей, которые наследует заданное определение роли. Только встроенные роли Azure AD поддерживают этот атрибут. |
|version|String| Указывает версию определения роли. Только для чтения, когда isBuiltIn является правдой.|

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`.

## <a name="example-1-updates-a-unifiedroledefinition-for-a-directory-provider"></a>Пример 1. Обновление **единой системыRoleDefinition** для поставщика каталогов

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroledefinition"
}-->

```http
PATCH https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/0d55728d-3e24-4309-9b1b-5ac09921475a
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
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-unifiedroledefinition-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-unifiedroledefinition-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.
> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
Content-type: application/json

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update unifiedroledefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="example-2-updates-a-unifiedroledefinition-for-a-cloudpc-provider"></a>Пример 2. Обновление **единогоroleDefinition** для поставщика CloudPC

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroledefinition_cloudpc"
}-->

```http
PATCH https://graph.microsoft.com/beta/roleManagement/cloudPc/roleDefinitions/b7f5ddc1-b7dc-4d37-abce-b9d6fc15ffff
Content-type: application/json

{
  "description": "Update basic properties and permission of application registrations",
  "displayName": "ExampleCustomRole",
  "rolePermissions":
    [
        {
            "allowedResourceActions": 
            [
                "Microsoft.CloudPC/CloudPCs/Read",
                "Microsoft.CloudPC/CloudPCs/Reprovision"
            ]
        }
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroledefinition-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-unifiedroledefinition-cloudpc-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-unifiedroledefinition-cloudpc-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.
> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
Content-type: application/json

```
