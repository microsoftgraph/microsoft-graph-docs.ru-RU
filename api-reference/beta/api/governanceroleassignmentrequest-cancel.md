---
title: Отмена governanceRoleAssignmentRequest
description: Отмена объекта governanceRoleAssignmentRequest.
localization_priority: Normal
ms.openlocfilehash: 21446acdab943ac238154ee1631ccf7ffd2f8326
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263534"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="a89c5-103">Отмена governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="a89c5-103">Cancel governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a89c5-104">Отмена объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="a89c5-104">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a89c5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a89c5-105">Permissions</span></span>
<span data-ttu-id="a89c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a89c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a89c5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a89c5-108">Permission type</span></span>      | <span data-ttu-id="a89c5-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a89c5-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a89c5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a89c5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a89c5-111">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="a89c5-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="a89c5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a89c5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a89c5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a89c5-113">Not supported.</span></span>    |
|<span data-ttu-id="a89c5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a89c5-114">Application</span></span> | <span data-ttu-id="a89c5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a89c5-115">Not supported.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="a89c5-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a89c5-116">Optional query parameters</span></span>
<span data-ttu-id="a89c5-117">Этот метод **не** поддерживает [параметры запросов OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a89c5-117">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="a89c5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a89c5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="a89c5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a89c5-119">Request headers</span></span>
| <span data-ttu-id="a89c5-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a89c5-120">Name</span></span>       | <span data-ttu-id="a89c5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a89c5-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a89c5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a89c5-122">Authorization</span></span>  | <span data-ttu-id="a89c5-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a89c5-123">Bearer {code}</span></span>|
| <span data-ttu-id="a89c5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a89c5-124">Content-type</span></span>  | <span data-ttu-id="a89c5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a89c5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a89c5-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a89c5-126">Request body</span></span>
<span data-ttu-id="a89c5-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a89c5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a89c5-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="a89c5-128">Response</span></span>
<span data-ttu-id="a89c5-p102">В случае успешного выполнения этот метод возвращает код отклика `204 NoContent`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a89c5-p102">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="a89c5-131">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="a89c5-131">Error codes</span></span>
<span data-ttu-id="a89c5-132">Этот API соответствует стандартным кодам протокола HTTP.</span><span class="sxs-lookup"><span data-stu-id="a89c5-132">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="a89c5-133">Кроме того, коды настраиваемых ошибок указаны ниже.</span><span class="sxs-lookup"><span data-stu-id="a89c5-133">Besides, the custom error codes are shown below.</span></span>
|<span data-ttu-id="a89c5-134">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="a89c5-134">Error code</span></span>     | <span data-ttu-id="a89c5-135">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="a89c5-135">Error message</span></span>              | <span data-ttu-id="a89c5-136">Сведения</span><span class="sxs-lookup"><span data-stu-id="a89c5-136">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="a89c5-137">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="a89c5-137">400 BadRequest</span></span> | <span data-ttu-id="a89c5-138">Ролеассигнментрекуестнотфаунд</span><span class="sxs-lookup"><span data-stu-id="a89c5-138">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="a89c5-139">GovernanceRoleAssignmentRequest не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="a89c5-139">The governanceRoleAssignmentRequest does not exist in system.</span></span>
| <span data-ttu-id="a89c5-140">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="a89c5-140">400 BadRequest</span></span> | <span data-ttu-id="a89c5-141">Рекуестканнотбеканцеллед</span><span class="sxs-lookup"><span data-stu-id="a89c5-141">RequestCannotBeCancelled</span></span>    | <span data-ttu-id="a89c5-142">Только те запросы, которые `Granted`находятся `PendingApproval`в `PendingApprovalProvisioning` состоянии `PendingAdminDecision` , и могут быть отменены.</span><span class="sxs-lookup"><span data-stu-id="a89c5-142">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span>

## <a name="example"></a><span data-ttu-id="a89c5-143">Пример</span><span class="sxs-lookup"><span data-stu-id="a89c5-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a89c5-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="a89c5-144">Request</span></span>
<span data-ttu-id="a89c5-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a89c5-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```

##### <a name="response"></a><span data-ttu-id="a89c5-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="a89c5-146">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a89c5-147">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="a89c5-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a89c5-148">C#</span><span class="sxs-lookup"><span data-stu-id="a89c5-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/cancel_governanceroleassignmentrequest-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a89c5-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="a89c5-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/cancel_governanceroleassignmentrequest-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a89c5-150">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a89c5-150">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/cancel_governanceroleassignmentrequest-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-cancel.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-cancel.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-cancel.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
