---
title: Отмена Привилежедролеассигнментрекуест
description: Отмена объекта Привилежедролеассигнментрекуест.
localization_priority: Normal
ms.openlocfilehash: 649ec481815ccb4ce903e51ecb98ccf99cdfa77f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337242"
---
# <a name="cancel-privilegedroleassignmentrequest"></a><span data-ttu-id="bdf89-103">Отмена Привилежедролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="bdf89-103">Cancel privilegedRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdf89-104">Отмена объекта [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="bdf89-104">Cancel a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bdf89-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bdf89-105">Permissions</span></span>
<span data-ttu-id="bdf89-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdf89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdf89-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdf89-108">Permission type</span></span>                        | <span data-ttu-id="bdf89-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdf89-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdf89-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdf89-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bdf89-111">Привилежедакцесс. ReadWrite. AzureAD, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="bdf89-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bdf89-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdf89-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdf89-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdf89-113">Not supported.</span></span> |
|<span data-ttu-id="bdf89-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bdf89-114">Application</span></span>                            | <span data-ttu-id="bdf89-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdf89-115">Not supported.</span></span> |


### <a name="http-request"></a><span data-ttu-id="bdf89-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdf89-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests({requestid})/cancel
```

## <a name="request-headers"></a><span data-ttu-id="bdf89-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bdf89-117">Request headers</span></span>
| <span data-ttu-id="bdf89-118">Имя</span><span class="sxs-lookup"><span data-stu-id="bdf89-118">Name</span></span>      |<span data-ttu-id="bdf89-119">Описание</span><span class="sxs-lookup"><span data-stu-id="bdf89-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bdf89-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bdf89-120">Authorization</span></span>  | <span data-ttu-id="bdf89-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bdf89-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bdf89-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bdf89-123">Request body</span></span>
<span data-ttu-id="bdf89-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bdf89-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bdf89-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdf89-125">Response</span></span>
<span data-ttu-id="bdf89-126">В случае успешного выполнения этот метод возвращает код отклика `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="bdf89-126">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="bdf89-127">Он возвращает [привилежедролеассигнментрекуест](../resources/privilegedRoleAssignmentRequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bdf89-127">It returns [privilegedRoleAssignmentRequest](../resources/privilegedRoleAssignmentRequest.md) in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="bdf89-128">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="bdf89-128">Error codes</span></span>
<span data-ttu-id="bdf89-129">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="bdf89-129">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="bdf89-130">Кроме того, он возвращает коды настраиваемых ошибок, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="bdf89-130">In addition, it returns the custom error codes listed in the following table.</span></span>

|<span data-ttu-id="bdf89-131">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="bdf89-131">Error code</span></span>     | <span data-ttu-id="bdf89-132">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="bdf89-132">Error message</span></span>              |
|:--------------------| :---------------------|
| <span data-ttu-id="bdf89-133">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="bdf89-133">400 BadRequest</span></span> | <span data-ttu-id="bdf89-134">RequestId не может иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="bdf89-134">RequestId cannot be Null.</span></span> |
| <span data-ttu-id="bdf89-135">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="bdf89-135">400 BadRequest</span></span> | <span data-ttu-id="bdf89-136">Запрос с ИДЕНТИФИКАТОРом запроса не найден.</span><span class="sxs-lookup"><span data-stu-id="bdf89-136">Request with request ID not found.</span></span> |
| <span data-ttu-id="bdf89-137">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="bdf89-137">400 BadRequest</span></span> | <span data-ttu-id="bdf89-138">Отмену можно выполнить только по запланированному состоянию и Пендингаппровал.</span><span class="sxs-lookup"><span data-stu-id="bdf89-138">Cancellation can be done only on status Scheduled and PendingApproval.</span></span> |
| <span data-ttu-id="bdf89-139">403 авторизация</span><span class="sxs-lookup"><span data-stu-id="bdf89-139">403 UnAuthorized</span></span> | <span data-ttu-id="bdf89-140">Инициатор запроса не может выполнить вызов отмены или запрос не найден.</span><span class="sxs-lookup"><span data-stu-id="bdf89-140">Requester not allowed to make Cancel call or request not found.</span></span> |

## <a name="example"></a><span data-ttu-id="bdf89-141">Пример</span><span class="sxs-lookup"><span data-stu-id="bdf89-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bdf89-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdf89-142">Request</span></span>
<span data-ttu-id="bdf89-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bdf89-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_privilegedRoleAssignmentRequests"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```

##### <a name="response"></a><span data-ttu-id="bdf89-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdf89-144">Response</span></span>
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
  "suppressions": []
}
-->
