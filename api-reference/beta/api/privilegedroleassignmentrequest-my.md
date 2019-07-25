---
title: 'Привилежедролеассигнментрекуест: My'
description: Получение запросов на назначение привилегированных ролей инициатора запроса.
localization_priority: Normal
ms.openlocfilehash: 669a3bca407e7cd5744a9a7f38031ff02abd48da
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875571"
---
# <a name="privilegedroleassignmentrequest-my"></a><span data-ttu-id="48930-103">Привилежедролеассигнментрекуест: My</span><span class="sxs-lookup"><span data-stu-id="48930-103">privilegedRoleAssignmentRequest: my</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48930-104">Получение запросов на назначение привилегированных ролей инициатора запроса.</span><span class="sxs-lookup"><span data-stu-id="48930-104">Get the requester's privileged role assignment requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="48930-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48930-105">Permissions</span></span>
<span data-ttu-id="48930-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48930-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48930-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48930-108">Permission type</span></span>                        | <span data-ttu-id="48930-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48930-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="48930-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48930-110">Delegated (work or school account)</span></span> | <span data-ttu-id="48930-111">Привилежедакцесс. ReadWrite. AzureAD, Directory. Read. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="48930-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="48930-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48930-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48930-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48930-113">Not supported.</span></span> |
|<span data-ttu-id="48930-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48930-114">Application</span></span>                            | <span data-ttu-id="48930-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48930-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="48930-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48930-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests/my
```
## <a name="optional-query-parameters"></a><span data-ttu-id="48930-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="48930-117">Optional query parameters</span></span>
<span data-ttu-id="48930-118">Этот метод поддерживает [параметры запросов OData](http://graph.microsoft.io/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="48930-118">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="48930-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48930-119">Request headers</span></span>
| <span data-ttu-id="48930-120">Имя</span><span class="sxs-lookup"><span data-stu-id="48930-120">Name</span></span>      |<span data-ttu-id="48930-121">Описание</span><span class="sxs-lookup"><span data-stu-id="48930-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="48930-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48930-122">Authorization</span></span>  | <span data-ttu-id="48930-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48930-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48930-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="48930-125">Request body</span></span>
<span data-ttu-id="48930-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="48930-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48930-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="48930-127">Response</span></span>
<span data-ttu-id="48930-128">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект коллекции [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="48930-128">If successful, this method returns `200 OK` response code and [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48930-129">Пример</span><span class="sxs-lookup"><span data-stu-id="48930-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48930-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="48930-130">Request</span></span>
<span data-ttu-id="48930-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48930-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="48930-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="48930-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignmentrequest_my)"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/my
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="48930-133">C#</span><span class="sxs-lookup"><span data-stu-id="48930-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignmentrequest-my-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="48930-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="48930-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignmentrequest-my-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="48930-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="48930-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignmentrequest-my-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="48930-136">Java</span><span class="sxs-lookup"><span data-stu-id="48930-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedroleassignmentrequest-my-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="48930-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="48930-137">Response</span></span>
<span data-ttu-id="48930-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="48930-138">The following is an example of the response.</span></span> <span data-ttu-id="48930-139">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="48930-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="48930-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48930-140">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests",
    "@odata.count": 4,
    "value": [{
        "schedule": {
            "type": "activation",
            "startDateTime": "2018-02-08T02:35:17.903Z",
            "endDateTime": null,
            "duration" : null
        },
        "id": "e13ef8a0-c1cb-4d03-aaae-9cd1c8ede2d1",
         "userId": "Self",
         "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
        "evaluateOnly": false,
        "type": "UserAdd",
        "assignmentState": "Active",
        "requestedDateTime": "2018-02-08T02:35:42.9137335Z",
        "status": "RequestedApproval",
        "duration": "2",
        "reason": "Activate the role for business purpose",
        "ticketNumber": "234",
        "ticketSystem": "system",
        "roleInfo@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests('e13ef8a0-c1cb-4d03-aaae-9cd1c8ede2d1')/roleInfo/$entity",
        "roleInfo": {
            "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
            "name": "Directory Readers"
        }
    }, {
        "schedule": {
            "type": "activation",
            "startDateTime": "2018-02-07T22:55:00Z",
            "endDateTime": null,
            "duration" : null
        },
        "id": "03ea0c3d-90a0-42d4-b220-11c049c506fb",
        "userId": "Self",
        "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
        "evaluateOnly": false,
        "type": "UserAdd",
        "assignmentState": "Active",
        "requestedDateTime": "2018-02-07T22:17:37.2215343Z",
        "status": "ApprovalAborted",
        "duration": "1",
        "reason": "Activate for testing",
        "ticketNumber": "222",
        "ticketSystem": "222",
        "roleInfo@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests('03ea0c3d-90a0-42d4-b220-11c049c506fb')/roleInfo/$entity",
        "roleInfo": {
            "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
            "name": "Directory Readers"
        }
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest: my",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
