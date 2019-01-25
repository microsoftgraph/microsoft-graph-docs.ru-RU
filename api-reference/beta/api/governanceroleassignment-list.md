---
title: Список governanceRoleAssignments
description: Получите коллекцию governanceRoleAssignments.
localization_priority: Normal
ms.openlocfilehash: b6b83397d93ab502758202c7f22513d97db37540
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524872"
---
# <a name="list-governanceroleassignments"></a><span data-ttu-id="9a5de-103">Список governanceRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="9a5de-103">List governanceRoleAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a5de-104">Получите коллекцию [governanceRoleAssignments](../resources/governanceroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9a5de-104">Retrieve a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9a5de-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a5de-105">Permissions</span></span>
<span data-ttu-id="9a5de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a5de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a5de-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a5de-108">Permission type</span></span>      | <span data-ttu-id="9a5de-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a5de-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a5de-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a5de-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9a5de-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="9a5de-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="9a5de-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a5de-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a5de-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a5de-113">Not supported.</span></span>    |
|<span data-ttu-id="9a5de-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a5de-114">Application</span></span> | <span data-ttu-id="9a5de-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="9a5de-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |


## <a name="http-request"></a><span data-ttu-id="9a5de-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a5de-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="9a5de-117">Список коллекцию [governanceRoleAssignments](../resources/governanceroleassignment.md) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="9a5de-117">List a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md) on a resource.</span></span>

><span data-ttu-id="9a5de-118">**Примечание:** Помимо области разрешений для этого запроса требуется инициатор запроса может иметь по крайней мере одна роль назначения для ресурса.</span><span class="sxs-lookup"><span data-stu-id="9a5de-118">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments
GET /privilegedAccess/azureResources/roleAssignments?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="9a5de-119">Список коллекцию [governanceRoleAssignments](../resources/governanceroleassignment.md) моей.</span><span class="sxs-lookup"><span data-stu-id="9a5de-119">List a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md) of mine.</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9a5de-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9a5de-120">Optional query parameters</span></span>
<span data-ttu-id="9a5de-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9a5de-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a5de-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a5de-122">Request headers</span></span>
| <span data-ttu-id="9a5de-123">Имя</span><span class="sxs-lookup"><span data-stu-id="9a5de-123">Name</span></span>      |<span data-ttu-id="9a5de-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9a5de-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9a5de-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a5de-125">Authorization</span></span>  | <span data-ttu-id="9a5de-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9a5de-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a5de-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9a5de-127">Request body</span></span>
<span data-ttu-id="9a5de-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9a5de-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a5de-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="9a5de-129">Response</span></span>
<span data-ttu-id="9a5de-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [governanceRoleAssignment](../resources/governanceroleassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9a5de-130">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignment](../resources/governanceroleassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9a5de-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9a5de-131">Example</span></span>

<span data-ttu-id="9a5de-132">В этом примере показано, как получить Мои назначения ролей по подписке Wingtip Toys - производственного.</span><span class="sxs-lookup"><span data-stu-id="9a5de-132">This example shows how to get my role assignments on the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignments"
}-->
##### <a name="request"></a><span data-ttu-id="9a5de-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a5de-133">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments?$filter=subjectId+eq+'918e54be-12c4-4f4c-a6d3-2ee0e3661c51'
```
##### <a name="response"></a><span data-ttu-id="9a5de-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="9a5de-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 2062

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignments",
    "value": [
        {
            "id": "20f4157d-5837-4356-9630-ebd3a832f227",
            "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
            "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": null,
            "externalId": null,
            "startDateTime": "2018-03-13T01:19:08.59Z",
            "endDateTime": "2018-06-11T01:18:37.08Z",
            "memberType": "Direct",
            "assignmentState": "Eligible",
            "status": "Provisioned"
        },
        {
            "id": "e327f4be-42a0-47a2-8579-0a39b025b394",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": null,
            "externalId": null,
            "startDateTime": "2018-03-28T16:56:48.243Z",
            "endDateTime": "2018-09-24T16:56:30.547Z",
            "memberType": "Direct",
            "assignmentState": "Eligible",
            "status": "Provisioned"
        },
        ...
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List roleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignment-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
