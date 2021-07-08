---
title: Удаление unifiedRoleDefinition
description: Удаление объекта unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7de16492df085b48d2fe580ff54d3cacf9dc0d22
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334373"
---
# <a name="delete-unifiedroledefinition"></a><span data-ttu-id="09ba2-103">Удаление unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="09ba2-103">Delete unifiedRoleDefinition</span></span>

<span data-ttu-id="09ba2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09ba2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09ba2-105">Удаление [объекта unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) для поставщика RBAC.</span><span class="sxs-lookup"><span data-stu-id="09ba2-105">Delete a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object for an RBAC provider.</span></span>

<span data-ttu-id="09ba2-106">В настоящее время поддерживаются следующие поставщики RBAC:</span><span class="sxs-lookup"><span data-stu-id="09ba2-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="09ba2-107">управление устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="09ba2-107">device management (Intune)</span></span>
- <span data-ttu-id="09ba2-108">каталог (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="09ba2-108">directory (Azure AD)</span></span> 

> [!NOTE]
> <span data-ttu-id="09ba2-109">Поставщик облачных ПК RBAC в настоящее время поддерживает только [список и](rbacapplication-list-roledefinitions.md) [получать](unifiedroledefinition-get.md) операции.</span><span class="sxs-lookup"><span data-stu-id="09ba2-109">The cloud PC RBAC provider currently supports only the [list](rbacapplication-list-roledefinitions.md) and [get](unifiedroledefinition-get.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="09ba2-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="09ba2-110">Permissions</span></span>

<span data-ttu-id="09ba2-111">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="09ba2-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="09ba2-112">Дополнительные новости, в том числе осторожность [перед](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) выбором более привилегированных разрешений, см. [в см. в руб. Permissions.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="09ba2-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, see [Permissions](/graph/permissions-reference).</span></span> 

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="09ba2-113">Для поставщика управления устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="09ba2-113">For Device management (Intune) provider</span></span>

|<span data-ttu-id="09ba2-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09ba2-114">Permission type</span></span>      | <span data-ttu-id="09ba2-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="09ba2-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09ba2-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09ba2-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="09ba2-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09ba2-117">DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="09ba2-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09ba2-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09ba2-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09ba2-119">Not supported.</span></span>    |
|<span data-ttu-id="09ba2-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="09ba2-120">Application</span></span> | <span data-ttu-id="09ba2-121">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09ba2-121">DeviceManagementRBAC.ReadWrite.All</span></span> |

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="09ba2-122">Поставщик каталогов (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="09ba2-122">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="09ba2-123">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09ba2-123">Permission type</span></span>      | <span data-ttu-id="09ba2-124">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="09ba2-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09ba2-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09ba2-125">Delegated (work or school account)</span></span> |  <span data-ttu-id="09ba2-126">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="09ba2-126">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="09ba2-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09ba2-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09ba2-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09ba2-128">Not supported.</span></span>    |
|<span data-ttu-id="09ba2-129">Приложение</span><span class="sxs-lookup"><span data-stu-id="09ba2-129">Application</span></span> | <span data-ttu-id="09ba2-130">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09ba2-130">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="09ba2-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09ba2-131">HTTP request</span></span>

<span data-ttu-id="09ba2-132">Удаление определения роли для поставщика управления устройствами:</span><span class="sxs-lookup"><span data-stu-id="09ba2-132">To delete a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /roleManagement/deviceManagement/roleDefinitions/{id}
```

<span data-ttu-id="09ba2-133">Удаление определения роли для поставщика каталогов:</span><span class="sxs-lookup"><span data-stu-id="09ba2-133">To delete a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /roleManagement/directory/roleDefinitions/{id}

```

## <a name="request-headers"></a><span data-ttu-id="09ba2-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09ba2-134">Request headers</span></span>

| <span data-ttu-id="09ba2-135">Имя</span><span class="sxs-lookup"><span data-stu-id="09ba2-135">Name</span></span>          | <span data-ttu-id="09ba2-136">Описание</span><span class="sxs-lookup"><span data-stu-id="09ba2-136">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="09ba2-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="09ba2-137">Authorization</span></span> | <span data-ttu-id="09ba2-138">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="09ba2-138">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="09ba2-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="09ba2-139">Request body</span></span>

<span data-ttu-id="09ba2-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="09ba2-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09ba2-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="09ba2-141">Response</span></span>

<span data-ttu-id="09ba2-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="09ba2-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09ba2-144">Пример</span><span class="sxs-lookup"><span data-stu-id="09ba2-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="09ba2-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="09ba2-145">Request</span></span>

<span data-ttu-id="09ba2-146">В следующем примере **удаляется единоеroleDefinition** для поставщика каталогов.</span><span class="sxs-lookup"><span data-stu-id="09ba2-146">The following example deletes a **unifiedRoleDefinition** for a directory provider.</span></span>

# <a name="http"></a>[<span data-ttu-id="09ba2-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="09ba2-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroledefinition"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="c"></a>[<span data-ttu-id="09ba2-148">C#</span><span class="sxs-lookup"><span data-stu-id="09ba2-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="09ba2-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09ba2-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="09ba2-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09ba2-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="09ba2-151">Java</span><span class="sxs-lookup"><span data-stu-id="09ba2-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="09ba2-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="09ba2-152">Response</span></span>

<span data-ttu-id="09ba2-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="09ba2-153">The following is an example of the response.</span></span>

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


