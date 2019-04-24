---
title: Список Говернанцеролеассигнментс
description: Получение коллекции Говернанцеролеассигнментс.
localization_priority: Normal
ms.openlocfilehash: b6b83397d93ab502758202c7f22513d97db37540
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465266"
---
# <a name="list-governanceroleassignments"></a><span data-ttu-id="297b3-103">Список Говернанцеролеассигнментс</span><span class="sxs-lookup"><span data-stu-id="297b3-103">List governanceRoleAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="297b3-104">Получение коллекции [говернанцеролеассигнментс](../resources/governanceroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="297b3-104">Retrieve a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="297b3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="297b3-105">Permissions</span></span>
<span data-ttu-id="297b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="297b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="297b3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="297b3-108">Permission type</span></span>      | <span data-ttu-id="297b3-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="297b3-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="297b3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="297b3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="297b3-111">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="297b3-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="297b3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="297b3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="297b3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="297b3-113">Not supported.</span></span>    |
|<span data-ttu-id="297b3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="297b3-114">Application</span></span> | <span data-ttu-id="297b3-115">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="297b3-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |


## <a name="http-request"></a><span data-ttu-id="297b3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="297b3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="297b3-117">ПереЧисление коллекции [говернанцеролеассигнментс](../resources/governanceroleassignment.md) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="297b3-117">List a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md) on a resource.</span></span>

><span data-ttu-id="297b3-118">**Примечание:** Кроме области разрешений, этот запрос требует, чтобы запрашивающая сторона состроила по крайней мере одно назначение роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="297b3-118">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments
GET /privilegedAccess/azureResources/roleAssignments?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="297b3-119">ПереЧисление коллекции [говернанцеролеассигнментс](../resources/governanceroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="297b3-119">List a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md) of mine.</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="297b3-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="297b3-120">Optional query parameters</span></span>
<span data-ttu-id="297b3-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="297b3-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="297b3-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="297b3-122">Request headers</span></span>
| <span data-ttu-id="297b3-123">Имя</span><span class="sxs-lookup"><span data-stu-id="297b3-123">Name</span></span>      |<span data-ttu-id="297b3-124">Описание</span><span class="sxs-lookup"><span data-stu-id="297b3-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="297b3-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="297b3-125">Authorization</span></span>  | <span data-ttu-id="297b3-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="297b3-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="297b3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="297b3-127">Request body</span></span>
<span data-ttu-id="297b3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="297b3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="297b3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="297b3-129">Response</span></span>
<span data-ttu-id="297b3-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [governanceRoleAssignment](../resources/governanceroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="297b3-130">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignment](../resources/governanceroleassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="297b3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="297b3-131">Example</span></span>

<span data-ttu-id="297b3-132">В этом примере показано, как получить назначения ролей для подписки Wingtip Toys — произ.</span><span class="sxs-lookup"><span data-stu-id="297b3-132">This example shows how to get my role assignments on the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignments"
}-->
##### <a name="request"></a><span data-ttu-id="297b3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="297b3-133">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments?$filter=subjectId+eq+'918e54be-12c4-4f4c-a6d3-2ee0e3661c51'
```
##### <a name="response"></a><span data-ttu-id="297b3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="297b3-134">Response</span></span>
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
