---
title: Отменить governanceRoleAssignmentRequest
description: Отмена governanceRoleAssignmentRequest.
localization_priority: Normal
ms.openlocfilehash: f155a832a0c29935216dbc740e7db6ae8708f429
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809109"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="931ff-103">Отменить governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="931ff-103">Cancel governanceRoleAssignmentRequest</span></span>

> <span data-ttu-id="931ff-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="931ff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="931ff-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="931ff-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="931ff-106">Отмена [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="931ff-106">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="931ff-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="931ff-107">Permissions</span></span>
<span data-ttu-id="931ff-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="931ff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="931ff-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="931ff-110">Permission type</span></span>      | <span data-ttu-id="931ff-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="931ff-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="931ff-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="931ff-112">Delegated (work or school account)</span></span> | <span data-ttu-id="931ff-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="931ff-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="931ff-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="931ff-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="931ff-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="931ff-115">Not supported.</span></span>    |
|<span data-ttu-id="931ff-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="931ff-116">Application</span></span> | <span data-ttu-id="931ff-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="931ff-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="931ff-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="931ff-118">Optional query parameters</span></span>
<span data-ttu-id="931ff-119">Этот метод **не** поддерживает [параметры запросов OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="931ff-119">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="931ff-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="931ff-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="931ff-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="931ff-121">Request headers</span></span>
| <span data-ttu-id="931ff-122">Имя</span><span class="sxs-lookup"><span data-stu-id="931ff-122">Name</span></span>       | <span data-ttu-id="931ff-123">Описание</span><span class="sxs-lookup"><span data-stu-id="931ff-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="931ff-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="931ff-124">Authorization</span></span>  | <span data-ttu-id="931ff-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="931ff-125">Bearer {code}</span></span>|
| <span data-ttu-id="931ff-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="931ff-126">Content-type</span></span>  | <span data-ttu-id="931ff-127">application/json</span><span class="sxs-lookup"><span data-stu-id="931ff-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="931ff-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="931ff-128">Request body</span></span>
<span data-ttu-id="931ff-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="931ff-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="931ff-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="931ff-130">Response</span></span>
<span data-ttu-id="931ff-p103">В случае успешного выполнения этот метод возвращает код отклика `204 NoContent`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="931ff-p103">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="931ff-133">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="931ff-133">Error codes</span></span>
<span data-ttu-id="931ff-134">Этот интерфейс API стандарту кодов HTTP.</span><span class="sxs-lookup"><span data-stu-id="931ff-134">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="931ff-135">Кроме того ниже перечислены коды пользовательских ошибок.</span><span class="sxs-lookup"><span data-stu-id="931ff-135">Besides, the custom error codes are shown below.</span></span>
|<span data-ttu-id="931ff-136">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="931ff-136">Error code</span></span>     | <span data-ttu-id="931ff-137">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="931ff-137">Error message</span></span>              | <span data-ttu-id="931ff-138">Сведения</span><span class="sxs-lookup"><span data-stu-id="931ff-138">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="931ff-139">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="931ff-139">400 BadRequest</span></span> | <span data-ttu-id="931ff-140">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="931ff-140">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="931ff-141">GovernanceRoleAssignmentRequest не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="931ff-141">The governanceRoleAssignmentRequest does not exist in system.</span></span>
| <span data-ttu-id="931ff-142">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="931ff-142">400 BadRequest</span></span> | <span data-ttu-id="931ff-143">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="931ff-143">RequestCannotBeCancelled</span></span>    | <span data-ttu-id="931ff-144">Только запросы в состояние `Granted`, `PendingApproval`, `PendingApprovalProvisioning` и `PendingAdminDecision` можно отменить.</span><span class="sxs-lookup"><span data-stu-id="931ff-144">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span>

## <a name="example"></a><span data-ttu-id="931ff-145">Пример</span><span class="sxs-lookup"><span data-stu-id="931ff-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="931ff-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="931ff-146">Request</span></span>
<span data-ttu-id="931ff-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="931ff-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```

##### <a name="response"></a><span data-ttu-id="931ff-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="931ff-148">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Cancel governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
