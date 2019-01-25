---
title: Получение governanceRoleAssignment
description: Извлечение свойств и отношения governanceRoleAssignment.
localization_priority: Normal
ms.openlocfilehash: f699e1b5332652b2b87f3972d2ae47b06894b2e4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508841"
---
# <a name="get-governanceroleassignment"></a><span data-ttu-id="900a6-103">Получение governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="900a6-103">Get governanceRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="900a6-104">Извлечение свойств и отношения [governanceRoleAssignment](../resources/governanceroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="900a6-104">Retrieve the properties and relationships of a [governanceRoleAssignment](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="900a6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="900a6-105">Permissions</span></span>
<span data-ttu-id="900a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="900a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="900a6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="900a6-108">Permission type</span></span>      | <span data-ttu-id="900a6-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="900a6-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="900a6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="900a6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="900a6-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="900a6-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="900a6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="900a6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="900a6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="900a6-113">Not supported.</span></span>    |
|<span data-ttu-id="900a6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="900a6-114">Application</span></span> | <span data-ttu-id="900a6-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="900a6-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="900a6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="900a6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
1. <span data-ttu-id="900a6-117">Получение [governanceRoleAssignment](../resources/governanceroleassignment.md) на ресурс</span><span class="sxs-lookup"><span data-stu-id="900a6-117">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on a resource</span></span>

    <span data-ttu-id="900a6-118">*Примечание: Помимо области разрешений требуется инициатор запроса может иметь по крайней мере одна роль назначения для ресурса.*</span><span class="sxs-lookup"><span data-stu-id="900a6-118">*Note: Besides the permission scope, it requires the requestor to have at least one role assignment on the resource.*</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments/{id}
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=resourceId+eq+'{resourceId}'
```
2. <span data-ttu-id="900a6-119">Получение [governanceRoleAssignment](../resources/governanceroleassignment.md) Мой</span><span class="sxs-lookup"><span data-stu-id="900a6-119">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=subjectId+eq+'{myId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="900a6-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="900a6-120">Optional query parameters</span></span>
<span data-ttu-id="900a6-121">Этот метод **поддерживает [Параметры запроса OData](/graph/query-parameters) , отличный от** `$filter` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="900a6-121">This method does **not** supports [OData Query Parameters](/graph/query-parameters) other than `$filter` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="900a6-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="900a6-122">Request headers</span></span>
| <span data-ttu-id="900a6-123">Имя</span><span class="sxs-lookup"><span data-stu-id="900a6-123">Name</span></span>      |<span data-ttu-id="900a6-124">Описание</span><span class="sxs-lookup"><span data-stu-id="900a6-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="900a6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="900a6-125">Authorization</span></span>  | <span data-ttu-id="900a6-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="900a6-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="900a6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="900a6-127">Request body</span></span>
<span data-ttu-id="900a6-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="900a6-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="900a6-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="900a6-129">Response</span></span>
<span data-ttu-id="900a6-130">Успешно завершена, этот метод возвращает `200 OK` объект [governanceRoleAssignment](../resources/governanceroleassignment.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="900a6-130">If successful, this method returns a `200 OK` response code and [governanceRoleAssignment](../resources/governanceroleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="900a6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="900a6-131">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignment"
}-->
<span data-ttu-id="900a6-132">Получить [governanceRoleAssignment](../resources/governanceroleassignment.md) по подписке «Производственного – Wingtip Toys»</span><span class="sxs-lookup"><span data-stu-id="900a6-132">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on subscription "Wingtip Toys - Prod"</span></span>
##### <a name="request"></a><span data-ttu-id="900a6-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="900a6-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/0ba78f41-ee7a-4227-adb9-1499431b2164?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="900a6-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="900a6-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 182

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignments/$entity",
    "id": "0ba78f41-ee7a-4227-adb9-1499431b2164",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
    "subjectId": "74487eb5-1630-4fa8-9581-0bb076ea5de3",
    "linkedEligibleRoleAssignmentId": null,
    "externalId": null,
    "startDateTime": "2018-01-22T23:47:19.687Z",
    "endDateTime": "2018-07-21T23:47:02.887Z",
    "memberType": "Direct",
    "assignmentState": "Eligible",
    "status": "Provisioned"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignment-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
