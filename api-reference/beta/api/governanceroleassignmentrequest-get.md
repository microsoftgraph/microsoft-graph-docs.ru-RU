---
title: Получение governanceRoleAssignmentRequest
description: 'Получите governanceRoleAssignmentRequest. '
localization_priority: Normal
ms.openlocfilehash: 6914dbe8c45bcc05bc684b08fb5fdf87405a045a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524137"
---
# <a name="get-governanceroleassignmentrequest"></a><span data-ttu-id="6ef06-103">Получение governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="6ef06-103">Get governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ef06-104">Получите [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="6ef06-104">Get a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="6ef06-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ef06-105">Permissions</span></span>
<span data-ttu-id="6ef06-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ef06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ef06-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ef06-108">Permission type</span></span>      | <span data-ttu-id="6ef06-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ef06-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ef06-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ef06-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6ef06-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="6ef06-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="6ef06-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ef06-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ef06-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ef06-113">Not supported.</span></span>    |
|<span data-ttu-id="6ef06-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ef06-114">Application</span></span> | <span data-ttu-id="6ef06-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="6ef06-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="6ef06-116">Помимо области разрешений требуемыми инициатора запроса</span><span class="sxs-lookup"><span data-stu-id="6ef06-116">Besides the permission scope, it requires the requestor</span></span> 
*   <span data-ttu-id="6ef06-117">Чтобы иметь по крайней мере одна роль назначения для ресурса; или</span><span class="sxs-lookup"><span data-stu-id="6ef06-117">to have at least one role assignment on the resource; or</span></span>
*   <span data-ttu-id="6ef06-118">— это тема [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="6ef06-118">is the subject of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="6ef06-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ef06-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleAssignmentRequests/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6ef06-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6ef06-120">Optional query parameters</span></span>
<span data-ttu-id="6ef06-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6ef06-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ef06-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ef06-122">Request headers</span></span>
| <span data-ttu-id="6ef06-123">Имя</span><span class="sxs-lookup"><span data-stu-id="6ef06-123">Name</span></span>      |<span data-ttu-id="6ef06-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6ef06-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6ef06-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ef06-125">Authorization</span></span>  | <span data-ttu-id="6ef06-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6ef06-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ef06-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ef06-127">Request body</span></span>
<span data-ttu-id="6ef06-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6ef06-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ef06-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ef06-129">Response</span></span>
<span data-ttu-id="6ef06-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6ef06-130">If successful, this method returns a `200 OK` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ef06-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6ef06-131">Example</span></span>
<span data-ttu-id="6ef06-132">Получите запрос назначения ролей</span><span class="sxs-lookup"><span data-stu-id="6ef06-132">Get a role assignment request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequest"
}-->
##### <a name="request"></a><span data-ttu-id="6ef06-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ef06-133">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/e68ff888-4af5-4ccb-8b74-39156090344b
```
##### <a name="response"></a><span data-ttu-id="6ef06-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ef06-134">Response</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
