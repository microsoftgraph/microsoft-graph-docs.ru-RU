---
title: Обновление unifiedRoleAssignmentMultiple
description: Обновление нового объекта unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 656addb026493a442e52f0db7a841f3b523f6566
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786462"
---
# <a name="update-unifiedroleassignmentmultiple"></a><span data-ttu-id="ad0bb-103">Обновление unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="ad0bb-103">Update unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="ad0bb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad0bb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad0bb-105">Обновление [существующего объекта unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) поставщика RBAC.</span><span class="sxs-lookup"><span data-stu-id="ad0bb-105">Update an existing [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object of an RBAC provider.</span></span> 

<span data-ttu-id="ad0bb-106">В настоящее время поддерживаются следующие поставщики RBAC:</span><span class="sxs-lookup"><span data-stu-id="ad0bb-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="ad0bb-107">облачный КОМПЬЮТЕР</span><span class="sxs-lookup"><span data-stu-id="ad0bb-107">cloud PC</span></span> 
- <span data-ttu-id="ad0bb-108">управление устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="ad0bb-108">device management (Intune)</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

<span data-ttu-id="ad0bb-109">Напротив, [unifiedRoleAssignment](../resources/unifiedroleassignment.md) не поддерживает обновление.</span><span class="sxs-lookup"><span data-stu-id="ad0bb-109">In contrast, [unifiedRoleAssignment](../resources/unifiedroleassignment.md) does not support update.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad0bb-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad0bb-110">Permissions</span></span>

<span data-ttu-id="ad0bb-111">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ad0bb-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="ad0bb-112">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad0bb-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="ad0bb-113">Поддерживаемый поставщик</span><span class="sxs-lookup"><span data-stu-id="ad0bb-113">Supported provider</span></span>      | <span data-ttu-id="ad0bb-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad0bb-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="ad0bb-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad0bb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad0bb-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ad0bb-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="ad0bb-117">Cloud PC</span><span class="sxs-lookup"><span data-stu-id="ad0bb-117">Cloud PC</span></span> | <span data-ttu-id="ad0bb-118">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad0bb-118">CloudPC.ReadWrite.All</span></span> | <span data-ttu-id="ad0bb-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad0bb-119">Not supported.</span></span> | <span data-ttu-id="ad0bb-120">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad0bb-120">CloudPC.ReadWrite.All</span></span> |
| <span data-ttu-id="ad0bb-121">Intune</span><span class="sxs-lookup"><span data-stu-id="ad0bb-121">Intune</span></span> | <span data-ttu-id="ad0bb-122">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad0bb-122">DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="ad0bb-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad0bb-123">Not supported.</span></span>| <span data-ttu-id="ad0bb-124">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad0bb-124">DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad0bb-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad0bb-125">HTTP request</span></span>

<span data-ttu-id="ad0bb-126">Обновление существующего unfiedRoleAssignmentMultiple для поставщика облачных ПК:</span><span class="sxs-lookup"><span data-stu-id="ad0bb-126">To update an existing unfiedRoleAssignmentMultiple for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/cloudPC/roleAssignments
```

<span data-ttu-id="ad0bb-127">Обновление существующего unfiedRoleAssignmentMultiple для поставщика Intune:</span><span class="sxs-lookup"><span data-stu-id="ad0bb-127">To update an existing unfiedRoleAssignmentMultiple for an Intune provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="ad0bb-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad0bb-128">Request headers</span></span>

| <span data-ttu-id="ad0bb-129">Имя</span><span class="sxs-lookup"><span data-stu-id="ad0bb-129">Name</span></span> | <span data-ttu-id="ad0bb-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ad0bb-130">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="ad0bb-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad0bb-131">Authorization</span></span> | <span data-ttu-id="ad0bb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad0bb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ad0bb-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ad0bb-134">Content-type</span></span> | <span data-ttu-id="ad0bb-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad0bb-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad0bb-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad0bb-137">Request body</span></span>

<span data-ttu-id="ad0bb-138">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="ad0bb-138">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ad0bb-139">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="ad0bb-139">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ad0bb-140">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ad0bb-140">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="ad0bb-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad0bb-141">Response</span></span>

<span data-ttu-id="ad0bb-142">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [unifiedAssignmentMultiple](../resources/unifiedroleassignmentMultiple.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ad0bb-142">If successful, this method returns a `200 OK` response code and an updated [unifiedAssignmentMultiple](../resources/unifiedroleassignmentMultiple.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad0bb-143">Пример</span><span class="sxs-lookup"><span data-stu-id="ad0bb-143">Example</span></span>

### <a name="example-1-update-an-existing-unfiedroleassignmentmultiple-in-an-intune-provider"></a><span data-ttu-id="ad0bb-144">Пример 1. Обновление существующего unfiedRoleAssignmentMultiple в поставщике Intune</span><span class="sxs-lookup"><span data-stu-id="ad0bb-144">Example 1: Update an existing unfiedRoleAssignmentMultiple in an Intune provider</span></span>
### <a name="request"></a><span data-ttu-id="ad0bb-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad0bb-145">Request</span></span>

<span data-ttu-id="ad0bb-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad0bb-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ad0bb-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad0bb-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ad0bb-148">C#</span><span class="sxs-lookup"><span data-stu-id="ad0bb-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad0bb-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad0bb-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad0bb-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad0bb-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad0bb-151">Java</span><span class="sxs-lookup"><span data-stu-id="ad0bb-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroleassignmentmultiple-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ad0bb-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad0bb-152">Response</span></span>

<span data-ttu-id="ad0bb-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ad0bb-153">The following is an example of the response.</span></span>
> <span data-ttu-id="ad0bb-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ad0bb-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 OK

```

## <a name="example-2-update-an-existing-unfiedroleassignmentmultiple-in-a-cloud-pc-provider"></a><span data-ttu-id="ad0bb-155">Пример 2. Обновление существующего unfiedRoleAssignmentMultiple в поставщике облачных ПК</span><span class="sxs-lookup"><span data-stu-id="ad0bb-155">Example 2: update an existing unfiedRoleAssignmentMultiple in a cloud PC provider</span></span>

### <a name="request"></a><span data-ttu-id="ad0bb-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad0bb-156">Request</span></span>

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


### <a name="response"></a><span data-ttu-id="ad0bb-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad0bb-157">Response</span></span>

> <span data-ttu-id="ad0bb-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad0bb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


