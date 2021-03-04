---
title: 'privilegedRoleAssignmentRequest: my'
description: Получите запросы на присвоение привилегированных ролей запрашиваемой запрашиваемой роли.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: b17b33ab069342dfabd5488bc295c9fd8ace1fb9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441160"
---
# <a name="privilegedroleassignmentrequest-my"></a><span data-ttu-id="a3aa7-103">privilegedRoleAssignmentRequest: my</span><span class="sxs-lookup"><span data-stu-id="a3aa7-103">privilegedRoleAssignmentRequest: my</span></span>

<span data-ttu-id="a3aa7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3aa7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3aa7-105">Получите запросы на присвоение привилегированных ролей запрашиваемой запрашиваемой роли.</span><span class="sxs-lookup"><span data-stu-id="a3aa7-105">Get the requester's privileged role assignment requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3aa7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a3aa7-106">Permissions</span></span>
<span data-ttu-id="a3aa7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3aa7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3aa7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3aa7-109">Permission type</span></span>                        | <span data-ttu-id="a3aa7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3aa7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3aa7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3aa7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a3aa7-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a3aa7-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a3aa7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3aa7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3aa7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3aa7-114">Not supported.</span></span> |
|<span data-ttu-id="a3aa7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3aa7-115">Application</span></span>                            | <span data-ttu-id="a3aa7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3aa7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3aa7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3aa7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests/my
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a3aa7-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a3aa7-118">Optional query parameters</span></span>
<span data-ttu-id="a3aa7-119">Этот метод поддерживает [параметры запросов OData](http://graph.microsoft.io/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a3aa7-119">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3aa7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3aa7-120">Request headers</span></span>
| <span data-ttu-id="a3aa7-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a3aa7-121">Name</span></span>      |<span data-ttu-id="a3aa7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a3aa7-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a3aa7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a3aa7-123">Authorization</span></span>  | <span data-ttu-id="a3aa7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3aa7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3aa7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a3aa7-126">Request body</span></span>
<span data-ttu-id="a3aa7-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a3aa7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3aa7-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3aa7-128">Response</span></span>
<span data-ttu-id="a3aa7-129">В случае успешного выполнения этот метод возвращает код ответа и объект `200 OK` [коллекции privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a3aa7-129">If successful, this method returns `200 OK` response code and [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3aa7-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a3aa7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3aa7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3aa7-131">Request</span></span>
<span data-ttu-id="a3aa7-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3aa7-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a3aa7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3aa7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignmentrequest_my)"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/my
```
# <a name="c"></a>[<span data-ttu-id="a3aa7-134">C#</span><span class="sxs-lookup"><span data-stu-id="a3aa7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignmentrequest-my-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3aa7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3aa7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignmentrequest-my-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3aa7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3aa7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignmentrequest-my-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3aa7-137">Java</span><span class="sxs-lookup"><span data-stu-id="a3aa7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedroleassignmentrequest-my-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a3aa7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3aa7-138">Response</span></span>
<span data-ttu-id="a3aa7-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a3aa7-139">The following is an example of the response.</span></span> <span data-ttu-id="a3aa7-140">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="a3aa7-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a3aa7-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a3aa7-141">All of the properties will be returned from an actual call.</span></span>
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


