---
title: Отмена Привилежедролеассигнментрекуест
description: Отмена объекта Привилежедролеассигнментрекуест.
localization_priority: Normal
ms.openlocfilehash: 99b02ac432eab2e0fe8f2b860b92e03719404b2c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264157"
---
# <a name="cancel-privilegedroleassignmentrequest"></a><span data-ttu-id="4c065-103">Отмена Привилежедролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="4c065-103">Cancel privilegedRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c065-104">Отмена объекта [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="4c065-104">Cancel a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c065-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c065-105">Permissions</span></span>
<span data-ttu-id="4c065-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c065-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c065-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c065-108">Permission type</span></span>                        | <span data-ttu-id="4c065-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c065-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c065-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c065-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4c065-111">Привилежедакцесс. ReadWrite. AzureAD, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="4c065-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4c065-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c065-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c065-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c065-113">Not supported.</span></span> |
|<span data-ttu-id="4c065-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c065-114">Application</span></span>                            | <span data-ttu-id="4c065-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c065-115">Not supported.</span></span> |


### <a name="http-request"></a><span data-ttu-id="4c065-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c065-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests({requestid})/cancel
```

## <a name="request-headers"></a><span data-ttu-id="4c065-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c065-117">Request headers</span></span>
| <span data-ttu-id="4c065-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4c065-118">Name</span></span>      |<span data-ttu-id="4c065-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4c065-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4c065-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c065-120">Authorization</span></span>  | <span data-ttu-id="4c065-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c065-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c065-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4c065-123">Request body</span></span>
<span data-ttu-id="4c065-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c065-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c065-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c065-125">Response</span></span>
<span data-ttu-id="4c065-126">В случае успешного выполнения этот метод возвращает код отклика `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="4c065-126">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="4c065-127">Он возвращает [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c065-127">It returns [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="4c065-128">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="4c065-128">Error codes</span></span>
<span data-ttu-id="4c065-129">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="4c065-129">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="4c065-130">Кроме того, он возвращает коды настраиваемых ошибок, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="4c065-130">In addition, it returns the custom error codes listed in the following table.</span></span>

|<span data-ttu-id="4c065-131">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="4c065-131">Error code</span></span>     | <span data-ttu-id="4c065-132">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="4c065-132">Error message</span></span>              |
|:--------------------| :---------------------|
| <span data-ttu-id="4c065-133">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="4c065-133">400 BadRequest</span></span> | <span data-ttu-id="4c065-134">RequestId не может иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="4c065-134">RequestId cannot be Null.</span></span> |
| <span data-ttu-id="4c065-135">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="4c065-135">400 BadRequest</span></span> | <span data-ttu-id="4c065-136">Запрос с ИДЕНТИФИКАТОРом запроса не найден.</span><span class="sxs-lookup"><span data-stu-id="4c065-136">Request with request ID not found.</span></span> |
| <span data-ttu-id="4c065-137">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="4c065-137">400 BadRequest</span></span> | <span data-ttu-id="4c065-138">Отмену можно выполнить только по запланированному состоянию и Пендингаппровал.</span><span class="sxs-lookup"><span data-stu-id="4c065-138">Cancellation can be done only on status Scheduled and PendingApproval.</span></span> |
| <span data-ttu-id="4c065-139">403 авторизация</span><span class="sxs-lookup"><span data-stu-id="4c065-139">403 UnAuthorized</span></span> | <span data-ttu-id="4c065-140">Инициатор запроса не может выполнить вызов отмены или запрос не найден.</span><span class="sxs-lookup"><span data-stu-id="4c065-140">Requester not allowed to make Cancel call or request not found.</span></span> |

## <a name="example"></a><span data-ttu-id="4c065-141">Пример</span><span class="sxs-lookup"><span data-stu-id="4c065-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c065-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c065-142">Request</span></span>
<span data-ttu-id="4c065-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c065-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_privilegedRoleAssignmentRequests"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```

##### <a name="response"></a><span data-ttu-id="4c065-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c065-144">Response</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="4c065-145">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="4c065-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4c065-146">C#</span><span class="sxs-lookup"><span data-stu-id="4c065-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/cancel_privilegedRoleAssignmentRequests-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4c065-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="4c065-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/cancel_privilegedRoleAssignmentRequests-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4c065-148">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4c065-148">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/cancel_privilegedRoleAssignmentRequests-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-cancel.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-cancel.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-cancel.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
