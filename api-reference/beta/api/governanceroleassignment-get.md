---
title: Получение governanceRoleAssignment
description: Получение свойств и связей объекта governanceRoleAssignment.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 80bf665931e31a86de973fdf22757b18a3489fdc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954209"
---
# <a name="get-governanceroleassignment"></a><span data-ttu-id="b7084-103">Получение governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="b7084-103">Get governanceRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7084-104">Получение свойств и связей объекта [governanceRoleAssignment](../resources/governanceroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b7084-104">Retrieve the properties and relationships of a [governanceRoleAssignment](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b7084-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7084-105">Permissions</span></span>
<span data-ttu-id="b7084-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7084-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7084-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7084-108">Permission type</span></span>      | <span data-ttu-id="b7084-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7084-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7084-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7084-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b7084-111">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="b7084-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="b7084-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7084-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7084-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7084-113">Not supported.</span></span>    |
|<span data-ttu-id="b7084-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7084-114">Application</span></span> | <span data-ttu-id="b7084-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7084-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7084-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7084-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
1. <span data-ttu-id="b7084-117">Получение [governanceRoleAssignment](../resources/governanceroleassignment.md) для ресурса</span><span class="sxs-lookup"><span data-stu-id="b7084-117">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on a resource</span></span>

    <span data-ttu-id="b7084-118">*Примечание. Кроме области разрешений, необходимо, чтобы запрашивающий был иметь по крайней мере одно назначение роли для ресурса.*</span><span class="sxs-lookup"><span data-stu-id="b7084-118">*Note: Besides the permission scope, it requires the requestor to have at least one role assignment on the resource.*</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments/{id}
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=resourceId+eq+'{resourceId}'
```
2. <span data-ttu-id="b7084-119">Получение [governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b7084-119">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=subjectId+eq+'{myId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b7084-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b7084-120">Optional query parameters</span></span>
<span data-ttu-id="b7084-121">Этот метод **не** поддерживает [параметры запросов OData](/graph/query-parameters) `$filter` , не позволяющие настраивать ответ.</span><span class="sxs-lookup"><span data-stu-id="b7084-121">This method does **not** supports [OData Query Parameters](/graph/query-parameters) other than `$filter` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7084-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7084-122">Request headers</span></span>
| <span data-ttu-id="b7084-123">Имя</span><span class="sxs-lookup"><span data-stu-id="b7084-123">Name</span></span>      |<span data-ttu-id="b7084-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b7084-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b7084-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7084-125">Authorization</span></span>  | <span data-ttu-id="b7084-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b7084-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7084-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7084-127">Request body</span></span>
<span data-ttu-id="b7084-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b7084-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b7084-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b7084-129">Response</span></span>
<span data-ttu-id="b7084-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [governanceRoleAssignment](../resources/governanceroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b7084-130">If successful, this method returns a `200 OK` response code and [governanceRoleAssignment](../resources/governanceroleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b7084-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b7084-131">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignment"
}-->
<span data-ttu-id="b7084-132">Получение [governanceRoleAssignment](../resources/governanceroleassignment.md) по подписке "Wingtip Toys — произ"</span><span class="sxs-lookup"><span data-stu-id="b7084-132">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on subscription "Wingtip Toys - Prod"</span></span>
##### <a name="request"></a><span data-ttu-id="b7084-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7084-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/0ba78f41-ee7a-4227-adb9-1499431b2164?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="b7084-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7084-134">Response</span></span>
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
