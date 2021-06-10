---
title: Обновление unifiedRoleAssignmentMultiple
description: Обновление нового объекта unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: c13242b11ed9cfdf58c3047d40937edc483c1cd6
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869928"
---
# <a name="update-unifiedroleassignmentmultiple"></a><span data-ttu-id="0e989-103">Обновление unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="0e989-103">Update unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="0e989-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e989-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e989-105">Обновление [существующего объекта unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) поставщика RBAC.</span><span class="sxs-lookup"><span data-stu-id="0e989-105">Update an existing [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object of an RBAC provider.</span></span> 

<span data-ttu-id="0e989-106">В настоящее время поддерживаются следующие поставщики RBAC:</span><span class="sxs-lookup"><span data-stu-id="0e989-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="0e989-107">облачный КОМПЬЮТЕР</span><span class="sxs-lookup"><span data-stu-id="0e989-107">cloud PC</span></span> 
- <span data-ttu-id="0e989-108">управление устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="0e989-108">device management (Intune)</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

<span data-ttu-id="0e989-109">Напротив, [unifiedRoleAssignment](../resources/unifiedroleassignment.md) не поддерживает обновление.</span><span class="sxs-lookup"><span data-stu-id="0e989-109">In contrast, [unifiedRoleAssignment](../resources/unifiedroleassignment.md) does not support update.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e989-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0e989-110">Permissions</span></span>

<span data-ttu-id="0e989-111">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0e989-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="0e989-112">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e989-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="0e989-113">Поддерживаемый поставщик</span><span class="sxs-lookup"><span data-stu-id="0e989-113">Supported provider</span></span>      | <span data-ttu-id="0e989-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e989-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="0e989-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e989-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e989-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="0e989-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="0e989-117">Cloud PC</span><span class="sxs-lookup"><span data-stu-id="0e989-117">Cloud PC</span></span> | <span data-ttu-id="0e989-118">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e989-118">CloudPC.ReadWrite.All</span></span> | <span data-ttu-id="0e989-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e989-119">Not supported.</span></span> | <span data-ttu-id="0e989-120">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e989-120">CloudPC.ReadWrite.All</span></span> |
| <span data-ttu-id="0e989-121">Intune</span><span class="sxs-lookup"><span data-stu-id="0e989-121">Intune</span></span> | <span data-ttu-id="0e989-122">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e989-122">DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="0e989-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e989-123">Not supported.</span></span>| <span data-ttu-id="0e989-124">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e989-124">DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e989-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e989-125">HTTP request</span></span>

<span data-ttu-id="0e989-126">Обновление существующего unfiedRoleAssignmentMultiple для поставщика облачных ПК:</span><span class="sxs-lookup"><span data-stu-id="0e989-126">To update an existing unfiedRoleAssignmentMultiple for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/cloudPC/roleAssignments
```

<span data-ttu-id="0e989-127">Обновление существующего unfiedRoleAssignmentMultiple для поставщика Intune:</span><span class="sxs-lookup"><span data-stu-id="0e989-127">To update an existing unfiedRoleAssignmentMultiple for an Intune provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="0e989-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e989-128">Request headers</span></span>

| <span data-ttu-id="0e989-129">Имя</span><span class="sxs-lookup"><span data-stu-id="0e989-129">Name</span></span> | <span data-ttu-id="0e989-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0e989-130">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="0e989-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e989-131">Authorization</span></span> | <span data-ttu-id="0e989-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e989-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0e989-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0e989-134">Content-type</span></span> | <span data-ttu-id="0e989-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e989-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e989-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e989-137">Request body</span></span>

<span data-ttu-id="0e989-138">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="0e989-138">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0e989-139">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="0e989-139">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0e989-140">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0e989-140">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="0e989-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e989-141">Response</span></span>

<span data-ttu-id="0e989-142">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [unifiedAssignmentMultiple](../resources/unifiedroleassignmentMultiple.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0e989-142">If successful, this method returns a `200 OK` response code and an updated [unifiedAssignmentMultiple](../resources/unifiedroleassignmentMultiple.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e989-143">Пример</span><span class="sxs-lookup"><span data-stu-id="0e989-143">Example</span></span>

### <a name="example-1-update-an-existing-unfiedroleassignmentmultiple-in-an-intune-provider"></a><span data-ttu-id="0e989-144">Пример 1. Обновление существующего unfiedRoleAssignmentMultiple в поставщике Intune</span><span class="sxs-lookup"><span data-stu-id="0e989-144">Example 1: Update an existing unfiedRoleAssignmentMultiple in an Intune provider</span></span>
### <a name="request"></a><span data-ttu-id="0e989-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e989-145">Request</span></span>

<span data-ttu-id="0e989-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e989-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0e989-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e989-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0e989-148">C#</span><span class="sxs-lookup"><span data-stu-id="0e989-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e989-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e989-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e989-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e989-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e989-151">Java</span><span class="sxs-lookup"><span data-stu-id="0e989-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroleassignmentmultiple-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0e989-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e989-152">Response</span></span>

<span data-ttu-id="0e989-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0e989-153">The following is an example of the response.</span></span>
> <span data-ttu-id="0e989-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0e989-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 OK

```

## <a name="example-2-update-an-existing-unfiedroleassignmentmultiple-in-a-cloud-pc-provider"></a><span data-ttu-id="0e989-155">Пример 2. Обновление существующего unfiedRoleAssignmentMultiple в поставщике облачных ПК</span><span class="sxs-lookup"><span data-stu-id="0e989-155">Example 2: update an existing unfiedRoleAssignmentMultiple in a cloud PC provider</span></span>

### <a name="request"></a><span data-ttu-id="0e989-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e989-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0e989-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e989-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0e989-158">C#</span><span class="sxs-lookup"><span data-stu-id="0e989-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e989-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e989-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e989-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e989-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e989-161">Java</span><span class="sxs-lookup"><span data-stu-id="0e989-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="0e989-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e989-162">Response</span></span>

> <span data-ttu-id="0e989-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0e989-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


