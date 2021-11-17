---
title: Обновление unifiedRoleDefinition
description: Обновление свойств объекта unifiedRoleDefinition.
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 1b276ef09c72d4945b74fff5ee660c20ab95cb10
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61017044"
---
# <a name="update-unifiedroledefinition"></a>Обновление unifiedRoleDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [unifiedRoleDefinition](../resources/unifiedroledefinition.md) для поставщика RBAC.

В настоящее время поддерживаются следующие поставщики RBAC:
- управление устройствами (Intune)
- каталог (Azure AD) 

> [!NOTE]
> Поставщик облачных ПК RBAC в настоящее время поддерживает только [список и](rbacapplication-list-roledefinitions.md) [получать](unifiedroledefinition-get.md) операции.

## <a name="permissions"></a>Разрешения

В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API. Дополнительные данные, [](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) в том числе осторожность перед выбором более привилегированных разрешений, поиск следующих разрешений в ссылке [Permissions](/graph/permissions-reference). 

### <a name="for-device-management-intune-provider"></a>Для поставщика управления устройствами (Intune)

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  DeviceManagementRBAC.ReadWrite.All   |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | DeviceManagementRBAC.ReadWrite.All |

### <a name="for-directory-azure-ad-provider"></a>Поставщик каталогов (Azure AD)

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

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:-----------|
| Authorization | Bearer {token} |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|Строка| Описание определения роли. Только для чтения, когда isBuiltIn является правдой. |
|displayName|String| Имя отображения для определения роли. Только для чтения, когда isBuiltIn является правдой. Обязательный.|
|id|String| Уникальный идентификатор определения роли. Key, not nullable, Read-only. |
|isBuiltIn|Boolean| Флаг, указывающий, является ли определение роли частью набора по умолчанию, включенного в продукт или настраиваемый. Только для чтения. |
|isEnabled|Boolean| Флаг, указывающий, включена ли роль для назначения. Если значение false, роль недоступна для назначения. Только для чтения, когда isBuiltIn является правдой. |
|resourceScopes|Коллекция String| К списку областей применяются разрешения, предоставленные определением ролей. В настоящее время поддерживается только "/". Только для чтения, когда isBuiltIn является правдой. **НЕ ИСПОЛЬЗУЙТЕ. В ближайшее время это свойство будет обесценилось. Прикрепить область к назначению ролей.**|
|rolePermissions|[коллекция unifiedRolePermission](../resources/unifiedrolepermission.md)| Список разрешений, включенных в роль. Только для чтения, когда isBuiltIn является правдой. Обязательный. |
|templateId|Строка| Настраиваемый идентификатор шаблона, который можно установить, когда isBuiltIn является ложным. Этот идентификатор обычно используется, если требуется, чтобы идентификатор был одинаковым в разных каталогах. Только для чтения, когда isBuiltIn является правдой. |
|inheritsPermissionsFrom| [коллекция unifiedRoleDefinition](../resources/unifiedroledefinition.md)| Только для чтения набор определений ролей, которые наследует заданное определение роли. Только встроенные роли Azure AD поддерживают этот атрибут. |
|version|String| Указывает версию определения роли. Только для чтения, когда isBuiltIn является правдой.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

В следующем примере **обновляется единоеroleDefinition** для поставщика каталогов.


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

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-unifiedroledefinition-go-snippets.md)]
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


