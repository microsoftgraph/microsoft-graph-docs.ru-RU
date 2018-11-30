---
title: Список governanceRoleAssignments
description: Получите коллекцию governanceRoleAssignments.
ms.openlocfilehash: 4b47756f75c7da1b0e9293eda449c5a244d015b6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075262"
---
# <a name="list-governanceroleassignments"></a><span data-ttu-id="373b4-103">Список governanceRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="373b4-103">List governanceRoleAssignments</span></span>

> <span data-ttu-id="373b4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="373b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="373b4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="373b4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="373b4-106">Получите коллекцию [governanceRoleAssignments](../resources/governanceroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="373b4-106">Retrieve a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="373b4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="373b4-107">Permissions</span></span>
<span data-ttu-id="373b4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="373b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="373b4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="373b4-110">Permission type</span></span>      | <span data-ttu-id="373b4-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="373b4-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="373b4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="373b4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="373b4-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="373b4-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="373b4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="373b4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="373b4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="373b4-115">Not supported.</span></span>    |
|<span data-ttu-id="373b4-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="373b4-116">Application</span></span> | <span data-ttu-id="373b4-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="373b4-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |


## <a name="http-request"></a><span data-ttu-id="373b4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="373b4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="373b4-119">Список коллекцию [governanceRoleAssignments](../resources/governanceroleassignment.md) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="373b4-119">List a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md) on a resource.</span></span>

><span data-ttu-id="373b4-120">**Примечание:** Помимо области разрешений для этого запроса требуется инициатор запроса может иметь по крайней мере одна роль назначения для ресурса.</span><span class="sxs-lookup"><span data-stu-id="373b4-120">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments
GET /privilegedAccess/azureResources/roleAssignments?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="373b4-121">Список коллекцию [governanceRoleAssignments](../resources/governanceroleassignment.md) моей.</span><span class="sxs-lookup"><span data-stu-id="373b4-121">List a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md) of mine.</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="373b4-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="373b4-122">Optional query parameters</span></span>
<span data-ttu-id="373b4-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="373b4-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="373b4-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="373b4-124">Request headers</span></span>
| <span data-ttu-id="373b4-125">Имя</span><span class="sxs-lookup"><span data-stu-id="373b4-125">Name</span></span>      |<span data-ttu-id="373b4-126">Описание</span><span class="sxs-lookup"><span data-stu-id="373b4-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="373b4-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="373b4-127">Authorization</span></span>  | <span data-ttu-id="373b4-128">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="373b4-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="373b4-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="373b4-129">Request body</span></span>
<span data-ttu-id="373b4-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="373b4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="373b4-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="373b4-131">Response</span></span>
<span data-ttu-id="373b4-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [governanceRoleAssignment](../resources/governanceroleassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="373b4-132">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignment](../resources/governanceroleassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="373b4-133">Пример</span><span class="sxs-lookup"><span data-stu-id="373b4-133">Example</span></span>

<span data-ttu-id="373b4-134">В этом примере показано, как получить Мои назначения ролей по подписке Wingtip Toys - производственного.</span><span class="sxs-lookup"><span data-stu-id="373b4-134">This example shows how to get my role assignments on the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignments"
}-->
##### <a name="request"></a><span data-ttu-id="373b4-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="373b4-135">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments?$filter=subjectId+eq+'918e54be-12c4-4f4c-a6d3-2ee0e3661c51'
```
##### <a name="response"></a><span data-ttu-id="373b4-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="373b4-136">Response</span></span>
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
            "isPermanent": false,
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
            "isPermanent": false,
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
<!-- {
  "type": "#page.annotation",
  "description": "List roleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
