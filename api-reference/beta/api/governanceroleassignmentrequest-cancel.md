---
title: Отмена governanceRoleAssignmentRequest
description: Отмена governanceRoleAssignmentRequest.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 624302e735eebf3fbbdf477636176a5e7f414bfe
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786994"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="cae05-103">Отмена governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="cae05-103">Cancel governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="cae05-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cae05-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cae05-105">Отмена [управленияRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="cae05-105">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cae05-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cae05-106">Permissions</span></span>
<span data-ttu-id="cae05-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="cae05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="cae05-109">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="cae05-109">Azure resources</span></span>

| <span data-ttu-id="cae05-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cae05-110">Permission type</span></span> | <span data-ttu-id="cae05-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cae05-111">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="cae05-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cae05-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cae05-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="cae05-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="cae05-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cae05-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cae05-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cae05-115">Not supported.</span></span> |
| <span data-ttu-id="cae05-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cae05-116">Application</span></span> | <span data-ttu-id="cae05-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cae05-117">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="cae05-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="cae05-118">Azure AD</span></span>

| <span data-ttu-id="cae05-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cae05-119">Permission type</span></span> | <span data-ttu-id="cae05-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cae05-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="cae05-121">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cae05-121">Delegated (work or school account)</span></span> | <span data-ttu-id="cae05-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="cae05-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="cae05-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cae05-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cae05-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cae05-124">Not supported.</span></span> |
| <span data-ttu-id="cae05-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cae05-125">Application</span></span> | <span data-ttu-id="cae05-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cae05-126">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="cae05-127">Группы</span><span class="sxs-lookup"><span data-stu-id="cae05-127">Groups</span></span>

|<span data-ttu-id="cae05-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cae05-128">Permission type</span></span> | <span data-ttu-id="cae05-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cae05-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="cae05-130">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cae05-130">Delegated (work or school account)</span></span> | <span data-ttu-id="cae05-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="cae05-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="cae05-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cae05-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cae05-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cae05-133">Not supported.</span></span> |
| <span data-ttu-id="cae05-134">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cae05-134">Application</span></span> | <span data-ttu-id="cae05-135">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cae05-135">Not supported.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="cae05-136">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cae05-136">Optional query parameters</span></span>
<span data-ttu-id="cae05-137">Этот метод **не поддерживает** [параметры запроса OData.](/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="cae05-137">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="cae05-138">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cae05-138">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="cae05-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cae05-139">Request headers</span></span>
| <span data-ttu-id="cae05-140">Имя</span><span class="sxs-lookup"><span data-stu-id="cae05-140">Name</span></span>       | <span data-ttu-id="cae05-141">Описание</span><span class="sxs-lookup"><span data-stu-id="cae05-141">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cae05-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cae05-142">Authorization</span></span>  | <span data-ttu-id="cae05-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cae05-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="cae05-145">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cae05-145">Content-type</span></span>  | <span data-ttu-id="cae05-146">application/json</span><span class="sxs-lookup"><span data-stu-id="cae05-146">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cae05-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cae05-147">Request body</span></span>
<span data-ttu-id="cae05-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cae05-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cae05-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="cae05-149">Response</span></span>
<span data-ttu-id="cae05-p103">В случае успешного выполнения этот метод возвращает код отклика `204 NoContent`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="cae05-p103">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="cae05-152">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="cae05-152">Error codes</span></span>
<span data-ttu-id="cae05-153">Этот API следует стандарту http-кодов.</span><span class="sxs-lookup"><span data-stu-id="cae05-153">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="cae05-154">Кроме того, ниже показаны пользовательские коды ошибок.</span><span class="sxs-lookup"><span data-stu-id="cae05-154">Besides, the custom error codes are shown below.</span></span>

| <span data-ttu-id="cae05-155">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="cae05-155">Error code</span></span> | <span data-ttu-id="cae05-156">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="cae05-156">Error message</span></span> | <span data-ttu-id="cae05-157">Сведения</span><span class="sxs-lookup"><span data-stu-id="cae05-157">Details</span></span> |
|:---------- |:------------- |:------- |
| <span data-ttu-id="cae05-158">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="cae05-158">400 BadRequest</span></span> | <span data-ttu-id="cae05-159">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="cae05-159">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="cae05-160">В системе не существует системы governanceRoleAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="cae05-160">The governanceRoleAssignmentRequest does not exist in system.</span></span> |
| <span data-ttu-id="cae05-161">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="cae05-161">400 BadRequest</span></span> | <span data-ttu-id="cae05-162">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="cae05-162">RequestCannotBeCancelled</span></span> | <span data-ttu-id="cae05-163">Только запросы в состоянии `Granted` , и могут быть `PendingApproval` `PendingApprovalProvisioning` `PendingAdminDecision` отменены.</span><span class="sxs-lookup"><span data-stu-id="cae05-163">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span> |

## <a name="example"></a><span data-ttu-id="cae05-164">Пример</span><span class="sxs-lookup"><span data-stu-id="cae05-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="cae05-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="cae05-165">Request</span></span>
<span data-ttu-id="cae05-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cae05-166">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cae05-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="cae05-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```
# <a name="c"></a>[<span data-ttu-id="cae05-168">C#</span><span class="sxs-lookup"><span data-stu-id="cae05-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cancel-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cae05-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cae05-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cancel-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cae05-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cae05-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cancel-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cae05-171">Java</span><span class="sxs-lookup"><span data-stu-id="cae05-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cancel-governanceroleassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cae05-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="cae05-172">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Cancel governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


