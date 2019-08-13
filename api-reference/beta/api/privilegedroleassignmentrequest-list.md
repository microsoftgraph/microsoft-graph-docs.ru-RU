---
title: Список Привилежедролеассигнментрекуестс
description: 'Получение коллекции Привилежедролеассигнментрекуест. '
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: ff6b9f2f9ba16002382661bf810f9c8ba657c8a8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361016"
---
# <a name="list-privilegedroleassignmentrequests"></a><span data-ttu-id="28d0b-103">Список Привилежедролеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="28d0b-103">List privilegedRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28d0b-104">Получение коллекции [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="28d0b-104">Retrieve a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span> 

<span data-ttu-id="28d0b-105">**Примечание:** Этот запрашивающий должно иметь по крайней мере одно назначение роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="28d0b-105">**Note:** This requester must have at least one role assignment on the resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="28d0b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28d0b-106">Permissions</span></span>
<span data-ttu-id="28d0b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28d0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28d0b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28d0b-109">Permission type</span></span>                        | <span data-ttu-id="28d0b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28d0b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="28d0b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28d0b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="28d0b-112">Привилежедакцесс. ReadWrite. AzureAD, Directory. Read. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="28d0b-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="28d0b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28d0b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28d0b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28d0b-114">Not supported.</span></span> |
|<span data-ttu-id="28d0b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28d0b-115">Application</span></span>                            | <span data-ttu-id="28d0b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28d0b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="28d0b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28d0b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="28d0b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="28d0b-118">Optional query parameters</span></span>
<span data-ttu-id="28d0b-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="28d0b-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28d0b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28d0b-120">Request headers</span></span>
| <span data-ttu-id="28d0b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="28d0b-121">Name</span></span>      |<span data-ttu-id="28d0b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="28d0b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="28d0b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28d0b-123">Authorization</span></span>  | <span data-ttu-id="28d0b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28d0b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28d0b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="28d0b-126">Request body</span></span>
<span data-ttu-id="28d0b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="28d0b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28d0b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="28d0b-128">Response</span></span>
<span data-ttu-id="28d0b-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="28d0b-129">If successful, this method returns a `200 OK` response code and a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28d0b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="28d0b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28d0b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="28d0b-131">Request</span></span>
<span data-ttu-id="28d0b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28d0b-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="28d0b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="28d0b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignmentrequest"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="28d0b-134">C#</span><span class="sxs-lookup"><span data-stu-id="28d0b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="28d0b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28d0b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="28d0b-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="28d0b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="28d0b-137">Java</span><span class="sxs-lookup"><span data-stu-id="28d0b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="28d0b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="28d0b-138">Response</span></span>
<span data-ttu-id="28d0b-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="28d0b-139">The following is an example of the response.</span></span> <span data-ttu-id="28d0b-140">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="28d0b-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="28d0b-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28d0b-141">All of the properties will be returned from an actual call.</span></span>
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
      },"id":"03ea0c3d-90a0-42d4-b220-11c049c506fb","userId": "Self","roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b","evaluateOnly":false,"type":"UserAdd","assignmentState":"Active","requestedDateTime":"2018-02-07T22:17:37.2215343Z","status":"ApprovalAborted","duration":"1","reason":"Activate for testing","ticketNumber":"222","ticketSystem":"222"
    },{
      "schedule":{
        "type":"assignment","startDateTime":"2018-01-23T02:43:15.258242Z","endDateTime":null,"duration" : null
      },"id":"fe4450bb-6d28-4583-8fc4-25b0ea91daf5","userId": "Self","roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b","evaluateOnly":false,"type":"UserAdd","assignmentState":"Active","requestedDateTime":"2018-01-23T02:42:55.628338Z","status":"Completed","duration":"1","reason":"asdf","ticketNumber":null,"ticketSystem":null
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
