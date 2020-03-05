---
title: Обновление Говернанцеролеассигнментрекуестс
description: Позволяет администраторам обновлять свои решения (`AdminApproved` или `AdminDenied`) в говернанцеролеассигнментрекуестс, которые находятся в состоянии `PendingAdminDecision`.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: d8fc97ff329b171050b0309161ec818a9996d4ec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42420950"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="eb8c7-103">Обновление Говернанцеролеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="eb8c7-103">Update governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="eb8c7-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eb8c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb8c7-105">Позволяет администраторам обновлять свои решения (`AdminApproved` или `AdminDenied`) в [говернанцеролеассигнментрекуестс](../resources/governanceroleassignmentrequest.md) , которые находятся в состоянии `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="eb8c7-105">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb8c7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eb8c7-106">Permissions</span></span>
<span data-ttu-id="eb8c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb8c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="eb8c7-109">**Примечание:** Кроме того, для этого API необходимо, чтобы у автора `Active` запроса было по крайней мере одно назначение роли администратора (`owner` или `user access administrator`) для ресурса, к которому относится [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="eb8c7-109">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

|<span data-ttu-id="eb8c7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb8c7-110">Permission type</span></span>      | <span data-ttu-id="eb8c7-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eb8c7-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb8c7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb8c7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eb8c7-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="eb8c7-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="eb8c7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb8c7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb8c7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb8c7-115">Not supported.</span></span>    |
|<span data-ttu-id="eb8c7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb8c7-116">Application</span></span> | <span data-ttu-id="eb8c7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb8c7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb8c7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb8c7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="eb8c7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb8c7-119">Request headers</span></span>
| <span data-ttu-id="eb8c7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="eb8c7-120">Name</span></span>           | <span data-ttu-id="eb8c7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="eb8c7-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="eb8c7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eb8c7-122">Authorization</span></span>  | <span data-ttu-id="eb8c7-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="eb8c7-123">Bearer {code}</span></span>|
| <span data-ttu-id="eb8c7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eb8c7-124">Content-type</span></span>  | <span data-ttu-id="eb8c7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eb8c7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb8c7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eb8c7-126">Request body</span></span>

|<span data-ttu-id="eb8c7-127">Параметры</span><span class="sxs-lookup"><span data-stu-id="eb8c7-127">Parameters</span></span>      |<span data-ttu-id="eb8c7-128">Тип</span><span class="sxs-lookup"><span data-stu-id="eb8c7-128">Type</span></span>                   |<span data-ttu-id="eb8c7-129">Обязательный</span><span class="sxs-lookup"><span data-stu-id="eb8c7-129">Required</span></span> |<span data-ttu-id="eb8c7-130">Описание</span><span class="sxs-lookup"><span data-stu-id="eb8c7-130">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="eb8c7-131">reason</span><span class="sxs-lookup"><span data-stu-id="eb8c7-131">reason</span></span>        |<span data-ttu-id="eb8c7-132">String</span><span class="sxs-lookup"><span data-stu-id="eb8c7-132">String</span></span>                 |<span data-ttu-id="eb8c7-133">✓</span><span class="sxs-lookup"><span data-stu-id="eb8c7-133">✓</span></span>        |<span data-ttu-id="eb8c7-134">Причина, предоставляемая администратором для своего решения.</span><span class="sxs-lookup"><span data-stu-id="eb8c7-134">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="eb8c7-135">решении</span><span class="sxs-lookup"><span data-stu-id="eb8c7-135">decision</span></span>        |<span data-ttu-id="eb8c7-136">String</span><span class="sxs-lookup"><span data-stu-id="eb8c7-136">String</span></span>                 |<span data-ttu-id="eb8c7-137">✓</span><span class="sxs-lookup"><span data-stu-id="eb8c7-137">✓</span></span>        |<span data-ttu-id="eb8c7-138">Принятие решения администратором запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="eb8c7-138">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="eb8c7-139">Значение должно быть Обновлено как `AdminApproved` или. `AdminDenied`</span><span class="sxs-lookup"><span data-stu-id="eb8c7-139">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="eb8c7-140">schedule</span><span class="sxs-lookup"><span data-stu-id="eb8c7-140">schedule</span></span>      |[<span data-ttu-id="eb8c7-141">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="eb8c7-141">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="eb8c7-142">Расписание запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="eb8c7-142">The schedule of the role assignment request.</span></span> <span data-ttu-id="eb8c7-143">Для состояния `AdminApproved`это обязательное требование.</span><span class="sxs-lookup"><span data-stu-id="eb8c7-143">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="eb8c7-144">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="eb8c7-144">assignmentState</span></span>      |<span data-ttu-id="eb8c7-145">String</span><span class="sxs-lookup"><span data-stu-id="eb8c7-145">String</span></span>|         | <span data-ttu-id="eb8c7-146">Состояние присваивания, а также значения: `Eligible` или. `Active`</span><span class="sxs-lookup"><span data-stu-id="eb8c7-146">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="eb8c7-147">Для решения `AdminApproved`это необходимо.</span><span class="sxs-lookup"><span data-stu-id="eb8c7-147">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="eb8c7-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb8c7-148">Response</span></span>
<span data-ttu-id="eb8c7-149">Этот метод можно применять только к запросам, которые находятся в состоянии `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="eb8c7-149">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="eb8c7-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="eb8c7-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb8c7-152">Пример</span><span class="sxs-lookup"><span data-stu-id="eb8c7-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb8c7-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb8c7-153">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="eb8c7-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb8c7-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
# <a name="c"></a>[<span data-ttu-id="eb8c7-155">C#</span><span class="sxs-lookup"><span data-stu-id="eb8c7-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updaterequest-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb8c7-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb8c7-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updaterequest-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb8c7-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb8c7-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updaterequest-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="request-body"></a><span data-ttu-id="eb8c7-158">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eb8c7-158">Request body</span></span>
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

##### <a name="response"></a><span data-ttu-id="eb8c7-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb8c7-159">Response</span></span>
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
