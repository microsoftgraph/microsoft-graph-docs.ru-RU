---
title: Обновление governanceRoleAssignmentRequests
description: Администраторы могли обновлять свои решения (`AdminApproved` или `AdminDenied`) на governanceRoleAssignmentRequests, находятся в состоянии `PendingAdminDecision`.
ms.openlocfilehash: 0f52b810b861e18a679ae8aea4ffdf7fd2d67abd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082292"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="d0ef3-103">Обновление governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="d0ef3-103">Update governanceRoleAssignmentRequests</span></span>

> <span data-ttu-id="d0ef3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d0ef3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0ef3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0ef3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d0ef3-106">Администраторы могли обновлять свои решения (`AdminApproved` или `AdminDenied`) на [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) , находятся в состоянии `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="d0ef3-106">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0ef3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0ef3-107">Permissions</span></span>
<span data-ttu-id="d0ef3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0ef3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0ef3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0ef3-110">Permission type</span></span>      | <span data-ttu-id="d0ef3-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="d0ef3-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0ef3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0ef3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d0ef3-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="d0ef3-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="d0ef3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0ef3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0ef3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0ef3-115">Not supported.</span></span>    |
|<span data-ttu-id="d0ef3-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="d0ef3-116">Application</span></span> | <span data-ttu-id="d0ef3-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="d0ef3-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="d0ef3-118">Помимо области разрешений этот интерфейс API требует инициатор запроса может иметь по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) на ресурс, который принадлежит [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="d0ef3-118">Besides the permission scope, this API requires the requestor to have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource, which the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

## <a name="http-request"></a><span data-ttu-id="d0ef3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0ef3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

### <a name="request-headers"></a><span data-ttu-id="d0ef3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0ef3-120">Request headers</span></span>
| <span data-ttu-id="d0ef3-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d0ef3-121">Name</span></span>           | <span data-ttu-id="d0ef3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d0ef3-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d0ef3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0ef3-123">Authorization</span></span>  | <span data-ttu-id="d0ef3-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d0ef3-124">Bearer {code}</span></span>|
| <span data-ttu-id="d0ef3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d0ef3-125">Content-type</span></span>  | <span data-ttu-id="d0ef3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d0ef3-126">application/json</span></span>|

### <a name="request-body"></a><span data-ttu-id="d0ef3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0ef3-127">Request body</span></span>
|<span data-ttu-id="d0ef3-128">Parameters</span><span class="sxs-lookup"><span data-stu-id="d0ef3-128">Parameters</span></span>      |<span data-ttu-id="d0ef3-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d0ef3-129">Type</span></span>                   |<span data-ttu-id="d0ef3-130">Обязательный</span><span class="sxs-lookup"><span data-stu-id="d0ef3-130">Required</span></span> |<span data-ttu-id="d0ef3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d0ef3-131">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="d0ef3-132">Причина</span><span class="sxs-lookup"><span data-stu-id="d0ef3-132">reason</span></span>        |<span data-ttu-id="d0ef3-133">String</span><span class="sxs-lookup"><span data-stu-id="d0ef3-133">String</span></span>                 |<span data-ttu-id="d0ef3-134">✓</span><span class="sxs-lookup"><span data-stu-id="d0ef3-134">✓</span></span>        |<span data-ttu-id="d0ef3-135">Причины, предоставленный администратором для его решение.</span><span class="sxs-lookup"><span data-stu-id="d0ef3-135">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="d0ef3-136">решение</span><span class="sxs-lookup"><span data-stu-id="d0ef3-136">decision</span></span>        |<span data-ttu-id="d0ef3-137">String</span><span class="sxs-lookup"><span data-stu-id="d0ef3-137">String</span></span>                 |<span data-ttu-id="d0ef3-138">✓</span><span class="sxs-lookup"><span data-stu-id="d0ef3-138">✓</span></span>        |<span data-ttu-id="d0ef3-139">Администратор решение для запроса назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="d0ef3-139">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="d0ef3-140">Значение должно быть обновлено как `AdminApproved` или `AdminDenied`.</span><span class="sxs-lookup"><span data-stu-id="d0ef3-140">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="d0ef3-141">расписание</span><span class="sxs-lookup"><span data-stu-id="d0ef3-141">schedule</span></span>      |[<span data-ttu-id="d0ef3-142">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="d0ef3-142">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="d0ef3-143">Расписание для запроса назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="d0ef3-143">The schedule of the role assignment request.</span></span> <span data-ttu-id="d0ef3-144">Состояние `AdminApproved`, это необходимо.</span><span class="sxs-lookup"><span data-stu-id="d0ef3-144">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="d0ef3-145">assignmentState</span><span class="sxs-lookup"><span data-stu-id="d0ef3-145">assignmentState</span></span>      |<span data-ttu-id="d0ef3-146">String</span><span class="sxs-lookup"><span data-stu-id="d0ef3-146">String</span></span>|         | <span data-ttu-id="d0ef3-147">Состояние назначения и значения, может быть `Eligible` или `Active`.</span><span class="sxs-lookup"><span data-stu-id="d0ef3-147">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="d0ef3-148">Для принятия решений о `AdminApproved`, это необходимо.</span><span class="sxs-lookup"><span data-stu-id="d0ef3-148">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="d0ef3-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="d0ef3-149">Response</span></span>
<span data-ttu-id="d0ef3-150">Этот метод может применяться только к запросам, которые находятся в состоянии `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="d0ef3-150">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="d0ef3-p106">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d0ef3-p106">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="d0ef3-153">Пример</span><span class="sxs-lookup"><span data-stu-id="d0ef3-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0ef3-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0ef3-154">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
##### <a name="request-body"></a><span data-ttu-id="d0ef3-155">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0ef3-155">Request body</span></span>
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

##### <a name="response"></a><span data-ttu-id="d0ef3-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0ef3-156">Response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UpdateRequest governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
