---
title: Список privilegedRoleAssignmentRequests
description: 'Получите коллекцию privilegedRoleAssignmentRequest. '
ms.openlocfilehash: c47ad101e4e4008985be6732f5f6358b705959b9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080169"
---
# <a name="list-privilegedroleassignmentrequests"></a><span data-ttu-id="fbd3a-103">Список privilegedRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="fbd3a-103">List privilegedRoleAssignmentRequests</span></span>

> <span data-ttu-id="fbd3a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fbd3a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fbd3a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbd3a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fbd3a-106">Получите коллекцию [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="fbd3a-106">Retrieve a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span> 

<span data-ttu-id="fbd3a-107">**Примечание:** В этом инициатор запроса должна иметь по крайней мере одно назначение роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="fbd3a-107">**Note:** This requester must have at least one role assignment on the resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="fbd3a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fbd3a-108">Permissions</span></span>
<span data-ttu-id="fbd3a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbd3a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbd3a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fbd3a-111">Permission type</span></span>                        | <span data-ttu-id="fbd3a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fbd3a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbd3a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fbd3a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fbd3a-114">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fbd3a-114">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fbd3a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fbd3a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbd3a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbd3a-116">Not supported.</span></span> |
|<span data-ttu-id="fbd3a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fbd3a-117">Application</span></span>                            | <span data-ttu-id="fbd3a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbd3a-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fbd3a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fbd3a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fbd3a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fbd3a-120">Optional query parameters</span></span>
<span data-ttu-id="fbd3a-121">Этот метод поддерживает [Параметры запроса OData](/graph/query-parameters) , которые помогут при настройке клиентов ответа.</span><span class="sxs-lookup"><span data-stu-id="fbd3a-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fbd3a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fbd3a-122">Request headers</span></span>
| <span data-ttu-id="fbd3a-123">Имя</span><span class="sxs-lookup"><span data-stu-id="fbd3a-123">Name</span></span>      |<span data-ttu-id="fbd3a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="fbd3a-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fbd3a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fbd3a-125">Authorization</span></span>  | <span data-ttu-id="fbd3a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbd3a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fbd3a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fbd3a-128">Request body</span></span>
<span data-ttu-id="fbd3a-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fbd3a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbd3a-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="fbd3a-130">Response</span></span>
<span data-ttu-id="fbd3a-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fbd3a-131">If successful, this method returns a `200 OK` response code and a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbd3a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="fbd3a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fbd3a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbd3a-133">Request</span></span>
<span data-ttu-id="fbd3a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbd3a-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignmentrequest"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
```
##### <a name="response"></a><span data-ttu-id="fbd3a-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="fbd3a-135">Response</span></span>
<span data-ttu-id="fbd3a-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fbd3a-136">The following is an example of the response.</span></span> <span data-ttu-id="fbd3a-137">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="fbd3a-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fbd3a-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fbd3a-138">All of the properties will be returned from an actual call.</span></span>
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
      },"id":"03ea0c3d-90a0-42d4-b220-11c049c506fb","userId": "Self"，"roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b","evaluateOnly":false,"type":"UserAdd","assignmentState":"Active","requestedDateTime":"2018-02-07T22:17:37.2215343Z","status":"ApprovalAborted","duration":"1","reason":"Activate for testing","ticketNumber":"222","ticketSystem":"222"
    },{
      "schedule":{
        "type":"assignment","startDateTime":"2018-01-23T02:43:15.258242Z","endDateTime":null,"duration" : null
      },"id":"fe4450bb-6d28-4583-8fc4-25b0ea91daf5","userId": "Self"，"roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b","evaluateOnly":false,"type":"UserAdd","assignmentState":"Active","requestedDateTime":"2018-01-23T02:42:55.628338Z","status":"Completed","duration":"1","reason":"asdf","ticketNumber":null,"ticketSystem":null
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
