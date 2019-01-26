---
title: 'privilegedRoleAssignmentRequest: Мой'
description: Получите запросы назначений привилегированной роль инициатора.
localization_priority: Normal
ms.openlocfilehash: 2107256f9ead89950ba23bec49a81839347f7b7e
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577370"
---
# <a name="privilegedroleassignmentrequest-my"></a><span data-ttu-id="ec1be-103">privilegedRoleAssignmentRequest: Мой</span><span class="sxs-lookup"><span data-stu-id="ec1be-103">privilegedRoleAssignmentRequest: my</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec1be-104">Получите запросы назначений привилегированной роль инициатора.</span><span class="sxs-lookup"><span data-stu-id="ec1be-104">Get the requester's privileged role assignment requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec1be-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec1be-105">Permissions</span></span>
<span data-ttu-id="ec1be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec1be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec1be-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec1be-108">Permission type</span></span>                        | <span data-ttu-id="ec1be-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec1be-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec1be-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec1be-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ec1be-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ec1be-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ec1be-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec1be-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec1be-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec1be-113">Not supported.</span></span> |
|<span data-ttu-id="ec1be-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec1be-114">Application</span></span>                            | <span data-ttu-id="ec1be-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec1be-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec1be-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec1be-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests/my
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ec1be-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ec1be-117">Optional query parameters</span></span>
<span data-ttu-id="ec1be-118">Этот метод поддерживает [параметры запросов OData](http://graph.microsoft.io/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ec1be-118">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec1be-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec1be-119">Request headers</span></span>
| <span data-ttu-id="ec1be-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ec1be-120">Name</span></span>      |<span data-ttu-id="ec1be-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ec1be-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ec1be-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec1be-122">Authorization</span></span>  | <span data-ttu-id="ec1be-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec1be-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec1be-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec1be-125">Request body</span></span>
<span data-ttu-id="ec1be-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ec1be-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec1be-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec1be-127">Response</span></span>
<span data-ttu-id="ec1be-128">Успешно завершена, этот метод возвращает `200 OK` кода и [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) коллекции объект ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ec1be-128">If successful, this method returns `200 OK` response code and [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec1be-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ec1be-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec1be-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec1be-130">Request</span></span>
<span data-ttu-id="ec1be-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec1be-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignmentrequest_my"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/my
```

##### <a name="response"></a><span data-ttu-id="ec1be-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec1be-132">Response</span></span>
<span data-ttu-id="ec1be-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ec1be-133">The following is an example of the response.</span></span> <span data-ttu-id="ec1be-134">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="ec1be-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ec1be-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ec1be-135">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-my.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
