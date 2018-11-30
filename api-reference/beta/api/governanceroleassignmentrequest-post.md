---
title: Создание governanceRoleAssignmentRequest
description: Создание роли назначения запроса для представления операции, требуется на назначения ролей. В следующей таблице перечислены операции.
ms.openlocfilehash: b0d9edab1182d4a6fa620cfb953df1cb8af20c66
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077684"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="8beda-104">Создание governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="8beda-104">Create governanceRoleAssignmentRequest</span></span>

> <span data-ttu-id="8beda-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8beda-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8beda-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8beda-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8beda-107">Создание роли назначения запроса для представления операции, требуется на назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="8beda-107">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="8beda-108">В следующей таблице перечислены операции.</span><span class="sxs-lookup"><span data-stu-id="8beda-108">The following table lists the operations.</span></span>

| <span data-ttu-id="8beda-109">Операция</span><span class="sxs-lookup"><span data-stu-id="8beda-109">Operation</span></span>       | <span data-ttu-id="8beda-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8beda-110">Type</span></span> | 
|:---------------|:----------|
| <span data-ttu-id="8beda-111">Назначение назначения ролей</span><span class="sxs-lookup"><span data-stu-id="8beda-111">Assign a role assignment</span></span>| <span data-ttu-id="8beda-112">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="8beda-112">AdminAdd</span></span> |
| <span data-ttu-id="8beda-113">Активация назначение подходящими роли</span><span class="sxs-lookup"><span data-stu-id="8beda-113">Activate an eligible role assignment</span></span>| <span data-ttu-id="8beda-114">UserAdd</span><span class="sxs-lookup"><span data-stu-id="8beda-114">UserAdd</span></span> | 
| <span data-ttu-id="8beda-115">Деактивация назначение активированные роли</span><span class="sxs-lookup"><span data-stu-id="8beda-115">Deactivate an activated role assignment</span></span>| <span data-ttu-id="8beda-116">UserRemove</span><span class="sxs-lookup"><span data-stu-id="8beda-116">UserRemove</span></span> | 
| <span data-ttu-id="8beda-117">Удаление назначения ролей</span><span class="sxs-lookup"><span data-stu-id="8beda-117">Remove a role assignment</span></span>| <span data-ttu-id="8beda-118">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="8beda-118">AdminRemove</span></span> |
| <span data-ttu-id="8beda-119">Обновление назначения ролей</span><span class="sxs-lookup"><span data-stu-id="8beda-119">Update a role assignment</span></span>| <span data-ttu-id="8beda-120">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="8beda-120">AdminUpdate</span></span> |
| <span data-ttu-id="8beda-121">Запрос на расширение my назначения роли</span><span class="sxs-lookup"><span data-stu-id="8beda-121">Request to extend my role assignment</span></span>| <span data-ttu-id="8beda-122">UserExtend</span><span class="sxs-lookup"><span data-stu-id="8beda-122">UserExtend</span></span> | 
| <span data-ttu-id="8beda-123">Расширение назначения ролей</span><span class="sxs-lookup"><span data-stu-id="8beda-123">Extend a role assignment</span></span>| <span data-ttu-id="8beda-124">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="8beda-124">AdminExtend</span></span> | 
| <span data-ttu-id="8beda-125">Запрос на обновление назначения ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="8beda-125">Request to renew my expired role assignment</span></span>| <span data-ttu-id="8beda-126">UserRenew</span><span class="sxs-lookup"><span data-stu-id="8beda-126">UserRenew</span></span> | 
| <span data-ttu-id="8beda-127">Обновление назначения ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="8beda-127">Renew an expired role assignment</span></span>| <span data-ttu-id="8beda-128">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="8beda-128">AdminRenew</span></span> | 

 
## <a name="permissions"></a><span data-ttu-id="8beda-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8beda-129">Permissions</span></span>
<span data-ttu-id="8beda-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8beda-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8beda-132">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8beda-132">Permission type</span></span>      | <span data-ttu-id="8beda-133">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8beda-133">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8beda-134">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8beda-134">Delegated (work or school account)</span></span> | <span data-ttu-id="8beda-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="8beda-135">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="8beda-136">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8beda-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8beda-137">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8beda-137">Not supported.</span></span>    |
|<span data-ttu-id="8beda-138">Для приложения</span><span class="sxs-lookup"><span data-stu-id="8beda-138">Application</span></span> | <span data-ttu-id="8beda-139">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="8beda-139">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="8beda-140">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8beda-140">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8beda-141">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8beda-141">Optional query parameters</span></span>
<span data-ttu-id="8beda-142">Метод не **поддерживает [Параметры запроса OData](/graph/query-parameters)** .</span><span class="sxs-lookup"><span data-stu-id="8beda-142">This method does **not** support [OData query parameters](/graph/query-parameters).</span></span>

### <a name="request-headers"></a><span data-ttu-id="8beda-143">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8beda-143">Request headers</span></span>
| <span data-ttu-id="8beda-144">Имя</span><span class="sxs-lookup"><span data-stu-id="8beda-144">Name</span></span>       | <span data-ttu-id="8beda-145">Описание</span><span class="sxs-lookup"><span data-stu-id="8beda-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8beda-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="8beda-146">Authorization</span></span>  | <span data-ttu-id="8beda-147">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8beda-147">Bearer {code}</span></span>|
| <span data-ttu-id="8beda-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8beda-148">Content-type</span></span>  | <span data-ttu-id="8beda-149">application/json</span><span class="sxs-lookup"><span data-stu-id="8beda-149">application/json</span></span>|

### <a name="request-body"></a><span data-ttu-id="8beda-150">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8beda-150">Request body</span></span>
<span data-ttu-id="8beda-151">В тексте запроса укажите представление JSON объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="8beda-151">In the request body, supply a JSON representation of [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="8beda-152">Свойство</span><span class="sxs-lookup"><span data-stu-id="8beda-152">Property</span></span>     | <span data-ttu-id="8beda-153">Тип</span><span class="sxs-lookup"><span data-stu-id="8beda-153">Type</span></span>    |<span data-ttu-id="8beda-154">Обязательный</span><span class="sxs-lookup"><span data-stu-id="8beda-154">Required</span></span>|  <span data-ttu-id="8beda-155">Описание</span><span class="sxs-lookup"><span data-stu-id="8beda-155">Description</span></span>|
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="8beda-156">resourceId</span><span class="sxs-lookup"><span data-stu-id="8beda-156">resourceId</span></span>|<span data-ttu-id="8beda-157">String</span><span class="sxs-lookup"><span data-stu-id="8beda-157">String</span></span>|<span data-ttu-id="8beda-158">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-158">Yes</span></span>|<span data-ttu-id="8beda-159">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="8beda-159">The ID of the resource.</span></span>|
|<span data-ttu-id="8beda-160">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8beda-160">roleDefinitionId</span></span>|<span data-ttu-id="8beda-161">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-161">String</span></span>|<span data-ttu-id="8beda-162">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-162">Yes</span></span>|<span data-ttu-id="8beda-163">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="8beda-163">The ID of the role definition.</span></span>|
|<span data-ttu-id="8beda-164">subjectId</span><span class="sxs-lookup"><span data-stu-id="8beda-164">subjectId</span></span>|<span data-ttu-id="8beda-165">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-165">String</span></span>|<span data-ttu-id="8beda-166">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-166">Yes</span></span>|<span data-ttu-id="8beda-167">Идентификатор субъекта.</span><span class="sxs-lookup"><span data-stu-id="8beda-167">The ID of the subject.</span></span>|
|<span data-ttu-id="8beda-168">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8beda-168">assignmentState</span></span>|<span data-ttu-id="8beda-169">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-169">String</span></span>|<span data-ttu-id="8beda-170">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-170">Yes</span></span>|<span data-ttu-id="8beda-171">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="8beda-171">The state of assignment.</span></span> <span data-ttu-id="8beda-172">Значение может быть ``Eligible`` и ``Active``.</span><span class="sxs-lookup"><span data-stu-id="8beda-172">The value can be ``Eligible`` and ``Active``.</span></span>|
|<span data-ttu-id="8beda-173">type</span><span class="sxs-lookup"><span data-stu-id="8beda-173">type</span></span>|<span data-ttu-id="8beda-174">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-174">String</span></span>|<span data-ttu-id="8beda-175">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-175">Yes</span></span>|<span data-ttu-id="8beda-176">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="8beda-176">The request type.</span></span> <span data-ttu-id="8beda-177">Значение может быть `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`и `AdminExtend`.</span><span class="sxs-lookup"><span data-stu-id="8beda-177">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span>|
|<span data-ttu-id="8beda-178">Причина</span><span class="sxs-lookup"><span data-stu-id="8beda-178">reason</span></span>|<span data-ttu-id="8beda-179">String</span><span class="sxs-lookup"><span data-stu-id="8beda-179">String</span></span>| |<span data-ttu-id="8beda-180">Причину должно предоставляться для запроса назначений ролей для аудита и предварительный просмотр цели.</span><span class="sxs-lookup"><span data-stu-id="8beda-180">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="8beda-181">расписание</span><span class="sxs-lookup"><span data-stu-id="8beda-181">schedule</span></span>|[<span data-ttu-id="8beda-182">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8beda-182">governanceSchedule</span></span>](../resources/governanceschedule.md)| | <span data-ttu-id="8beda-183">Расписание для запроса назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="8beda-183">The schedule of the role assignment request.</span></span> <span data-ttu-id="8beda-184">Для запроса типа `UserAdd`, `AdminAdd`, `AdminUpdate`, и `AdminExtend`, это необходимо.</span><span class="sxs-lookup"><span data-stu-id="8beda-184">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span>|

### <a name="response"></a><span data-ttu-id="8beda-185">Ответ</span><span class="sxs-lookup"><span data-stu-id="8beda-185">Response</span></span>
<span data-ttu-id="8beda-186">Успешно завершена, этот метод возвращает `201, Created` код ответа и объект [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8beda-186">If successful, this method returns a `201, Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

## <a name="error-codes"></a><span data-ttu-id="8beda-187">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="8beda-187">Error codes</span></span>
<span data-ttu-id="8beda-188">Этот интерфейс API стандарту кодов HTTP, кроме кодов ошибок, перечисленных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="8beda-188">This API follows the standard of HTTP codes, in addition to the error codes listed in the following table.</span></span>

|<span data-ttu-id="8beda-189">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="8beda-189">Error code</span></span>     | <span data-ttu-id="8beda-190">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="8beda-190">Error message</span></span>              | <span data-ttu-id="8beda-191">Сведения</span><span class="sxs-lookup"><span data-stu-id="8beda-191">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="8beda-192">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="8beda-192">400 BadRequest</span></span> | <span data-ttu-id="8beda-193">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="8beda-193">RoleNotFound</span></span>    | <span data-ttu-id="8beda-194">`roleDefinitionId` Условии, что в запросе не удается найти текст.</span><span class="sxs-lookup"><span data-stu-id="8beda-194">The `roleDefinitionId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="8beda-195">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="8beda-195">400 BadRequest</span></span> | <span data-ttu-id="8beda-196">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="8beda-196">ResourceIsLocked</span></span>    | <span data-ttu-id="8beda-197">Ресурс, представленные в тексте запроса находится в состоянии из `Locked` и не могут создавать запросы назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="8beda-197">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span>
| <span data-ttu-id="8beda-198">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="8beda-198">400 BadRequest</span></span> | <span data-ttu-id="8beda-199">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="8beda-199">SubjectNotFound</span></span>    | <span data-ttu-id="8beda-200">`subjectId` Условии, что в запросе не удается найти текст.</span><span class="sxs-lookup"><span data-stu-id="8beda-200">The `subjectId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="8beda-201">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="8beda-201">400 BadRequest</span></span> | <span data-ttu-id="8beda-202">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="8beda-202">PendingRoleAssignmentRequest</span></span>    | <span data-ttu-id="8beda-203">Уже существует ожидающие [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в системе.</span><span class="sxs-lookup"><span data-stu-id="8beda-203">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span>
| <span data-ttu-id="8beda-204">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="8beda-204">400 BadRequest</span></span> | <span data-ttu-id="8beda-205">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="8beda-205">RoleAssignmentExists</span></span>    | <span data-ttu-id="8beda-206">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) запрошено будет создан уже существует в системе.</span><span class="sxs-lookup"><span data-stu-id="8beda-206">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span>
| <span data-ttu-id="8beda-207">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="8beda-207">400 BadRequest</span></span> | <span data-ttu-id="8beda-208">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="8beda-208">RoleAssignmentDoesNotExist</span></span>    | <span data-ttu-id="8beda-209">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) запрос на обновление/расширить не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="8beda-209">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span>
| <span data-ttu-id="8beda-210">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="8beda-210">400 BadRequest</span></span> | <span data-ttu-id="8beda-211">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="8beda-211">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="8beda-212">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) не соответствует внутренней политик и не может быть создан.</span><span class="sxs-lookup"><span data-stu-id="8beda-212">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span>

## <a name="example-1"></a><span data-ttu-id="8beda-213">Пример 1</span><span class="sxs-lookup"><span data-stu-id="8beda-213">Example 1</span></span>
<span data-ttu-id="8beda-214">В этом примере администраторам назначение роли выставления счетов читатель nawu@fimdev.net пользователя.</span><span class="sxs-lookup"><span data-stu-id="8beda-214">In this example, administrators assign user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="8beda-215">**Примечание:** Помимо разрешение, в этом примере требуется инициатор запроса может иметь по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="8beda-215">**Note:** Besides the permission, this example requires the requestor to have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="8beda-216">Свойство</span><span class="sxs-lookup"><span data-stu-id="8beda-216">Property</span></span>     | <span data-ttu-id="8beda-217">Тип</span><span class="sxs-lookup"><span data-stu-id="8beda-217">Type</span></span>    |<span data-ttu-id="8beda-218">Обязательный</span><span class="sxs-lookup"><span data-stu-id="8beda-218">Required</span></span>|  <span data-ttu-id="8beda-219">Значение</span><span class="sxs-lookup"><span data-stu-id="8beda-219">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="8beda-220">resourceId</span><span class="sxs-lookup"><span data-stu-id="8beda-220">resourceId</span></span>|<span data-ttu-id="8beda-221">String</span><span class="sxs-lookup"><span data-stu-id="8beda-221">String</span></span>|<span data-ttu-id="8beda-222">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-222">Yes</span></span>|<span data-ttu-id="8beda-223">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="8beda-223">\<resourceId\></span></span>|
|<span data-ttu-id="8beda-224">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8beda-224">roleDefinitionId</span></span>|<span data-ttu-id="8beda-225">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-225">String</span></span>|<span data-ttu-id="8beda-226">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-226">Yes</span></span>|<span data-ttu-id="8beda-227">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="8beda-227">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="8beda-228">subjectId</span><span class="sxs-lookup"><span data-stu-id="8beda-228">subjectId</span></span>|<span data-ttu-id="8beda-229">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-229">String</span></span>|<span data-ttu-id="8beda-230">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-230">Yes</span></span>|<span data-ttu-id="8beda-231">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="8beda-231">\<subjectId\></span></span>|
|<span data-ttu-id="8beda-232">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8beda-232">assignmentState</span></span>|<span data-ttu-id="8beda-233">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-233">String</span></span>|<span data-ttu-id="8beda-234">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-234">Yes</span></span>| <span data-ttu-id="8beda-235">Допустимость / Active</span><span class="sxs-lookup"><span data-stu-id="8beda-235">Eligible / Active</span></span>|
|<span data-ttu-id="8beda-236">type</span><span class="sxs-lookup"><span data-stu-id="8beda-236">type</span></span>|<span data-ttu-id="8beda-237">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-237">String</span></span>|<span data-ttu-id="8beda-238">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-238">Yes</span></span>| <span data-ttu-id="8beda-239">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="8beda-239">AdminAdd</span></span>|
|<span data-ttu-id="8beda-240">Причина</span><span class="sxs-lookup"><span data-stu-id="8beda-240">reason</span></span>|<span data-ttu-id="8beda-241">String</span><span class="sxs-lookup"><span data-stu-id="8beda-241">String</span></span>| <span data-ttu-id="8beda-242">зависит от роли параметров</span><span class="sxs-lookup"><span data-stu-id="8beda-242">depends on role Settings</span></span>||
|<span data-ttu-id="8beda-243">расписание</span><span class="sxs-lookup"><span data-stu-id="8beda-243">schedule</span></span>|[<span data-ttu-id="8beda-244">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8beda-244">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="8beda-245">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-245">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="8beda-246">Запрос</span><span class="sxs-lookup"><span data-stu-id="8beda-246">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
"resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Eligible",
"type":"AdminAdd",
"reason":"Assign an eligible role",
"schedule":{
  "startDateTime":"2018-05-12T23:37:43.356Z",
  "endDateTime":"2018-11-08T23:37:43.356Z",
  "type":"Once"
  }
}
```
##### <a name="response"></a><span data-ttu-id="8beda-247">Ответ</span><span class="sxs-lookup"><span data-stu-id="8beda-247">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
    "id": "1232e4ea-741a-4be5-8044-5edabdd61672",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
    "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
    "linkedEligibleRoleAssignmentId": "",
    "type": "AdminAdd",
    "assignmentState": "Eligible",
    "requestedDateTime": "0001-01-01T00:00:00Z",
    "roleAssignmentStartDateTime": "2018-05-12T23:38:34.6007266Z",
    "roleAssignmentEndDateTime": "2018-11-08T23:37:43.356Z",
    "reason": "Evaluate Only",
    "status": {
        "status": "InProgress",
        "subStatus": "Granted",
        "statusDetails": [
            {
                "key": "AdminRequestRule",
                "value": "Grant"
            },
            {
                "key": "ExpirationRule",
                "value": "Grant"
            },
            {
                "key": "MfaRule",
                "value": "Grant"
            }
        ]
    },
    "schedule": {
        "type": "Once",
        "startDateTime": "2018-05-12T23:37:43.356Z",
        "endDateTime": "2018-11-08T23:37:43.356Z",
        "duration": "PT0S"
    }
}
```

## <a name="example-2"></a><span data-ttu-id="8beda-248">Пример 2</span><span class="sxs-lookup"><span data-stu-id="8beda-248">Example 2</span></span>
<span data-ttu-id="8beda-249">В этом примере nawu@fimdev.net пользователь активирует право чтения выставления счетов роли.</span><span class="sxs-lookup"><span data-stu-id="8beda-249">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="8beda-250">Свойство</span><span class="sxs-lookup"><span data-stu-id="8beda-250">Property</span></span>     | <span data-ttu-id="8beda-251">Тип</span><span class="sxs-lookup"><span data-stu-id="8beda-251">Type</span></span>    |<span data-ttu-id="8beda-252">Обязательный</span><span class="sxs-lookup"><span data-stu-id="8beda-252">Required</span></span>|  <span data-ttu-id="8beda-253">Значение</span><span class="sxs-lookup"><span data-stu-id="8beda-253">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="8beda-254">resourceId</span><span class="sxs-lookup"><span data-stu-id="8beda-254">resourceId</span></span>|<span data-ttu-id="8beda-255">String</span><span class="sxs-lookup"><span data-stu-id="8beda-255">String</span></span>|<span data-ttu-id="8beda-256">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-256">Yes</span></span>|<span data-ttu-id="8beda-257">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="8beda-257">\<resourceId\></span></span>|
|<span data-ttu-id="8beda-258">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8beda-258">roleDefinitionId</span></span>|<span data-ttu-id="8beda-259">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-259">String</span></span>|<span data-ttu-id="8beda-260">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-260">Yes</span></span>|<span data-ttu-id="8beda-261">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="8beda-261">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="8beda-262">subjectId</span><span class="sxs-lookup"><span data-stu-id="8beda-262">subjectId</span></span>|<span data-ttu-id="8beda-263">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-263">String</span></span>|<span data-ttu-id="8beda-264">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-264">Yes</span></span>|<span data-ttu-id="8beda-265">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="8beda-265">\<subjectId\></span></span>|
|<span data-ttu-id="8beda-266">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8beda-266">assignmentState</span></span>|<span data-ttu-id="8beda-267">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-267">String</span></span>|<span data-ttu-id="8beda-268">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-268">Yes</span></span>| <span data-ttu-id="8beda-269">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="8beda-269">Active</span></span>|
|<span data-ttu-id="8beda-270">type</span><span class="sxs-lookup"><span data-stu-id="8beda-270">type</span></span>|<span data-ttu-id="8beda-271">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-271">String</span></span>|<span data-ttu-id="8beda-272">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-272">Yes</span></span>| <span data-ttu-id="8beda-273">UserAdd</span><span class="sxs-lookup"><span data-stu-id="8beda-273">UserAdd</span></span>|
|<span data-ttu-id="8beda-274">Причина</span><span class="sxs-lookup"><span data-stu-id="8beda-274">reason</span></span>|<span data-ttu-id="8beda-275">String</span><span class="sxs-lookup"><span data-stu-id="8beda-275">String</span></span>| <span data-ttu-id="8beda-276">зависит от роли параметров</span><span class="sxs-lookup"><span data-stu-id="8beda-276">depends on role Settings</span></span>||
|<span data-ttu-id="8beda-277">расписание</span><span class="sxs-lookup"><span data-stu-id="8beda-277">schedule</span></span>|[<span data-ttu-id="8beda-278">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8beda-278">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="8beda-279">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-279">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="8beda-280">Запрос</span><span class="sxs-lookup"><span data-stu-id="8beda-280">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"8b4d1d51-08e9-4254-b0a6-b16177aae376",
"resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Active",
"type":"UserAdd",
"reason": "Activate the owner role",
"schedule":{
  "type":"Once",
  "startDateTime":"2018-05-12T23:28:43.537Z",
  "duration":"PT9H"
  },
"linkedEligibleRoleAssignmentId":"e327f4be-42a0-47a2-8579-0a39b025b394"
}
```
##### <a name="response"></a><span data-ttu-id="8beda-281">Ответ</span><span class="sxs-lookup"><span data-stu-id="8beda-281">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
    "id": "3ad49a7c-918e-4d86-9f84-fab28f8658c0",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
    "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
    "linkedEligibleRoleAssignmentId": "e327f4be-42a0-47a2-8579-0a39b025b394",
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "0001-01-01T00:00:00Z",
    "roleAssignmentStartDateTime": "2018-05-12T23:29:29.5123911Z",
    "roleAssignmentEndDateTime": "2018-05-13T08:28:43.537Z",
    "reason": "Activate the owner role",
    "status": {
        "status": "InProgress",
        "subStatus": "Granted",
        "statusDetails": [
            {
                "key": "EligibilityRule",
                "value": "Grant"
            },
            {
                "key": "ExpirationRule",
                "value": "Grant"
            },
            {
                "key": "MfaRule",
                "value": "Grant"
            },
            {
                "key": "JustificationRule",
                "value": "Grant"
            },
            {
                "key": "ActivationDayRule",
                "value": "Grant"
            },
            {
                "key": "ApprovalRule",
                "value": "Grant"
            }
        ]
    },
    "schedule": {
        "type": "Once",
        "startDateTime": "2018-05-12T23:28:43.537Z",
        "endDateTime": "0001-01-01T00:00:00Z",
        "duration": "PT9H"
    }
}
```

## <a name="example-3"></a><span data-ttu-id="8beda-282">Пример 3</span><span class="sxs-lookup"><span data-stu-id="8beda-282">Example 3</span></span>
<span data-ttu-id="8beda-283">В этом примере пользователь nawu@fimdev.net деактивирует активная роль чтения выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="8beda-283">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="8beda-284">Свойство</span><span class="sxs-lookup"><span data-stu-id="8beda-284">Property</span></span>     | <span data-ttu-id="8beda-285">Тип</span><span class="sxs-lookup"><span data-stu-id="8beda-285">Type</span></span>    |<span data-ttu-id="8beda-286">Обязательный</span><span class="sxs-lookup"><span data-stu-id="8beda-286">Required</span></span>|  <span data-ttu-id="8beda-287">Значение</span><span class="sxs-lookup"><span data-stu-id="8beda-287">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="8beda-288">resourceId</span><span class="sxs-lookup"><span data-stu-id="8beda-288">resourceId</span></span>|<span data-ttu-id="8beda-289">String</span><span class="sxs-lookup"><span data-stu-id="8beda-289">String</span></span>|<span data-ttu-id="8beda-290">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-290">Yes</span></span>|<span data-ttu-id="8beda-291">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="8beda-291">\<resourceId\></span></span>|
|<span data-ttu-id="8beda-292">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8beda-292">roleDefinitionId</span></span>|<span data-ttu-id="8beda-293">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-293">String</span></span>|<span data-ttu-id="8beda-294">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-294">Yes</span></span>|<span data-ttu-id="8beda-295">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="8beda-295">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="8beda-296">subjectId</span><span class="sxs-lookup"><span data-stu-id="8beda-296">subjectId</span></span>|<span data-ttu-id="8beda-297">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-297">String</span></span>|<span data-ttu-id="8beda-298">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-298">Yes</span></span>|<span data-ttu-id="8beda-299">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="8beda-299">\<subjectId\></span></span>|
|<span data-ttu-id="8beda-300">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8beda-300">assignmentState</span></span>|<span data-ttu-id="8beda-301">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-301">String</span></span>|<span data-ttu-id="8beda-302">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-302">Yes</span></span>| <span data-ttu-id="8beda-303">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="8beda-303">Active</span></span>|
|<span data-ttu-id="8beda-304">type</span><span class="sxs-lookup"><span data-stu-id="8beda-304">type</span></span>|<span data-ttu-id="8beda-305">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-305">String</span></span>|<span data-ttu-id="8beda-306">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-306">Yes</span></span>| <span data-ttu-id="8beda-307">UserRemove</span><span class="sxs-lookup"><span data-stu-id="8beda-307">UserRemove</span></span>|
|<span data-ttu-id="8beda-308">Причина</span><span class="sxs-lookup"><span data-stu-id="8beda-308">reason</span></span>|<span data-ttu-id="8beda-309">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-309">String</span></span>| <span data-ttu-id="8beda-310">Нет</span><span class="sxs-lookup"><span data-stu-id="8beda-310">No</span></span>||
|<span data-ttu-id="8beda-311">расписание</span><span class="sxs-lookup"><span data-stu-id="8beda-311">schedule</span></span>|[<span data-ttu-id="8beda-312">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8beda-312">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="8beda-313">Нет</span><span class="sxs-lookup"><span data-stu-id="8beda-313">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="8beda-314">Запрос</span><span class="sxs-lookup"><span data-stu-id="8beda-314">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"bc75b4e6-7403-4243-bf2f-d1f6990be122",
"resourceId":"fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Active",
"type":"UserRemove",
"reason":"Deactivate the role",
"linkedEligibleRoleAssignmentId":"cb8a533e-02d5-42ad-8499-916b1e4822ec"
}
```
##### <a name="response"></a><span data-ttu-id="8beda-315">Ответ</span><span class="sxs-lookup"><span data-stu-id="8beda-315">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
    "id": "abfcdb57-8e5d-42a0-ae67-7598b96fddb1",
    "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
    "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
    "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
    "linkedEligibleRoleAssignmentId": "cb8a533e-02d5-42ad-8499-916b1e4822ec",
    "type": "UserRemove",
    "assignmentState": "Active",
    "requestedDateTime": "0001-01-01T00:00:00Z",
    "roleAssignmentStartDateTime": null,
    "roleAssignmentEndDateTime": null,
    "reason": "Evaluate only",
    "schedule": null,
    "status": {
        "status": "Closed",
        "subStatus": "Revoked",
        "statusDetails": []
    }
}
```

### <a name="example-4"></a><span data-ttu-id="8beda-316">Пример 4</span><span class="sxs-lookup"><span data-stu-id="8beda-316">Example 4</span></span>
<span data-ttu-id="8beda-317">В этом примере администраторам удалить nawu@fimdev.net пользователя из роли выставления счетов чтения.</span><span class="sxs-lookup"><span data-stu-id="8beda-317">In this example, administrators remove the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="8beda-318">**Примечание:** Помимо области разрешений в этом примере требуется инициатор запроса может иметь по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="8beda-318">**Note:** Besides the permission scope, this example requires the requestor to have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="8beda-319">Свойство</span><span class="sxs-lookup"><span data-stu-id="8beda-319">Property</span></span>     | <span data-ttu-id="8beda-320">Тип</span><span class="sxs-lookup"><span data-stu-id="8beda-320">Type</span></span>    |<span data-ttu-id="8beda-321">Обязательный</span><span class="sxs-lookup"><span data-stu-id="8beda-321">Required</span></span>|  <span data-ttu-id="8beda-322">Значение</span><span class="sxs-lookup"><span data-stu-id="8beda-322">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="8beda-323">resourceId</span><span class="sxs-lookup"><span data-stu-id="8beda-323">resourceId</span></span>|<span data-ttu-id="8beda-324">String</span><span class="sxs-lookup"><span data-stu-id="8beda-324">String</span></span>|<span data-ttu-id="8beda-325">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-325">Yes</span></span>|<span data-ttu-id="8beda-326">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="8beda-326">\<resourceId\></span></span>|
|<span data-ttu-id="8beda-327">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8beda-327">roleDefinitionId</span></span>|<span data-ttu-id="8beda-328">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-328">String</span></span>|<span data-ttu-id="8beda-329">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-329">Yes</span></span>|<span data-ttu-id="8beda-330">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="8beda-330">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="8beda-331">subjectId</span><span class="sxs-lookup"><span data-stu-id="8beda-331">subjectId</span></span>|<span data-ttu-id="8beda-332">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-332">String</span></span>|<span data-ttu-id="8beda-333">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-333">Yes</span></span>|<span data-ttu-id="8beda-334">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="8beda-334">\<subjectId\></span></span>|
|<span data-ttu-id="8beda-335">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8beda-335">assignmentState</span></span>|<span data-ttu-id="8beda-336">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-336">String</span></span>|<span data-ttu-id="8beda-337">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-337">Yes</span></span>| <span data-ttu-id="8beda-338">Допустимость / Active</span><span class="sxs-lookup"><span data-stu-id="8beda-338">Eligible / Active</span></span>|
|<span data-ttu-id="8beda-339">type</span><span class="sxs-lookup"><span data-stu-id="8beda-339">type</span></span>|<span data-ttu-id="8beda-340">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-340">String</span></span>|<span data-ttu-id="8beda-341">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-341">Yes</span></span>| <span data-ttu-id="8beda-342">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="8beda-342">AdminRemove</span></span>|
|<span data-ttu-id="8beda-343">Причина</span><span class="sxs-lookup"><span data-stu-id="8beda-343">reason</span></span>|<span data-ttu-id="8beda-344">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-344">String</span></span>| <span data-ttu-id="8beda-345">Нет</span><span class="sxs-lookup"><span data-stu-id="8beda-345">No</span></span>||
|<span data-ttu-id="8beda-346">расписание</span><span class="sxs-lookup"><span data-stu-id="8beda-346">schedule</span></span>|[<span data-ttu-id="8beda-347">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8beda-347">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="8beda-348">Нет</span><span class="sxs-lookup"><span data-stu-id="8beda-348">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="8beda-349">Запрос</span><span class="sxs-lookup"><span data-stu-id="8beda-349">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState":"Eligible",
  "type":"AdminRemove"
}
```
##### <a name="response"></a><span data-ttu-id="8beda-350">Ответ</span><span class="sxs-lookup"><span data-stu-id="8beda-350">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"c934fcb9-cf53-42ac-a8b4-6246f6726299",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminRemove",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "roleAssignmentStartDateTime":null,
  "roleAssignmentEndDateTime":null,
  "reason":null,
  "status":{
    "status":"Closed",
    "subStatus":"Revoked",
    "statusDetails":[]
  },
  "schedule":null
}
```

### <a name="example-5"></a><span data-ttu-id="8beda-351">Пример 5</span><span class="sxs-lookup"><span data-stu-id="8beda-351">Example 5</span></span>
<span data-ttu-id="8beda-352">В этом примере Администраторы обновление назначения ролей для пользователя nawu@fimdev.net владельцу.</span><span class="sxs-lookup"><span data-stu-id="8beda-352">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="8beda-353">**Примечание:** Помимо области разрешений в этом примере требуется инициатор запроса может иметь по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="8beda-353">**Note:** Besides the permission scope, this example requires the requestor to have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 
| <span data-ttu-id="8beda-354">Свойство</span><span class="sxs-lookup"><span data-stu-id="8beda-354">Property</span></span>     | <span data-ttu-id="8beda-355">Тип</span><span class="sxs-lookup"><span data-stu-id="8beda-355">Type</span></span>    |<span data-ttu-id="8beda-356">Обязательный</span><span class="sxs-lookup"><span data-stu-id="8beda-356">Required</span></span>|  <span data-ttu-id="8beda-357">Значение</span><span class="sxs-lookup"><span data-stu-id="8beda-357">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="8beda-358">resourceId</span><span class="sxs-lookup"><span data-stu-id="8beda-358">resourceId</span></span>|<span data-ttu-id="8beda-359">String</span><span class="sxs-lookup"><span data-stu-id="8beda-359">String</span></span>|<span data-ttu-id="8beda-360">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-360">Yes</span></span>|<span data-ttu-id="8beda-361">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="8beda-361">\<resourceId\></span></span>|
|<span data-ttu-id="8beda-362">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8beda-362">roleDefinitionId</span></span>|<span data-ttu-id="8beda-363">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-363">String</span></span>|<span data-ttu-id="8beda-364">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-364">Yes</span></span>|<span data-ttu-id="8beda-365">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="8beda-365">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="8beda-366">subjectId</span><span class="sxs-lookup"><span data-stu-id="8beda-366">subjectId</span></span>|<span data-ttu-id="8beda-367">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-367">String</span></span>|<span data-ttu-id="8beda-368">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-368">Yes</span></span>|<span data-ttu-id="8beda-369">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="8beda-369">\<subjectId\></span></span>|
|<span data-ttu-id="8beda-370">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8beda-370">assignmentState</span></span>|<span data-ttu-id="8beda-371">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-371">String</span></span>|<span data-ttu-id="8beda-372">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-372">Yes</span></span>| <span data-ttu-id="8beda-373">Допустимость / Active</span><span class="sxs-lookup"><span data-stu-id="8beda-373">Eligible / Active</span></span>|
|<span data-ttu-id="8beda-374">type</span><span class="sxs-lookup"><span data-stu-id="8beda-374">type</span></span>|<span data-ttu-id="8beda-375">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-375">String</span></span>|<span data-ttu-id="8beda-376">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-376">Yes</span></span>| <span data-ttu-id="8beda-377">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="8beda-377">AdminUpdate</span></span>|
|<span data-ttu-id="8beda-378">Причина</span><span class="sxs-lookup"><span data-stu-id="8beda-378">reason</span></span>|<span data-ttu-id="8beda-379">String</span><span class="sxs-lookup"><span data-stu-id="8beda-379">String</span></span>| <span data-ttu-id="8beda-380">зависит от roleSettings</span><span class="sxs-lookup"><span data-stu-id="8beda-380">depends on roleSettings</span></span>||
|<span data-ttu-id="8beda-381">расписание</span><span class="sxs-lookup"><span data-stu-id="8beda-381">schedule</span></span>|[<span data-ttu-id="8beda-382">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8beda-382">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="8beda-383">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-383">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="8beda-384">Запрос</span><span class="sxs-lookup"><span data-stu-id="8beda-384">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"1566d11d-d2b6-444a-a8de-28698682c445",
  "assignmentState":"Eligible",
  "type":"AdminUpdate",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-03-08T05:42:45.317Z",
    "endDateTime":"2018-06-05T05:42:31.000Z"
  }
}
```
##### <a name="response"></a><span data-ttu-id="8beda-385">Ответ</span><span class="sxs-lookup"><span data-stu-id="8beda-385">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"4f6d4802-b3ac-4f5a-86d7-a6a4edd7d383",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "subjectId":"1566d11d-d2b6-444a-a8de-28698682c445",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminUpdate",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "roleAssignmentStartDateTime":"2018-05-12T23:50:03.4755896Z",
  "roleAssignmentEndDateTime":"2018-06-05T05:42:31Z",
  "reason":null,
  "status":{
    "status":"InProgress",
    "subStatus":"Granted",
    "statusDetails":[
      {
        "key":"AdminRequestRule","value":"Grant"
      },{
        "key":"ExpirationRule","value":"Grant"
      },{
        "key":"MfaRule","value":"Grant"
      }
    ]
  },
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-03-08T05:42:45.317Z",
    "endDateTime":"2018-06-05T05:42:31Z",
    "duration":"PT0S"
  }
}
```

### <a name="example-6"></a><span data-ttu-id="8beda-386">В примере 6</span><span class="sxs-lookup"><span data-stu-id="8beda-386">Example 6</span></span>
<span data-ttu-id="8beda-387">В этом примере расширяет истекающим сроком действия назначения ролей для пользователя ANUJCUSER для участника службы управления API.</span><span class="sxs-lookup"><span data-stu-id="8beda-387">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="8beda-388">**Примечание:** Помимо области разрешений в этом примере требуется инициатор запроса может иметь по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="8beda-388">**Note:** Besides the permission scope, this example requires the requestor to have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="8beda-389">Свойство</span><span class="sxs-lookup"><span data-stu-id="8beda-389">Property</span></span>     | <span data-ttu-id="8beda-390">Тип</span><span class="sxs-lookup"><span data-stu-id="8beda-390">Type</span></span>    |<span data-ttu-id="8beda-391">Обязательный</span><span class="sxs-lookup"><span data-stu-id="8beda-391">Required</span></span>|  <span data-ttu-id="8beda-392">Значение</span><span class="sxs-lookup"><span data-stu-id="8beda-392">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="8beda-393">resourceId</span><span class="sxs-lookup"><span data-stu-id="8beda-393">resourceId</span></span>|<span data-ttu-id="8beda-394">String</span><span class="sxs-lookup"><span data-stu-id="8beda-394">String</span></span>|<span data-ttu-id="8beda-395">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-395">Yes</span></span>|<span data-ttu-id="8beda-396">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="8beda-396">\<resourceId\></span></span>|
|<span data-ttu-id="8beda-397">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8beda-397">roleDefinitionId</span></span>|<span data-ttu-id="8beda-398">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-398">String</span></span>|<span data-ttu-id="8beda-399">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-399">Yes</span></span>|<span data-ttu-id="8beda-400">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="8beda-400">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="8beda-401">subjectId</span><span class="sxs-lookup"><span data-stu-id="8beda-401">subjectId</span></span>|<span data-ttu-id="8beda-402">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-402">String</span></span>|<span data-ttu-id="8beda-403">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-403">Yes</span></span>|<span data-ttu-id="8beda-404">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="8beda-404">\<subjectId\></span></span>|
|<span data-ttu-id="8beda-405">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8beda-405">assignmentState</span></span>|<span data-ttu-id="8beda-406">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-406">String</span></span>|<span data-ttu-id="8beda-407">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-407">Yes</span></span>| <span data-ttu-id="8beda-408">Допустимость / Active</span><span class="sxs-lookup"><span data-stu-id="8beda-408">Eligible / Active</span></span> |
|<span data-ttu-id="8beda-409">type</span><span class="sxs-lookup"><span data-stu-id="8beda-409">type</span></span>|<span data-ttu-id="8beda-410">Строка</span><span class="sxs-lookup"><span data-stu-id="8beda-410">String</span></span>|<span data-ttu-id="8beda-411">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-411">Yes</span></span>| <span data-ttu-id="8beda-412">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="8beda-412">AdminExtend</span></span>|
|<span data-ttu-id="8beda-413">Причина</span><span class="sxs-lookup"><span data-stu-id="8beda-413">reason</span></span>|<span data-ttu-id="8beda-414">String</span><span class="sxs-lookup"><span data-stu-id="8beda-414">String</span></span>| <span data-ttu-id="8beda-415">зависит от roleSettings</span><span class="sxs-lookup"><span data-stu-id="8beda-415">depends on roleSettings</span></span>||
|<span data-ttu-id="8beda-416">расписание</span><span class="sxs-lookup"><span data-stu-id="8beda-416">schedule</span></span>|[<span data-ttu-id="8beda-417">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8beda-417">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="8beda-418">Да</span><span class="sxs-lookup"><span data-stu-id="8beda-418">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="8beda-419">Запрос</span><span class="sxs-lookup"><span data-stu-id="8beda-419">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState":"Eligible",
  "type":"AdminExtend",
  "reason":"extend role assignment",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-05-12T23:53:55.327Z",
    "endDateTime":"2018-08-10T23:53:55.327Z"
  }
}
```
##### <a name="response"></a><span data-ttu-id="8beda-420">Ответ</span><span class="sxs-lookup"><span data-stu-id="8beda-420">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"486f0c05-47c8-4498-9c06-086a78c83004",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminExtend",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "roleAssignmentStartDateTime":"2018-05-12T23:54:09.7221332Z",
  "roleAssignmentEndDateTime":"2018-08-10T23:53:55.327Z",
  "reason":"extend role assignment",
  "status":{
    "status":"InProgress",
    "subStatus":"Granted",
    "statusDetails":[
      {
        "key":"AdminRequestRule","value":"Grant"
      },{
        "key":"ExpirationRule","value":"Grant"
      },{
        "key":"MfaRule","value":"Grant"
      }
    ]
  },
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-05-12T23:53:55.327Z",
    "endDateTime":"2018-08-10T23:53:55.327Z",
    "duration":"PT0S"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Post roleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
