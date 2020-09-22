---
title: Отмена Привилежедролеассигнментрекуест
description: Отмена объекта Привилежедролеассигнментрекуест.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: abb1bbd8c7d8c866ab1149d7a3c2ed810dcc4fde
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034989"
---
# <a name="cancel-privilegedroleassignmentrequest"></a><span data-ttu-id="9ab9c-103">Отмена Привилежедролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="9ab9c-103">Cancel privilegedRoleAssignmentRequest</span></span>

<span data-ttu-id="9ab9c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ab9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ab9c-105">Отмена объекта [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="9ab9c-105">Cancel a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9ab9c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ab9c-106">Permissions</span></span>
<span data-ttu-id="9ab9c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ab9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ab9c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ab9c-109">Permission type</span></span>                        | <span data-ttu-id="9ab9c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ab9c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ab9c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ab9c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9ab9c-112">Привилежедакцесс. ReadWrite. AzureAD, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="9ab9c-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9ab9c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ab9c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ab9c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ab9c-114">Not supported.</span></span> |
|<span data-ttu-id="9ab9c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ab9c-115">Application</span></span>                            | <span data-ttu-id="9ab9c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ab9c-116">Not supported.</span></span> |


### <a name="http-request"></a><span data-ttu-id="9ab9c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ab9c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests({requestid})/cancel
```

## <a name="request-headers"></a><span data-ttu-id="9ab9c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ab9c-118">Request headers</span></span>
| <span data-ttu-id="9ab9c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9ab9c-119">Name</span></span>      |<span data-ttu-id="9ab9c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9ab9c-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9ab9c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ab9c-121">Authorization</span></span>  | <span data-ttu-id="9ab9c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ab9c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ab9c-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ab9c-124">Request body</span></span>
<span data-ttu-id="9ab9c-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9ab9c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ab9c-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ab9c-126">Response</span></span>
<span data-ttu-id="9ab9c-127">В случае успешного выполнения этот метод возвращает код отклика `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="9ab9c-127">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="9ab9c-128">Он возвращает [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9ab9c-128">It returns [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="9ab9c-129">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="9ab9c-129">Error codes</span></span>
<span data-ttu-id="9ab9c-130">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="9ab9c-130">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="9ab9c-131">Кроме того, он возвращает коды настраиваемых ошибок, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="9ab9c-131">In addition, it returns the custom error codes listed in the following table.</span></span>

|<span data-ttu-id="9ab9c-132">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="9ab9c-132">Error code</span></span>     | <span data-ttu-id="9ab9c-133">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="9ab9c-133">Error message</span></span>              |
|:--------------------| :---------------------|
| <span data-ttu-id="9ab9c-134">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="9ab9c-134">400 BadRequest</span></span> | <span data-ttu-id="9ab9c-135">RequestId не может иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="9ab9c-135">RequestId cannot be Null.</span></span> |
| <span data-ttu-id="9ab9c-136">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="9ab9c-136">400 BadRequest</span></span> | <span data-ttu-id="9ab9c-137">Запрос с ИДЕНТИФИКАТОРом запроса не найден.</span><span class="sxs-lookup"><span data-stu-id="9ab9c-137">Request with request ID not found.</span></span> |
| <span data-ttu-id="9ab9c-138">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="9ab9c-138">400 BadRequest</span></span> | <span data-ttu-id="9ab9c-139">Отмену можно выполнить только по запланированному состоянию и Пендингаппровал.</span><span class="sxs-lookup"><span data-stu-id="9ab9c-139">Cancellation can be done only on status Scheduled and PendingApproval.</span></span> |
| <span data-ttu-id="9ab9c-140">403 авторизация</span><span class="sxs-lookup"><span data-stu-id="9ab9c-140">403 UnAuthorized</span></span> | <span data-ttu-id="9ab9c-141">Инициатор запроса не может выполнить вызов отмены или запрос не найден.</span><span class="sxs-lookup"><span data-stu-id="9ab9c-141">Requester not allowed to make Cancel call or request not found.</span></span> |

## <a name="example"></a><span data-ttu-id="9ab9c-142">Пример</span><span class="sxs-lookup"><span data-stu-id="9ab9c-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9ab9c-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ab9c-143">Request</span></span>
<span data-ttu-id="9ab9c-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ab9c-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9ab9c-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ab9c-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cancel_privilegedRoleAssignmentRequests"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```
# <a name="c"></a>[<span data-ttu-id="9ab9c-146">C#</span><span class="sxs-lookup"><span data-stu-id="9ab9c-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cancel-privilegedroleassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ab9c-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ab9c-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cancel-privilegedroleassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ab9c-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ab9c-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cancel-privilegedroleassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9ab9c-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ab9c-149">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
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
    "userId": "Self",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Cancel privilegedRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


