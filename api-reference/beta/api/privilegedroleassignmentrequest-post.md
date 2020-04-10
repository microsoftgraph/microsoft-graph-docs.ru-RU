---
title: Создание Привилежедролеассигнментрекуест
description: Создание объекта привилежедролеассигнментрекуест.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: afc7251bafdb6570eca801abc41ff39216d7381b
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218670"
---
# <a name="create-privilegedroleassignmentrequest"></a><span data-ttu-id="ca287-103">Создание Привилежедролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="ca287-103">Create privilegedRoleAssignmentRequest</span></span>

<span data-ttu-id="ca287-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca287-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca287-105">Создание объекта [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="ca287-105">Create a [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca287-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca287-106">Permissions</span></span>
<span data-ttu-id="ca287-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca287-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca287-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca287-109">Permission type</span></span>                        | <span data-ttu-id="ca287-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca287-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca287-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca287-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ca287-112">Привилежедакцесс. ReadWrite. AzureAD, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="ca287-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ca287-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca287-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca287-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca287-114">Not supported.</span></span> |
|<span data-ttu-id="ca287-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca287-115">Application</span></span>                            | <span data-ttu-id="ca287-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca287-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca287-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca287-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="ca287-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca287-118">Request headers</span></span>
| <span data-ttu-id="ca287-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ca287-119">Name</span></span>      |<span data-ttu-id="ca287-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ca287-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ca287-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca287-121">Authorization</span></span>  | <span data-ttu-id="ca287-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca287-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca287-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca287-124">Request body</span></span>
<span data-ttu-id="ca287-125">В тексте запроса добавьте представление объекта [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca287-125">In the request body, supply a JSON representation of [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="ca287-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca287-126">Property</span></span>     | <span data-ttu-id="ca287-127">Тип</span><span class="sxs-lookup"><span data-stu-id="ca287-127">Type</span></span>    |  <span data-ttu-id="ca287-128">Описание</span><span class="sxs-lookup"><span data-stu-id="ca287-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca287-129">roleId</span><span class="sxs-lookup"><span data-stu-id="ca287-129">roleId</span></span>|<span data-ttu-id="ca287-130">Строка</span><span class="sxs-lookup"><span data-stu-id="ca287-130">String</span></span>|<span data-ttu-id="ca287-131">Идентификатор роли.</span><span class="sxs-lookup"><span data-stu-id="ca287-131">The ID of the role.</span></span> <span data-ttu-id="ca287-132">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="ca287-132">Required.</span></span>|
|<span data-ttu-id="ca287-133">type</span><span class="sxs-lookup"><span data-stu-id="ca287-133">type</span></span>|<span data-ttu-id="ca287-134">String</span><span class="sxs-lookup"><span data-stu-id="ca287-134">String</span></span>|<span data-ttu-id="ca287-135">Представляет тип операции для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="ca287-135">Represents the type of the operation on the role assignment.</span></span> <span data-ttu-id="ca287-136">Возможные значения `AdminAdd`: администраторы добавляют пользователей к ролям; `UserAdd`: Пользователи добавляют назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="ca287-136">The value can be `AdminAdd`: Administrators add users to roles;`UserAdd`: Users add role assignments.</span></span> <span data-ttu-id="ca287-137">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="ca287-137">Required.</span></span>|
|<span data-ttu-id="ca287-138">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="ca287-138">assignmentState</span></span>|<span data-ttu-id="ca287-139">Строка</span><span class="sxs-lookup"><span data-stu-id="ca287-139">String</span></span>|<span data-ttu-id="ca287-140">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="ca287-140">The state of the assignment.</span></span> <span data-ttu-id="ca287-141">Значение может быть `Eligible` для правого назначения `Active` , если оно напрямую назначено `Active` администраторами или активировано в соответствии с подходящими пользователями.</span><span class="sxs-lookup"><span data-stu-id="ca287-141">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span> <span data-ttu-id="ca287-142">Возможные значения: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span><span class="sxs-lookup"><span data-stu-id="ca287-142">Possible values are: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span></span> <span data-ttu-id="ca287-143">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="ca287-143">Required.</span></span>|
|<span data-ttu-id="ca287-144">reason</span><span class="sxs-lookup"><span data-stu-id="ca287-144">reason</span></span>|<span data-ttu-id="ca287-145">Строка</span><span class="sxs-lookup"><span data-stu-id="ca287-145">String</span></span>|<span data-ttu-id="ca287-146">Необходимо указать причину для запроса на назначение роли для аудита и проверки.</span><span class="sxs-lookup"><span data-stu-id="ca287-146">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="ca287-147">schedule</span><span class="sxs-lookup"><span data-stu-id="ca287-147">schedule</span></span>|[<span data-ttu-id="ca287-148">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="ca287-148">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="ca287-149">Расписание запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="ca287-149">The schedule of the role assignment request.</span></span>|

## <a name="response"></a><span data-ttu-id="ca287-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca287-150">Response</span></span>
<span data-ttu-id="ca287-151">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ca287-151">If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="ca287-152">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="ca287-152">Error codes</span></span>
<span data-ttu-id="ca287-153">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="ca287-153">This API returns that standard HTTP error codes.</span></span> <span data-ttu-id="ca287-154">Кроме того, он может возвращать коды ошибок, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="ca287-154">In addition, it can return the error codes listed in the following table.</span></span>

|<span data-ttu-id="ca287-155">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="ca287-155">Error code</span></span>     | <span data-ttu-id="ca287-156">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="ca287-156">Error message</span></span>              | 
|:--------------------| :---------------------|
| <span data-ttu-id="ca287-157">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="ca287-157">400 BadRequest</span></span> | <span data-ttu-id="ca287-158">Свойство Ролеассигнментрекуест имеет значение NULL</span><span class="sxs-lookup"><span data-stu-id="ca287-158">RoleAssignmentRequest property was NULL</span></span> |
| <span data-ttu-id="ca287-159">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="ca287-159">400 BadRequest</span></span> | <span data-ttu-id="ca287-160">Не удается десериализовать объект Ролеассигнментрекуест.</span><span class="sxs-lookup"><span data-stu-id="ca287-160">Unable to deserialize roleAssignmentRequest Object.</span></span> |
| <span data-ttu-id="ca287-161">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="ca287-161">400 BadRequest</span></span> | <span data-ttu-id="ca287-162">RoleId является обязательным.</span><span class="sxs-lookup"><span data-stu-id="ca287-162">RoleId is required.</span></span> |
| <span data-ttu-id="ca287-163">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="ca287-163">400 BadRequest</span></span> | <span data-ttu-id="ca287-164">Дата начала расписания должна быть указана и должна быть больше, чем сейчас.</span><span class="sxs-lookup"><span data-stu-id="ca287-164">Schedule start date must be specified and should be greater than Now.</span></span> |
| <span data-ttu-id="ca287-165">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="ca287-165">400 BadRequest</span></span> | <span data-ttu-id="ca287-166">Расписание для этого пользователя, роли и типа расписания уже существует.</span><span class="sxs-lookup"><span data-stu-id="ca287-166">A schedule already exists for this user, role and schedule type.</span></span> |
| <span data-ttu-id="ca287-167">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="ca287-167">400 BadRequest</span></span> | <span data-ttu-id="ca287-168">Для этого пользователя, роли и типа утверждения уже существует ожидающее утверждение.</span><span class="sxs-lookup"><span data-stu-id="ca287-168">A pending approval already exists for this user, role and approval type.</span></span> |
| <span data-ttu-id="ca287-169">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="ca287-169">400 BadRequest</span></span> | <span data-ttu-id="ca287-170">Не указана причина запрашивающей стороны.</span><span class="sxs-lookup"><span data-stu-id="ca287-170">Requestor reason is missing.</span></span> |
| <span data-ttu-id="ca287-171">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="ca287-171">400 BadRequest</span></span> | <span data-ttu-id="ca287-172">Срок запрашивающего не должен быть меньше 500 символов.</span><span class="sxs-lookup"><span data-stu-id="ca287-172">Requestor reason should be less than 500 characters.</span></span> |
| <span data-ttu-id="ca287-173">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="ca287-173">400 BadRequest</span></span> | <span data-ttu-id="ca287-174">Длительность возвышения должна быть между 0,5 и {from Setting}.</span><span class="sxs-lookup"><span data-stu-id="ca287-174">Elevation duration must be between 0.5 and {from setting}.</span></span> |
| <span data-ttu-id="ca287-175">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="ca287-175">400 BadRequest</span></span> | <span data-ttu-id="ca287-176">Между запланированной активацией и запросом существует перекрытие.</span><span class="sxs-lookup"><span data-stu-id="ca287-176">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="ca287-177">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="ca287-177">400 BadRequest</span></span> | <span data-ttu-id="ca287-178">Роль уже активирована.</span><span class="sxs-lookup"><span data-stu-id="ca287-178">The role is already activated.</span></span> |
| <span data-ttu-id="ca287-179">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="ca287-179">400 BadRequest</span></span> | <span data-ttu-id="ca287-180">Женерицелеватеусерторолеассигнментс: Тикктинг сведения являются обязательными и не предоставляются в процессе активации.</span><span class="sxs-lookup"><span data-stu-id="ca287-180">GenericElevateUserToRoleAssignments: Tickting information is required and not supplied in the activation process.</span></span> |
| <span data-ttu-id="ca287-181">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="ca287-181">400 BadRequest</span></span> | <span data-ttu-id="ca287-182">Между запланированной активацией и запросом существует перекрытие.</span><span class="sxs-lookup"><span data-stu-id="ca287-182">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="ca287-183">403 авторизация</span><span class="sxs-lookup"><span data-stu-id="ca287-183">403 UnAuthorized</span></span> | <span data-ttu-id="ca287-184">Для повышения требуется многофакторная проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="ca287-184">Elevation requires Multi-Factor Authentication.</span></span> |
| <span data-ttu-id="ca287-185">403 авторизация</span><span class="sxs-lookup"><span data-stu-id="ca287-185">403 UnAuthorized</span></span> | <span data-ttu-id="ca287-186">От имени повышения прав не разрешено.</span><span class="sxs-lookup"><span data-stu-id="ca287-186">On behalf of elevation is not allowed.</span></span> |

## <a name="example"></a><span data-ttu-id="ca287-187">Пример</span><span class="sxs-lookup"><span data-stu-id="ca287-187">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ca287-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca287-188">Request</span></span>
<span data-ttu-id="ca287-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca287-189">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ca287-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca287-190">HTTP</span></span>](#tab/http)
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
    "evaluateOnly": false,
    "type": "UserAdd",
    "assignmentState": "Active",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```
# <a name="c"></a>[<span data-ttu-id="ca287-191">C#</span><span class="sxs-lookup"><span data-stu-id="ca287-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-privilegedroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca287-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca287-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-privilegedroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca287-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca287-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-privilegedroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ca287-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca287-194">Response</span></span>
<span data-ttu-id="ca287-195">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ca287-195">The following is an example of the response.</span></span> <span data-ttu-id="ca287-196">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="ca287-196">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ca287-197">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ca287-197">All of the properties will be returned from an actual call.</span></span>
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
    "evaluateOnly": false,
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
