---
title: Получение governanceRoleAssignment
description: Получение свойств и связей объекта governanceRoleAssignment.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 78042d16d736f644cddc70fe5665ef04defb01de
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42421160"
---
# <a name="get-governanceroleassignment"></a><span data-ttu-id="edbdc-103">Получение governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="edbdc-103">Get governanceRoleAssignment</span></span>

<span data-ttu-id="edbdc-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="edbdc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edbdc-105">Получение свойств и связей объекта [governanceRoleAssignment](../resources/governanceroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="edbdc-105">Retrieve the properties and relationships of a [governanceRoleAssignment](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="edbdc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="edbdc-106">Permissions</span></span>
<span data-ttu-id="edbdc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edbdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edbdc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="edbdc-109">Permission type</span></span>      | <span data-ttu-id="edbdc-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="edbdc-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="edbdc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="edbdc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="edbdc-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="edbdc-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="edbdc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="edbdc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="edbdc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edbdc-114">Not supported.</span></span>    |
|<span data-ttu-id="edbdc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="edbdc-115">Application</span></span> | <span data-ttu-id="edbdc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edbdc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="edbdc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="edbdc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
1. <span data-ttu-id="edbdc-118">Получение [governanceRoleAssignment](../resources/governanceroleassignment.md) для ресурса</span><span class="sxs-lookup"><span data-stu-id="edbdc-118">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on a resource</span></span>

    <span data-ttu-id="edbdc-119">*Примечание. Кроме области разрешений, необходимо, чтобы запрашивающий был иметь по крайней мере одно назначение роли для ресурса.*</span><span class="sxs-lookup"><span data-stu-id="edbdc-119">*Note: Besides the permission scope, it requires the requestor to have at least one role assignment on the resource.*</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments/{id}
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=resourceId+eq+'{resourceId}'
```
2. <span data-ttu-id="edbdc-120">Получение [governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="edbdc-120">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=subjectId+eq+'{myId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="edbdc-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="edbdc-121">Optional query parameters</span></span>
<span data-ttu-id="edbdc-122">Этот метод **не** поддерживает [параметры запросов OData](/graph/query-parameters) `$filter` , не позволяющие настраивать ответ.</span><span class="sxs-lookup"><span data-stu-id="edbdc-122">This method does **not** supports [OData Query Parameters](/graph/query-parameters) other than `$filter` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="edbdc-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="edbdc-123">Request headers</span></span>
| <span data-ttu-id="edbdc-124">Имя</span><span class="sxs-lookup"><span data-stu-id="edbdc-124">Name</span></span>      |<span data-ttu-id="edbdc-125">Описание</span><span class="sxs-lookup"><span data-stu-id="edbdc-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="edbdc-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="edbdc-126">Authorization</span></span>  | <span data-ttu-id="edbdc-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="edbdc-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="edbdc-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="edbdc-128">Request body</span></span>
<span data-ttu-id="edbdc-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="edbdc-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="edbdc-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="edbdc-130">Response</span></span>
<span data-ttu-id="edbdc-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [governanceRoleAssignment](../resources/governanceroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="edbdc-131">If successful, this method returns a `200 OK` response code and [governanceRoleAssignment](../resources/governanceroleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="edbdc-132">Пример</span><span class="sxs-lookup"><span data-stu-id="edbdc-132">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignment"
}-->
<span data-ttu-id="edbdc-133">Получение [governanceRoleAssignment](../resources/governanceroleassignment.md) по подписке "Wingtip Toys — произ"</span><span class="sxs-lookup"><span data-stu-id="edbdc-133">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on subscription "Wingtip Toys - Prod"</span></span>
##### <a name="request"></a><span data-ttu-id="edbdc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="edbdc-134">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/0ba78f41-ee7a-4227-adb9-1499431b2164?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="edbdc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="edbdc-135">Response</span></span>
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
  "suppressions": []
}
-->
