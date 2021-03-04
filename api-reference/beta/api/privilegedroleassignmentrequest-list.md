---
title: Список привилегированныхRoleAssignmentRequests
description: 'Извлечение коллекции privilegedRoleAssignmentRequest. '
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 7df9eab695ae60884274a01487f87369751bfb19
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441179"
---
# <a name="list-privilegedroleassignmentrequests"></a><span data-ttu-id="e898d-103">Список привилегированныхRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="e898d-103">List privilegedRoleAssignmentRequests</span></span>

<span data-ttu-id="e898d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e898d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e898d-105">Извлечения коллекции [привилегированныхRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="e898d-105">Retrieve a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span> 

<span data-ttu-id="e898d-106">**Примечание:** Этот запрашиватель должен иметь как минимум одно назначение ролей на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="e898d-106">**Note:** This requester must have at least one role assignment on the resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="e898d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e898d-107">Permissions</span></span>
<span data-ttu-id="e898d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e898d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e898d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e898d-110">Permission type</span></span>                        | <span data-ttu-id="e898d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e898d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e898d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e898d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e898d-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e898d-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e898d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e898d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e898d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e898d-115">Not supported.</span></span> |
|<span data-ttu-id="e898d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e898d-116">Application</span></span>                            | <span data-ttu-id="e898d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e898d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e898d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e898d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e898d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e898d-119">Optional query parameters</span></span>
<span data-ttu-id="e898d-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e898d-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e898d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e898d-121">Request headers</span></span>
| <span data-ttu-id="e898d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="e898d-122">Name</span></span>      |<span data-ttu-id="e898d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e898d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e898d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e898d-124">Authorization</span></span>  | <span data-ttu-id="e898d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e898d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e898d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e898d-127">Request body</span></span>
<span data-ttu-id="e898d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e898d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e898d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e898d-129">Response</span></span>
<span data-ttu-id="e898d-130">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e898d-130">If successful, this method returns a `200 OK` response code and a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e898d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e898d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e898d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e898d-132">Request</span></span>
<span data-ttu-id="e898d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e898d-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e898d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e898d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignmentrequest"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
```
# <a name="c"></a>[<span data-ttu-id="e898d-135">C#</span><span class="sxs-lookup"><span data-stu-id="e898d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e898d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e898d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e898d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e898d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e898d-138">Java</span><span class="sxs-lookup"><span data-stu-id="e898d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e898d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="e898d-139">Response</span></span>
<span data-ttu-id="e898d-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e898d-140">The following is an example of the response.</span></span> <span data-ttu-id="e898d-141">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="e898d-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e898d-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e898d-142">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
  "@odata.context":"https://https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests",
  "value":[
    {
      "schedule":{
        "type":"activation","startDateTime":"2018-02-07T22:55:00Z","endDateTime":null,"duration" : null
      },"id":"03ea0c3d-90a0-42d4-b220-11c049c506fb","userId": "Self","roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b","type":"UserAdd","assignmentState":"Active","requestedDateTime":"2018-02-07T22:17:37.2215343Z","status":"ApprovalAborted","duration":"1","reason":"Activate for testing","ticketNumber":"222","ticketSystem":"222"
    },{
      "schedule":{
        "type":"assignment","startDateTime":"2018-01-23T02:43:15.258242Z","endDateTime":null,"duration" : null
      },"id":"fe4450bb-6d28-4583-8fc4-25b0ea91daf5","userId": "Self","roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b","type":"UserAdd","assignmentState":"Active","requestedDateTime":"2018-01-23T02:42:55.628338Z","status":"Completed","duration":"1","reason":"asdf","ticketNumber":null,"ticketSystem":null
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


