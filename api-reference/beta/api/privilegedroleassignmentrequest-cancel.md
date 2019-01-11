---
title: Отменить privilegedRoleAssignmentRequest
description: Отмена privilegedRoleAssignmentRequest.
localization_priority: Normal
ms.openlocfilehash: 2a3e24a0e78170af23ef15ce99d1f6df72297360
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835009"
---
# <a name="cancel-privilegedroleassignmentrequest"></a><span data-ttu-id="0d8e2-103">Отменить privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="0d8e2-103">Cancel privilegedRoleAssignmentRequest</span></span>

> <span data-ttu-id="0d8e2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0d8e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d8e2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d8e2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0d8e2-106">Отмена [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="0d8e2-106">Cancel a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0d8e2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d8e2-107">Permissions</span></span>
<span data-ttu-id="0d8e2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d8e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d8e2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d8e2-110">Permission type</span></span>                        | <span data-ttu-id="0d8e2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d8e2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d8e2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d8e2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0d8e2-113">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0d8e2-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0d8e2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d8e2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d8e2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d8e2-115">Not supported.</span></span> |
|<span data-ttu-id="0d8e2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d8e2-116">Application</span></span>                            | <span data-ttu-id="0d8e2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d8e2-117">Not supported.</span></span> |


### <a name="http-request"></a><span data-ttu-id="0d8e2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d8e2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests({requestid})/cancel
```

## <a name="request-headers"></a><span data-ttu-id="0d8e2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d8e2-119">Request headers</span></span>
| <span data-ttu-id="0d8e2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0d8e2-120">Name</span></span>      |<span data-ttu-id="0d8e2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0d8e2-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0d8e2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d8e2-122">Authorization</span></span>  | <span data-ttu-id="0d8e2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d8e2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d8e2-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0d8e2-125">Request body</span></span>
<span data-ttu-id="0d8e2-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0d8e2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d8e2-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d8e2-127">Response</span></span>
<span data-ttu-id="0d8e2-128">В случае успешного выполнения этот метод возвращает код отклика `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="0d8e2-128">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="0d8e2-129">Возвращает [privilegedRoleAssignmentRequest] (.. / resources/privilegedRoleAssignmentRequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0d8e2-129">It returns [privilegedRoleAssignmentRequest] (../resources/privilegedRoleAssignmentRequest.md) in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="0d8e2-130">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="0d8e2-130">Error codes</span></span>
<span data-ttu-id="0d8e2-131">Этот интерфейс API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="0d8e2-131">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="0d8e2-132">Кроме того он возвращает коды пользовательских ошибок, перечисленных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="0d8e2-132">In addition, it returns the custom error codes listed in the following table.</span></span>

|<span data-ttu-id="0d8e2-133">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="0d8e2-133">Error code</span></span>     | <span data-ttu-id="0d8e2-134">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="0d8e2-134">Error message</span></span>              |
|:--------------------| :---------------------|
| <span data-ttu-id="0d8e2-135">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="0d8e2-135">400 BadRequest</span></span> | <span data-ttu-id="0d8e2-136">RequestId не может быть Null.</span><span class="sxs-lookup"><span data-stu-id="0d8e2-136">RequestId cannot be Null.</span></span> |
| <span data-ttu-id="0d8e2-137">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="0d8e2-137">400 BadRequest</span></span> | <span data-ttu-id="0d8e2-138">Запрос с Идентификатором запроса не найден.</span><span class="sxs-lookup"><span data-stu-id="0d8e2-138">Request with request ID not found.</span></span> |
| <span data-ttu-id="0d8e2-139">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="0d8e2-139">400 BadRequest</span></span> | <span data-ttu-id="0d8e2-140">Отмены можно выполнить только на состояние расписанию и ожидает утверждения.</span><span class="sxs-lookup"><span data-stu-id="0d8e2-140">Cancellation can be done only on status Scheduled and PendingApproval.</span></span> |
| <span data-ttu-id="0d8e2-141">403 доступ запрещен</span><span class="sxs-lookup"><span data-stu-id="0d8e2-141">403 UnAuthorized</span></span> | <span data-ttu-id="0d8e2-142">Автор запроса не может совершать вызов отмены или запрос не найден.</span><span class="sxs-lookup"><span data-stu-id="0d8e2-142">Requester not allowed to make Cancel call or request not found.</span></span> |

## <a name="example"></a><span data-ttu-id="0d8e2-143">Пример</span><span class="sxs-lookup"><span data-stu-id="0d8e2-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d8e2-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d8e2-144">Request</span></span>
<span data-ttu-id="0d8e2-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d8e2-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_privilegedRoleAssignmentRequests"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests('7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee')/cancel
```

##### <a name="response"></a><span data-ttu-id="0d8e2-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d8e2-146">Response</span></span>
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
