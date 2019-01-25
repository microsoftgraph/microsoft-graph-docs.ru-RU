---
title: Список privilegedRoleAssignmentRequests
description: 'Получите коллекцию privilegedRoleAssignmentRequest. '
localization_priority: Normal
ms.openlocfilehash: 06a6c66bcb566df0b6db5193bd753832bd9235a3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519985"
---
# <a name="list-privilegedroleassignmentrequests"></a><span data-ttu-id="a3afb-103">Список privilegedRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="a3afb-103">List privilegedRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3afb-104">Получите коллекцию [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="a3afb-104">Retrieve a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span> 

<span data-ttu-id="a3afb-105">**Примечание:** В этом инициатор запроса должна иметь по крайней мере одно назначение роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="a3afb-105">**Note:** This requester must have at least one role assignment on the resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3afb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a3afb-106">Permissions</span></span>
<span data-ttu-id="a3afb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3afb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3afb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3afb-109">Permission type</span></span>                        | <span data-ttu-id="a3afb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3afb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3afb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3afb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a3afb-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a3afb-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a3afb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3afb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3afb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3afb-114">Not supported.</span></span> |
|<span data-ttu-id="a3afb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3afb-115">Application</span></span>                            | <span data-ttu-id="a3afb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3afb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3afb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3afb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a3afb-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a3afb-118">Optional query parameters</span></span>
<span data-ttu-id="a3afb-119">Этот метод поддерживает [Параметры запроса OData](/graph/query-parameters) , которые помогут при настройке клиентов ответа.</span><span class="sxs-lookup"><span data-stu-id="a3afb-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3afb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3afb-120">Request headers</span></span>
| <span data-ttu-id="a3afb-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a3afb-121">Name</span></span>      |<span data-ttu-id="a3afb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a3afb-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a3afb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a3afb-123">Authorization</span></span>  | <span data-ttu-id="a3afb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3afb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3afb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3afb-126">Request body</span></span>
<span data-ttu-id="a3afb-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a3afb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3afb-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="a3afb-128">Response</span></span>
<span data-ttu-id="a3afb-129">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a3afb-129">If successful, this method returns a `200 OK` response code and a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3afb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a3afb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3afb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3afb-131">Request</span></span>
<span data-ttu-id="a3afb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3afb-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignmentrequest"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
```
##### <a name="response"></a><span data-ttu-id="a3afb-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="a3afb-133">Response</span></span>
<span data-ttu-id="a3afb-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a3afb-134">The following is an example of the response.</span></span> <span data-ttu-id="a3afb-135">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="a3afb-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a3afb-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a3afb-136">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
