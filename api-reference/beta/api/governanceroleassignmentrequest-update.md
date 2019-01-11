---
title: Обновление governanceRoleAssignmentRequests
description: Администраторы могли обновлять свои решения (`AdminApproved` или `AdminDenied`) на governanceRoleAssignmentRequests, находятся в состоянии `PendingAdminDecision`.
localization_priority: Normal
ms.openlocfilehash: 3d68e06688922177e2a1a183a9fe4bfc6be6a91d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874937"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="d1eaa-103">Обновление governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="d1eaa-103">Update governanceRoleAssignmentRequests</span></span>

> <span data-ttu-id="d1eaa-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d1eaa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1eaa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1eaa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d1eaa-106">Администраторы могли обновлять свои решения (`AdminApproved` или `AdminDenied`) на [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) , находятся в состоянии `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="d1eaa-106">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1eaa-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1eaa-107">Permissions</span></span>
<span data-ttu-id="d1eaa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1eaa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="d1eaa-110">**Примечание:** Этот интерфейс API также требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) на ресурс, к которой принадлежит [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="d1eaa-110">**Note:** This API also requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

|<span data-ttu-id="d1eaa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1eaa-111">Permission type</span></span>      | <span data-ttu-id="d1eaa-112">Permissions</span><span class="sxs-lookup"><span data-stu-id="d1eaa-112">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1eaa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1eaa-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d1eaa-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="d1eaa-114">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="d1eaa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1eaa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1eaa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1eaa-116">Not supported.</span></span>    |
|<span data-ttu-id="d1eaa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1eaa-117">Application</span></span> | <span data-ttu-id="d1eaa-118">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="d1eaa-118">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1eaa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1eaa-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="d1eaa-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1eaa-120">Request headers</span></span>
| <span data-ttu-id="d1eaa-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d1eaa-121">Name</span></span>           | <span data-ttu-id="d1eaa-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d1eaa-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d1eaa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1eaa-123">Authorization</span></span>  | <span data-ttu-id="d1eaa-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d1eaa-124">Bearer {code}</span></span>|
| <span data-ttu-id="d1eaa-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d1eaa-125">Content-type</span></span>  | <span data-ttu-id="d1eaa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1eaa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1eaa-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d1eaa-127">Request body</span></span>

|<span data-ttu-id="d1eaa-128">Параметры</span><span class="sxs-lookup"><span data-stu-id="d1eaa-128">Parameters</span></span>      |<span data-ttu-id="d1eaa-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d1eaa-129">Type</span></span>                   |<span data-ttu-id="d1eaa-130">Обязательный</span><span class="sxs-lookup"><span data-stu-id="d1eaa-130">Required</span></span> |<span data-ttu-id="d1eaa-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d1eaa-131">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="d1eaa-132">Причина</span><span class="sxs-lookup"><span data-stu-id="d1eaa-132">reason</span></span>        |<span data-ttu-id="d1eaa-133">Строка</span><span class="sxs-lookup"><span data-stu-id="d1eaa-133">String</span></span>                 |<span data-ttu-id="d1eaa-134">✓</span><span class="sxs-lookup"><span data-stu-id="d1eaa-134">✓</span></span>        |<span data-ttu-id="d1eaa-135">Причины, предоставленный администратором для его решение.</span><span class="sxs-lookup"><span data-stu-id="d1eaa-135">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="d1eaa-136">решение</span><span class="sxs-lookup"><span data-stu-id="d1eaa-136">decision</span></span>        |<span data-ttu-id="d1eaa-137">Строка</span><span class="sxs-lookup"><span data-stu-id="d1eaa-137">String</span></span>                 |<span data-ttu-id="d1eaa-138">✓</span><span class="sxs-lookup"><span data-stu-id="d1eaa-138">✓</span></span>        |<span data-ttu-id="d1eaa-139">Администратор решение для запроса назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="d1eaa-139">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="d1eaa-140">Значение должно быть обновлено как `AdminApproved` или `AdminDenied`.</span><span class="sxs-lookup"><span data-stu-id="d1eaa-140">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="d1eaa-141">расписание</span><span class="sxs-lookup"><span data-stu-id="d1eaa-141">schedule</span></span>      |[<span data-ttu-id="d1eaa-142">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="d1eaa-142">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="d1eaa-143">Расписание для запроса назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="d1eaa-143">The schedule of the role assignment request.</span></span> <span data-ttu-id="d1eaa-144">Состояние `AdminApproved`, это необходимо.</span><span class="sxs-lookup"><span data-stu-id="d1eaa-144">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="d1eaa-145">assignmentState</span><span class="sxs-lookup"><span data-stu-id="d1eaa-145">assignmentState</span></span>      |<span data-ttu-id="d1eaa-146">Строка</span><span class="sxs-lookup"><span data-stu-id="d1eaa-146">String</span></span>|         | <span data-ttu-id="d1eaa-147">Состояние назначения и значения, может быть `Eligible` или `Active`.</span><span class="sxs-lookup"><span data-stu-id="d1eaa-147">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="d1eaa-148">Для принятия решений о `AdminApproved`, это необходимо.</span><span class="sxs-lookup"><span data-stu-id="d1eaa-148">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="d1eaa-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="d1eaa-149">Response</span></span>
<span data-ttu-id="d1eaa-150">Этот метод может применяться только к запросам, которые находятся в состоянии `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="d1eaa-150">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="d1eaa-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d1eaa-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1eaa-153">Пример</span><span class="sxs-lookup"><span data-stu-id="d1eaa-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1eaa-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1eaa-154">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
##### <a name="request-body"></a><span data-ttu-id="d1eaa-155">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d1eaa-155">Request body</span></span>
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

##### <a name="response"></a><span data-ttu-id="d1eaa-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1eaa-156">Response</span></span>
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
