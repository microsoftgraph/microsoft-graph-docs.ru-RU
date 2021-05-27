---
title: Обновление unifiedRoleEligibilityScheduleRequest
description: Обновление свойств объекта unifiedRoleEligibilityScheduleRequest.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d5b39a4c10f077ff71c2e8288000efe76c83f655
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682371"
---
# <a name="update-unifiedroleeligibilityschedulerequest"></a><span data-ttu-id="e7f2a-103">Обновление unifiedRoleEligibilityScheduleRequest</span><span class="sxs-lookup"><span data-stu-id="e7f2a-103">Update unifiedRoleEligibilityScheduleRequest</span></span>
<span data-ttu-id="e7f2a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7f2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7f2a-105">Обновление свойств объекта [unifiedRoleEligibilityScheduleRequest.](../resources/unifiedroleeligibilityschedulerequest.md)</span><span class="sxs-lookup"><span data-stu-id="e7f2a-105">Update the properties of an [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7f2a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e7f2a-106">Permissions</span></span>
<span data-ttu-id="e7f2a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7f2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7f2a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7f2a-109">Permission type</span></span>|<span data-ttu-id="e7f2a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7f2a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7f2a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7f2a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e7f2a-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="e7f2a-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="e7f2a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7f2a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7f2a-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e7f2a-114">Not supported</span></span>|
|<span data-ttu-id="e7f2a-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="e7f2a-115">Application</span></span>|<span data-ttu-id="e7f2a-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e7f2a-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7f2a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7f2a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}
```

## <a name="request-headers"></a><span data-ttu-id="e7f2a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7f2a-118">Request headers</span></span>
|<span data-ttu-id="e7f2a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e7f2a-119">Name</span></span>|<span data-ttu-id="e7f2a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e7f2a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e7f2a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e7f2a-121">Authorization</span></span>|<span data-ttu-id="e7f2a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e7f2a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e7f2a-124">Content-Type</span></span>|<span data-ttu-id="e7f2a-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7f2a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e7f2a-127">Request body</span></span>
<span data-ttu-id="e7f2a-128">В теле запроса поставляем представление JSON объекта [unifiedRoleEligibilityScheduleRequest.](../resources/unifiedroleeligibilityschedulerequest.md)</span><span class="sxs-lookup"><span data-stu-id="e7f2a-128">In the request body, supply a JSON representation of the [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) object.</span></span>

<span data-ttu-id="e7f2a-129">В следующей таблице показаны свойства, необходимые при обновлении [единой системыRoleEligibilityScheduleRequest.](../resources/unifiedroleeligibilityschedulerequest.md)</span><span class="sxs-lookup"><span data-stu-id="e7f2a-129">The following table shows the properties that are required when you update the [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md).</span></span>

|<span data-ttu-id="e7f2a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7f2a-130">Property</span></span>|<span data-ttu-id="e7f2a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e7f2a-131">Type</span></span>|<span data-ttu-id="e7f2a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e7f2a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7f2a-133">id</span><span class="sxs-lookup"><span data-stu-id="e7f2a-133">id</span></span>|<span data-ttu-id="e7f2a-134">String</span><span class="sxs-lookup"><span data-stu-id="e7f2a-134">String</span></span>|<span data-ttu-id="e7f2a-135">Уникальный идентификатор для unifiedRoleEligibilityScheduleRequest.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-135">The unique identifier for the unifiedRoleEligibilityScheduleRequest.</span></span> <span data-ttu-id="e7f2a-136">Key, not nullable, Read-only</span><span class="sxs-lookup"><span data-stu-id="e7f2a-136">Key, not nullable, Read-only</span></span>|
|<span data-ttu-id="e7f2a-137">action</span><span class="sxs-lookup"><span data-stu-id="e7f2a-137">action</span></span>|<span data-ttu-id="e7f2a-138">String</span><span class="sxs-lookup"><span data-stu-id="e7f2a-138">String</span></span>|<span data-ttu-id="e7f2a-139">Представление типа операции при назначении ролей.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-139">Representing the type of the operation on the role assignment.</span></span> <span data-ttu-id="e7f2a-140">Значение может быть</span><span class="sxs-lookup"><span data-stu-id="e7f2a-140">The value can be</span></span> <ul><li><span data-ttu-id="e7f2a-141">`AdminAdd`: Администраторы назначают пользователям и группам роли;</span><span class="sxs-lookup"><span data-stu-id="e7f2a-141">`AdminAdd`: Administrators assign users/groups to roles;</span></span></li><li><span data-ttu-id="e7f2a-142">`UserAdd`: Пользователи активируют подходящие назначения;</span><span class="sxs-lookup"><span data-stu-id="e7f2a-142">`UserAdd`: Users activate eligible assignments;</span></span></li><li> <span data-ttu-id="e7f2a-143">`AdminUpdate`: Администраторы изменяют существующие назначения ролей</span><span class="sxs-lookup"><span data-stu-id="e7f2a-143">`AdminUpdate`: Administrators change existing role assignments</span></span></li><li><span data-ttu-id="e7f2a-144">`AdminRemove`: Администраторы удаляют пользователей и группы из ролей;</span><span class="sxs-lookup"><span data-stu-id="e7f2a-144">`AdminRemove`: Administrators remove users/groups from roles;</span></span><li><span data-ttu-id="e7f2a-145">`UserRemove`: Пользователи деактивируют активные назначения;</span><span class="sxs-lookup"><span data-stu-id="e7f2a-145">`UserRemove`: Users deactivate active assignments;</span></span><li><span data-ttu-id="e7f2a-146">`UserExtend`: Пользователи просят продлить срок действия назначений;</span><span class="sxs-lookup"><span data-stu-id="e7f2a-146">`UserExtend`: Users request to extend their expiring assignments;</span></span></li><li><span data-ttu-id="e7f2a-147">`AdminExtend`. Администраторы расширяют назначения по истечении срока действия.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-147">`AdminExtend`: Administrators extend expiring assignments.</span></span></li><li><span data-ttu-id="e7f2a-148">`UserRenew`: Пользователи просят продлить срок действия назначений;</span><span class="sxs-lookup"><span data-stu-id="e7f2a-148">`UserRenew`: Users request to renew their expired assignments;</span></span></li><li><span data-ttu-id="e7f2a-149">`AdminRenew`. Администраторы расширяют назначения по истечении срока действия.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-149">`AdminRenew`: Administrators extend expiring assignments.</span></span></li></ul>|
|<span data-ttu-id="e7f2a-150">principalId</span><span class="sxs-lookup"><span data-stu-id="e7f2a-150">principalId</span></span>|<span data-ttu-id="e7f2a-151">String</span><span class="sxs-lookup"><span data-stu-id="e7f2a-151">String</span></span>|<span data-ttu-id="e7f2a-152">Объект объекта, которому предоставляется назначение.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-152">Objectid of the principal to which the assignment is being granted to.</span></span>|
|<span data-ttu-id="e7f2a-153">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="e7f2a-153">roleDefinitionId</span></span>|<span data-ttu-id="e7f2a-154">String</span><span class="sxs-lookup"><span data-stu-id="e7f2a-154">String</span></span>|<span data-ttu-id="e7f2a-155">ID унифицированногоRoleDefinition для назначения.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-155">ID of the unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="e7f2a-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-156">Read only.</span></span>|
|<span data-ttu-id="e7f2a-157">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="e7f2a-157">directoryScopeId</span></span>|<span data-ttu-id="e7f2a-158">String</span><span class="sxs-lookup"><span data-stu-id="e7f2a-158">String</span></span>|<span data-ttu-id="e7f2a-159">Id объекта каталога, представляющего область назначения.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-159">Id of the directory object representing the scope of the assignment.</span></span> <span data-ttu-id="e7f2a-160">Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-160">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="e7f2a-161">Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-161">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="e7f2a-162">Области приложений — это области, которые определяются и понимаются только этим приложением.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-162">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="e7f2a-163">appScopeId</span><span class="sxs-lookup"><span data-stu-id="e7f2a-163">appScopeId</span></span>|<span data-ttu-id="e7f2a-164">String</span><span class="sxs-lookup"><span data-stu-id="e7f2a-164">String</span></span>|<span data-ttu-id="e7f2a-165">Id конкретной области приложения, когда область назначения является конкретной.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-165">Id of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="e7f2a-166">Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-166">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="e7f2a-167">Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-167">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="e7f2a-168">Используйте "/" для области для клиента.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-168">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="e7f2a-169">Области приложений — это области, которые определяются и понимаются только этим приложением.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-169">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="e7f2a-170">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="e7f2a-170">isValidationOnly</span></span>|<span data-ttu-id="e7f2a-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7f2a-171">Boolean</span></span>|<span data-ttu-id="e7f2a-172">Boolean, определяющая, является ли вызов проверкой или фактическим вызовом.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-172">A boolean that determines whether the call is a validation or an actual call.</span></span> <span data-ttu-id="e7f2a-173">Только задайте это свойство, если необходимо проверить, подчиняется ли активация дополнительным правилам, таким как MFA, перед отправкой запроса.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-173">Only set this property if you want to check whether an activation is subject to additional rules like MFA before actually submitting the request.</span></span>|
|<span data-ttu-id="e7f2a-174">targetScheduleId</span><span class="sxs-lookup"><span data-stu-id="e7f2a-174">targetScheduleId</span></span>|<span data-ttu-id="e7f2a-175">String</span><span class="sxs-lookup"><span data-stu-id="e7f2a-175">String</span></span>|<span data-ttu-id="e7f2a-176">ID объекта расписания, прикрепленного к назначению.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-176">ID of the schedule object attached to the assignment.</span></span>|
|<span data-ttu-id="e7f2a-177">обоснование</span><span class="sxs-lookup"><span data-stu-id="e7f2a-177">justification</span></span>|<span data-ttu-id="e7f2a-178">String</span><span class="sxs-lookup"><span data-stu-id="e7f2a-178">String</span></span>|<span data-ttu-id="e7f2a-179">Сообщение, предоставленное пользователями и администраторами при создании запроса о необходимости.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-179">A message provided by users and administrators when create the request about why it is needed.</span></span>|
|<span data-ttu-id="e7f2a-180">scheduleInfo</span><span class="sxs-lookup"><span data-stu-id="e7f2a-180">scheduleInfo</span></span>|[<span data-ttu-id="e7f2a-181">requestSchedule</span><span class="sxs-lookup"><span data-stu-id="e7f2a-181">requestSchedule</span></span>](../resources/requestschedule.md)|<span data-ttu-id="e7f2a-182">Объект расписания запроса назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-182">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="e7f2a-183">ticketInfo</span><span class="sxs-lookup"><span data-stu-id="e7f2a-183">ticketInfo</span></span>|[<span data-ttu-id="e7f2a-184">ticketInfo</span><span class="sxs-lookup"><span data-stu-id="e7f2a-184">ticketInfo</span></span>](../resources/ticketinfo.md)|<span data-ttu-id="e7f2a-185">Объект ticketInfo, присоединенный к запросу назначения ролей, который включает сведения о номере билета и системе билетов.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-185">The ticketInfo object attached to the role assignment request which includes details of the ticket number and ticket system.</span></span>|



## <a name="response"></a><span data-ttu-id="e7f2a-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7f2a-186">Response</span></span>

<span data-ttu-id="e7f2a-187">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-187">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e7f2a-188">Примеры</span><span class="sxs-lookup"><span data-stu-id="e7f2a-188">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e7f2a-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7f2a-189">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e7f2a-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7f2a-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroleeligibilityschedulerequest"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}
Content-Type: application/json
Content-length: 467

{
  "@odata.type": "#microsoft.graph.unifiedRoleEligibilityScheduleRequest",
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
# <a name="c"></a>[<span data-ttu-id="e7f2a-191">C#</span><span class="sxs-lookup"><span data-stu-id="e7f2a-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroleeligibilityschedulerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e7f2a-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7f2a-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroleeligibilityschedulerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e7f2a-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e7f2a-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroleeligibilityschedulerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e7f2a-194">Java</span><span class="sxs-lookup"><span data-stu-id="e7f2a-194">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroleeligibilityschedulerequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e7f2a-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7f2a-195">Response</span></span>
<span data-ttu-id="e7f2a-196">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e7f2a-196">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleRequest"
}
-->
```http
HTTP/1.1 204 OK

```
<!--
{
  "@odata.type": "#microsoft.graph.unifiedRoleEligibilityScheduleRequest",
  "id": "a2e242a0-42a0-a2e2-a042-e2a2a042e2a2",
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
-->
