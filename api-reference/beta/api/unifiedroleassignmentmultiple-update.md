---
title: Обновление unifiedRoleAssignmentMultiple
description: Обновление нового объекта unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 3423c216e9b0c5b6928d0473c1e7db021e1344c9
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334495"
---
# <a name="update-unifiedroleassignmentmultiple"></a><span data-ttu-id="ad666-103">Обновление unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="ad666-103">Update unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="ad666-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad666-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad666-105">Обновление [существующего объекта unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) поставщика RBAC.</span><span class="sxs-lookup"><span data-stu-id="ad666-105">Update an existing [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object of an RBAC provider.</span></span> 

<span data-ttu-id="ad666-106">В настоящее время поддерживаются следующие поставщики RBAC:</span><span class="sxs-lookup"><span data-stu-id="ad666-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="ad666-107">облачный КОМПЬЮТЕР</span><span class="sxs-lookup"><span data-stu-id="ad666-107">cloud PC</span></span> 
- <span data-ttu-id="ad666-108">управление устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="ad666-108">device management (Intune)</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

<span data-ttu-id="ad666-109">Напротив, [unifiedRoleAssignment](../resources/unifiedroleassignment.md) не поддерживает обновление.</span><span class="sxs-lookup"><span data-stu-id="ad666-109">In contrast, [unifiedRoleAssignment](../resources/unifiedroleassignment.md) does not support update.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad666-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad666-110">Permissions</span></span>

<span data-ttu-id="ad666-111">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ad666-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="ad666-112">Дополнительные новости, в том числе осторожность [перед](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) выбором более привилегированных разрешений, см. [в см. в руб. Permissions.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="ad666-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, see [Permissions](/graph/permissions-reference).</span></span> 

### <a name="for-cloud-pc-provider"></a><span data-ttu-id="ad666-113">Поставщик облачных ПК</span><span class="sxs-lookup"><span data-stu-id="ad666-113">For Cloud PC provider</span></span>

|<span data-ttu-id="ad666-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad666-114">Permission type</span></span>      | <span data-ttu-id="ad666-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad666-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad666-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad666-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="ad666-117">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad666-117">CloudPC.ReadWrite.All</span></span>   |
|<span data-ttu-id="ad666-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad666-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad666-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad666-119">Not supported.</span></span>    |
|<span data-ttu-id="ad666-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="ad666-120">Application</span></span> | <span data-ttu-id="ad666-121">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad666-121">CloudPC.ReadWrite.All</span></span>  |

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="ad666-122">Для поставщика управления устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="ad666-122">For Device management (Intune) provider</span></span>

|<span data-ttu-id="ad666-123">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad666-123">Permission type</span></span>      | <span data-ttu-id="ad666-124">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad666-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad666-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad666-125">Delegated (work or school account)</span></span> |  <span data-ttu-id="ad666-126">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad666-126">DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="ad666-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad666-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad666-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad666-128">Not supported.</span></span>    |
|<span data-ttu-id="ad666-129">Приложение</span><span class="sxs-lookup"><span data-stu-id="ad666-129">Application</span></span> | <span data-ttu-id="ad666-130">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad666-130">DeviceManagementRBAC.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="ad666-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad666-131">HTTP request</span></span>

<span data-ttu-id="ad666-132">Обновление существующего unfiedRoleAssignmentMultiple для поставщика облачных ПК:</span><span class="sxs-lookup"><span data-stu-id="ad666-132">To update an existing unfiedRoleAssignmentMultiple for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/cloudPC/roleAssignments
```

<span data-ttu-id="ad666-133">Обновление существующего unfiedRoleAssignmentMultiple для поставщика Intune:</span><span class="sxs-lookup"><span data-stu-id="ad666-133">To update an existing unfiedRoleAssignmentMultiple for an Intune provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="ad666-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad666-134">Request headers</span></span>

| <span data-ttu-id="ad666-135">Имя</span><span class="sxs-lookup"><span data-stu-id="ad666-135">Name</span></span> | <span data-ttu-id="ad666-136">Описание</span><span class="sxs-lookup"><span data-stu-id="ad666-136">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="ad666-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad666-137">Authorization</span></span> | <span data-ttu-id="ad666-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad666-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ad666-140">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ad666-140">Content-type</span></span> | <span data-ttu-id="ad666-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad666-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad666-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad666-143">Request body</span></span>

<span data-ttu-id="ad666-144">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="ad666-144">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ad666-145">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="ad666-145">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ad666-146">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ad666-146">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="ad666-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad666-147">Response</span></span>

<span data-ttu-id="ad666-148">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [unifiedAssignmentMultiple](../resources/unifiedroleassignmentMultiple.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ad666-148">If successful, this method returns a `200 OK` response code and an updated [unifiedAssignmentMultiple](../resources/unifiedroleassignmentMultiple.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad666-149">Пример</span><span class="sxs-lookup"><span data-stu-id="ad666-149">Example</span></span>

### <a name="example-1-update-an-existing-unfiedroleassignmentmultiple-in-an-intune-provider"></a><span data-ttu-id="ad666-150">Пример 1. Обновление существующего unfiedRoleAssignmentMultiple в поставщике Intune</span><span class="sxs-lookup"><span data-stu-id="ad666-150">Example 1: Update an existing unfiedRoleAssignmentMultiple in an Intune provider</span></span>
### <a name="request"></a><span data-ttu-id="ad666-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad666-151">Request</span></span>

<span data-ttu-id="ad666-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad666-152">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ad666-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad666-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroleassignmentmultiple_from_rbacapplication"
}-->

```http
PATCH https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
Content-type: application/json

{ 
    "principalIds": ["0aeec2c1-fee7-4e02-b534-6f920d25b300", "2d5386a7-732f-44db-9cf8-f82dd2a1c0e0"]
}
```
# <a name="c"></a>[<span data-ttu-id="ad666-154">C#</span><span class="sxs-lookup"><span data-stu-id="ad666-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad666-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad666-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad666-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad666-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad666-157">Java</span><span class="sxs-lookup"><span data-stu-id="ad666-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroleassignmentmultiple-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ad666-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad666-158">Response</span></span>

<span data-ttu-id="ad666-159">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ad666-159">The following is an example of the response.</span></span>
> <span data-ttu-id="ad666-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ad666-160">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 OK

```

## <a name="example-2-update-an-existing-unfiedroleassignmentmultiple-in-a-cloud-pc-provider"></a><span data-ttu-id="ad666-161">Пример 2. Обновление существующего unfiedRoleAssignmentMultiple в поставщике облачных ПК</span><span class="sxs-lookup"><span data-stu-id="ad666-161">Example 2: update an existing unfiedRoleAssignmentMultiple in a cloud PC provider</span></span>

### <a name="request"></a><span data-ttu-id="ad666-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad666-162">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ad666-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad666-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroleassignmentmultiple_from_rbacapplication_cloudpc"
}-->

```http
PATCH https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments/dbe9d288-fd87-41f4-b33d-b498ed207096
Content-type: application/json

{
    "displayName": "NewName",
    "description": "A new roleAssignment"
}
```
# <a name="c"></a>[<span data-ttu-id="ad666-164">C#</span><span class="sxs-lookup"><span data-stu-id="ad666-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad666-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad666-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad666-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad666-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad666-167">Java</span><span class="sxs-lookup"><span data-stu-id="ad666-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ad666-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad666-168">Response</span></span>

> <span data-ttu-id="ad666-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad666-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleAssignments/$entity",
    "id": "dbe9d288-fd87-41f4-b33d-b498ed207096",
    "description": "A new roleAssignment",
    "displayName": "NewName",
    "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
    "principalIds": [
        "0aeec2c1-fee7-4e02-b534-6f920d25b300",
        "2d5386a7-732f-44db-9cf8-f82dd2a1c0e0"
    ],
    "directoryScopeIds": [
        "/"
    ],
    "appScopeIds": []
}
```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update unifiedRoleAssignmentMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


