---
title: Отменить privilegedRoleAssignmentRequest
description: Отмена privilegedRoleAssignmentRequest.
ms.openlocfilehash: 99c1102235e93ca365dcdd0e619bcceac9f396f1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079537"
---
# <a name="cancel-privilegedroleassignmentrequest"></a><span data-ttu-id="c8e7d-103">Отменить privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="c8e7d-103">Cancel privilegedRoleAssignmentRequest</span></span>

> <span data-ttu-id="c8e7d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c8e7d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8e7d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8e7d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c8e7d-106">Отмена [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="c8e7d-106">Cancel a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c8e7d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8e7d-107">Permissions</span></span>
<span data-ttu-id="c8e7d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8e7d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8e7d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8e7d-110">Permission type</span></span>                        | <span data-ttu-id="c8e7d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8e7d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8e7d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8e7d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c8e7d-113">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c8e7d-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c8e7d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8e7d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8e7d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8e7d-115">Not supported.</span></span> |
|<span data-ttu-id="c8e7d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8e7d-116">Application</span></span>                            | <span data-ttu-id="c8e7d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8e7d-117">Not supported.</span></span> |


### <a name="http-request"></a><span data-ttu-id="c8e7d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8e7d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests({requestid})/cancel
```

## <a name="request-headers"></a><span data-ttu-id="c8e7d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8e7d-119">Request headers</span></span>
| <span data-ttu-id="c8e7d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c8e7d-120">Name</span></span>      |<span data-ttu-id="c8e7d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c8e7d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c8e7d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8e7d-122">Authorization</span></span>  | <span data-ttu-id="c8e7d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8e7d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8e7d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8e7d-125">Request body</span></span>
<span data-ttu-id="c8e7d-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c8e7d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8e7d-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8e7d-127">Response</span></span>
<span data-ttu-id="c8e7d-128">В случае успешного выполнения этот метод возвращает код отклика `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="c8e7d-128">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="c8e7d-129">Возвращает [privilegedRoleAssignmentRequest] (.. / resources/privilegedRoleAssignmentRequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c8e7d-129">It returns [privilegedRoleAssignmentRequest] (../resources/privilegedRoleAssignmentRequest.md) in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="c8e7d-130">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="c8e7d-130">Error codes</span></span>
<span data-ttu-id="c8e7d-131">Этот интерфейс API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="c8e7d-131">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="c8e7d-132">Кроме того он возвращает коды пользовательских ошибок, перечисленных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="c8e7d-132">In addition, it returns the custom error codes listed in the following table.</span></span>

|<span data-ttu-id="c8e7d-133">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="c8e7d-133">Error code</span></span>     | <span data-ttu-id="c8e7d-134">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="c8e7d-134">Error message</span></span>              |
|:--------------------| :---------------------|
| <span data-ttu-id="c8e7d-135">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c8e7d-135">400 BadRequest</span></span> | <span data-ttu-id="c8e7d-136">RequestId не может быть Null.</span><span class="sxs-lookup"><span data-stu-id="c8e7d-136">RequestId cannot be Null.</span></span> |
| <span data-ttu-id="c8e7d-137">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c8e7d-137">400 BadRequest</span></span> | <span data-ttu-id="c8e7d-138">Запрос с Идентификатором запроса не найден.</span><span class="sxs-lookup"><span data-stu-id="c8e7d-138">Request with request ID not found.</span></span> |
| <span data-ttu-id="c8e7d-139">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c8e7d-139">400 BadRequest</span></span> | <span data-ttu-id="c8e7d-140">Отмены можно выполнить только на состояние расписанию и ожидает утверждения.</span><span class="sxs-lookup"><span data-stu-id="c8e7d-140">Cancellation can be done only on status Scheduled and PendingApproval.</span></span> |
| <span data-ttu-id="c8e7d-141">403 доступ запрещен</span><span class="sxs-lookup"><span data-stu-id="c8e7d-141">403 UnAuthorized</span></span> | <span data-ttu-id="c8e7d-142">Автор запроса не может совершать вызов отмены или запрос не найден.</span><span class="sxs-lookup"><span data-stu-id="c8e7d-142">Requester not allowed to make Cancel call or request not found.</span></span> |

## <a name="example"></a><span data-ttu-id="c8e7d-143">Пример</span><span class="sxs-lookup"><span data-stu-id="c8e7d-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c8e7d-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8e7d-144">Request</span></span>
<span data-ttu-id="c8e7d-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8e7d-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_privilegedRoleAssignmentRequests"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests('7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee')/cancel
```

##### <a name="response"></a><span data-ttu-id="c8e7d-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8e7d-146">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequests"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests/$entity",
    "schedule": {
        "type": "activation",
        "startDateTime": "2018-02-08T02:35:17.903Z",
        "endDateTime": null,
        "duration" : null
    },
    "id": "bcfb11e3-fc0d-49ea-b3d5-7d60a48e5043",
    "evaluateOnly": false,
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "2018-02-08T02:35:42.9137335Z",
    "status": "Cancelling",
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "userId": "Self"，
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Cancel privilegedRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
