---
title: Создание privilegedRoleAssignmentRequest
description: Создайте объект privilegedroleassignmentrequest.
localization_priority: Normal
ms.openlocfilehash: e3158e918d061f09dec9e74c9e3bfd66d95fa48d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521070"
---
# <a name="create-privilegedroleassignmentrequest"></a><span data-ttu-id="bf2b8-103">Создание privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="bf2b8-103">Create privilegedRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf2b8-104">Создайте объект [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="bf2b8-104">Create a [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf2b8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bf2b8-105">Permissions</span></span>
<span data-ttu-id="bf2b8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf2b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf2b8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf2b8-108">Permission type</span></span>                        | <span data-ttu-id="bf2b8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf2b8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf2b8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf2b8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bf2b8-111">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bf2b8-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bf2b8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf2b8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf2b8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-113">Not supported.</span></span> |
|<span data-ttu-id="bf2b8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf2b8-114">Application</span></span>                            | <span data-ttu-id="bf2b8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf2b8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf2b8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="bf2b8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf2b8-117">Request headers</span></span>
| <span data-ttu-id="bf2b8-118">Имя</span><span class="sxs-lookup"><span data-stu-id="bf2b8-118">Name</span></span>      |<span data-ttu-id="bf2b8-119">Описание</span><span class="sxs-lookup"><span data-stu-id="bf2b8-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bf2b8-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf2b8-120">Authorization</span></span>  | <span data-ttu-id="bf2b8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bf2b8-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf2b8-123">Request body</span></span>
<span data-ttu-id="bf2b8-124">В тексте запроса укажите представление JSON объекта [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="bf2b8-124">In the request body, supply a JSON representation of [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="bf2b8-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf2b8-125">Property</span></span>     | <span data-ttu-id="bf2b8-126">Тип</span><span class="sxs-lookup"><span data-stu-id="bf2b8-126">Type</span></span>    |  <span data-ttu-id="bf2b8-127">Описание</span><span class="sxs-lookup"><span data-stu-id="bf2b8-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf2b8-128">roleId</span><span class="sxs-lookup"><span data-stu-id="bf2b8-128">roleId</span></span>|<span data-ttu-id="bf2b8-129">String</span><span class="sxs-lookup"><span data-stu-id="bf2b8-129">String</span></span>|<span data-ttu-id="bf2b8-130">Идентификатор роли.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-130">The ID of the role.</span></span> <span data-ttu-id="bf2b8-131">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-131">Required.</span></span>|
|<span data-ttu-id="bf2b8-132">type</span><span class="sxs-lookup"><span data-stu-id="bf2b8-132">type</span></span>|<span data-ttu-id="bf2b8-133">String</span><span class="sxs-lookup"><span data-stu-id="bf2b8-133">String</span></span>|<span data-ttu-id="bf2b8-134">Представляет тип операции в назначении ролей.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-134">Represents the the type of the operation on the role assignment.</span></span> <span data-ttu-id="bf2b8-135">Значение может быть `AdminAdd`: администраторам Добавление пользователей в роли. `UserAdd`: Добавление назначений ролей пользователей.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-135">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span> <span data-ttu-id="bf2b8-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-136">Required.</span></span>|
|<span data-ttu-id="bf2b8-137">assignmentState</span><span class="sxs-lookup"><span data-stu-id="bf2b8-137">assignmentState</span></span>|<span data-ttu-id="bf2b8-138">String</span><span class="sxs-lookup"><span data-stu-id="bf2b8-138">String</span></span>|<span data-ttu-id="bf2b8-139">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-139">The state of the assignment.</span></span> <span data-ttu-id="bf2b8-140">Значение может быть `Eligible` подходящими назначения `Active` - если она назначена непосредственно `Active` администраторами, или активируемого на допустимость назначения для пользователей.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-140">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span> <span data-ttu-id="bf2b8-141">Возможные значения: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-141">Possible values are: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span></span> <span data-ttu-id="bf2b8-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-142">Required.</span></span>|
|<span data-ttu-id="bf2b8-143">Reason</span><span class="sxs-lookup"><span data-stu-id="bf2b8-143">reason</span></span>|<span data-ttu-id="bf2b8-144">String</span><span class="sxs-lookup"><span data-stu-id="bf2b8-144">String</span></span>|<span data-ttu-id="bf2b8-145">Причину должно предоставляться для запроса назначений ролей для аудита и предварительный просмотр цели.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-145">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="bf2b8-146">Расписание</span><span class="sxs-lookup"><span data-stu-id="bf2b8-146">schedule</span></span>|[<span data-ttu-id="bf2b8-147">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="bf2b8-147">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="bf2b8-148">Расписание для запроса назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-148">The schedule of the role assignment request.</span></span>|

## <a name="response"></a><span data-ttu-id="bf2b8-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="bf2b8-149">Response</span></span>
<span data-ttu-id="bf2b8-150">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-150">If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="bf2b8-151">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="bf2b8-151">Error codes</span></span>
<span data-ttu-id="bf2b8-152">Этот интерфейс API возвращает этому стандарту коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-152">This API returns that standard HTTP error codes.</span></span> <span data-ttu-id="bf2b8-153">Кроме того он может вернуть коды ошибок, перечисленных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-153">In addition, it can return the error codes listed in the following table.</span></span>

|<span data-ttu-id="bf2b8-154">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="bf2b8-154">Error code</span></span>     | <span data-ttu-id="bf2b8-155">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="bf2b8-155">Error message</span></span>              | 
|:--------------------| :---------------------|
| <span data-ttu-id="bf2b8-156">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="bf2b8-156">400 BadRequest</span></span> | <span data-ttu-id="bf2b8-157">Свойство RoleAssignmentRequest был равен NULL</span><span class="sxs-lookup"><span data-stu-id="bf2b8-157">RoleAssignmentRequest property was NULL</span></span> |
| <span data-ttu-id="bf2b8-158">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="bf2b8-158">400 BadRequest</span></span> | <span data-ttu-id="bf2b8-159">Не удается десериализации roleAssignmentRequest объекта.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-159">Unable to deserialize roleAssignmentRequest Object.</span></span> |
| <span data-ttu-id="bf2b8-160">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="bf2b8-160">400 BadRequest</span></span> | <span data-ttu-id="bf2b8-161">RoleId является обязательным.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-161">RoleId is required.</span></span> |
| <span data-ttu-id="bf2b8-162">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="bf2b8-162">400 BadRequest</span></span> | <span data-ttu-id="bf2b8-163">Дата начала расписания должен быть указан и должен быть больше, чем сейчас.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-163">Schedule start date must be specified and should be greater than Now.</span></span> |
| <span data-ttu-id="bf2b8-164">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="bf2b8-164">400 BadRequest</span></span> | <span data-ttu-id="bf2b8-165">Расписание для этого типа пользователей, ролей и расписание уже существует.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-165">A schedule already exists for this user, role and schedule type.</span></span> |
| <span data-ttu-id="bf2b8-166">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="bf2b8-166">400 BadRequest</span></span> | <span data-ttu-id="bf2b8-167">Обновление, ожидающее утверждения уже существует для этого типа пользователей, ролей и утверждения.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-167">A pending approval already exists for this user, role and approval type.</span></span> |
| <span data-ttu-id="bf2b8-168">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="bf2b8-168">400 BadRequest</span></span> | <span data-ttu-id="bf2b8-169">Запросившая сторона причину, отсутствует.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-169">Requestor reason is missing.</span></span> |
| <span data-ttu-id="bf2b8-170">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="bf2b8-170">400 BadRequest</span></span> | <span data-ttu-id="bf2b8-171">Запросившая сторона причина должна быть не более 500 символов.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-171">Requestor reason should be less than 500 characters.</span></span> |
| <span data-ttu-id="bf2b8-172">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="bf2b8-172">400 BadRequest</span></span> | <span data-ttu-id="bf2b8-173">Несанкционированное получение длительность должна быть между 0,5 и {из параметра}.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-173">Elevation duration must be between 0.5 and {from setting}.</span></span> |
| <span data-ttu-id="bf2b8-174">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="bf2b8-174">400 BadRequest</span></span> | <span data-ttu-id="bf2b8-175">Существует перекрытия запланированного активации и запрос.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-175">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="bf2b8-176">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="bf2b8-176">400 BadRequest</span></span> | <span data-ttu-id="bf2b8-177">Роль уже активировано.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-177">The role is already activated.</span></span> |
| <span data-ttu-id="bf2b8-178">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="bf2b8-178">400 BadRequest</span></span> | <span data-ttu-id="bf2b8-179">GenericElevateUserToRoleAssignments: Tickting сведения необходимо и не указано в процессе активации.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-179">GenericElevateUserToRoleAssignments: Tickting information is required and not supplied in the activation process.</span></span> |
| <span data-ttu-id="bf2b8-180">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="bf2b8-180">400 BadRequest</span></span> | <span data-ttu-id="bf2b8-181">Существует перекрытия запланированного активации и запрос.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-181">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="bf2b8-182">403 доступ запрещен</span><span class="sxs-lookup"><span data-stu-id="bf2b8-182">403 UnAuthorized</span></span> | <span data-ttu-id="bf2b8-183">Несанкционированное получение требуется многофакторная проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-183">Elevation requires Multi-Factor Authentication.</span></span> |
| <span data-ttu-id="bf2b8-184">403 доступ запрещен</span><span class="sxs-lookup"><span data-stu-id="bf2b8-184">403 UnAuthorized</span></span> | <span data-ttu-id="bf2b8-185">От имени повышения прав не допускается.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-185">On behalf of elevation is not allowed.</span></span> |

## <a name="example"></a><span data-ttu-id="bf2b8-186">Пример</span><span class="sxs-lookup"><span data-stu-id="bf2b8-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bf2b8-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf2b8-187">Request</span></span>
<span data-ttu-id="bf2b8-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-188">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="bf2b8-189">Ответ</span><span class="sxs-lookup"><span data-stu-id="bf2b8-189">Response</span></span>
<span data-ttu-id="bf2b8-190">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-190">The following is an example of the response.</span></span> <span data-ttu-id="bf2b8-191">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-191">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bf2b8-192">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bf2b8-192">All of the properties will be returned from an actual call.</span></span>
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
    "userId": "Self"，
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
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
