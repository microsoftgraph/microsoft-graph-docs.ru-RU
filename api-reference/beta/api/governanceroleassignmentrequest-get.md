---
title: Get governanceRoleAssignmentRequest
description: 'Получите governanceRoleAssignmentRequest. '
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 87eae92aac54284407da6e33158e65819eadbd4e
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350770"
---
# <a name="get-governanceroleassignmentrequest"></a><span data-ttu-id="df127-103">Get governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="df127-103">Get governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="df127-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df127-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df127-105">Получите [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="df127-105">Get a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="df127-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="df127-106">Permissions</span></span>
<span data-ttu-id="df127-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="df127-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="df127-109">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="df127-109">Azure resources</span></span>

| <span data-ttu-id="df127-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df127-110">Permission type</span></span> | <span data-ttu-id="df127-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="df127-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="df127-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df127-112">Delegated (work or school account)</span></span> | <span data-ttu-id="df127-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="df127-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="df127-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df127-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df127-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df127-115">Not supported.</span></span> |
| <span data-ttu-id="df127-116">Application</span><span class="sxs-lookup"><span data-stu-id="df127-116">Application</span></span> | <span data-ttu-id="df127-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="df127-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="df127-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="df127-118">Azure AD</span></span>

| <span data-ttu-id="df127-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df127-119">Permission type</span></span> | <span data-ttu-id="df127-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="df127-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="df127-121">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df127-121">Delegated (work or school account)</span></span> | <span data-ttu-id="df127-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="df127-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="df127-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df127-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df127-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df127-124">Not supported.</span></span> |
| <span data-ttu-id="df127-125">Application</span><span class="sxs-lookup"><span data-stu-id="df127-125">Application</span></span> | <span data-ttu-id="df127-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="df127-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="df127-127">Группы</span><span class="sxs-lookup"><span data-stu-id="df127-127">Groups</span></span>

|<span data-ttu-id="df127-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df127-128">Permission type</span></span> | <span data-ttu-id="df127-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="df127-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="df127-130">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df127-130">Delegated (work or school account)</span></span> | <span data-ttu-id="df127-131">PrivilegedAccess.ReadWrite.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="df127-131">PrivilegedAccess.ReadWrite.AzureADGroup</span></span> |
| <span data-ttu-id="df127-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df127-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df127-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df127-133">Not supported.</span></span> |
| <span data-ttu-id="df127-134">Application</span><span class="sxs-lookup"><span data-stu-id="df127-134">Application</span></span> | <span data-ttu-id="df127-135">PrivilegedAccess.Read.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="df127-135">PrivilegedAccess.Read.AzureADGroup</span></span> |

<span data-ttu-id="df127-136">Помимо области разрешений, для этого требуется запросчик</span><span class="sxs-lookup"><span data-stu-id="df127-136">Besides the permission scope, it requires the requestor</span></span> 
*   <span data-ttu-id="df127-137">иметь хотя бы одно назначение роли на ресурсе; или</span><span class="sxs-lookup"><span data-stu-id="df127-137">to have at least one role assignment on the resource; or</span></span>
*   <span data-ttu-id="df127-138">является предметом [управленияRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="df127-138">is the subject of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="df127-139">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df127-139">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleAssignmentRequests/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="df127-140">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="df127-140">Optional query parameters</span></span>
<span data-ttu-id="df127-141">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="df127-141">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="df127-142">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="df127-142">Request headers</span></span>
| <span data-ttu-id="df127-143">Имя</span><span class="sxs-lookup"><span data-stu-id="df127-143">Name</span></span>      |<span data-ttu-id="df127-144">Описание</span><span class="sxs-lookup"><span data-stu-id="df127-144">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="df127-145">Авторизация</span><span class="sxs-lookup"><span data-stu-id="df127-145">Authorization</span></span>  | <span data-ttu-id="df127-146">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="df127-146">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="df127-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="df127-147">Request body</span></span>
<span data-ttu-id="df127-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="df127-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df127-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="df127-149">Response</span></span>
<span data-ttu-id="df127-150">В случае успешного выполнения этот метод возвращает код ответа и объект `200 OK` [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="df127-150">If successful, this method returns a `200 OK` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df127-151">Пример</span><span class="sxs-lookup"><span data-stu-id="df127-151">Example</span></span>
<span data-ttu-id="df127-152">Получить запрос на назначение ролей</span><span class="sxs-lookup"><span data-stu-id="df127-152">Get a role assignment request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequest"
}-->
##### <a name="request"></a><span data-ttu-id="df127-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="df127-153">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/e68ff888-4af5-4ccb-8b74-39156090344b
```
##### <a name="response"></a><span data-ttu-id="df127-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="df127-154">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"e68ff888-4af5-4ccb-8b74-39156090344b",
  "resourceId":"ec3a00f7-81dc-43b3-bbe7-650d3a5f7d46",
  "roleDefinitionId":"be0767b9-2c31-4b0d-b820-726228e7ff5c",
  "subjectId":"a4c5a837-b546-4ec5-a7df-e61547a46a4b",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminRemove",
  "assignmentState":"Eligible",
  "requestedDateTime":"2018-05-09T21:26:15.73-07:00",
  "reason":null,
  "status":{
    "status":"Closed",
    "subStatus":"Revoked",
    "statusDetails":[]
  },
  "schedule":null
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


