---
title: Обновление Говернанцеролеассигнментрекуестс
description: Позволяет администраторам обновлять свои решения ( `AdminApproved` или `AdminDenied` ) в говернанцеролеассигнментрекуестс, которые находятся в состоянии `PendingAdminDecision` .
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 95ff7dbf174a5dc6287be0fc7476c21596e651ba
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634874"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="2a9f9-103">Обновление Говернанцеролеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="2a9f9-103">Update governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="2a9f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a9f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a9f9-105">Позволяет администраторам обновлять свои решения ( `AdminApproved` или `AdminDenied` ) в [говернанцеролеассигнментрекуестс](../resources/governanceroleassignmentrequest.md) , которые находятся в состоянии `PendingAdminDecision` .</span><span class="sxs-lookup"><span data-stu-id="2a9f9-105">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a9f9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a9f9-106">Permissions</span></span>
<span data-ttu-id="2a9f9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="2a9f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

><span data-ttu-id="2a9f9-109">**Примечание:** Кроме того, для этого API необходимо, чтобы у автора запроса было по крайней мере одно `Active` назначение роли администратора ( `owner` или `user access administrator` ) для ресурса, к которому относится [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="2a9f9-109">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

### <a name="azure-resources"></a><span data-ttu-id="2a9f9-110">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="2a9f9-110">Azure resources</span></span>

| <span data-ttu-id="2a9f9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a9f9-111">Permission type</span></span> | <span data-ttu-id="2a9f9-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a9f9-112">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="2a9f9-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a9f9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2a9f9-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="2a9f9-114">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="2a9f9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a9f9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a9f9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a9f9-116">Not supported.</span></span> |
| <span data-ttu-id="2a9f9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a9f9-117">Application</span></span> | <span data-ttu-id="2a9f9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a9f9-118">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="2a9f9-119">Azure AD</span><span class="sxs-lookup"><span data-stu-id="2a9f9-119">Azure AD</span></span>

| <span data-ttu-id="2a9f9-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a9f9-120">Permission type</span></span> | <span data-ttu-id="2a9f9-121">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a9f9-121">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="2a9f9-122">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a9f9-122">Delegated (work or school account)</span></span> | <span data-ttu-id="2a9f9-123">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="2a9f9-123">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="2a9f9-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a9f9-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a9f9-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a9f9-125">Not supported.</span></span> |
| <span data-ttu-id="2a9f9-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a9f9-126">Application</span></span> | <span data-ttu-id="2a9f9-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a9f9-127">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="2a9f9-128">Группы</span><span class="sxs-lookup"><span data-stu-id="2a9f9-128">Groups</span></span>

|<span data-ttu-id="2a9f9-129">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a9f9-129">Permission type</span></span> | <span data-ttu-id="2a9f9-130">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a9f9-130">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="2a9f9-131">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a9f9-131">Delegated (work or school account)</span></span> | <span data-ttu-id="2a9f9-132">Привилежедакцесс. ReadWrite. Азуреадграупс</span><span class="sxs-lookup"><span data-stu-id="2a9f9-132">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="2a9f9-133">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a9f9-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a9f9-134">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a9f9-134">Not supported.</span></span> |
| <span data-ttu-id="2a9f9-135">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a9f9-135">Application</span></span> | <span data-ttu-id="2a9f9-136">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a9f9-136">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a9f9-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a9f9-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="2a9f9-138">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a9f9-138">Request headers</span></span>
| <span data-ttu-id="2a9f9-139">Имя</span><span class="sxs-lookup"><span data-stu-id="2a9f9-139">Name</span></span>           | <span data-ttu-id="2a9f9-140">Описание</span><span class="sxs-lookup"><span data-stu-id="2a9f9-140">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2a9f9-141">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a9f9-141">Authorization</span></span>  | <span data-ttu-id="2a9f9-142">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2a9f9-142">Bearer {code}</span></span>|
| <span data-ttu-id="2a9f9-143">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2a9f9-143">Content-type</span></span>  | <span data-ttu-id="2a9f9-144">application/json</span><span class="sxs-lookup"><span data-stu-id="2a9f9-144">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a9f9-145">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2a9f9-145">Request body</span></span>

|<span data-ttu-id="2a9f9-146">Параметры</span><span class="sxs-lookup"><span data-stu-id="2a9f9-146">Parameters</span></span>      |<span data-ttu-id="2a9f9-147">Тип</span><span class="sxs-lookup"><span data-stu-id="2a9f9-147">Type</span></span>                   |<span data-ttu-id="2a9f9-148">Обязательный</span><span class="sxs-lookup"><span data-stu-id="2a9f9-148">Required</span></span> |<span data-ttu-id="2a9f9-149">Описание</span><span class="sxs-lookup"><span data-stu-id="2a9f9-149">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="2a9f9-150">reason</span><span class="sxs-lookup"><span data-stu-id="2a9f9-150">reason</span></span>        |<span data-ttu-id="2a9f9-151">String</span><span class="sxs-lookup"><span data-stu-id="2a9f9-151">String</span></span>                 |<span data-ttu-id="2a9f9-152">✓</span><span class="sxs-lookup"><span data-stu-id="2a9f9-152">✓</span></span>        |<span data-ttu-id="2a9f9-153">Причина, предоставляемая администратором для своего решения.</span><span class="sxs-lookup"><span data-stu-id="2a9f9-153">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="2a9f9-154">решении</span><span class="sxs-lookup"><span data-stu-id="2a9f9-154">decision</span></span>        |<span data-ttu-id="2a9f9-155">String</span><span class="sxs-lookup"><span data-stu-id="2a9f9-155">String</span></span>                 |<span data-ttu-id="2a9f9-156">✓</span><span class="sxs-lookup"><span data-stu-id="2a9f9-156">✓</span></span>        |<span data-ttu-id="2a9f9-157">Принятие решения администратором запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="2a9f9-157">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="2a9f9-158">Значение должно быть Обновлено как `AdminApproved` или `AdminDenied` .</span><span class="sxs-lookup"><span data-stu-id="2a9f9-158">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="2a9f9-159">schedule</span><span class="sxs-lookup"><span data-stu-id="2a9f9-159">schedule</span></span>      |[<span data-ttu-id="2a9f9-160">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2a9f9-160">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="2a9f9-161">Расписание запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="2a9f9-161">The schedule of the role assignment request.</span></span> <span data-ttu-id="2a9f9-162">Для состояния `AdminApproved` это обязательное требование.</span><span class="sxs-lookup"><span data-stu-id="2a9f9-162">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="2a9f9-163">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="2a9f9-163">assignmentState</span></span>      |<span data-ttu-id="2a9f9-164">String</span><span class="sxs-lookup"><span data-stu-id="2a9f9-164">String</span></span>|         | <span data-ttu-id="2a9f9-165">Состояние присваивания, а также значения `Eligible` `Active` : или.</span><span class="sxs-lookup"><span data-stu-id="2a9f9-165">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="2a9f9-166">Для решения `AdminApproved` это необходимо.</span><span class="sxs-lookup"><span data-stu-id="2a9f9-166">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="2a9f9-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="2a9f9-167">Response</span></span>
<span data-ttu-id="2a9f9-168">Этот метод можно применять только к запросам, которые находятся в состоянии `PendingAdminDecision` .</span><span class="sxs-lookup"><span data-stu-id="2a9f9-168">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="2a9f9-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2a9f9-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a9f9-171">Пример</span><span class="sxs-lookup"><span data-stu-id="2a9f9-171">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2a9f9-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a9f9-172">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2a9f9-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a9f9-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
# <a name="c"></a>[<span data-ttu-id="2a9f9-174">C#</span><span class="sxs-lookup"><span data-stu-id="2a9f9-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updaterequest-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a9f9-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a9f9-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updaterequest-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a9f9-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a9f9-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updaterequest-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="request-body"></a><span data-ttu-id="2a9f9-177">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a9f9-177">Request body</span></span>
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

##### <a name="response"></a><span data-ttu-id="2a9f9-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a9f9-178">Response</span></span>
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


