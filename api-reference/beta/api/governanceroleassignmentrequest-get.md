---
title: Получение governanceRoleAssignmentRequest
description: 'Получение governanceRoleAssignmentRequest. '
localization_priority: Normal
ms.openlocfilehash: 6914dbe8c45bcc05bc684b08fb5fdf87405a045a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503704"
---
# <a name="get-governanceroleassignmentrequest"></a><span data-ttu-id="30276-103">Получение governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="30276-103">Get governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30276-104">Получение [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="30276-104">Get a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="30276-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30276-105">Permissions</span></span>
<span data-ttu-id="30276-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30276-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30276-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30276-108">Permission type</span></span>      | <span data-ttu-id="30276-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30276-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30276-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30276-110">Delegated (work or school account)</span></span> | <span data-ttu-id="30276-111">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="30276-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="30276-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30276-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30276-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30276-113">Not supported.</span></span>    |
|<span data-ttu-id="30276-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30276-114">Application</span></span> | <span data-ttu-id="30276-115">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="30276-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="30276-116">Кроме области разрешений, для него требуется запрашивающий</span><span class="sxs-lookup"><span data-stu-id="30276-116">Besides the permission scope, it requires the requestor</span></span> 
*   <span data-ttu-id="30276-117">для ресурса по крайней мере одно назначение роли; также</span><span class="sxs-lookup"><span data-stu-id="30276-117">to have at least one role assignment on the resource; or</span></span>
*   <span data-ttu-id="30276-118">— Это тема [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="30276-118">is the subject of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="30276-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30276-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleAssignmentRequests/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="30276-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="30276-120">Optional query parameters</span></span>
<span data-ttu-id="30276-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="30276-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30276-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30276-122">Request headers</span></span>
| <span data-ttu-id="30276-123">Имя</span><span class="sxs-lookup"><span data-stu-id="30276-123">Name</span></span>      |<span data-ttu-id="30276-124">Описание</span><span class="sxs-lookup"><span data-stu-id="30276-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="30276-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30276-125">Authorization</span></span>  | <span data-ttu-id="30276-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="30276-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="30276-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30276-127">Request body</span></span>
<span data-ttu-id="30276-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="30276-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30276-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="30276-129">Response</span></span>
<span data-ttu-id="30276-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="30276-130">If successful, this method returns a `200 OK` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30276-131">Пример</span><span class="sxs-lookup"><span data-stu-id="30276-131">Example</span></span>
<span data-ttu-id="30276-132">Получение запроса на назначение роли</span><span class="sxs-lookup"><span data-stu-id="30276-132">Get a role assignment request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequest"
}-->
##### <a name="request"></a><span data-ttu-id="30276-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="30276-133">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/e68ff888-4af5-4ccb-8b74-39156090344b
```
##### <a name="response"></a><span data-ttu-id="30276-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="30276-134">Response</span></span>
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
