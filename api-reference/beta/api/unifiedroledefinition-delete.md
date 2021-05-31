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
# <a name="delete-unifiedroledefinition"></a><span data-ttu-id="c0fdc-103">Удаление unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c0fdc-103">Delete unifiedRoleDefinition</span></span>

<span data-ttu-id="c0fdc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0fdc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0fdc-105">Удаление [объекта unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) для поставщика RBAC.</span><span class="sxs-lookup"><span data-stu-id="c0fdc-105">Delete a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object for an RBAC provider.</span></span>

<span data-ttu-id="c0fdc-106">В настоящее время поддерживаются следующие поставщики RBAC:</span><span class="sxs-lookup"><span data-stu-id="c0fdc-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="c0fdc-107">управление устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="c0fdc-107">device management (Intune)</span></span>
- <span data-ttu-id="c0fdc-108">каталог (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="c0fdc-108">directory (Azure AD)</span></span> 

> [!NOTE]
> <span data-ttu-id="c0fdc-109">Поставщик облачных ПК RBAC в настоящее время поддерживает только [список и](rbacapplication-list-roledefinitions.md) [получать](unifiedroledefinition-get.md) операции.</span><span class="sxs-lookup"><span data-stu-id="c0fdc-109">The cloud PC RBAC provider currently supports only the [list](rbacapplication-list-roledefinitions.md) and [get](unifiedroledefinition-get.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0fdc-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0fdc-110">Permissions</span></span>

<span data-ttu-id="c0fdc-111">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c0fdc-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="c0fdc-112">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0fdc-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="c0fdc-113">Поддерживаемый поставщик</span><span class="sxs-lookup"><span data-stu-id="c0fdc-113">Supported provider</span></span>      | <span data-ttu-id="c0fdc-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0fdc-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="c0fdc-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0fdc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0fdc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0fdc-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="c0fdc-117">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="c0fdc-117">Device management</span></span> | <span data-ttu-id="c0fdc-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0fdc-118">DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="c0fdc-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0fdc-119">Not supported.</span></span> | <span data-ttu-id="c0fdc-120">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0fdc-120">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="c0fdc-121">Каталог</span><span class="sxs-lookup"><span data-stu-id="c0fdc-121">Directory</span></span> | <span data-ttu-id="c0fdc-122">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c0fdc-122">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> | <span data-ttu-id="c0fdc-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0fdc-123">Not supported.</span></span>| <span data-ttu-id="c0fdc-124">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0fdc-124">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0fdc-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0fdc-125">HTTP request</span></span>

<span data-ttu-id="c0fdc-126">Удаление определения роли для поставщика управления устройствами:</span><span class="sxs-lookup"><span data-stu-id="c0fdc-126">To delete a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /roleManagement/deviceManagement/roleDefinitions/{id}
```

<span data-ttu-id="c0fdc-127">Удаление определения роли для поставщика каталогов:</span><span class="sxs-lookup"><span data-stu-id="c0fdc-127">To delete a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /roleManagement/directory/roleDefinitions/{id}

```

## <a name="request-headers"></a><span data-ttu-id="c0fdc-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0fdc-128">Request headers</span></span>

| <span data-ttu-id="c0fdc-129">Имя</span><span class="sxs-lookup"><span data-stu-id="c0fdc-129">Name</span></span>          | <span data-ttu-id="c0fdc-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c0fdc-130">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c0fdc-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0fdc-131">Authorization</span></span> | <span data-ttu-id="c0fdc-132">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="c0fdc-132">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0fdc-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0fdc-133">Request body</span></span>

<span data-ttu-id="c0fdc-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0fdc-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0fdc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0fdc-135">Response</span></span>

<span data-ttu-id="c0fdc-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c0fdc-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0fdc-138">Пример</span><span class="sxs-lookup"><span data-stu-id="c0fdc-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0fdc-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0fdc-139">Request</span></span>

<span data-ttu-id="c0fdc-140">В следующем примере **удаляется единоеroleDefinition** для поставщика каталогов.</span><span class="sxs-lookup"><span data-stu-id="c0fdc-140">The following example deletes a **unifiedRoleDefinition** for a directory provider.</span></span>

# <a name="http"></a>[<span data-ttu-id="c0fdc-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0fdc-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroledefinition"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="c"></a>[<span data-ttu-id="c0fdc-142">C#</span><span class="sxs-lookup"><span data-stu-id="c0fdc-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0fdc-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0fdc-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0fdc-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0fdc-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0fdc-145">Java</span><span class="sxs-lookup"><span data-stu-id="c0fdc-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c0fdc-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0fdc-146">Response</span></span>

<span data-ttu-id="c0fdc-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c0fdc-147">The following is an example of the response.</span></span>

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


