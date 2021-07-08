---
title: Удаление unifiedRoleAssignmentMultiple
description: Удаление объекта unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 476f9a0dc37d919ea2977602298a4b438bbd1956
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334572"
---
# <a name="delete-unifiedroleassignmentmultiple"></a><span data-ttu-id="96775-103">Удаление unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="96775-103">Delete unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="96775-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96775-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96775-105">Удаление [объекта unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) поставщика RBAC.</span><span class="sxs-lookup"><span data-stu-id="96775-105">Delete a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object of an RBAC provider.</span></span> 

<span data-ttu-id="96775-106">Это применимо для приложения RBAC, которое поддерживает несколько принципов и областей.</span><span class="sxs-lookup"><span data-stu-id="96775-106">This is applicable for a RBAC application that supports multiple principals and scopes.</span></span> <span data-ttu-id="96775-107">В настоящее время поддерживаются следующие поставщики RBAC:</span><span class="sxs-lookup"><span data-stu-id="96775-107">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="96775-108">облачный КОМПЬЮТЕР</span><span class="sxs-lookup"><span data-stu-id="96775-108">cloud PC</span></span> 
- <span data-ttu-id="96775-109">управление устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="96775-109">device management (Intune)</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="96775-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="96775-110">Permissions</span></span>

<span data-ttu-id="96775-111">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="96775-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="96775-112">Дополнительные новости, в том числе осторожность [перед](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) выбором более привилегированных разрешений, см. [в см. в руб. Permissions.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="96775-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, see [Permissions](/graph/permissions-reference).</span></span> 

### <a name="for-cloud-pc-provider"></a><span data-ttu-id="96775-113">Поставщик облачных ПК</span><span class="sxs-lookup"><span data-stu-id="96775-113">For Cloud PC provider</span></span>

|<span data-ttu-id="96775-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96775-114">Permission type</span></span>      | <span data-ttu-id="96775-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="96775-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96775-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96775-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="96775-117">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96775-117">CloudPC.ReadWrite.All</span></span>   |
|<span data-ttu-id="96775-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96775-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96775-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96775-119">Not supported.</span></span>    |
|<span data-ttu-id="96775-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="96775-120">Application</span></span> | <span data-ttu-id="96775-121">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96775-121">CloudPC.ReadWrite.All</span></span>  |

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="96775-122">Для поставщика управления устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="96775-122">For Device management (Intune) provider</span></span>

|<span data-ttu-id="96775-123">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96775-123">Permission type</span></span>      | <span data-ttu-id="96775-124">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="96775-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96775-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96775-125">Delegated (work or school account)</span></span> |  <span data-ttu-id="96775-126">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96775-126">DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="96775-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96775-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96775-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96775-128">Not supported.</span></span>    |
|<span data-ttu-id="96775-129">Приложение</span><span class="sxs-lookup"><span data-stu-id="96775-129">Application</span></span> | <span data-ttu-id="96775-130">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96775-130">DeviceManagementRBAC.ReadWrite.All</span></span> |



## <a name="http-request"></a><span data-ttu-id="96775-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96775-131">HTTP request</span></span>

<span data-ttu-id="96775-132">Удаление единой системыRoleAssignmentMultiple для поставщика облачных ПК:</span><span class="sxs-lookup"><span data-stu-id="96775-132">To delete a unifiedRoleAssignmentMultiple for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/cloudPC/roleAssignments/{id}
```

<span data-ttu-id="96775-133">Удаление единой системыRoleAssignmentMultiple для поставщика Intune:</span><span class="sxs-lookup"><span data-stu-id="96775-133">To delete a unifiedRoleAssignmentMultiple for an Intune provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="96775-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96775-134">Request headers</span></span>

| <span data-ttu-id="96775-135">Имя</span><span class="sxs-lookup"><span data-stu-id="96775-135">Name</span></span> | <span data-ttu-id="96775-136">Описание</span><span class="sxs-lookup"><span data-stu-id="96775-136">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="96775-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="96775-137">Authorization</span></span> | <span data-ttu-id="96775-138">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="96775-138">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="96775-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96775-139">Request body</span></span>

<span data-ttu-id="96775-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="96775-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96775-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="96775-141">Response</span></span>

<span data-ttu-id="96775-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="96775-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96775-144">Пример</span><span class="sxs-lookup"><span data-stu-id="96775-144">Example</span></span>

### <a name="example-1-delete-a-unifiedroleassignmentmultiple-in-an-intune-provider"></a><span data-ttu-id="96775-145">Пример 1. Удаление единой системыRoleAssignmentMultiple в поставщике Intune</span><span class="sxs-lookup"><span data-stu-id="96775-145">Example 1: Delete a unifiedRoleAssignmentMultiple in an Intune provider</span></span>

### <a name="request"></a><span data-ttu-id="96775-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="96775-146">Request</span></span>

<span data-ttu-id="96775-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96775-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="96775-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="96775-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignmentMultiple"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="96775-149">C#</span><span class="sxs-lookup"><span data-stu-id="96775-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignmentmultiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96775-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96775-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignmentmultiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96775-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96775-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignmentmultiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96775-152">Java</span><span class="sxs-lookup"><span data-stu-id="96775-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignmentmultiple-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="96775-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="96775-153">Response</span></span>

<span data-ttu-id="96775-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="96775-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-delete-a-unifiedroleassignmentmultiple-in-a-cloud-pc-provider"></a><span data-ttu-id="96775-155">Пример 2. Удаление единой системыRoleAssignmentMultiple в поставщике облачных ПК</span><span class="sxs-lookup"><span data-stu-id="96775-155">Example 2: Delete a unifiedRoleAssignmentMultiple in a cloud PC provider</span></span>

### <a name="request"></a><span data-ttu-id="96775-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="96775-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="96775-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="96775-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignmentMultiple_cloudpc"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments/id
```
# <a name="c"></a>[<span data-ttu-id="96775-158">C#</span><span class="sxs-lookup"><span data-stu-id="96775-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignmentmultiple-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96775-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96775-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignmentmultiple-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96775-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96775-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignmentmultiple-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96775-161">Java</span><span class="sxs-lookup"><span data-stu-id="96775-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignmentmultiple-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="96775-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="96775-162">Response</span></span>

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
  "description": "Delete unifiedRoleAssignmentMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


