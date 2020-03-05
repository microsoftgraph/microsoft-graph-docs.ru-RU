---
title: Отмена governanceRoleAssignmentRequest
description: Отмена объекта governanceRoleAssignmentRequest.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: e2f245766c826b8776504f0835a79a33b370aaba
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42421125"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="2cf72-103">Отмена governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="2cf72-103">Cancel governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="2cf72-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2cf72-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cf72-105">Отмена объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="2cf72-105">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2cf72-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2cf72-106">Permissions</span></span>
<span data-ttu-id="2cf72-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cf72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cf72-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2cf72-109">Permission type</span></span>      | <span data-ttu-id="2cf72-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2cf72-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2cf72-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2cf72-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2cf72-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="2cf72-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="2cf72-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2cf72-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2cf72-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cf72-114">Not supported.</span></span>    |
|<span data-ttu-id="2cf72-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2cf72-115">Application</span></span> | <span data-ttu-id="2cf72-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cf72-116">Not supported.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="2cf72-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2cf72-117">Optional query parameters</span></span>
<span data-ttu-id="2cf72-118">Этот метод **не** поддерживает [параметры запросов OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2cf72-118">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="2cf72-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2cf72-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="2cf72-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2cf72-120">Request headers</span></span>
| <span data-ttu-id="2cf72-121">Имя</span><span class="sxs-lookup"><span data-stu-id="2cf72-121">Name</span></span>       | <span data-ttu-id="2cf72-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2cf72-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2cf72-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2cf72-123">Authorization</span></span>  | <span data-ttu-id="2cf72-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2cf72-124">Bearer {code}</span></span>|
| <span data-ttu-id="2cf72-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2cf72-125">Content-type</span></span>  | <span data-ttu-id="2cf72-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2cf72-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cf72-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2cf72-127">Request body</span></span>
<span data-ttu-id="2cf72-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2cf72-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2cf72-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="2cf72-129">Response</span></span>
<span data-ttu-id="2cf72-p102">В случае успешного выполнения этот метод возвращает код отклика `204 NoContent`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2cf72-p102">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="2cf72-132">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="2cf72-132">Error codes</span></span>
<span data-ttu-id="2cf72-133">Этот API соответствует стандартным кодам протокола HTTP.</span><span class="sxs-lookup"><span data-stu-id="2cf72-133">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="2cf72-134">Кроме того, коды настраиваемых ошибок указаны ниже.</span><span class="sxs-lookup"><span data-stu-id="2cf72-134">Besides, the custom error codes are shown below.</span></span>
|<span data-ttu-id="2cf72-135">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="2cf72-135">Error code</span></span>     | <span data-ttu-id="2cf72-136">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="2cf72-136">Error message</span></span>              | <span data-ttu-id="2cf72-137">Сведения</span><span class="sxs-lookup"><span data-stu-id="2cf72-137">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="2cf72-138">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="2cf72-138">400 BadRequest</span></span> | <span data-ttu-id="2cf72-139">ролеассигнментрекуестнотфаунд</span><span class="sxs-lookup"><span data-stu-id="2cf72-139">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="2cf72-140">GovernanceRoleAssignmentRequest не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="2cf72-140">The governanceRoleAssignmentRequest does not exist in system.</span></span>
| <span data-ttu-id="2cf72-141">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="2cf72-141">400 BadRequest</span></span> | <span data-ttu-id="2cf72-142">рекуестканнотбеканцеллед</span><span class="sxs-lookup"><span data-stu-id="2cf72-142">RequestCannotBeCancelled</span></span>    | <span data-ttu-id="2cf72-143">Только те запросы, которые `Granted`находятся `PendingApproval`в `PendingApprovalProvisioning` состоянии `PendingAdminDecision` , и могут быть отменены.</span><span class="sxs-lookup"><span data-stu-id="2cf72-143">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span>

## <a name="example"></a><span data-ttu-id="2cf72-144">Пример</span><span class="sxs-lookup"><span data-stu-id="2cf72-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2cf72-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="2cf72-145">Request</span></span>
<span data-ttu-id="2cf72-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2cf72-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2cf72-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="2cf72-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```
# <a name="c"></a>[<span data-ttu-id="2cf72-148">C#</span><span class="sxs-lookup"><span data-stu-id="2cf72-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cancel-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2cf72-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2cf72-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cancel-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2cf72-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2cf72-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cancel-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2cf72-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cf72-151">Response</span></span>
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
