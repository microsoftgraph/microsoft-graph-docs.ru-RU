---
title: Удаление unifiedRoleAssignmentMultiple
description: Удаление объекта unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 14ae5e8c899378e76fb201856bea2929a0ba3168
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870061"
---
# <a name="delete-unifiedroleassignmentmultiple"></a><span data-ttu-id="0fcdc-103">Удаление unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="0fcdc-103">Delete unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="0fcdc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fcdc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fcdc-105">Удаление [объекта unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) поставщика RBAC.</span><span class="sxs-lookup"><span data-stu-id="0fcdc-105">Delete a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object of an RBAC provider.</span></span> 

<span data-ttu-id="0fcdc-106">Это применимо для приложения RBAC, которое поддерживает несколько принципов и областей.</span><span class="sxs-lookup"><span data-stu-id="0fcdc-106">This is applicable for a RBAC application that supports multiple principals and scopes.</span></span> <span data-ttu-id="0fcdc-107">В настоящее время поддерживаются следующие поставщики RBAC:</span><span class="sxs-lookup"><span data-stu-id="0fcdc-107">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="0fcdc-108">облачный КОМПЬЮТЕР</span><span class="sxs-lookup"><span data-stu-id="0fcdc-108">cloud PC</span></span> 
- <span data-ttu-id="0fcdc-109">управление устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="0fcdc-109">device management (Intune)</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="0fcdc-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0fcdc-110">Permissions</span></span>

<span data-ttu-id="0fcdc-111">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0fcdc-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="0fcdc-112">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fcdc-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="0fcdc-113">Поддерживаемый поставщик</span><span class="sxs-lookup"><span data-stu-id="0fcdc-113">Supported provider</span></span>      | <span data-ttu-id="0fcdc-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0fcdc-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="0fcdc-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0fcdc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fcdc-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="0fcdc-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="0fcdc-117">Cloud PC</span><span class="sxs-lookup"><span data-stu-id="0fcdc-117">Cloud PC</span></span> | <span data-ttu-id="0fcdc-118">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fcdc-118">CloudPC.ReadWrite.All</span></span> | <span data-ttu-id="0fcdc-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fcdc-119">Not supported.</span></span> | <span data-ttu-id="0fcdc-120">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fcdc-120">CloudPC.ReadWrite.All</span></span> |
| <span data-ttu-id="0fcdc-121">Intune</span><span class="sxs-lookup"><span data-stu-id="0fcdc-121">Intune</span></span> | <span data-ttu-id="0fcdc-122">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fcdc-122">DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="0fcdc-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fcdc-123">Not supported.</span></span>| <span data-ttu-id="0fcdc-124">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fcdc-124">DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fcdc-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0fcdc-125">HTTP request</span></span>

<span data-ttu-id="0fcdc-126">Удаление единой системыRoleAssignmentMultiple для поставщика облачных ПК:</span><span class="sxs-lookup"><span data-stu-id="0fcdc-126">To delete a unifiedRoleAssignmentMultiple for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/cloudPC/roleAssignments/{id}
```

<span data-ttu-id="0fcdc-127">Удаление единой системыRoleAssignmentMultiple для поставщика Intune:</span><span class="sxs-lookup"><span data-stu-id="0fcdc-127">To delete a unifiedRoleAssignmentMultiple for an Intune provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0fcdc-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0fcdc-128">Request headers</span></span>

| <span data-ttu-id="0fcdc-129">Имя</span><span class="sxs-lookup"><span data-stu-id="0fcdc-129">Name</span></span> | <span data-ttu-id="0fcdc-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0fcdc-130">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="0fcdc-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0fcdc-131">Authorization</span></span> | <span data-ttu-id="0fcdc-132">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="0fcdc-132">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0fcdc-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0fcdc-133">Request body</span></span>

<span data-ttu-id="0fcdc-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0fcdc-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fcdc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fcdc-135">Response</span></span>

<span data-ttu-id="0fcdc-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0fcdc-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fcdc-138">Пример</span><span class="sxs-lookup"><span data-stu-id="0fcdc-138">Example</span></span>

### <a name="example-1-delete-a-unifiedroleassignmentmultiple-in-an-intune-provider"></a><span data-ttu-id="0fcdc-139">Пример 1. Удаление единой системыRoleAssignmentMultiple в поставщике Intune</span><span class="sxs-lookup"><span data-stu-id="0fcdc-139">Example 1: Delete a unifiedRoleAssignmentMultiple in an Intune provider</span></span>

### <a name="request"></a><span data-ttu-id="0fcdc-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fcdc-140">Request</span></span>

<span data-ttu-id="0fcdc-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0fcdc-141">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0fcdc-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fcdc-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignmentMultiple"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="0fcdc-143">C#</span><span class="sxs-lookup"><span data-stu-id="0fcdc-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignmentmultiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0fcdc-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fcdc-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignmentmultiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0fcdc-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0fcdc-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignmentmultiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0fcdc-146">Java</span><span class="sxs-lookup"><span data-stu-id="0fcdc-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignmentmultiple-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0fcdc-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fcdc-147">Response</span></span>

<span data-ttu-id="0fcdc-148">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0fcdc-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-delete-a-unifiedroleassignmentmultiple-in-a-cloud-pc-provider"></a><span data-ttu-id="0fcdc-149">Пример 2. Удаление единой системыRoleAssignmentMultiple в поставщике облачных ПК</span><span class="sxs-lookup"><span data-stu-id="0fcdc-149">Example 2: Delete a unifiedRoleAssignmentMultiple in a cloud PC provider</span></span>

### <a name="request"></a><span data-ttu-id="0fcdc-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fcdc-150">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0fcdc-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fcdc-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignmentMultiple_cloudpc"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments/id
```
# <a name="c"></a>[<span data-ttu-id="0fcdc-152">C#</span><span class="sxs-lookup"><span data-stu-id="0fcdc-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignmentmultiple-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0fcdc-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fcdc-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignmentmultiple-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0fcdc-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0fcdc-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignmentmultiple-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0fcdc-155">Java</span><span class="sxs-lookup"><span data-stu-id="0fcdc-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignmentmultiple-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="0fcdc-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fcdc-156">Response</span></span>

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


