---
title: Обновление unifiedRoleAssignmentScheduleRequest
description: Обновление свойств объекта unifiedRoleAssignmentScheduleRequest.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1afb8a42c0bb914655c198313cba1668ee8cda0b
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680404"
---
# <a name="update-unifiedroleassignmentschedulerequest"></a><span data-ttu-id="c0526-103">Обновление unifiedRoleAssignmentScheduleRequest</span><span class="sxs-lookup"><span data-stu-id="c0526-103">Update unifiedRoleAssignmentScheduleRequest</span></span>
<span data-ttu-id="c0526-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0526-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0526-105">Обновление свойств объекта [unifiedRoleAssignmentScheduleRequest.](../resources/unifiedroleassignmentschedulerequest.md)</span><span class="sxs-lookup"><span data-stu-id="c0526-105">Update the properties of an [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0526-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0526-106">Permissions</span></span>
<span data-ttu-id="c0526-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0526-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0526-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0526-109">Permission type</span></span>|<span data-ttu-id="c0526-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0526-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0526-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0526-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c0526-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="c0526-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="c0526-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0526-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0526-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c0526-114">Not supported</span></span>|
|<span data-ttu-id="c0526-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="c0526-115">Application</span></span>|<span data-ttu-id="c0526-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c0526-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0526-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0526-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}
```

## <a name="request-headers"></a><span data-ttu-id="c0526-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0526-118">Request headers</span></span>
|<span data-ttu-id="c0526-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c0526-119">Name</span></span>|<span data-ttu-id="c0526-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c0526-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c0526-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0526-121">Authorization</span></span>|<span data-ttu-id="c0526-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0526-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c0526-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c0526-124">Content-Type</span></span>|<span data-ttu-id="c0526-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0526-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0526-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0526-127">Request body</span></span>
<span data-ttu-id="c0526-128">В теле запроса поставляем представление JSON объекта [unifiedRoleAssignmentScheduleRequest.](../resources/unifiedroleassignmentschedulerequest.md)</span><span class="sxs-lookup"><span data-stu-id="c0526-128">In the request body, supply a JSON representation of the [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) object.</span></span>

<span data-ttu-id="c0526-129">В следующей таблице показаны свойства, необходимые при обновлении [единой системыRoleAssignmentScheduleRequest.](../resources/unifiedroleassignmentschedulerequest.md)</span><span class="sxs-lookup"><span data-stu-id="c0526-129">The following table shows the properties that are required when you update the [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md).</span></span>

|<span data-ttu-id="c0526-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0526-130">Property</span></span>|<span data-ttu-id="c0526-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c0526-131">Type</span></span>|<span data-ttu-id="c0526-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c0526-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0526-133">id</span><span class="sxs-lookup"><span data-stu-id="c0526-133">id</span></span>|<span data-ttu-id="c0526-134">String</span><span class="sxs-lookup"><span data-stu-id="c0526-134">String</span></span>|<span data-ttu-id="c0526-135">Уникальный идентификатор для unifiedRoleAssignmentScheduleRequest.</span><span class="sxs-lookup"><span data-stu-id="c0526-135">The unique identifier for the unifiedRoleAssignmentScheduleRequest.</span></span> <span data-ttu-id="c0526-136">Key, not nullable, Read-only.</span><span class="sxs-lookup"><span data-stu-id="c0526-136">Key, not nullable, Read-only.</span></span>|
|<span data-ttu-id="c0526-137">action</span><span class="sxs-lookup"><span data-stu-id="c0526-137">action</span></span>|<span data-ttu-id="c0526-138">String</span><span class="sxs-lookup"><span data-stu-id="c0526-138">String</span></span>|<span data-ttu-id="c0526-139">Представление типа операции при назначении ролей.</span><span class="sxs-lookup"><span data-stu-id="c0526-139">Representing the type of the operation on the role assignment.</span></span> <span data-ttu-id="c0526-140">Значение может быть</span><span class="sxs-lookup"><span data-stu-id="c0526-140">The value can be</span></span> <ul><li><span data-ttu-id="c0526-141">`AdminAdd`: Администраторы назначают пользователям и группам роли;</span><span class="sxs-lookup"><span data-stu-id="c0526-141">`AdminAdd`: Administrators assign users/groups to roles;</span></span></li><li><span data-ttu-id="c0526-142">`UserAdd`: Пользователи активируют подходящие назначения;</span><span class="sxs-lookup"><span data-stu-id="c0526-142">`UserAdd`: Users activate eligible assignments;</span></span></li><li> <span data-ttu-id="c0526-143">`AdminUpdate`: Администраторы изменяют существующие назначения ролей</span><span class="sxs-lookup"><span data-stu-id="c0526-143">`AdminUpdate`: Administrators change existing role assignments</span></span></li><li><span data-ttu-id="c0526-144">`AdminRemove`: Администраторы удаляют пользователей и группы из ролей;</span><span class="sxs-lookup"><span data-stu-id="c0526-144">`AdminRemove`: Administrators remove users/groups from roles;</span></span><li><span data-ttu-id="c0526-145">`UserRemove`: Пользователи деактивируют активные назначения;</span><span class="sxs-lookup"><span data-stu-id="c0526-145">`UserRemove`: Users deactivate active assignments;</span></span><li><span data-ttu-id="c0526-146">`UserExtend`: Пользователи просят продлить срок действия назначений;</span><span class="sxs-lookup"><span data-stu-id="c0526-146">`UserExtend`: Users request to extend their expiring assignments;</span></span></li><li><span data-ttu-id="c0526-147">`AdminExtend`. Администраторы расширяют назначения по истечении срока действия.</span><span class="sxs-lookup"><span data-stu-id="c0526-147">`AdminExtend`: Administrators extend expiring assignments.</span></span></li><li><span data-ttu-id="c0526-148">`UserRenew`: Пользователи просят продлить срок действия назначений;</span><span class="sxs-lookup"><span data-stu-id="c0526-148">`UserRenew`: Users request to renew their expired assignments;</span></span></li><li><span data-ttu-id="c0526-149">`AdminRenew`. Администраторы расширяют назначения по истечении срока действия.</span><span class="sxs-lookup"><span data-stu-id="c0526-149">`AdminRenew`: Administrators extend expiring assignments.</span></span></li></ul>|
|<span data-ttu-id="c0526-150">principalId</span><span class="sxs-lookup"><span data-stu-id="c0526-150">principalId</span></span>|<span data-ttu-id="c0526-151">String</span><span class="sxs-lookup"><span data-stu-id="c0526-151">String</span></span>|<span data-ttu-id="c0526-152">Объект объекта, которому предоставляется назначение.</span><span class="sxs-lookup"><span data-stu-id="c0526-152">Objectid of the principal to which the assignment is being granted to.</span></span>|
|<span data-ttu-id="c0526-153">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c0526-153">roleDefinitionId</span></span>|<span data-ttu-id="c0526-154">String</span><span class="sxs-lookup"><span data-stu-id="c0526-154">String</span></span>|<span data-ttu-id="c0526-155">ID унифицированногоRoleDefinition для назначения.</span><span class="sxs-lookup"><span data-stu-id="c0526-155">ID of the unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="c0526-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c0526-156">Read only.</span></span>|
|<span data-ttu-id="c0526-157">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="c0526-157">directoryScopeId</span></span>|<span data-ttu-id="c0526-158">String</span><span class="sxs-lookup"><span data-stu-id="c0526-158">String</span></span>|<span data-ttu-id="c0526-159">Id объекта каталога, представляющего область назначения.</span><span class="sxs-lookup"><span data-stu-id="c0526-159">Id of the directory object representing the scope of the assignment.</span></span> <span data-ttu-id="c0526-160">Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="c0526-160">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="c0526-161">Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям.</span><span class="sxs-lookup"><span data-stu-id="c0526-161">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="c0526-162">Области приложений — это области, которые определяются и понимаются только этим приложением.</span><span class="sxs-lookup"><span data-stu-id="c0526-162">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="c0526-163">appScopeId</span><span class="sxs-lookup"><span data-stu-id="c0526-163">appScopeId</span></span>|<span data-ttu-id="c0526-164">String</span><span class="sxs-lookup"><span data-stu-id="c0526-164">String</span></span>|<span data-ttu-id="c0526-165">Id конкретной области приложения, когда область назначения является конкретной.</span><span class="sxs-lookup"><span data-stu-id="c0526-165">Id of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="c0526-166">Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="c0526-166">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="c0526-167">Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям.</span><span class="sxs-lookup"><span data-stu-id="c0526-167">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="c0526-168">Используйте "/" для области для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0526-168">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="c0526-169">Области приложений — это области, которые определяются и понимаются только этим приложением.</span><span class="sxs-lookup"><span data-stu-id="c0526-169">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="c0526-170">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="c0526-170">isValidationOnly</span></span>|<span data-ttu-id="c0526-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0526-171">Boolean</span></span>|<span data-ttu-id="c0526-172">Boolean, определяющая, является ли вызов проверкой или фактическим вызовом.</span><span class="sxs-lookup"><span data-stu-id="c0526-172">A boolean that determines whether the call is a validation or an actual call.</span></span> <span data-ttu-id="c0526-173">Только задайте это свойство, если необходимо проверить, подчиняется ли активация дополнительным правилам, таким как MFA, перед отправкой запроса.</span><span class="sxs-lookup"><span data-stu-id="c0526-173">Only set this property if you want to check whether an activation is subject to additional rules like MFA before actually submitting the request.</span></span>|
|<span data-ttu-id="c0526-174">targetScheduleId</span><span class="sxs-lookup"><span data-stu-id="c0526-174">targetScheduleId</span></span>|<span data-ttu-id="c0526-175">String</span><span class="sxs-lookup"><span data-stu-id="c0526-175">String</span></span>|<span data-ttu-id="c0526-176">ID объекта расписания, прикрепленного к назначению.</span><span class="sxs-lookup"><span data-stu-id="c0526-176">ID of the schedule object attached to the assignment.</span></span>|
|<span data-ttu-id="c0526-177">обоснование</span><span class="sxs-lookup"><span data-stu-id="c0526-177">justification</span></span>|<span data-ttu-id="c0526-178">String</span><span class="sxs-lookup"><span data-stu-id="c0526-178">String</span></span>|<span data-ttu-id="c0526-179">Сообщение, предоставленное пользователями и администраторами при создании запроса о необходимости.</span><span class="sxs-lookup"><span data-stu-id="c0526-179">A message provided by users and administrators when create the request about why it is needed.</span></span>|
|<span data-ttu-id="c0526-180">scheduleInfo</span><span class="sxs-lookup"><span data-stu-id="c0526-180">scheduleInfo</span></span>|[<span data-ttu-id="c0526-181">requestSchedule</span><span class="sxs-lookup"><span data-stu-id="c0526-181">requestSchedule</span></span>](../resources/requestschedule.md)|<span data-ttu-id="c0526-182">Объект расписания запроса назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="c0526-182">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="c0526-183">ticketInfo</span><span class="sxs-lookup"><span data-stu-id="c0526-183">ticketInfo</span></span>|[<span data-ttu-id="c0526-184">ticketInfo</span><span class="sxs-lookup"><span data-stu-id="c0526-184">ticketInfo</span></span>](../resources/ticketinfo.md)|<span data-ttu-id="c0526-185">Объект ticketInfo, присоединенный к запросу назначения ролей, который включает сведения о номере билета и системе билетов.</span><span class="sxs-lookup"><span data-stu-id="c0526-185">The ticketInfo object attached to the role assignment request which includes details of the ticket number and ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="c0526-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0526-186">Response</span></span>

<span data-ttu-id="c0526-187">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c0526-187">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c0526-188">Примеры</span><span class="sxs-lookup"><span data-stu-id="c0526-188">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c0526-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0526-189">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c0526-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0526-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroleassignmentschedulerequest"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}
Content-Type: application/json
Content-length: 466

{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentScheduleRequest",
  "action": "String",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "isValidationOnly": "Boolean",
  "targetScheduleId": "String",
  "justification": "String",
  "scheduleInfo": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "ticketInfo": {
    "@odata.type": "microsoft.graph.ticketInfo"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="c0526-191">C#</span><span class="sxs-lookup"><span data-stu-id="c0526-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroleassignmentschedulerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0526-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0526-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroleassignmentschedulerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0526-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0526-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroleassignmentschedulerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0526-194">Java</span><span class="sxs-lookup"><span data-stu-id="c0526-194">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroleassignmentschedulerequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c0526-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0526-195">Response</span></span>
<span data-ttu-id="c0526-196">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c0526-196">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleRequest"
}
-->
```http
HTTP/1.1 204 OK

```

<!--
{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentScheduleRequest",
  "id": "c13ee236-e236-c13e-36e2-3ec136e23ec1",
  "action": "String",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "isValidationOnly": "Boolean",
  "targetScheduleId": "String",
  "justification": "String",
  "scheduleInfo": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "ticketInfo": {
    "@odata.type": "microsoft.graph.ticketInfo"
  }
}
```-->

