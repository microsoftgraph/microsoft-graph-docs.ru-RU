---
title: Обновление governanceRoleAssignmentRequests
description: Включить администраторов для обновления своих решений `AdminApproved` (или) по `AdminDenied` governanceRoleAssignmentRequests, которые находятся в состоянии `PendingAdminDecision` .
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 59080cf19cf96d82f029d3ba9513cd16a042157a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435856"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="b6a3c-103">Обновление governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="b6a3c-103">Update governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="b6a3c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6a3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6a3c-105">Включить администраторов для обновления своих решений `AdminApproved` (или) по `AdminDenied` [governanceRoleAssignmentRequests,](../resources/governanceroleassignmentrequest.md) которые находятся в состоянии `PendingAdminDecision` .</span><span class="sxs-lookup"><span data-stu-id="b6a3c-105">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6a3c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b6a3c-106">Permissions</span></span>
<span data-ttu-id="b6a3c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="b6a3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

><span data-ttu-id="b6a3c-109">**Примечание:** Этот API также требует, чтобы у запрашиваемого по крайней мере одно назначение роли администратора (или) на ресурсе, к который принадлежит `Active` `owner` `user access administrator` [governanceRoleAssignmentRequest.](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="b6a3c-109">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

### <a name="azure-resources"></a><span data-ttu-id="b6a3c-110">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="b6a3c-110">Azure resources</span></span>

| <span data-ttu-id="b6a3c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6a3c-111">Permission type</span></span> | <span data-ttu-id="b6a3c-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b6a3c-112">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="b6a3c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6a3c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b6a3c-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="b6a3c-114">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="b6a3c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6a3c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6a3c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6a3c-116">Not supported.</span></span> |
| <span data-ttu-id="b6a3c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6a3c-117">Application</span></span> | <span data-ttu-id="b6a3c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6a3c-118">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="b6a3c-119">Azure AD</span><span class="sxs-lookup"><span data-stu-id="b6a3c-119">Azure AD</span></span>

| <span data-ttu-id="b6a3c-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6a3c-120">Permission type</span></span> | <span data-ttu-id="b6a3c-121">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b6a3c-121">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="b6a3c-122">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6a3c-122">Delegated (work or school account)</span></span> | <span data-ttu-id="b6a3c-123">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="b6a3c-123">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="b6a3c-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6a3c-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6a3c-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6a3c-125">Not supported.</span></span> |
| <span data-ttu-id="b6a3c-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6a3c-126">Application</span></span> | <span data-ttu-id="b6a3c-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6a3c-127">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="b6a3c-128">Группы</span><span class="sxs-lookup"><span data-stu-id="b6a3c-128">Groups</span></span>

|<span data-ttu-id="b6a3c-129">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6a3c-129">Permission type</span></span> | <span data-ttu-id="b6a3c-130">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b6a3c-130">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="b6a3c-131">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6a3c-131">Delegated (work or school account)</span></span> | <span data-ttu-id="b6a3c-132">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="b6a3c-132">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="b6a3c-133">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6a3c-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6a3c-134">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6a3c-134">Not supported.</span></span> |
| <span data-ttu-id="b6a3c-135">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6a3c-135">Application</span></span> | <span data-ttu-id="b6a3c-136">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6a3c-136">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6a3c-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6a3c-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="b6a3c-138">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6a3c-138">Request headers</span></span>
| <span data-ttu-id="b6a3c-139">Имя</span><span class="sxs-lookup"><span data-stu-id="b6a3c-139">Name</span></span>           | <span data-ttu-id="b6a3c-140">Описание</span><span class="sxs-lookup"><span data-stu-id="b6a3c-140">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b6a3c-141">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6a3c-141">Authorization</span></span>  | <span data-ttu-id="b6a3c-142">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b6a3c-142">Bearer {code}</span></span>|
| <span data-ttu-id="b6a3c-143">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b6a3c-143">Content-type</span></span>  | <span data-ttu-id="b6a3c-144">application/json</span><span class="sxs-lookup"><span data-stu-id="b6a3c-144">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6a3c-145">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b6a3c-145">Request body</span></span>

|<span data-ttu-id="b6a3c-146">Параметры</span><span class="sxs-lookup"><span data-stu-id="b6a3c-146">Parameters</span></span>      |<span data-ttu-id="b6a3c-147">Тип</span><span class="sxs-lookup"><span data-stu-id="b6a3c-147">Type</span></span>                   |<span data-ttu-id="b6a3c-148">Обязательный</span><span class="sxs-lookup"><span data-stu-id="b6a3c-148">Required</span></span> |<span data-ttu-id="b6a3c-149">Описание</span><span class="sxs-lookup"><span data-stu-id="b6a3c-149">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="b6a3c-150">reason</span><span class="sxs-lookup"><span data-stu-id="b6a3c-150">reason</span></span>        |<span data-ttu-id="b6a3c-151">String</span><span class="sxs-lookup"><span data-stu-id="b6a3c-151">String</span></span>                 |<span data-ttu-id="b6a3c-152">✓</span><span class="sxs-lookup"><span data-stu-id="b6a3c-152">✓</span></span>        |<span data-ttu-id="b6a3c-153">Причина, по которой администратор принял решение.</span><span class="sxs-lookup"><span data-stu-id="b6a3c-153">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="b6a3c-154">решение</span><span class="sxs-lookup"><span data-stu-id="b6a3c-154">decision</span></span>        |<span data-ttu-id="b6a3c-155">String</span><span class="sxs-lookup"><span data-stu-id="b6a3c-155">String</span></span>                 |<span data-ttu-id="b6a3c-156">✓</span><span class="sxs-lookup"><span data-stu-id="b6a3c-156">✓</span></span>        |<span data-ttu-id="b6a3c-157">Решение администратора запроса на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="b6a3c-157">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="b6a3c-158">Значение должно быть обновлено как `AdminApproved` или `AdminDenied` .</span><span class="sxs-lookup"><span data-stu-id="b6a3c-158">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="b6a3c-159">schedule</span><span class="sxs-lookup"><span data-stu-id="b6a3c-159">schedule</span></span>      |[<span data-ttu-id="b6a3c-160">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="b6a3c-160">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="b6a3c-161">Расписание запроса на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="b6a3c-161">The schedule of the role assignment request.</span></span> <span data-ttu-id="b6a3c-162">Для состояния `AdminApproved` требуется.</span><span class="sxs-lookup"><span data-stu-id="b6a3c-162">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="b6a3c-163">assignmentState</span><span class="sxs-lookup"><span data-stu-id="b6a3c-163">assignmentState</span></span>      |<span data-ttu-id="b6a3c-164">String</span><span class="sxs-lookup"><span data-stu-id="b6a3c-164">String</span></span>|         | <span data-ttu-id="b6a3c-165">Состояние назначения и значения могут быть `Eligible` или `Active` .</span><span class="sxs-lookup"><span data-stu-id="b6a3c-165">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="b6a3c-166">Для принятия `AdminApproved` решения требуется.</span><span class="sxs-lookup"><span data-stu-id="b6a3c-166">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="b6a3c-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6a3c-167">Response</span></span>
<span data-ttu-id="b6a3c-168">Этот метод может применяться только к запросам, которые находятся в состоянии `PendingAdminDecision` .</span><span class="sxs-lookup"><span data-stu-id="b6a3c-168">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="b6a3c-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b6a3c-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6a3c-171">Пример</span><span class="sxs-lookup"><span data-stu-id="b6a3c-171">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b6a3c-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6a3c-172">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b6a3c-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6a3c-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
# <a name="c"></a>[<span data-ttu-id="b6a3c-174">C#</span><span class="sxs-lookup"><span data-stu-id="b6a3c-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updaterequest-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6a3c-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6a3c-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updaterequest-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6a3c-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6a3c-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updaterequest-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b6a3c-177">Java</span><span class="sxs-lookup"><span data-stu-id="b6a3c-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/updaterequest-governanceroleassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="request-body"></a><span data-ttu-id="b6a3c-178">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6a3c-178">Request body</span></span>
```json
{
  "reason":"approve the request to extend role assignment",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-02-20T07:31:13.451Z",
    "stopDateTime":"2018-05-21T07:31:13.451Z",
    },
  "decision":"AdminApproved",
  "assignmentState": "Eligible"
}
```

##### <a name="response"></a><span data-ttu-id="b6a3c-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6a3c-179">Response</span></span>
<!-- {
  "blockType": "response",
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
  "description": "UpdateRequest governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


