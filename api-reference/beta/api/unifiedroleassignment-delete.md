---
title: Удаление unifiedRoleAssignment
description: Удаление объекта unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 01ce2f1aa786c0f62147a370c00f6aed4d9d0bc6
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351040"
---
# <a name="delete-unifiedroleassignment"></a><span data-ttu-id="4c5a5-103">Удаление unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="4c5a5-103">Delete unifiedRoleAssignment</span></span>

<span data-ttu-id="4c5a5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c5a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c5a5-105">Удаление [объекта unifiedRoleAssignment.](../resources/unifiedRoleAssignment.md)</span><span class="sxs-lookup"><span data-stu-id="4c5a5-105">Delete a [unifiedRoleAssignment](../resources/unifiedRoleAssignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c5a5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c5a5-106">Permissions</span></span>

<span data-ttu-id="4c5a5-107">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4c5a5-107">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="4c5a5-108">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c5a5-108">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="4c5a5-109">Поставщик каталогов (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="4c5a5-109">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="4c5a5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c5a5-110">Permission type</span></span>      | <span data-ttu-id="4c5a5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c5a5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c5a5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c5a5-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="4c5a5-113">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="4c5a5-113">RoleManagement.ReadWrite.Directory</span></span>   |
|<span data-ttu-id="4c5a5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c5a5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c5a5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c5a5-115">Not supported.</span></span>    |
|<span data-ttu-id="4c5a5-116">Application</span><span class="sxs-lookup"><span data-stu-id="4c5a5-116">Application</span></span> | <span data-ttu-id="4c5a5-117">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="4c5a5-117">RoleManagement.ReadWrite.Directory</span></span> |

### <a name="for-entitlement-management-provider"></a><span data-ttu-id="4c5a5-118">Поставщик прав на управление правами</span><span class="sxs-lookup"><span data-stu-id="4c5a5-118">For Entitlement management provider</span></span>

|<span data-ttu-id="4c5a5-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c5a5-119">Permission type</span></span>      | <span data-ttu-id="4c5a5-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c5a5-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c5a5-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c5a5-121">Delegated (work or school account)</span></span> |  <span data-ttu-id="4c5a5-122">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c5a5-122">EntitlementManagement.ReadWrite.All</span></span>  |
|<span data-ttu-id="4c5a5-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c5a5-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c5a5-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c5a5-124">Not supported.</span></span>    |
|<span data-ttu-id="4c5a5-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c5a5-125">Application</span></span> | <span data-ttu-id="4c5a5-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c5a5-126">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c5a5-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c5a5-127">HTTP request</span></span>

<span data-ttu-id="4c5a5-128">Удаление назначения ролей у поставщика каталогов:</span><span class="sxs-lookup"><span data-stu-id="4c5a5-128">Remove a role assignment from a directory provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/directory/roleAssignments/{id}
```

<span data-ttu-id="4c5a5-129">Удаление назначения роли у поставщика управления правами:</span><span class="sxs-lookup"><span data-stu-id="4c5a5-129">Remove a role assignment from the entitlement management provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/entitlementManagement/roleAssignments/{id}
```


## <a name="request-headers"></a><span data-ttu-id="4c5a5-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c5a5-130">Request headers</span></span>

| <span data-ttu-id="4c5a5-131">Имя</span><span class="sxs-lookup"><span data-stu-id="4c5a5-131">Name</span></span>          | <span data-ttu-id="4c5a5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4c5a5-132">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4c5a5-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c5a5-133">Authorization</span></span> | <span data-ttu-id="4c5a5-134">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="4c5a5-134">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c5a5-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c5a5-135">Request body</span></span>

<span data-ttu-id="4c5a5-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c5a5-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c5a5-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c5a5-137">Response</span></span>

<span data-ttu-id="4c5a5-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4c5a5-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c5a5-140">Пример</span><span class="sxs-lookup"><span data-stu-id="4c5a5-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c5a5-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c5a5-141">Request</span></span>

<span data-ttu-id="4c5a5-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c5a5-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4c5a5-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c5a5-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="4c5a5-144">C#</span><span class="sxs-lookup"><span data-stu-id="4c5a5-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c5a5-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c5a5-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c5a5-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c5a5-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4c5a5-147">Java</span><span class="sxs-lookup"><span data-stu-id="4c5a5-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4c5a5-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c5a5-148">Response</span></span>

<span data-ttu-id="4c5a5-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4c5a5-149">The following is an example of the response.</span></span>

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
  "description": "Delete unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


