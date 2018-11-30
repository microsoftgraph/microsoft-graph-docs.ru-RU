---
title: Получение governanceRoleAssignmentRequest
description: 'Получите governanceRoleAssignmentRequest. '
ms.openlocfilehash: 4dca14c081edc9cd3609bd4eab1c79a10953e433
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079387"
---
# <a name="get-governanceroleassignmentrequest"></a><span data-ttu-id="b5dff-103">Получение governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="b5dff-103">Get governanceRoleAssignmentRequest</span></span>

> <span data-ttu-id="b5dff-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b5dff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5dff-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5dff-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b5dff-106">Получите [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="b5dff-106">Get a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="b5dff-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5dff-107">Permissions</span></span>
<span data-ttu-id="b5dff-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5dff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5dff-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5dff-110">Permission type</span></span>      | <span data-ttu-id="b5dff-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="b5dff-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5dff-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5dff-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b5dff-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="b5dff-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="b5dff-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5dff-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5dff-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5dff-115">Not supported.</span></span>    |
|<span data-ttu-id="b5dff-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="b5dff-116">Application</span></span> | <span data-ttu-id="b5dff-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="b5dff-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="b5dff-118">Помимо области разрешений требуемыми инициатора запроса</span><span class="sxs-lookup"><span data-stu-id="b5dff-118">Besides the permission scope, it requires the requestor</span></span> 
*   <span data-ttu-id="b5dff-119">Чтобы иметь по крайней мере одна роль назначения для ресурса; или</span><span class="sxs-lookup"><span data-stu-id="b5dff-119">to have at least one role assignment on the resource; or</span></span>
*   <span data-ttu-id="b5dff-120">— это тема [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="b5dff-120">is the subject of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="b5dff-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5dff-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleAssignmentRequests/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b5dff-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b5dff-122">Optional query parameters</span></span>
<span data-ttu-id="b5dff-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b5dff-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5dff-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5dff-124">Request headers</span></span>
| <span data-ttu-id="b5dff-125">Имя</span><span class="sxs-lookup"><span data-stu-id="b5dff-125">Name</span></span>      |<span data-ttu-id="b5dff-126">Описание</span><span class="sxs-lookup"><span data-stu-id="b5dff-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b5dff-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5dff-127">Authorization</span></span>  | <span data-ttu-id="b5dff-128">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b5dff-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5dff-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5dff-129">Request body</span></span>
<span data-ttu-id="b5dff-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b5dff-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5dff-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="b5dff-131">Response</span></span>
<span data-ttu-id="b5dff-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b5dff-132">If successful, this method returns a `200 OK` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5dff-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b5dff-133">Example</span></span>
<span data-ttu-id="b5dff-134">Получите запрос назначения ролей</span><span class="sxs-lookup"><span data-stu-id="b5dff-134">Get a role assignment request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequest"
}-->
##### <a name="request"></a><span data-ttu-id="b5dff-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5dff-135">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/e68ff888-4af5-4ccb-8b74-39156090344b
```
##### <a name="response"></a><span data-ttu-id="b5dff-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="b5dff-136">Response</span></span>
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
  "roleAssignmentStartDateTime":null,
  "roleAssignmentEndDateTime":null,
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
<!-- {
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->