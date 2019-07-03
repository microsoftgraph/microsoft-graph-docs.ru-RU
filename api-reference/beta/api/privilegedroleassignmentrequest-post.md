---
title: Создание Привилежедролеассигнментрекуест
description: Создание объекта привилежедролеассигнментрекуест.
localization_priority: Normal
ms.openlocfilehash: 809bbbbead7a34cd775db8561ae58cb101afe079
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444843"
---
# <a name="create-privilegedroleassignmentrequest"></a><span data-ttu-id="c23a7-103">Создание Привилежедролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="c23a7-103">Create privilegedRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c23a7-104">Создание объекта [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="c23a7-104">Create a [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c23a7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c23a7-105">Permissions</span></span>
<span data-ttu-id="c23a7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c23a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c23a7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c23a7-108">Permission type</span></span>                        | <span data-ttu-id="c23a7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c23a7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c23a7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c23a7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c23a7-111">Привилежедакцесс. ReadWrite. AzureAD, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="c23a7-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c23a7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c23a7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c23a7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c23a7-113">Not supported.</span></span> |
|<span data-ttu-id="c23a7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c23a7-114">Application</span></span>                            | <span data-ttu-id="c23a7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c23a7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c23a7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c23a7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="c23a7-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c23a7-117">Request headers</span></span>
| <span data-ttu-id="c23a7-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c23a7-118">Name</span></span>      |<span data-ttu-id="c23a7-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c23a7-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c23a7-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c23a7-120">Authorization</span></span>  | <span data-ttu-id="c23a7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c23a7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c23a7-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c23a7-123">Request body</span></span>
<span data-ttu-id="c23a7-124">В тексте запроса добавьте представление объекта [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c23a7-124">In the request body, supply a JSON representation of [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="c23a7-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="c23a7-125">Property</span></span>     | <span data-ttu-id="c23a7-126">Тип</span><span class="sxs-lookup"><span data-stu-id="c23a7-126">Type</span></span>    |  <span data-ttu-id="c23a7-127">Описание</span><span class="sxs-lookup"><span data-stu-id="c23a7-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c23a7-128">roleId</span><span class="sxs-lookup"><span data-stu-id="c23a7-128">roleId</span></span>|<span data-ttu-id="c23a7-129">String</span><span class="sxs-lookup"><span data-stu-id="c23a7-129">String</span></span>|<span data-ttu-id="c23a7-130">Идентификатор роли.</span><span class="sxs-lookup"><span data-stu-id="c23a7-130">The ID of the role.</span></span> <span data-ttu-id="c23a7-131">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="c23a7-131">Required.</span></span>|
|<span data-ttu-id="c23a7-132">type</span><span class="sxs-lookup"><span data-stu-id="c23a7-132">type</span></span>|<span data-ttu-id="c23a7-133">String</span><span class="sxs-lookup"><span data-stu-id="c23a7-133">String</span></span>|<span data-ttu-id="c23a7-134">Представляет тип операции для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="c23a7-134">Represents the the type of the operation on the role assignment.</span></span> <span data-ttu-id="c23a7-135">Возможные значения `AdminAdd`: Администраторы Add Users to Roles; `UserAdd`: Пользователи добавляют назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="c23a7-135">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span> <span data-ttu-id="c23a7-136">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="c23a7-136">Required.</span></span>|
|<span data-ttu-id="c23a7-137">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="c23a7-137">assignmentState</span></span>|<span data-ttu-id="c23a7-138">String</span><span class="sxs-lookup"><span data-stu-id="c23a7-138">String</span></span>|<span data-ttu-id="c23a7-139">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="c23a7-139">The state of the assignment.</span></span> <span data-ttu-id="c23a7-140">Значение может быть `Eligible` для правого назначения `Active` , если оно напрямую назначено `Active` администраторами или активировано в соответствии с подходящими пользователями.</span><span class="sxs-lookup"><span data-stu-id="c23a7-140">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span> <span data-ttu-id="c23a7-141">Возможные значения: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span><span class="sxs-lookup"><span data-stu-id="c23a7-141">Possible values are: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span></span> <span data-ttu-id="c23a7-142">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="c23a7-142">Required.</span></span>|
|<span data-ttu-id="c23a7-143">причиной</span><span class="sxs-lookup"><span data-stu-id="c23a7-143">reason</span></span>|<span data-ttu-id="c23a7-144">String</span><span class="sxs-lookup"><span data-stu-id="c23a7-144">String</span></span>|<span data-ttu-id="c23a7-145">Необходимо указать причину для запроса на назначение роли для аудита и проверки.</span><span class="sxs-lookup"><span data-stu-id="c23a7-145">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="c23a7-146">schedule</span><span class="sxs-lookup"><span data-stu-id="c23a7-146">schedule</span></span>|[<span data-ttu-id="c23a7-147">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c23a7-147">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="c23a7-148">Расписание запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="c23a7-148">The schedule of the role assignment request.</span></span>|

## <a name="response"></a><span data-ttu-id="c23a7-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="c23a7-149">Response</span></span>
<span data-ttu-id="c23a7-150">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c23a7-150">If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="c23a7-151">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="c23a7-151">Error codes</span></span>
<span data-ttu-id="c23a7-152">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="c23a7-152">This API returns that standard HTTP error codes.</span></span> <span data-ttu-id="c23a7-153">Кроме того, он может возвращать коды ошибок, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="c23a7-153">In addition, it can return the error codes listed in the following table.</span></span>

|<span data-ttu-id="c23a7-154">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="c23a7-154">Error code</span></span>     | <span data-ttu-id="c23a7-155">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="c23a7-155">Error message</span></span>              | 
|:--------------------| :---------------------|
| <span data-ttu-id="c23a7-156">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="c23a7-156">400 BadRequest</span></span> | <span data-ttu-id="c23a7-157">Свойство Ролеассигнментрекуест имеет значение NULL</span><span class="sxs-lookup"><span data-stu-id="c23a7-157">RoleAssignmentRequest property was NULL</span></span> |
| <span data-ttu-id="c23a7-158">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="c23a7-158">400 BadRequest</span></span> | <span data-ttu-id="c23a7-159">Не удается десериализовать объект Ролеассигнментрекуест.</span><span class="sxs-lookup"><span data-stu-id="c23a7-159">Unable to deserialize roleAssignmentRequest Object.</span></span> |
| <span data-ttu-id="c23a7-160">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="c23a7-160">400 BadRequest</span></span> | <span data-ttu-id="c23a7-161">RoleId является обязательным.</span><span class="sxs-lookup"><span data-stu-id="c23a7-161">RoleId is required.</span></span> |
| <span data-ttu-id="c23a7-162">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="c23a7-162">400 BadRequest</span></span> | <span data-ttu-id="c23a7-163">Дата начала расписания должна быть указана и должна быть больше, чем сейчас.</span><span class="sxs-lookup"><span data-stu-id="c23a7-163">Schedule start date must be specified and should be greater than Now.</span></span> |
| <span data-ttu-id="c23a7-164">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="c23a7-164">400 BadRequest</span></span> | <span data-ttu-id="c23a7-165">Расписание для этого пользователя, роли и типа расписания уже существует.</span><span class="sxs-lookup"><span data-stu-id="c23a7-165">A schedule already exists for this user, role and schedule type.</span></span> |
| <span data-ttu-id="c23a7-166">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="c23a7-166">400 BadRequest</span></span> | <span data-ttu-id="c23a7-167">Для этого пользователя, роли и типа утверждения уже существует ожидающее утверждение.</span><span class="sxs-lookup"><span data-stu-id="c23a7-167">A pending approval already exists for this user, role and approval type.</span></span> |
| <span data-ttu-id="c23a7-168">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="c23a7-168">400 BadRequest</span></span> | <span data-ttu-id="c23a7-169">Не указана причина запрашивающей стороны.</span><span class="sxs-lookup"><span data-stu-id="c23a7-169">Requestor reason is missing.</span></span> |
| <span data-ttu-id="c23a7-170">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="c23a7-170">400 BadRequest</span></span> | <span data-ttu-id="c23a7-171">Срок запрашивающего не должен быть меньше 500 символов.</span><span class="sxs-lookup"><span data-stu-id="c23a7-171">Requestor reason should be less than 500 characters.</span></span> |
| <span data-ttu-id="c23a7-172">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="c23a7-172">400 BadRequest</span></span> | <span data-ttu-id="c23a7-173">Длительность возвышения должна быть между 0,5 и {from Setting}.</span><span class="sxs-lookup"><span data-stu-id="c23a7-173">Elevation duration must be between 0.5 and {from setting}.</span></span> |
| <span data-ttu-id="c23a7-174">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="c23a7-174">400 BadRequest</span></span> | <span data-ttu-id="c23a7-175">Между запланированной активацией и запросом существует перекрытие.</span><span class="sxs-lookup"><span data-stu-id="c23a7-175">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="c23a7-176">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="c23a7-176">400 BadRequest</span></span> | <span data-ttu-id="c23a7-177">Роль уже активирована.</span><span class="sxs-lookup"><span data-stu-id="c23a7-177">The role is already activated.</span></span> |
| <span data-ttu-id="c23a7-178">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="c23a7-178">400 BadRequest</span></span> | <span data-ttu-id="c23a7-179">Женерицелеватеусерторолеассигнментс: Тикктинг сведения являются обязательными и не предоставляются в процессе активации.</span><span class="sxs-lookup"><span data-stu-id="c23a7-179">GenericElevateUserToRoleAssignments: Tickting information is required and not supplied in the activation process.</span></span> |
| <span data-ttu-id="c23a7-180">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="c23a7-180">400 BadRequest</span></span> | <span data-ttu-id="c23a7-181">Между запланированной активацией и запросом существует перекрытие.</span><span class="sxs-lookup"><span data-stu-id="c23a7-181">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="c23a7-182">403 авторизация</span><span class="sxs-lookup"><span data-stu-id="c23a7-182">403 UnAuthorized</span></span> | <span data-ttu-id="c23a7-183">Для повышения требуется многофакторная проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="c23a7-183">Elevation requires Multi-Factor Authentication.</span></span> |
| <span data-ttu-id="c23a7-184">403 авторизация</span><span class="sxs-lookup"><span data-stu-id="c23a7-184">403 UnAuthorized</span></span> | <span data-ttu-id="c23a7-185">От имени повышения прав не разрешено.</span><span class="sxs-lookup"><span data-stu-id="c23a7-185">On behalf of elevation is not allowed.</span></span> |

## <a name="example"></a><span data-ttu-id="c23a7-186">Пример</span><span class="sxs-lookup"><span data-stu-id="c23a7-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c23a7-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="c23a7-187">Request</span></span>
<span data-ttu-id="c23a7-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c23a7-188">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c23a7-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="c23a7-189">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="c23a7-190">C#</span><span class="sxs-lookup"><span data-stu-id="c23a7-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-privilegedroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c23a7-191">Javascript</span><span class="sxs-lookup"><span data-stu-id="c23a7-191">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-privilegedroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c23a7-192">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c23a7-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-privilegedroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c23a7-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="c23a7-193">Response</span></span>
<span data-ttu-id="c23a7-194">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c23a7-194">The following is an example of the response.</span></span> <span data-ttu-id="c23a7-195">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="c23a7-195">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c23a7-196">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c23a7-196">All of the properties will be returned from an actual call.</span></span>
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
