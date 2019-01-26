---
title: Обновление governanceRoleAssignmentRequests
description: Администраторы могли обновлять свои решения (`AdminApproved` или `AdminDenied`) на governanceRoleAssignmentRequests, находятся в состоянии `PendingAdminDecision`.
localization_priority: Normal
ms.openlocfilehash: 01178492517ae0ce1e2ed011e749e54af8e5d805
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576530"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="91c11-103">Обновление governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="91c11-103">Update governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91c11-104">Администраторы могли обновлять свои решения (`AdminApproved` или `AdminDenied`) на [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) , находятся в состоянии `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="91c11-104">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="91c11-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91c11-105">Permissions</span></span>
<span data-ttu-id="91c11-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91c11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="91c11-108">**Примечание:** Этот интерфейс API также требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) на ресурс, к которой принадлежит [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="91c11-108">**Note:** This API also requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

|<span data-ttu-id="91c11-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91c11-109">Permission type</span></span>      | <span data-ttu-id="91c11-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91c11-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91c11-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91c11-111">Delegated (work or school account)</span></span> | <span data-ttu-id="91c11-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="91c11-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="91c11-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91c11-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91c11-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91c11-114">Not supported.</span></span>    |
|<span data-ttu-id="91c11-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91c11-115">Application</span></span> | <span data-ttu-id="91c11-116">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="91c11-116">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="91c11-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91c11-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="91c11-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91c11-118">Request headers</span></span>
| <span data-ttu-id="91c11-119">Имя</span><span class="sxs-lookup"><span data-stu-id="91c11-119">Name</span></span>           | <span data-ttu-id="91c11-120">Описание</span><span class="sxs-lookup"><span data-stu-id="91c11-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="91c11-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="91c11-121">Authorization</span></span>  | <span data-ttu-id="91c11-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="91c11-122">Bearer {code}</span></span>|
| <span data-ttu-id="91c11-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="91c11-123">Content-type</span></span>  | <span data-ttu-id="91c11-124">application/json</span><span class="sxs-lookup"><span data-stu-id="91c11-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91c11-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91c11-125">Request body</span></span>

|<span data-ttu-id="91c11-126">Параметры</span><span class="sxs-lookup"><span data-stu-id="91c11-126">Parameters</span></span>      |<span data-ttu-id="91c11-127">Тип</span><span class="sxs-lookup"><span data-stu-id="91c11-127">Type</span></span>                   |<span data-ttu-id="91c11-128">Обязательный</span><span class="sxs-lookup"><span data-stu-id="91c11-128">Required</span></span> |<span data-ttu-id="91c11-129">Описание</span><span class="sxs-lookup"><span data-stu-id="91c11-129">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="91c11-130">Причина</span><span class="sxs-lookup"><span data-stu-id="91c11-130">reason</span></span>        |<span data-ttu-id="91c11-131">Строка</span><span class="sxs-lookup"><span data-stu-id="91c11-131">String</span></span>                 |<span data-ttu-id="91c11-132">✓</span><span class="sxs-lookup"><span data-stu-id="91c11-132">✓</span></span>        |<span data-ttu-id="91c11-133">Причины, предоставленный администратором для его решение.</span><span class="sxs-lookup"><span data-stu-id="91c11-133">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="91c11-134">решение</span><span class="sxs-lookup"><span data-stu-id="91c11-134">decision</span></span>        |<span data-ttu-id="91c11-135">Строка</span><span class="sxs-lookup"><span data-stu-id="91c11-135">String</span></span>                 |<span data-ttu-id="91c11-136">✓</span><span class="sxs-lookup"><span data-stu-id="91c11-136">✓</span></span>        |<span data-ttu-id="91c11-137">Администратор решение для запроса назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="91c11-137">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="91c11-138">Значение должно быть обновлено как `AdminApproved` или `AdminDenied`.</span><span class="sxs-lookup"><span data-stu-id="91c11-138">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="91c11-139">расписание</span><span class="sxs-lookup"><span data-stu-id="91c11-139">schedule</span></span>      |[<span data-ttu-id="91c11-140">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="91c11-140"> microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="91c11-141">Расписание для запроса назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="91c11-141">The schedule of the role assignment request.</span></span> <span data-ttu-id="91c11-142">Состояние `AdminApproved`, это необходимо.</span><span class="sxs-lookup"><span data-stu-id="91c11-142">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="91c11-143">assignmentState</span><span class="sxs-lookup"><span data-stu-id="91c11-143">assignmentState</span></span>      |<span data-ttu-id="91c11-144">Строка</span><span class="sxs-lookup"><span data-stu-id="91c11-144">String</span></span>|         | <span data-ttu-id="91c11-145">Состояние назначения и значения, может быть `Eligible` или `Active`.</span><span class="sxs-lookup"><span data-stu-id="91c11-145">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="91c11-146">Для принятия решений о `AdminApproved`, это необходимо.</span><span class="sxs-lookup"><span data-stu-id="91c11-146">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="91c11-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="91c11-147">Response</span></span>
<span data-ttu-id="91c11-148">Этот метод может применяться только к запросам, которые находятся в состоянии `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="91c11-148">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="91c11-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="91c11-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91c11-151">Пример</span><span class="sxs-lookup"><span data-stu-id="91c11-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91c11-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="91c11-152">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
##### <a name="request-body"></a><span data-ttu-id="91c11-153">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91c11-153">Request body</span></span>
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

##### <a name="response"></a><span data-ttu-id="91c11-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="91c11-154">Response</span></span>
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
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
