---
title: Обновление Говернанцеролеассигнментрекуестс
description: Позволяет администраторам обновлять свои решения (`AdminApproved` или `AdminDenied`) в говернанцеролеассигнментрекуестс, которые находятся в состоянии `PendingAdminDecision`.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identitiy-platform
ms.openlocfilehash: 17e4c273a4ab3da5c5d4da4a54c9b57e339b5b81
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639809"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="afbe6-103">Обновление Говернанцеролеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="afbe6-103">Update governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="afbe6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afbe6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afbe6-105">Позволяет администраторам обновлять свои решения (`AdminApproved` или `AdminDenied`) в [говернанцеролеассигнментрекуестс](../resources/governanceroleassignmentrequest.md) , которые находятся в состоянии `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="afbe6-105">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="afbe6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="afbe6-106">Permissions</span></span>
<span data-ttu-id="afbe6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afbe6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="afbe6-109">**Примечание:** Кроме того, для этого API необходимо, чтобы у автора `Active` запроса было по крайней мере одно назначение роли администратора (`owner` или `user access administrator`) для ресурса, к которому относится [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="afbe6-109">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

|<span data-ttu-id="afbe6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="afbe6-110">Permission type</span></span>      | <span data-ttu-id="afbe6-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="afbe6-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="afbe6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="afbe6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="afbe6-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="afbe6-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="afbe6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="afbe6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afbe6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afbe6-115">Not supported.</span></span>    |
|<span data-ttu-id="afbe6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="afbe6-116">Application</span></span> | <span data-ttu-id="afbe6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afbe6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="afbe6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="afbe6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="afbe6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="afbe6-119">Request headers</span></span>
| <span data-ttu-id="afbe6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="afbe6-120">Name</span></span>           | <span data-ttu-id="afbe6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="afbe6-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="afbe6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="afbe6-122">Authorization</span></span>  | <span data-ttu-id="afbe6-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="afbe6-123">Bearer {code}</span></span>|
| <span data-ttu-id="afbe6-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="afbe6-124">Content-type</span></span>  | <span data-ttu-id="afbe6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="afbe6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afbe6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="afbe6-126">Request body</span></span>

|<span data-ttu-id="afbe6-127">Параметры</span><span class="sxs-lookup"><span data-stu-id="afbe6-127">Parameters</span></span>      |<span data-ttu-id="afbe6-128">Тип</span><span class="sxs-lookup"><span data-stu-id="afbe6-128">Type</span></span>                   |<span data-ttu-id="afbe6-129">Обязательный</span><span class="sxs-lookup"><span data-stu-id="afbe6-129">Required</span></span> |<span data-ttu-id="afbe6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="afbe6-130">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="afbe6-131">reason</span><span class="sxs-lookup"><span data-stu-id="afbe6-131">reason</span></span>        |<span data-ttu-id="afbe6-132">Строка</span><span class="sxs-lookup"><span data-stu-id="afbe6-132">String</span></span>                 |<span data-ttu-id="afbe6-133">✓</span><span class="sxs-lookup"><span data-stu-id="afbe6-133">✓</span></span>        |<span data-ttu-id="afbe6-134">Причина, предоставляемая администратором для своего решения.</span><span class="sxs-lookup"><span data-stu-id="afbe6-134">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="afbe6-135">решении</span><span class="sxs-lookup"><span data-stu-id="afbe6-135">decision</span></span>        |<span data-ttu-id="afbe6-136">Строка</span><span class="sxs-lookup"><span data-stu-id="afbe6-136">String</span></span>                 |<span data-ttu-id="afbe6-137">✓</span><span class="sxs-lookup"><span data-stu-id="afbe6-137">✓</span></span>        |<span data-ttu-id="afbe6-138">Принятие решения администратором запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="afbe6-138">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="afbe6-139">Значение должно быть Обновлено как `AdminApproved` или. `AdminDenied`</span><span class="sxs-lookup"><span data-stu-id="afbe6-139">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="afbe6-140">schedule</span><span class="sxs-lookup"><span data-stu-id="afbe6-140">schedule</span></span>      |[<span data-ttu-id="afbe6-141">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="afbe6-141">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="afbe6-142">Расписание запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="afbe6-142">The schedule of the role assignment request.</span></span> <span data-ttu-id="afbe6-143">Для состояния `AdminApproved`это обязательное требование.</span><span class="sxs-lookup"><span data-stu-id="afbe6-143">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="afbe6-144">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="afbe6-144">assignmentState</span></span>      |<span data-ttu-id="afbe6-145">Строка</span><span class="sxs-lookup"><span data-stu-id="afbe6-145">String</span></span>|         | <span data-ttu-id="afbe6-146">Состояние присваивания, а также значения: `Eligible` или. `Active`</span><span class="sxs-lookup"><span data-stu-id="afbe6-146">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="afbe6-147">Для решения `AdminApproved`это необходимо.</span><span class="sxs-lookup"><span data-stu-id="afbe6-147">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="afbe6-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="afbe6-148">Response</span></span>
<span data-ttu-id="afbe6-149">Этот метод можно применять только к запросам, которые находятся в состоянии `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="afbe6-149">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="afbe6-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="afbe6-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afbe6-152">Пример</span><span class="sxs-lookup"><span data-stu-id="afbe6-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="afbe6-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="afbe6-153">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="afbe6-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="afbe6-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
# <a name="c"></a>[<span data-ttu-id="afbe6-155">C#</span><span class="sxs-lookup"><span data-stu-id="afbe6-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updaterequest-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="afbe6-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="afbe6-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updaterequest-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="afbe6-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="afbe6-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updaterequest-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="request-body"></a><span data-ttu-id="afbe6-158">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="afbe6-158">Request body</span></span>
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

##### <a name="response"></a><span data-ttu-id="afbe6-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="afbe6-159">Response</span></span>
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
