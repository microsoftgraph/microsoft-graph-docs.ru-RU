---
title: Создание privilegedRoleAssignmentRequest
description: Создайте объект privilegedroleassignmentrequest.
ms.openlocfilehash: e262682b5a5e8bffa7fb089ae783f3bb7e67803c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078737"
---
# <a name="create-privilegedroleassignmentrequest"></a><span data-ttu-id="91bbc-103">Создание privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="91bbc-103">Create privilegedRoleAssignmentRequest</span></span>

> <span data-ttu-id="91bbc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="91bbc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91bbc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91bbc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91bbc-106">Создайте объект [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="91bbc-106">Create a [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="91bbc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91bbc-107">Permissions</span></span>
<span data-ttu-id="91bbc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91bbc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91bbc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91bbc-110">Permission type</span></span>                        | <span data-ttu-id="91bbc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91bbc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="91bbc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91bbc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="91bbc-113">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="91bbc-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="91bbc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91bbc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91bbc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91bbc-115">Not supported.</span></span> |
|<span data-ttu-id="91bbc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91bbc-116">Application</span></span>                            | <span data-ttu-id="91bbc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91bbc-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="91bbc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91bbc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="91bbc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91bbc-119">Request headers</span></span>
| <span data-ttu-id="91bbc-120">Имя</span><span class="sxs-lookup"><span data-stu-id="91bbc-120">Name</span></span>      |<span data-ttu-id="91bbc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="91bbc-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="91bbc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91bbc-122">Authorization</span></span>  | <span data-ttu-id="91bbc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91bbc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91bbc-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91bbc-125">Request body</span></span>
<span data-ttu-id="91bbc-126">В тексте запроса укажите представление JSON объекта [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="91bbc-126">In the request body, supply a JSON representation of [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="91bbc-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="91bbc-127">Property</span></span>     | <span data-ttu-id="91bbc-128">Тип</span><span class="sxs-lookup"><span data-stu-id="91bbc-128">Type</span></span>    |  <span data-ttu-id="91bbc-129">Description</span><span class="sxs-lookup"><span data-stu-id="91bbc-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91bbc-130">roleId</span><span class="sxs-lookup"><span data-stu-id="91bbc-130">roleId</span></span>|<span data-ttu-id="91bbc-131">String</span><span class="sxs-lookup"><span data-stu-id="91bbc-131">String</span></span>|<span data-ttu-id="91bbc-132">Идентификатор роли.</span><span class="sxs-lookup"><span data-stu-id="91bbc-132">The ID of the role.</span></span> <span data-ttu-id="91bbc-133">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="91bbc-133">Required.</span></span>|
|<span data-ttu-id="91bbc-134">type</span><span class="sxs-lookup"><span data-stu-id="91bbc-134">type</span></span>|<span data-ttu-id="91bbc-135">String</span><span class="sxs-lookup"><span data-stu-id="91bbc-135">String</span></span>|<span data-ttu-id="91bbc-136">Представляет тип операции в назначении ролей.</span><span class="sxs-lookup"><span data-stu-id="91bbc-136">Represents the the type of the operation on the role assignment.</span></span> <span data-ttu-id="91bbc-137">Значение может быть `AdminAdd`: администраторам Добавление пользователей в роли. `UserAdd`: Добавление назначений ролей пользователей.</span><span class="sxs-lookup"><span data-stu-id="91bbc-137">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span> <span data-ttu-id="91bbc-138">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="91bbc-138">Required.</span></span>|
|<span data-ttu-id="91bbc-139">assignmentState</span><span class="sxs-lookup"><span data-stu-id="91bbc-139">assignmentState</span></span>|<span data-ttu-id="91bbc-140">String</span><span class="sxs-lookup"><span data-stu-id="91bbc-140">String</span></span>|<span data-ttu-id="91bbc-141">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="91bbc-141">The state of the assignment.</span></span> <span data-ttu-id="91bbc-142">Значение может быть `Eligible` подходящими назначения `Active` - если она назначена непосредственно `Active` администраторами, или активируемого на допустимость назначения для пользователей.</span><span class="sxs-lookup"><span data-stu-id="91bbc-142">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span> <span data-ttu-id="91bbc-143">Возможные значения: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span><span class="sxs-lookup"><span data-stu-id="91bbc-143">Possible values are: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span></span> <span data-ttu-id="91bbc-144">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="91bbc-144">Required.</span></span>|
|<span data-ttu-id="91bbc-145">Причина</span><span class="sxs-lookup"><span data-stu-id="91bbc-145">reason</span></span>|<span data-ttu-id="91bbc-146">String</span><span class="sxs-lookup"><span data-stu-id="91bbc-146">String</span></span>|<span data-ttu-id="91bbc-147">Причину должно предоставляться для запроса назначений ролей для аудита и предварительный просмотр цели.</span><span class="sxs-lookup"><span data-stu-id="91bbc-147">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="91bbc-148">расписание</span><span class="sxs-lookup"><span data-stu-id="91bbc-148">schedule</span></span>|[<span data-ttu-id="91bbc-149">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="91bbc-149">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="91bbc-150">Расписание для запроса назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="91bbc-150">The schedule of the role assignment request.</span></span>|

## <a name="response"></a><span data-ttu-id="91bbc-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="91bbc-151">Response</span></span>
<span data-ttu-id="91bbc-152">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="91bbc-152">If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="91bbc-153">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="91bbc-153">Error codes</span></span>
<span data-ttu-id="91bbc-154">Этот интерфейс API возвращает этому стандарту коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="91bbc-154">This API returns that standard HTTP error codes.</span></span> <span data-ttu-id="91bbc-155">Кроме того он может вернуть коды ошибок, перечисленных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="91bbc-155">In addition, it can return the error codes listed in the following table.</span></span>

|<span data-ttu-id="91bbc-156">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="91bbc-156">Error code</span></span>     | <span data-ttu-id="91bbc-157">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="91bbc-157">Error message</span></span>              | 
|:--------------------| :---------------------|
| <span data-ttu-id="91bbc-158">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="91bbc-158">400 BadRequest</span></span> | <span data-ttu-id="91bbc-159">Свойство RoleAssignmentRequest был равен NULL</span><span class="sxs-lookup"><span data-stu-id="91bbc-159">RoleAssignmentRequest property was NULL</span></span> |
| <span data-ttu-id="91bbc-160">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="91bbc-160">400 BadRequest</span></span> | <span data-ttu-id="91bbc-161">Не удается десериализации roleAssignmentRequest объекта.</span><span class="sxs-lookup"><span data-stu-id="91bbc-161">Unable to deserialize roleAssignmentRequest Object.</span></span> |
| <span data-ttu-id="91bbc-162">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="91bbc-162">400 BadRequest</span></span> | <span data-ttu-id="91bbc-163">RoleId является обязательным.</span><span class="sxs-lookup"><span data-stu-id="91bbc-163">RoleId is required.</span></span> |
| <span data-ttu-id="91bbc-164">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="91bbc-164">400 BadRequest</span></span> | <span data-ttu-id="91bbc-165">Дата начала расписания должен быть указан и должен быть больше, чем сейчас.</span><span class="sxs-lookup"><span data-stu-id="91bbc-165">Schedule start date must be specified and should be greater than Now.</span></span> |
| <span data-ttu-id="91bbc-166">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="91bbc-166">400 BadRequest</span></span> | <span data-ttu-id="91bbc-167">Расписание для этого типа пользователей, ролей и расписание уже существует.</span><span class="sxs-lookup"><span data-stu-id="91bbc-167">A schedule already exists for this user, role and schedule type.</span></span> |
| <span data-ttu-id="91bbc-168">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="91bbc-168">400 BadRequest</span></span> | <span data-ttu-id="91bbc-169">Обновление, ожидающее утверждения уже существует для этого типа пользователей, ролей и утверждения.</span><span class="sxs-lookup"><span data-stu-id="91bbc-169">A pending approval already exists for this user, role and approval type.</span></span> |
| <span data-ttu-id="91bbc-170">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="91bbc-170">400 BadRequest</span></span> | <span data-ttu-id="91bbc-171">Запросившая сторона причину, отсутствует.</span><span class="sxs-lookup"><span data-stu-id="91bbc-171">Requestor reason is missing.</span></span> |
| <span data-ttu-id="91bbc-172">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="91bbc-172">400 BadRequest</span></span> | <span data-ttu-id="91bbc-173">Запросившая сторона причина должна быть не более 500 символов.</span><span class="sxs-lookup"><span data-stu-id="91bbc-173">Requestor reason should be less than 500 characters.</span></span> |
| <span data-ttu-id="91bbc-174">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="91bbc-174">400 BadRequest</span></span> | <span data-ttu-id="91bbc-175">Несанкционированное получение длительность должна быть между 0,5 и {из параметра}.</span><span class="sxs-lookup"><span data-stu-id="91bbc-175">Elevation duration must be between 0.5 and {from setting}.</span></span> |
| <span data-ttu-id="91bbc-176">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="91bbc-176">400 BadRequest</span></span> | <span data-ttu-id="91bbc-177">Существует перекрытия запланированного активации и запрос.</span><span class="sxs-lookup"><span data-stu-id="91bbc-177">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="91bbc-178">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="91bbc-178">400 BadRequest</span></span> | <span data-ttu-id="91bbc-179">Роль уже активировано.</span><span class="sxs-lookup"><span data-stu-id="91bbc-179">The role is already activated.</span></span> |
| <span data-ttu-id="91bbc-180">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="91bbc-180">400 BadRequest</span></span> | <span data-ttu-id="91bbc-181">GenericElevateUserToRoleAssignments: Tickting сведения необходимо и не указано в процессе активации.</span><span class="sxs-lookup"><span data-stu-id="91bbc-181">GenericElevateUserToRoleAssignments: Tickting information is required and not supplied in the activation process.</span></span> |
| <span data-ttu-id="91bbc-182">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="91bbc-182">400 BadRequest</span></span> | <span data-ttu-id="91bbc-183">Существует перекрытия запланированного активации и запрос.</span><span class="sxs-lookup"><span data-stu-id="91bbc-183">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="91bbc-184">403 доступ запрещен</span><span class="sxs-lookup"><span data-stu-id="91bbc-184">403 UnAuthorized</span></span> | <span data-ttu-id="91bbc-185">Несанкционированное получение требуется многофакторная проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="91bbc-185">Elevation requires Multi-Factor Authentication.</span></span> |
| <span data-ttu-id="91bbc-186">403 доступ запрещен</span><span class="sxs-lookup"><span data-stu-id="91bbc-186">403 UnAuthorized</span></span> | <span data-ttu-id="91bbc-187">От имени повышения прав не допускается.</span><span class="sxs-lookup"><span data-stu-id="91bbc-187">On behalf of elevation is not allowed.</span></span> |

## <a name="example"></a><span data-ttu-id="91bbc-188">Пример</span><span class="sxs-lookup"><span data-stu-id="91bbc-188">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91bbc-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="91bbc-189">Request</span></span>
<span data-ttu-id="91bbc-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91bbc-190">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="91bbc-191">Ответ</span><span class="sxs-lookup"><span data-stu-id="91bbc-191">Response</span></span>
<span data-ttu-id="91bbc-192">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="91bbc-192">The following is an example of the response.</span></span> <span data-ttu-id="91bbc-193">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="91bbc-193">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="91bbc-194">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="91bbc-194">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Post privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
