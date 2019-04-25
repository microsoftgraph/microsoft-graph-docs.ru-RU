---
title: Создание Привилежедролеассигнментрекуест
description: Создание объекта привилежедролеассигнментрекуест.
localization_priority: Normal
ms.openlocfilehash: e3158e918d061f09dec9e74c9e3bfd66d95fa48d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538654"
---
# <a name="create-privilegedroleassignmentrequest"></a><span data-ttu-id="34030-103">Создание Привилежедролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="34030-103">Create privilegedRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34030-104">Создание объекта [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="34030-104">Create a [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="34030-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="34030-105">Permissions</span></span>
<span data-ttu-id="34030-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34030-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34030-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34030-108">Permission type</span></span>                        | <span data-ttu-id="34030-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="34030-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="34030-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34030-110">Delegated (work or school account)</span></span> | <span data-ttu-id="34030-111">Привилежедакцесс. ReadWrite. AzureAD, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="34030-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="34030-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34030-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34030-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34030-113">Not supported.</span></span> |
|<span data-ttu-id="34030-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34030-114">Application</span></span>                            | <span data-ttu-id="34030-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34030-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="34030-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34030-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="34030-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34030-117">Request headers</span></span>
| <span data-ttu-id="34030-118">Имя</span><span class="sxs-lookup"><span data-stu-id="34030-118">Name</span></span>      |<span data-ttu-id="34030-119">Описание</span><span class="sxs-lookup"><span data-stu-id="34030-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="34030-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="34030-120">Authorization</span></span>  | <span data-ttu-id="34030-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34030-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="34030-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34030-123">Request body</span></span>
<span data-ttu-id="34030-124">В тексте запроса добавьте представление объекта [Привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34030-124">In the request body, supply a JSON representation of [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="34030-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="34030-125">Property</span></span>     | <span data-ttu-id="34030-126">Тип</span><span class="sxs-lookup"><span data-stu-id="34030-126">Type</span></span>    |  <span data-ttu-id="34030-127">Описание</span><span class="sxs-lookup"><span data-stu-id="34030-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34030-128">roleId</span><span class="sxs-lookup"><span data-stu-id="34030-128">roleId</span></span>|<span data-ttu-id="34030-129">String</span><span class="sxs-lookup"><span data-stu-id="34030-129">String</span></span>|<span data-ttu-id="34030-130">Идентификатор роли.</span><span class="sxs-lookup"><span data-stu-id="34030-130">The ID of the role.</span></span> <span data-ttu-id="34030-131">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="34030-131">Required.</span></span>|
|<span data-ttu-id="34030-132">type</span><span class="sxs-lookup"><span data-stu-id="34030-132">type</span></span>|<span data-ttu-id="34030-133">String</span><span class="sxs-lookup"><span data-stu-id="34030-133">String</span></span>|<span data-ttu-id="34030-134">Представляет тип операции для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="34030-134">Represents the the type of the operation on the role assignment.</span></span> <span data-ttu-id="34030-135">Возможные значения `AdminAdd`: Администраторы Add Users to Roles; `UserAdd`: Пользователи добавляют назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="34030-135">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span> <span data-ttu-id="34030-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34030-136">Required.</span></span>|
|<span data-ttu-id="34030-137">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="34030-137">assignmentState</span></span>|<span data-ttu-id="34030-138">String</span><span class="sxs-lookup"><span data-stu-id="34030-138">String</span></span>|<span data-ttu-id="34030-139">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="34030-139">The state of the assignment.</span></span> <span data-ttu-id="34030-140">Значение может быть `Eligible` для правого назначения `Active` , если оно напрямую назначено `Active` администраторами или активировано в соответствии с подходящими пользователями.</span><span class="sxs-lookup"><span data-stu-id="34030-140">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span> <span data-ttu-id="34030-141">Возможные значения: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span><span class="sxs-lookup"><span data-stu-id="34030-141">Possible values are: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span></span> <span data-ttu-id="34030-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34030-142">Required.</span></span>|
|<span data-ttu-id="34030-143">причиной</span><span class="sxs-lookup"><span data-stu-id="34030-143">reason</span></span>|<span data-ttu-id="34030-144">String</span><span class="sxs-lookup"><span data-stu-id="34030-144">String</span></span>|<span data-ttu-id="34030-145">Необходимо указать причину для запроса на назначение роли для аудита и проверки.</span><span class="sxs-lookup"><span data-stu-id="34030-145">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="34030-146">Диспетчер</span><span class="sxs-lookup"><span data-stu-id="34030-146">schedule</span></span>|[<span data-ttu-id="34030-147">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="34030-147">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="34030-148">Расписание запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="34030-148">The schedule of the role assignment request.</span></span>|

## <a name="response"></a><span data-ttu-id="34030-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="34030-149">Response</span></span>
<span data-ttu-id="34030-150">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="34030-150">If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="34030-151">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="34030-151">Error codes</span></span>
<span data-ttu-id="34030-152">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="34030-152">This API returns that standard HTTP error codes.</span></span> <span data-ttu-id="34030-153">Кроме того, он может возвращать коды ошибок, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="34030-153">In addition, it can return the error codes listed in the following table.</span></span>

|<span data-ttu-id="34030-154">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="34030-154">Error code</span></span>     | <span data-ttu-id="34030-155">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="34030-155">Error message</span></span>              | 
|:--------------------| :---------------------|
| <span data-ttu-id="34030-156">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="34030-156">400 BadRequest</span></span> | <span data-ttu-id="34030-157">Свойство Ролеассигнментрекуест имеет значение NULL</span><span class="sxs-lookup"><span data-stu-id="34030-157">RoleAssignmentRequest property was NULL</span></span> |
| <span data-ttu-id="34030-158">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="34030-158">400 BadRequest</span></span> | <span data-ttu-id="34030-159">Не удается десериализовать объект Ролеассигнментрекуест.</span><span class="sxs-lookup"><span data-stu-id="34030-159">Unable to deserialize roleAssignmentRequest Object.</span></span> |
| <span data-ttu-id="34030-160">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="34030-160">400 BadRequest</span></span> | <span data-ttu-id="34030-161">RoleId является обязательным.</span><span class="sxs-lookup"><span data-stu-id="34030-161">RoleId is required.</span></span> |
| <span data-ttu-id="34030-162">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="34030-162">400 BadRequest</span></span> | <span data-ttu-id="34030-163">Дата начала расписания должна быть указана и должна быть больше, чем сейчас.</span><span class="sxs-lookup"><span data-stu-id="34030-163">Schedule start date must be specified and should be greater than Now.</span></span> |
| <span data-ttu-id="34030-164">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="34030-164">400 BadRequest</span></span> | <span data-ttu-id="34030-165">Расписание для этого пользователя, роли и типа расписания уже существует.</span><span class="sxs-lookup"><span data-stu-id="34030-165">A schedule already exists for this user, role and schedule type.</span></span> |
| <span data-ttu-id="34030-166">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="34030-166">400 BadRequest</span></span> | <span data-ttu-id="34030-167">Для этого пользователя, роли и типа утверждения уже существует ожидающее утверждение.</span><span class="sxs-lookup"><span data-stu-id="34030-167">A pending approval already exists for this user, role and approval type.</span></span> |
| <span data-ttu-id="34030-168">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="34030-168">400 BadRequest</span></span> | <span data-ttu-id="34030-169">Не указана причина запрашивающей стороны.</span><span class="sxs-lookup"><span data-stu-id="34030-169">Requestor reason is missing.</span></span> |
| <span data-ttu-id="34030-170">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="34030-170">400 BadRequest</span></span> | <span data-ttu-id="34030-171">Срок запрашивающего не должен быть меньше 500 символов.</span><span class="sxs-lookup"><span data-stu-id="34030-171">Requestor reason should be less than 500 characters.</span></span> |
| <span data-ttu-id="34030-172">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="34030-172">400 BadRequest</span></span> | <span data-ttu-id="34030-173">Длительность возвышения должна быть между 0,5 и {from Setting}.</span><span class="sxs-lookup"><span data-stu-id="34030-173">Elevation duration must be between 0.5 and {from setting}.</span></span> |
| <span data-ttu-id="34030-174">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="34030-174">400 BadRequest</span></span> | <span data-ttu-id="34030-175">Между запланированной активацией и запросом существует перекрытие.</span><span class="sxs-lookup"><span data-stu-id="34030-175">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="34030-176">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="34030-176">400 BadRequest</span></span> | <span data-ttu-id="34030-177">Роль уже активирована.</span><span class="sxs-lookup"><span data-stu-id="34030-177">The role is already activated.</span></span> |
| <span data-ttu-id="34030-178">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="34030-178">400 BadRequest</span></span> | <span data-ttu-id="34030-179">Женерицелеватеусерторолеассигнментс: Тикктинг сведения являются обязательными и не предоставляются в процессе активации.</span><span class="sxs-lookup"><span data-stu-id="34030-179">GenericElevateUserToRoleAssignments: Tickting information is required and not supplied in the activation process.</span></span> |
| <span data-ttu-id="34030-180">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="34030-180">400 BadRequest</span></span> | <span data-ttu-id="34030-181">Между запланированной активацией и запросом существует перекрытие.</span><span class="sxs-lookup"><span data-stu-id="34030-181">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="34030-182">403 авторизация</span><span class="sxs-lookup"><span data-stu-id="34030-182">403 UnAuthorized</span></span> | <span data-ttu-id="34030-183">Для повышения требуется многоФакторная проверка поДлинности.</span><span class="sxs-lookup"><span data-stu-id="34030-183">Elevation requires Multi-Factor Authentication.</span></span> |
| <span data-ttu-id="34030-184">403 авторизация</span><span class="sxs-lookup"><span data-stu-id="34030-184">403 UnAuthorized</span></span> | <span data-ttu-id="34030-185">От имени повышения прав не разрешено.</span><span class="sxs-lookup"><span data-stu-id="34030-185">On behalf of elevation is not allowed.</span></span> |

## <a name="example"></a><span data-ttu-id="34030-186">Пример</span><span class="sxs-lookup"><span data-stu-id="34030-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34030-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="34030-187">Request</span></span>
<span data-ttu-id="34030-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34030-188">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="34030-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="34030-189">Response</span></span>
<span data-ttu-id="34030-190">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="34030-190">The following is an example of the response.</span></span> <span data-ttu-id="34030-191">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="34030-191">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="34030-192">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="34030-192">All of the properties will be returned from an actual call.</span></span>
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
