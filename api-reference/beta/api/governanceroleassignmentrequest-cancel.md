---
title: Отмена governanceRoleAssignmentRequest
description: Отмена governanceRoleAssignmentRequest.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 1fad0311a688a2093e216a8b8d53405260d1fa19
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435933"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="4862d-103">Отмена governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="4862d-103">Cancel governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="4862d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4862d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4862d-105">Отмена [управленияRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="4862d-105">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4862d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4862d-106">Permissions</span></span>
<span data-ttu-id="4862d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="4862d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="4862d-109">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="4862d-109">Azure resources</span></span>

| <span data-ttu-id="4862d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4862d-110">Permission type</span></span> | <span data-ttu-id="4862d-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4862d-111">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="4862d-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4862d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4862d-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="4862d-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="4862d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4862d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4862d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4862d-115">Not supported.</span></span> |
| <span data-ttu-id="4862d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4862d-116">Application</span></span> | <span data-ttu-id="4862d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4862d-117">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="4862d-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="4862d-118">Azure AD</span></span>

| <span data-ttu-id="4862d-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4862d-119">Permission type</span></span> | <span data-ttu-id="4862d-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4862d-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="4862d-121">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4862d-121">Delegated (work or school account)</span></span> | <span data-ttu-id="4862d-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="4862d-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="4862d-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4862d-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4862d-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4862d-124">Not supported.</span></span> |
| <span data-ttu-id="4862d-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4862d-125">Application</span></span> | <span data-ttu-id="4862d-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4862d-126">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="4862d-127">Группы</span><span class="sxs-lookup"><span data-stu-id="4862d-127">Groups</span></span>

|<span data-ttu-id="4862d-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4862d-128">Permission type</span></span> | <span data-ttu-id="4862d-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4862d-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="4862d-130">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4862d-130">Delegated (work or school account)</span></span> | <span data-ttu-id="4862d-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="4862d-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="4862d-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4862d-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4862d-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4862d-133">Not supported.</span></span> |
| <span data-ttu-id="4862d-134">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4862d-134">Application</span></span> | <span data-ttu-id="4862d-135">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4862d-135">Not supported.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="4862d-136">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4862d-136">Optional query parameters</span></span>
<span data-ttu-id="4862d-137">Этот метод **не поддерживает** [параметры запроса OData.](/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="4862d-137">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="4862d-138">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4862d-138">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="4862d-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4862d-139">Request headers</span></span>
| <span data-ttu-id="4862d-140">Имя</span><span class="sxs-lookup"><span data-stu-id="4862d-140">Name</span></span>       | <span data-ttu-id="4862d-141">Описание</span><span class="sxs-lookup"><span data-stu-id="4862d-141">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4862d-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4862d-142">Authorization</span></span>  | <span data-ttu-id="4862d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4862d-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="4862d-145">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4862d-145">Content-type</span></span>  | <span data-ttu-id="4862d-146">application/json</span><span class="sxs-lookup"><span data-stu-id="4862d-146">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4862d-147">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4862d-147">Request body</span></span>
<span data-ttu-id="4862d-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4862d-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4862d-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="4862d-149">Response</span></span>
<span data-ttu-id="4862d-p103">В случае успешного выполнения этот метод возвращает код отклика `204 NoContent`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4862d-p103">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="4862d-152">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="4862d-152">Error codes</span></span>
<span data-ttu-id="4862d-153">Этот API следует стандарту http-кодов.</span><span class="sxs-lookup"><span data-stu-id="4862d-153">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="4862d-154">Кроме того, ниже показаны пользовательские коды ошибок.</span><span class="sxs-lookup"><span data-stu-id="4862d-154">Besides, the custom error codes are shown below.</span></span>

| <span data-ttu-id="4862d-155">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="4862d-155">Error code</span></span> | <span data-ttu-id="4862d-156">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="4862d-156">Error message</span></span> | <span data-ttu-id="4862d-157">Сведения</span><span class="sxs-lookup"><span data-stu-id="4862d-157">Details</span></span> |
|:---------- |:------------- |:------- |
| <span data-ttu-id="4862d-158">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4862d-158">400 BadRequest</span></span> | <span data-ttu-id="4862d-159">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="4862d-159">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="4862d-160">В системе не существует системы governanceRoleAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="4862d-160">The governanceRoleAssignmentRequest does not exist in system.</span></span> |
| <span data-ttu-id="4862d-161">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4862d-161">400 BadRequest</span></span> | <span data-ttu-id="4862d-162">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="4862d-162">RequestCannotBeCancelled</span></span> | <span data-ttu-id="4862d-163">Только запросы в состоянии `Granted` , и могут быть `PendingApproval` `PendingApprovalProvisioning` `PendingAdminDecision` отменены.</span><span class="sxs-lookup"><span data-stu-id="4862d-163">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span> |

## <a name="example"></a><span data-ttu-id="4862d-164">Пример</span><span class="sxs-lookup"><span data-stu-id="4862d-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="4862d-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="4862d-165">Request</span></span>
<span data-ttu-id="4862d-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4862d-166">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4862d-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="4862d-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```
# <a name="c"></a>[<span data-ttu-id="4862d-168">C#</span><span class="sxs-lookup"><span data-stu-id="4862d-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cancel-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4862d-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4862d-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cancel-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4862d-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4862d-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cancel-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4862d-171">Java</span><span class="sxs-lookup"><span data-stu-id="4862d-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cancel-governanceroleassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4862d-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="4862d-172">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.None"
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


