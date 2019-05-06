---
title: Список Привилежедролеассигнментрекуестс
description: 'Получение коллекции Привилежедролеассигнментрекуест. '
localization_priority: Normal
ms.openlocfilehash: 887eeda1c357e31ffa56be0e2e0f9d5f5de041df
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593790"
---
# <a name="list-privilegedroleassignmentrequests"></a><span data-ttu-id="0e208-103">Список Привилежедролеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="0e208-103">List privilegedRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e208-104">Получение коллекции [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="0e208-104">Retrieve a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span> 

<span data-ttu-id="0e208-105">**Примечание:** Этот запрашивающий должно иметь по крайней мере одно назначение роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="0e208-105">**Note:** This requester must have at least one role assignment on the resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e208-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0e208-106">Permissions</span></span>
<span data-ttu-id="0e208-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e208-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e208-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e208-109">Permission type</span></span>                        | <span data-ttu-id="0e208-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e208-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e208-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e208-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0e208-112">Привилежедакцесс. ReadWrite. AzureAD, Directory. Read. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="0e208-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0e208-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e208-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e208-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e208-114">Not supported.</span></span> |
|<span data-ttu-id="0e208-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e208-115">Application</span></span>                            | <span data-ttu-id="0e208-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e208-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e208-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e208-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0e208-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0e208-118">Optional query parameters</span></span>
<span data-ttu-id="0e208-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0e208-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e208-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e208-120">Request headers</span></span>
| <span data-ttu-id="0e208-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0e208-121">Name</span></span>      |<span data-ttu-id="0e208-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0e208-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0e208-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e208-123">Authorization</span></span>  | <span data-ttu-id="0e208-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e208-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e208-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e208-126">Request body</span></span>
<span data-ttu-id="0e208-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0e208-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e208-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="0e208-128">Response</span></span>
<span data-ttu-id="0e208-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0e208-129">If successful, this method returns a `200 OK` response code and a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e208-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0e208-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e208-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e208-131">Request</span></span>
<span data-ttu-id="0e208-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e208-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignmentrequest"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
```
##### <a name="response"></a><span data-ttu-id="0e208-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e208-133">Response</span></span>
<span data-ttu-id="0e208-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0e208-134">The following is an example of the response.</span></span> <span data-ttu-id="0e208-135">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="0e208-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0e208-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0e208-136">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0e208-137">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="0e208-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0e208-138">Языках</span><span class="sxs-lookup"><span data-stu-id="0e208-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_privilegedroleassignmentrequest-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0e208-139">Язык</span><span class="sxs-lookup"><span data-stu-id="0e208-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_privilegedroleassignmentrequest-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
