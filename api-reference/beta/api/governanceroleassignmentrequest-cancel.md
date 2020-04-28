---
title: Отмена governanceRoleAssignmentRequest
description: Отмена объекта governanceRoleAssignmentRequest.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 8179fa2d2bd1e8f52df9aa09bac5a965812e2122
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218887"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="abe85-103">Отмена governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="abe85-103">Cancel governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="abe85-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abe85-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abe85-105">Отмена объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="abe85-105">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="abe85-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="abe85-106">Permissions</span></span>
<span data-ttu-id="abe85-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abe85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abe85-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="abe85-109">Permission type</span></span>      | <span data-ttu-id="abe85-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="abe85-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="abe85-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="abe85-111">Delegated (work or school account)</span></span> | <span data-ttu-id="abe85-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="abe85-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="abe85-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="abe85-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abe85-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abe85-114">Not supported.</span></span>    |
|<span data-ttu-id="abe85-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="abe85-115">Application</span></span> | <span data-ttu-id="abe85-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abe85-116">Not supported.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="abe85-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="abe85-117">Optional query parameters</span></span>
<span data-ttu-id="abe85-118">Этот метод **не** поддерживает [параметры запросов OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="abe85-118">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="abe85-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="abe85-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="abe85-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="abe85-120">Request headers</span></span>
| <span data-ttu-id="abe85-121">Имя</span><span class="sxs-lookup"><span data-stu-id="abe85-121">Name</span></span>       | <span data-ttu-id="abe85-122">Описание</span><span class="sxs-lookup"><span data-stu-id="abe85-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="abe85-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="abe85-123">Authorization</span></span>  | <span data-ttu-id="abe85-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="abe85-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="abe85-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="abe85-126">Content-type</span></span>  | <span data-ttu-id="abe85-127">application/json</span><span class="sxs-lookup"><span data-stu-id="abe85-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abe85-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="abe85-128">Request body</span></span>
<span data-ttu-id="abe85-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="abe85-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abe85-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="abe85-130">Response</span></span>
<span data-ttu-id="abe85-p103">В случае успешного выполнения этот метод возвращает код отклика `204 NoContent`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="abe85-p103">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="abe85-133">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="abe85-133">Error codes</span></span>
<span data-ttu-id="abe85-134">Этот API соответствует стандартным кодам протокола HTTP.</span><span class="sxs-lookup"><span data-stu-id="abe85-134">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="abe85-135">Кроме того, коды настраиваемых ошибок указаны ниже.</span><span class="sxs-lookup"><span data-stu-id="abe85-135">Besides, the custom error codes are shown below.</span></span>
| <span data-ttu-id="abe85-136">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="abe85-136">Error code</span></span> | <span data-ttu-id="abe85-137">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="abe85-137">Error message</span></span> | <span data-ttu-id="abe85-138">Сведения</span><span class="sxs-lookup"><span data-stu-id="abe85-138">Details</span></span> |
|:---------- |:------------- |:------- |
| <span data-ttu-id="abe85-139">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="abe85-139">400 BadRequest</span></span> | <span data-ttu-id="abe85-140">ролеассигнментрекуестнотфаунд</span><span class="sxs-lookup"><span data-stu-id="abe85-140">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="abe85-141">GovernanceRoleAssignmentRequest не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="abe85-141">The governanceRoleAssignmentRequest does not exist in system.</span></span> |
| <span data-ttu-id="abe85-142">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="abe85-142">400 BadRequest</span></span> | <span data-ttu-id="abe85-143">рекуестканнотбеканцеллед</span><span class="sxs-lookup"><span data-stu-id="abe85-143">RequestCannotBeCancelled</span></span> | <span data-ttu-id="abe85-144">Только те запросы, которые `Granted`находятся `PendingApproval`в `PendingApprovalProvisioning` состоянии `PendingAdminDecision` , и могут быть отменены.</span><span class="sxs-lookup"><span data-stu-id="abe85-144">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span> |

## <a name="example"></a><span data-ttu-id="abe85-145">Пример</span><span class="sxs-lookup"><span data-stu-id="abe85-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="abe85-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="abe85-146">Request</span></span>
<span data-ttu-id="abe85-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="abe85-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="abe85-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="abe85-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```
# <a name="c"></a>[<span data-ttu-id="abe85-149">C#</span><span class="sxs-lookup"><span data-stu-id="abe85-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cancel-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="abe85-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="abe85-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cancel-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="abe85-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="abe85-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cancel-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="abe85-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="abe85-152">Response</span></span>
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
