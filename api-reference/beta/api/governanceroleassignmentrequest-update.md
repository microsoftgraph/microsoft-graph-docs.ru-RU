---
title: Обновление Говернанцеролеассигнментрекуестс
description: Позволяет администраторам обновлять свои решения (`AdminApproved` или `AdminDenied`) в говернанцеролеассигнментрекуестс, которые находятся в состоянии `PendingAdminDecision`.
localization_priority: Normal
ms.openlocfilehash: 7931ae00eae01ca6ccd6f8d5f658fa0b2aa5fd8f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263513"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="42005-103">Обновление Говернанцеролеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="42005-103">Update governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42005-104">Позволяет администраторам обновлять свои решения (`AdminApproved` или `AdminDenied`) в [говернанцеролеассигнментрекуестс](../resources/governanceroleassignmentrequest.md) , которые находятся в состоянии `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="42005-104">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="42005-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42005-105">Permissions</span></span>
<span data-ttu-id="42005-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42005-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="42005-108">**Примечание:** Кроме того, для этого API необходимо, чтобы у автора `Active` запроса было по крайней мере одно назначение роли администратора (`owner` или `user access administrator`) для ресурса, к которому относится [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="42005-108">**Note:** This API also requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

|<span data-ttu-id="42005-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42005-109">Permission type</span></span>      | <span data-ttu-id="42005-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42005-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42005-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42005-111">Delegated (work or school account)</span></span> | <span data-ttu-id="42005-112">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="42005-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="42005-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42005-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42005-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42005-114">Not supported.</span></span>    |
|<span data-ttu-id="42005-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42005-115">Application</span></span> | <span data-ttu-id="42005-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42005-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="42005-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42005-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="42005-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42005-118">Request headers</span></span>
| <span data-ttu-id="42005-119">Имя</span><span class="sxs-lookup"><span data-stu-id="42005-119">Name</span></span>           | <span data-ttu-id="42005-120">Описание</span><span class="sxs-lookup"><span data-stu-id="42005-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="42005-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42005-121">Authorization</span></span>  | <span data-ttu-id="42005-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="42005-122">Bearer {code}</span></span>|
| <span data-ttu-id="42005-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="42005-123">Content-type</span></span>  | <span data-ttu-id="42005-124">application/json</span><span class="sxs-lookup"><span data-stu-id="42005-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42005-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="42005-125">Request body</span></span>

|<span data-ttu-id="42005-126">Параметры</span><span class="sxs-lookup"><span data-stu-id="42005-126">Parameters</span></span>      |<span data-ttu-id="42005-127">Тип</span><span class="sxs-lookup"><span data-stu-id="42005-127">Type</span></span>                   |<span data-ttu-id="42005-128">Обязательный</span><span class="sxs-lookup"><span data-stu-id="42005-128">Required</span></span> |<span data-ttu-id="42005-129">Описание</span><span class="sxs-lookup"><span data-stu-id="42005-129">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="42005-130">причиной</span><span class="sxs-lookup"><span data-stu-id="42005-130">reason</span></span>        |<span data-ttu-id="42005-131">String</span><span class="sxs-lookup"><span data-stu-id="42005-131">String</span></span>                 |<span data-ttu-id="42005-132">✓</span><span class="sxs-lookup"><span data-stu-id="42005-132">✓</span></span>        |<span data-ttu-id="42005-133">Причина, предоставляемая администратором для своего решения.</span><span class="sxs-lookup"><span data-stu-id="42005-133">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="42005-134">решении</span><span class="sxs-lookup"><span data-stu-id="42005-134">decision</span></span>        |<span data-ttu-id="42005-135">String</span><span class="sxs-lookup"><span data-stu-id="42005-135">String</span></span>                 |<span data-ttu-id="42005-136">✓</span><span class="sxs-lookup"><span data-stu-id="42005-136">✓</span></span>        |<span data-ttu-id="42005-137">Принятие решения администратором запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="42005-137">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="42005-138">Значение должно быть Обновлено как `AdminApproved` или. `AdminDenied`</span><span class="sxs-lookup"><span data-stu-id="42005-138">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="42005-139">schedule</span><span class="sxs-lookup"><span data-stu-id="42005-139">schedule</span></span>      |[<span data-ttu-id="42005-140">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="42005-140">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="42005-141">Расписание запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="42005-141">The schedule of the role assignment request.</span></span> <span data-ttu-id="42005-142">Для состояния `AdminApproved`это обязательное требование.</span><span class="sxs-lookup"><span data-stu-id="42005-142">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="42005-143">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="42005-143">assignmentState</span></span>      |<span data-ttu-id="42005-144">String</span><span class="sxs-lookup"><span data-stu-id="42005-144">String</span></span>|         | <span data-ttu-id="42005-145">Состояние присваивания, а также значения: `Eligible` или. `Active`</span><span class="sxs-lookup"><span data-stu-id="42005-145">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="42005-146">Для решения `AdminApproved`это необходимо.</span><span class="sxs-lookup"><span data-stu-id="42005-146">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="42005-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="42005-147">Response</span></span>
<span data-ttu-id="42005-148">Этот метод можно применять только к запросам, которые находятся в состоянии `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="42005-148">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="42005-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="42005-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42005-151">Пример</span><span class="sxs-lookup"><span data-stu-id="42005-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42005-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="42005-152">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
##### <a name="request-body"></a><span data-ttu-id="42005-153">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="42005-153">Request body</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="42005-154">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="42005-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="42005-155">C#</span><span class="sxs-lookup"><span data-stu-id="42005-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/updaterequest_governanceroleassignmentrequest-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="42005-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="42005-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/updaterequest_governanceroleassignmentrequest-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="42005-157">Цель — C</span><span class="sxs-lookup"><span data-stu-id="42005-157">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/updaterequest_governanceroleassignmentrequest-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="response"></a><span data-ttu-id="42005-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="42005-158">Response</span></span>
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
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
