---
title: Создание privilegedRoleAssignmentRequest
description: Создание объекта privilegedroleassignmentrequest.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 8899aa70125809f73e2f247a8cf5b83cad0c7731
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441156"
---
# <a name="create-privilegedroleassignmentrequest"></a><span data-ttu-id="042a8-103">Создание privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="042a8-103">Create privilegedRoleAssignmentRequest</span></span>

<span data-ttu-id="042a8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="042a8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="042a8-105">Создание [объекта privilegedroleassignmentrequest.](../resources/privilegedroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="042a8-105">Create a [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="042a8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="042a8-106">Permissions</span></span>
<span data-ttu-id="042a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="042a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="042a8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="042a8-109">Permission type</span></span>                        | <span data-ttu-id="042a8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="042a8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="042a8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="042a8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="042a8-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="042a8-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="042a8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="042a8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="042a8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="042a8-114">Not supported.</span></span> |
|<span data-ttu-id="042a8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="042a8-115">Application</span></span>                            | <span data-ttu-id="042a8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="042a8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="042a8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="042a8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="042a8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="042a8-118">Request headers</span></span>
| <span data-ttu-id="042a8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="042a8-119">Name</span></span>      |<span data-ttu-id="042a8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="042a8-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="042a8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="042a8-121">Authorization</span></span>  | <span data-ttu-id="042a8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="042a8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="042a8-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="042a8-124">Request body</span></span>
<span data-ttu-id="042a8-125">В теле запроса поставляем представление JSON объекта [privilegedroleassignmentrequest.](../resources/privilegedroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="042a8-125">In the request body, supply a JSON representation of [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="042a8-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="042a8-126">Property</span></span>     | <span data-ttu-id="042a8-127">Тип</span><span class="sxs-lookup"><span data-stu-id="042a8-127">Type</span></span>    |  <span data-ttu-id="042a8-128">Описание</span><span class="sxs-lookup"><span data-stu-id="042a8-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="042a8-129">roleId</span><span class="sxs-lookup"><span data-stu-id="042a8-129">roleId</span></span>|<span data-ttu-id="042a8-130">String</span><span class="sxs-lookup"><span data-stu-id="042a8-130">String</span></span>|<span data-ttu-id="042a8-131">ID роли.</span><span class="sxs-lookup"><span data-stu-id="042a8-131">The ID of the role.</span></span> <span data-ttu-id="042a8-132">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="042a8-132">Required.</span></span>|
|<span data-ttu-id="042a8-133">type</span><span class="sxs-lookup"><span data-stu-id="042a8-133">type</span></span>|<span data-ttu-id="042a8-134">String</span><span class="sxs-lookup"><span data-stu-id="042a8-134">String</span></span>|<span data-ttu-id="042a8-135">Представляет тип операции при назначении ролей.</span><span class="sxs-lookup"><span data-stu-id="042a8-135">Represents the type of the operation on the role assignment.</span></span> <span data-ttu-id="042a8-136">Значение может `AdminAdd` быть: Администраторы добавляют пользователей в роли; `UserAdd` : Пользователи добавляют назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="042a8-136">The value can be `AdminAdd`: Administrators add users to roles;`UserAdd`: Users add role assignments.</span></span> <span data-ttu-id="042a8-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="042a8-137">Required.</span></span>|
|<span data-ttu-id="042a8-138">assignmentState</span><span class="sxs-lookup"><span data-stu-id="042a8-138">assignmentState</span></span>|<span data-ttu-id="042a8-139">String</span><span class="sxs-lookup"><span data-stu-id="042a8-139">String</span></span>|<span data-ttu-id="042a8-140">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="042a8-140">The state of the assignment.</span></span> <span data-ttu-id="042a8-141">Это значение может быть для присвоения, если оно непосредственно назначено администраторами или активировано при назначении, назначенного `Eligible` `Active` `Active` пользователями.</span><span class="sxs-lookup"><span data-stu-id="042a8-141">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span> <span data-ttu-id="042a8-142">Возможные значения: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span><span class="sxs-lookup"><span data-stu-id="042a8-142">Possible values are: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span></span> <span data-ttu-id="042a8-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="042a8-143">Required.</span></span>|
|<span data-ttu-id="042a8-144">reason</span><span class="sxs-lookup"><span data-stu-id="042a8-144">reason</span></span>|<span data-ttu-id="042a8-145">String</span><span class="sxs-lookup"><span data-stu-id="042a8-145">String</span></span>|<span data-ttu-id="042a8-146">Причина должна быть предоставлена для запроса назначения ролей для целей аудита и проверки.</span><span class="sxs-lookup"><span data-stu-id="042a8-146">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="042a8-147">schedule</span><span class="sxs-lookup"><span data-stu-id="042a8-147">schedule</span></span>|[<span data-ttu-id="042a8-148">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="042a8-148">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="042a8-149">Расписание запроса на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="042a8-149">The schedule of the role assignment request.</span></span>|

## <a name="response"></a><span data-ttu-id="042a8-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="042a8-150">Response</span></span>
<span data-ttu-id="042a8-151">В случае успешного выполнения этот метод возвращает код ответа и объект `201 Created` [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="042a8-151">If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="042a8-152">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="042a8-152">Error codes</span></span>
<span data-ttu-id="042a8-153">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="042a8-153">This API returns that standard HTTP error codes.</span></span> <span data-ttu-id="042a8-154">Кроме того, он может возвращать коды ошибок, перечисленные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="042a8-154">In addition, it can return the error codes listed in the following table.</span></span>

|<span data-ttu-id="042a8-155">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="042a8-155">Error code</span></span>     | <span data-ttu-id="042a8-156">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="042a8-156">Error message</span></span>              | 
|:--------------------| :---------------------|
| <span data-ttu-id="042a8-157">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="042a8-157">400 BadRequest</span></span> | <span data-ttu-id="042a8-158">Свойство RoleAssignmentRequest было NULL</span><span class="sxs-lookup"><span data-stu-id="042a8-158">RoleAssignmentRequest property was NULL</span></span> |
| <span data-ttu-id="042a8-159">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="042a8-159">400 BadRequest</span></span> | <span data-ttu-id="042a8-160">Не удается deserialize roleAssignmentRequest Object.</span><span class="sxs-lookup"><span data-stu-id="042a8-160">Unable to deserialize roleAssignmentRequest Object.</span></span> |
| <span data-ttu-id="042a8-161">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="042a8-161">400 BadRequest</span></span> | <span data-ttu-id="042a8-162">RoleId необходим.</span><span class="sxs-lookup"><span data-stu-id="042a8-162">RoleId is required.</span></span> |
| <span data-ttu-id="042a8-163">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="042a8-163">400 BadRequest</span></span> | <span data-ttu-id="042a8-164">Дата начала расписания должна быть указана и должна быть больше, чем сейчас.</span><span class="sxs-lookup"><span data-stu-id="042a8-164">Schedule start date must be specified and should be greater than Now.</span></span> |
| <span data-ttu-id="042a8-165">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="042a8-165">400 BadRequest</span></span> | <span data-ttu-id="042a8-166">Для этого пользователя, роли и типа расписания уже существует расписание.</span><span class="sxs-lookup"><span data-stu-id="042a8-166">A schedule already exists for this user, role and schedule type.</span></span> |
| <span data-ttu-id="042a8-167">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="042a8-167">400 BadRequest</span></span> | <span data-ttu-id="042a8-168">Ожидается утверждение уже существует для этого пользователя, роли и утверждения типа.</span><span class="sxs-lookup"><span data-stu-id="042a8-168">A pending approval already exists for this user, role and approval type.</span></span> |
| <span data-ttu-id="042a8-169">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="042a8-169">400 BadRequest</span></span> | <span data-ttu-id="042a8-170">Причина запроса отсутствует.</span><span class="sxs-lookup"><span data-stu-id="042a8-170">Requestor reason is missing.</span></span> |
| <span data-ttu-id="042a8-171">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="042a8-171">400 BadRequest</span></span> | <span data-ttu-id="042a8-172">Причина запроса должна быть менее 500 символов.</span><span class="sxs-lookup"><span data-stu-id="042a8-172">Requestor reason should be less than 500 characters.</span></span> |
| <span data-ttu-id="042a8-173">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="042a8-173">400 BadRequest</span></span> | <span data-ttu-id="042a8-174">Продолжительность высоты должна быть между 0,5 и {from setting}.</span><span class="sxs-lookup"><span data-stu-id="042a8-174">Elevation duration must be between 0.5 and {from setting}.</span></span> |
| <span data-ttu-id="042a8-175">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="042a8-175">400 BadRequest</span></span> | <span data-ttu-id="042a8-176">Существует совпадение между запланированной активацией и запросом.</span><span class="sxs-lookup"><span data-stu-id="042a8-176">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="042a8-177">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="042a8-177">400 BadRequest</span></span> | <span data-ttu-id="042a8-178">Роль уже активирована.</span><span class="sxs-lookup"><span data-stu-id="042a8-178">The role is already activated.</span></span> |
| <span data-ttu-id="042a8-179">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="042a8-179">400 BadRequest</span></span> | <span data-ttu-id="042a8-180">GenericElevateUserToRoleAssignments: сведения о тикинге необходимы и не поставляются в процессе активации.</span><span class="sxs-lookup"><span data-stu-id="042a8-180">GenericElevateUserToRoleAssignments: Tickting information is required and not supplied in the activation process.</span></span> |
| <span data-ttu-id="042a8-181">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="042a8-181">400 BadRequest</span></span> | <span data-ttu-id="042a8-182">Существует совпадение между запланированной активацией и запросом.</span><span class="sxs-lookup"><span data-stu-id="042a8-182">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="042a8-183">403 UnAuthorized</span><span class="sxs-lookup"><span data-stu-id="042a8-183">403 UnAuthorized</span></span> | <span data-ttu-id="042a8-184">Высота требует многофакторной проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="042a8-184">Elevation requires Multi-Factor Authentication.</span></span> |
| <span data-ttu-id="042a8-185">403 UnAuthorized</span><span class="sxs-lookup"><span data-stu-id="042a8-185">403 UnAuthorized</span></span> | <span data-ttu-id="042a8-186">От имени высоты не допускается.</span><span class="sxs-lookup"><span data-stu-id="042a8-186">On behalf of elevation is not allowed.</span></span> |

## <a name="example"></a><span data-ttu-id="042a8-187">Пример</span><span class="sxs-lookup"><span data-stu-id="042a8-187">Example</span></span>
##### <a name="request"></a><span data-ttu-id="042a8-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="042a8-188">Request</span></span>
<span data-ttu-id="042a8-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="042a8-189">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="042a8-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="042a8-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_privilegedroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
Content-type: application/json

{
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "schedule": {
        "startDateTime": "2018-02-08T02:35:17.903Z"
    },
    "type": "UserAdd",
    "assignmentState": "Active",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```
# <a name="c"></a>[<span data-ttu-id="042a8-191">C#</span><span class="sxs-lookup"><span data-stu-id="042a8-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-privilegedroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="042a8-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="042a8-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-privilegedroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="042a8-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="042a8-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-privilegedroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="042a8-194">Java</span><span class="sxs-lookup"><span data-stu-id="042a8-194">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-privilegedroleassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="042a8-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="042a8-195">Response</span></span>
<span data-ttu-id="042a8-196">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="042a8-196">The following is an example of the response.</span></span> <span data-ttu-id="042a8-197">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="042a8-197">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="042a8-198">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="042a8-198">All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests/$entity",
    "schedule": {
        "type": "activation",
        "startDateTime": "2018-02-08T02:35:17.903Z",
        "endDateTime": null,
        "duration" : null
    },
    "id": "e13ef8a0-c1cb-4d03-aaae-9cd1c8ede2d1",
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "2018-02-08T02:35:42.9137335Z",
    "status": "NotStarted",
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
  "description": "Post privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


