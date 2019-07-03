---
title: Обновление Говернанцеролеассигнментрекуестс
description: Позволяет администраторам обновлять свои решения (`AdminApproved` или `AdminDenied`) в говернанцеролеассигнментрекуестс, которые находятся в состоянии `PendingAdminDecision`.
localization_priority: Normal
ms.openlocfilehash: 03f8d87d75a8edfa9c6b8fdc818114e0b41661ce
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440773"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="25fb5-103">Обновление Говернанцеролеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="25fb5-103">Update governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25fb5-104">Позволяет администраторам обновлять свои решения (`AdminApproved` или `AdminDenied`) в [говернанцеролеассигнментрекуестс](../resources/governanceroleassignmentrequest.md) , которые находятся в состоянии `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="25fb5-104">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="25fb5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25fb5-105">Permissions</span></span>
<span data-ttu-id="25fb5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25fb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="25fb5-108">**Примечание:** Кроме того, для этого API необходимо, чтобы у автора `Active` запроса было по крайней мере одно назначение роли администратора (`owner` или `user access administrator`) для ресурса, к которому относится [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="25fb5-108">**Note:** This API also requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

|<span data-ttu-id="25fb5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25fb5-109">Permission type</span></span>      | <span data-ttu-id="25fb5-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25fb5-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25fb5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25fb5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="25fb5-112">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="25fb5-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="25fb5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25fb5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25fb5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25fb5-114">Not supported.</span></span>    |
|<span data-ttu-id="25fb5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25fb5-115">Application</span></span> | <span data-ttu-id="25fb5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25fb5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="25fb5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25fb5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="25fb5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25fb5-118">Request headers</span></span>
| <span data-ttu-id="25fb5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="25fb5-119">Name</span></span>           | <span data-ttu-id="25fb5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="25fb5-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="25fb5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25fb5-121">Authorization</span></span>  | <span data-ttu-id="25fb5-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="25fb5-122">Bearer {code}</span></span>|
| <span data-ttu-id="25fb5-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="25fb5-123">Content-type</span></span>  | <span data-ttu-id="25fb5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="25fb5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25fb5-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="25fb5-125">Request body</span></span>

|<span data-ttu-id="25fb5-126">Параметры</span><span class="sxs-lookup"><span data-stu-id="25fb5-126">Parameters</span></span>      |<span data-ttu-id="25fb5-127">Тип</span><span class="sxs-lookup"><span data-stu-id="25fb5-127">Type</span></span>                   |<span data-ttu-id="25fb5-128">Обязательный</span><span class="sxs-lookup"><span data-stu-id="25fb5-128">Required</span></span> |<span data-ttu-id="25fb5-129">Описание</span><span class="sxs-lookup"><span data-stu-id="25fb5-129">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="25fb5-130">причиной</span><span class="sxs-lookup"><span data-stu-id="25fb5-130">reason</span></span>        |<span data-ttu-id="25fb5-131">String</span><span class="sxs-lookup"><span data-stu-id="25fb5-131">String</span></span>                 |<span data-ttu-id="25fb5-132">✓</span><span class="sxs-lookup"><span data-stu-id="25fb5-132">✓</span></span>        |<span data-ttu-id="25fb5-133">Причина, предоставляемая администратором для своего решения.</span><span class="sxs-lookup"><span data-stu-id="25fb5-133">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="25fb5-134">решении</span><span class="sxs-lookup"><span data-stu-id="25fb5-134">decision</span></span>        |<span data-ttu-id="25fb5-135">String</span><span class="sxs-lookup"><span data-stu-id="25fb5-135">String</span></span>                 |<span data-ttu-id="25fb5-136">✓</span><span class="sxs-lookup"><span data-stu-id="25fb5-136">✓</span></span>        |<span data-ttu-id="25fb5-137">Принятие решения администратором запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="25fb5-137">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="25fb5-138">Значение должно быть Обновлено как `AdminApproved` или. `AdminDenied`</span><span class="sxs-lookup"><span data-stu-id="25fb5-138">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="25fb5-139">schedule</span><span class="sxs-lookup"><span data-stu-id="25fb5-139">schedule</span></span>      |[<span data-ttu-id="25fb5-140">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="25fb5-140">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="25fb5-141">Расписание запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="25fb5-141">The schedule of the role assignment request.</span></span> <span data-ttu-id="25fb5-142">Для состояния `AdminApproved`это обязательное требование.</span><span class="sxs-lookup"><span data-stu-id="25fb5-142">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="25fb5-143">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="25fb5-143">assignmentState</span></span>      |<span data-ttu-id="25fb5-144">String</span><span class="sxs-lookup"><span data-stu-id="25fb5-144">String</span></span>|         | <span data-ttu-id="25fb5-145">Состояние присваивания, а также значения: `Eligible` или. `Active`</span><span class="sxs-lookup"><span data-stu-id="25fb5-145">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="25fb5-146">Для решения `AdminApproved`это необходимо.</span><span class="sxs-lookup"><span data-stu-id="25fb5-146">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="25fb5-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="25fb5-147">Response</span></span>
<span data-ttu-id="25fb5-148">Этот метод можно применять только к запросам, которые находятся в состоянии `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="25fb5-148">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="25fb5-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="25fb5-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25fb5-151">Пример</span><span class="sxs-lookup"><span data-stu-id="25fb5-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="25fb5-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="25fb5-152">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="25fb5-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="25fb5-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="25fb5-154">C#</span><span class="sxs-lookup"><span data-stu-id="25fb5-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updaterequest-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="25fb5-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="25fb5-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updaterequest-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="25fb5-156">Цель — C</span><span class="sxs-lookup"><span data-stu-id="25fb5-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updaterequest-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="request-body"></a><span data-ttu-id="25fb5-157">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="25fb5-157">Request body</span></span>
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

##### <a name="response"></a><span data-ttu-id="25fb5-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="25fb5-158">Response</span></span>
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
