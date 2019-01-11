---
title: Получение governanceRoleAssignment
description: Извлечение свойств и отношения governanceRoleAssignment.
localization_priority: Normal
ms.openlocfilehash: 838c096ccb8b719d9a07741aa80f3e132071a0c9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887572"
---
# <a name="get-governanceroleassignment"></a><span data-ttu-id="93f6a-103">Получение governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="93f6a-103">Get governanceRoleAssignment</span></span>

> <span data-ttu-id="93f6a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="93f6a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93f6a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93f6a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="93f6a-106">Извлечение свойств и отношения [governanceRoleAssignment](../resources/governanceroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="93f6a-106">Retrieve the properties and relationships of a [governanceRoleAssignment](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="93f6a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93f6a-107">Permissions</span></span>
<span data-ttu-id="93f6a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93f6a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93f6a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93f6a-110">Permission type</span></span>      | <span data-ttu-id="93f6a-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="93f6a-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93f6a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93f6a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="93f6a-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="93f6a-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="93f6a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93f6a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93f6a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93f6a-115">Not supported.</span></span>    |
|<span data-ttu-id="93f6a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93f6a-116">Application</span></span> | <span data-ttu-id="93f6a-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="93f6a-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="93f6a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93f6a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
1. <span data-ttu-id="93f6a-119">Получение [governanceRoleAssignment](../resources/governanceroleassignment.md) на ресурс</span><span class="sxs-lookup"><span data-stu-id="93f6a-119">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on a resource</span></span>

    <span data-ttu-id="93f6a-120">*Примечание: Помимо области разрешений требуется инициатор запроса может иметь по крайней мере одна роль назначения для ресурса.*</span><span class="sxs-lookup"><span data-stu-id="93f6a-120">*Note: Besides the permission scope, it requires the requestor to have at least one role assignment on the resource.*</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments/{id}
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=resourceId+eq+'{resourceId}'
```
2. <span data-ttu-id="93f6a-121">Получение [governanceRoleAssignment](../resources/governanceroleassignment.md) Мой</span><span class="sxs-lookup"><span data-stu-id="93f6a-121">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=subjectId+eq+'{myId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="93f6a-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="93f6a-122">Optional query parameters</span></span>
<span data-ttu-id="93f6a-123">Этот метод **поддерживает [Параметры запроса OData](/graph/query-parameters) , отличный от** `$filter` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="93f6a-123">This method does **not** supports [OData Query Parameters](/graph/query-parameters) other than `$filter` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93f6a-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93f6a-124">Request headers</span></span>
| <span data-ttu-id="93f6a-125">Имя</span><span class="sxs-lookup"><span data-stu-id="93f6a-125">Name</span></span>      |<span data-ttu-id="93f6a-126">Описание</span><span class="sxs-lookup"><span data-stu-id="93f6a-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="93f6a-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="93f6a-127">Authorization</span></span>  | <span data-ttu-id="93f6a-128">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="93f6a-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="93f6a-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="93f6a-129">Request body</span></span>
<span data-ttu-id="93f6a-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="93f6a-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="93f6a-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="93f6a-131">Response</span></span>
<span data-ttu-id="93f6a-132">Успешно завершена, этот метод возвращает `200 OK` объект [governanceRoleAssignment](../resources/governanceroleassignment.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="93f6a-132">If successful, this method returns a `200 OK` response code and [governanceRoleAssignment](../resources/governanceroleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="93f6a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="93f6a-133">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignment"
}-->
<span data-ttu-id="93f6a-134">Получить [governanceRoleAssignment](../resources/governanceroleassignment.md) по подписке «Производственного – Wingtip Toys»</span><span class="sxs-lookup"><span data-stu-id="93f6a-134">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on subscription "Wingtip Toys - Prod"</span></span>
##### <a name="request"></a><span data-ttu-id="93f6a-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="93f6a-135">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/0ba78f41-ee7a-4227-adb9-1499431b2164?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="93f6a-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="93f6a-136">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
