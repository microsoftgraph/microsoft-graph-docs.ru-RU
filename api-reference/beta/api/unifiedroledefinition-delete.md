---
title: Удаление unifiedRoleDefinition
description: Удаление объекта unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: e9f2d549cef274a536575a2671e454198dbb9f5f
ms.sourcegitcommit: 30903b12daf4cf2841524c57743889e23d11f85a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2021
ms.locfileid: "52709504"
---
# <a name="delete-unifiedroledefinition"></a>Удаление unifiedRoleDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удаление [объекта unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) для поставщика RBAC.

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

Удаление определения роли для поставщика управления устройствами:
<!-- { "blockType": "ignored" } -->
```http
DELETE /roleManagement/deviceManagement/roleDefinitions/{id}
```

Удаление определения роли для поставщика каталогов:
<!-- { "blockType": "ignored" } -->
```http
DELETE /roleManagement/directory/roleDefinitions/{id}

```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {token} |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

В следующем примере **удаляется единоеroleDefinition** для поставщика каталогов.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroledefinition"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


