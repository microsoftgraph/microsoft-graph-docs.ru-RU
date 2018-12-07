---
title: Создание governanceRoleAssignmentRequest
description: Создание роли назначения запроса для представления операции, требуется на назначения ролей. В следующей таблице перечислены операции.
ms.openlocfilehash: 775cc8e22e7d273bfe387e5be2cc183d3d919a38
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191174"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="106a3-104">Создание governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="106a3-104">Create governanceRoleAssignmentRequest</span></span>

> <span data-ttu-id="106a3-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="106a3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="106a3-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="106a3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="106a3-107">Создание роли назначения запроса для представления операции, требуется на назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="106a3-107">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="106a3-108">В следующей таблице перечислены операции.</span><span class="sxs-lookup"><span data-stu-id="106a3-108">The following table lists the operations.</span></span>

| <span data-ttu-id="106a3-109">Операция</span><span class="sxs-lookup"><span data-stu-id="106a3-109">Operation</span></span>       | <span data-ttu-id="106a3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="106a3-110">Type</span></span> | 
|:---------------|:----------|
| <span data-ttu-id="106a3-111">Назначение назначения ролей</span><span class="sxs-lookup"><span data-stu-id="106a3-111">Assign a role assignment</span></span>| <span data-ttu-id="106a3-112">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="106a3-112">AdminAdd</span></span> |
| <span data-ttu-id="106a3-113">Активация назначение подходящими роли</span><span class="sxs-lookup"><span data-stu-id="106a3-113">Activate an eligible role assignment</span></span>| <span data-ttu-id="106a3-114">UserAdd</span><span class="sxs-lookup"><span data-stu-id="106a3-114">UserAdd</span></span> | 
| <span data-ttu-id="106a3-115">Деактивация назначение активированные роли</span><span class="sxs-lookup"><span data-stu-id="106a3-115">Deactivate an activated role assignment</span></span>| <span data-ttu-id="106a3-116">UserRemove</span><span class="sxs-lookup"><span data-stu-id="106a3-116">UserRemove</span></span> | 
| <span data-ttu-id="106a3-117">Удаление назначения ролей</span><span class="sxs-lookup"><span data-stu-id="106a3-117">Remove a role assignment</span></span>| <span data-ttu-id="106a3-118">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="106a3-118">AdminRemove</span></span> |
| <span data-ttu-id="106a3-119">Обновление назначения ролей</span><span class="sxs-lookup"><span data-stu-id="106a3-119">Update a role assignment</span></span>| <span data-ttu-id="106a3-120">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="106a3-120">AdminUpdate</span></span> |
| <span data-ttu-id="106a3-121">Запрос на расширение my назначения роли</span><span class="sxs-lookup"><span data-stu-id="106a3-121">Request to extend my role assignment</span></span>| <span data-ttu-id="106a3-122">UserExtend</span><span class="sxs-lookup"><span data-stu-id="106a3-122">UserExtend</span></span> | 
| <span data-ttu-id="106a3-123">Расширение назначения ролей</span><span class="sxs-lookup"><span data-stu-id="106a3-123">Extend a role assignment</span></span>| <span data-ttu-id="106a3-124">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="106a3-124">AdminExtend</span></span> | 
| <span data-ttu-id="106a3-125">Запрос на обновление назначения ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="106a3-125">Request to renew my expired role assignment</span></span>| <span data-ttu-id="106a3-126">UserRenew</span><span class="sxs-lookup"><span data-stu-id="106a3-126">UserRenew</span></span> | 
| <span data-ttu-id="106a3-127">Обновление назначения ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="106a3-127">Renew an expired role assignment</span></span>| <span data-ttu-id="106a3-128">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="106a3-128">AdminRenew</span></span> | 

 
## <a name="permissions"></a><span data-ttu-id="106a3-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="106a3-129">Permissions</span></span>
<span data-ttu-id="106a3-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="106a3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="106a3-132">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="106a3-132">Permission type</span></span>      | <span data-ttu-id="106a3-133">Разрешения</span><span class="sxs-lookup"><span data-stu-id="106a3-133">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="106a3-134">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="106a3-134">Delegated (work or school account)</span></span> | <span data-ttu-id="106a3-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="106a3-135">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="106a3-136">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="106a3-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="106a3-137">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="106a3-137">Not supported.</span></span>    |
|<span data-ttu-id="106a3-138">Для приложений</span><span class="sxs-lookup"><span data-stu-id="106a3-138">Application</span></span> | <span data-ttu-id="106a3-139">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="106a3-139">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="106a3-140">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="106a3-140">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="106a3-141">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="106a3-141">Request headers</span></span>
| <span data-ttu-id="106a3-142">Имя</span><span class="sxs-lookup"><span data-stu-id="106a3-142">Name</span></span>       | <span data-ttu-id="106a3-143">Описание</span><span class="sxs-lookup"><span data-stu-id="106a3-143">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="106a3-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="106a3-144">Authorization</span></span>  | <span data-ttu-id="106a3-145">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="106a3-145">Bearer {code}</span></span>|
| <span data-ttu-id="106a3-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="106a3-146">Content-type</span></span>  | <span data-ttu-id="106a3-147">application/json</span><span class="sxs-lookup"><span data-stu-id="106a3-147">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="106a3-148">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="106a3-148">Request body</span></span>
<span data-ttu-id="106a3-149">В тексте запроса укажите представление JSON объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="106a3-149">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="106a3-150">Свойство</span><span class="sxs-lookup"><span data-stu-id="106a3-150">Property</span></span>     | <span data-ttu-id="106a3-151">Тип</span><span class="sxs-lookup"><span data-stu-id="106a3-151">Type</span></span>    |<span data-ttu-id="106a3-152">Обязательный</span><span class="sxs-lookup"><span data-stu-id="106a3-152">Required</span></span>|  <span data-ttu-id="106a3-153">Описание</span><span class="sxs-lookup"><span data-stu-id="106a3-153">Description</span></span>|
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="106a3-154">resourceId</span><span class="sxs-lookup"><span data-stu-id="106a3-154">resourceId</span></span>|<span data-ttu-id="106a3-155">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-155">String</span></span>|<span data-ttu-id="106a3-156">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-156">Yes</span></span>|<span data-ttu-id="106a3-157">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="106a3-157">The ID of the resource.</span></span>|
|<span data-ttu-id="106a3-158">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="106a3-158">roleDefinitionId</span></span>|<span data-ttu-id="106a3-159">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-159">String</span></span>|<span data-ttu-id="106a3-160">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-160">Yes</span></span>|<span data-ttu-id="106a3-161">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="106a3-161">The ID of the role definition.</span></span>|
|<span data-ttu-id="106a3-162">subjectId</span><span class="sxs-lookup"><span data-stu-id="106a3-162">subjectId</span></span>|<span data-ttu-id="106a3-163">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-163">String</span></span>|<span data-ttu-id="106a3-164">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-164">Yes</span></span>|<span data-ttu-id="106a3-165">Идентификатор субъекта.</span><span class="sxs-lookup"><span data-stu-id="106a3-165">The ID of the subject.</span></span>|
|<span data-ttu-id="106a3-166">assignmentState</span><span class="sxs-lookup"><span data-stu-id="106a3-166">assignmentState</span></span>|<span data-ttu-id="106a3-167">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-167">String</span></span>|<span data-ttu-id="106a3-168">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-168">Yes</span></span>|<span data-ttu-id="106a3-169">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="106a3-169">The state of assignment.</span></span> <span data-ttu-id="106a3-170">Значение может быть ``Eligible`` и ``Active``.</span><span class="sxs-lookup"><span data-stu-id="106a3-170">The value can be ``Eligible`` and ``Active``.</span></span>|
|<span data-ttu-id="106a3-171">type</span><span class="sxs-lookup"><span data-stu-id="106a3-171">type</span></span>|<span data-ttu-id="106a3-172">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-172">String</span></span>|<span data-ttu-id="106a3-173">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-173">Yes</span></span>|<span data-ttu-id="106a3-174">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="106a3-174">The request type.</span></span> <span data-ttu-id="106a3-175">Значение может быть `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`и `AdminExtend`.</span><span class="sxs-lookup"><span data-stu-id="106a3-175">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span>|
|<span data-ttu-id="106a3-176">Причина</span><span class="sxs-lookup"><span data-stu-id="106a3-176">reason</span></span>|<span data-ttu-id="106a3-177">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-177">String</span></span>| |<span data-ttu-id="106a3-178">Причину должно предоставляться для запроса назначений ролей для аудита и предварительный просмотр цели.</span><span class="sxs-lookup"><span data-stu-id="106a3-178">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="106a3-179">расписание</span><span class="sxs-lookup"><span data-stu-id="106a3-179">schedule</span></span>|[<span data-ttu-id="106a3-180">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="106a3-180">governanceSchedule</span></span>](../resources/governanceschedule.md)| | <span data-ttu-id="106a3-181">Расписание для запроса назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="106a3-181">The schedule of the role assignment request.</span></span> <span data-ttu-id="106a3-182">Для запроса типа `UserAdd`, `AdminAdd`, `AdminUpdate`, и `AdminExtend`, это необходимо.</span><span class="sxs-lookup"><span data-stu-id="106a3-182">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span>|

## <a name="response"></a><span data-ttu-id="106a3-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="106a3-183">Response</span></span>
<span data-ttu-id="106a3-184">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="106a3-184">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="106a3-185">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="106a3-185">Error codes</span></span>
<span data-ttu-id="106a3-186">Этот интерфейс API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="106a3-186">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="106a3-187">Кроме того он возвращает коды ошибок, перечисленных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="106a3-187">In addition, it also returns the error codes listed in the following table.</span></span>

|<span data-ttu-id="106a3-188">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="106a3-188">Error code</span></span>     | <span data-ttu-id="106a3-189">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="106a3-189">Error message</span></span>              | <span data-ttu-id="106a3-190">Сведения</span><span class="sxs-lookup"><span data-stu-id="106a3-190">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="106a3-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="106a3-191">400 BadRequest</span></span> | <span data-ttu-id="106a3-192">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="106a3-192">RoleNotFound</span></span>    | <span data-ttu-id="106a3-193">`roleDefinitionId` Условии, что в запросе не удается найти текст.</span><span class="sxs-lookup"><span data-stu-id="106a3-193">The `roleDefinitionId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="106a3-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="106a3-194">400 BadRequest</span></span> | <span data-ttu-id="106a3-195">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="106a3-195">ResourceIsLocked</span></span>    | <span data-ttu-id="106a3-196">Ресурс, представленные в тексте запроса находится в состоянии из `Locked` и не могут создавать запросы назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="106a3-196">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span>
| <span data-ttu-id="106a3-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="106a3-197">400 BadRequest</span></span> | <span data-ttu-id="106a3-198">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="106a3-198">SubjectNotFound</span></span>    | <span data-ttu-id="106a3-199">`subjectId` Условии, что в запросе не удается найти текст.</span><span class="sxs-lookup"><span data-stu-id="106a3-199">The `subjectId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="106a3-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="106a3-200">400 BadRequest</span></span> | <span data-ttu-id="106a3-201">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="106a3-201">PendingRoleAssignmentRequest</span></span>    | <span data-ttu-id="106a3-202">Уже существует ожидающие [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в системе.</span><span class="sxs-lookup"><span data-stu-id="106a3-202">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span>
| <span data-ttu-id="106a3-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="106a3-203">400 BadRequest</span></span> | <span data-ttu-id="106a3-204">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="106a3-204">RoleAssignmentExists</span></span>    | <span data-ttu-id="106a3-205">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) запрошено будет создан уже существует в системе.</span><span class="sxs-lookup"><span data-stu-id="106a3-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span>
| <span data-ttu-id="106a3-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="106a3-206">400 BadRequest</span></span> | <span data-ttu-id="106a3-207">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="106a3-207">RoleAssignmentDoesNotExist</span></span>    | <span data-ttu-id="106a3-208">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) запрос на обновление/расширить не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="106a3-208">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span>
| <span data-ttu-id="106a3-209">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="106a3-209">400 BadRequest</span></span> | <span data-ttu-id="106a3-210">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="106a3-210">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="106a3-211">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) не соответствует внутренней политик и не может быть создан.</span><span class="sxs-lookup"><span data-stu-id="106a3-211">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span>

## <a name="examples"></a><span data-ttu-id="106a3-212">Примеры</span><span class="sxs-lookup"><span data-stu-id="106a3-212">Examples</span></span>
<span data-ttu-id="106a3-213">В приведенных ниже примерах показано, как использовать этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="106a3-213">The following examples show how to use this API.</span></span>

### <a name="example-1"></a><span data-ttu-id="106a3-214">Пример 1</span><span class="sxs-lookup"><span data-stu-id="106a3-214">Example 1</span></span>
<span data-ttu-id="106a3-215">В этом примере администраторам назначение роли выставления счетов читатель nawu@fimdev.net пользователя.</span><span class="sxs-lookup"><span data-stu-id="106a3-215">In this example, administrators assign user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="106a3-216">**Примечание:** В дополнение к разрешение, в этом примере требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="106a3-216">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="106a3-217">Свойство</span><span class="sxs-lookup"><span data-stu-id="106a3-217">Property</span></span>     | <span data-ttu-id="106a3-218">Тип</span><span class="sxs-lookup"><span data-stu-id="106a3-218">Type</span></span>    |<span data-ttu-id="106a3-219">Обязательный</span><span class="sxs-lookup"><span data-stu-id="106a3-219">Required</span></span>|  <span data-ttu-id="106a3-220">Значение</span><span class="sxs-lookup"><span data-stu-id="106a3-220">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="106a3-221">resourceId</span><span class="sxs-lookup"><span data-stu-id="106a3-221">resourceId</span></span>|<span data-ttu-id="106a3-222">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-222">String</span></span>|<span data-ttu-id="106a3-223">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-223">Yes</span></span>|<span data-ttu-id="106a3-224">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="106a3-224">\<resourceId\></span></span>|
|<span data-ttu-id="106a3-225">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="106a3-225">roleDefinitionId</span></span>|<span data-ttu-id="106a3-226">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-226">String</span></span>|<span data-ttu-id="106a3-227">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-227">Yes</span></span>|<span data-ttu-id="106a3-228">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="106a3-228">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="106a3-229">subjectId</span><span class="sxs-lookup"><span data-stu-id="106a3-229">subjectId</span></span>|<span data-ttu-id="106a3-230">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-230">String</span></span>|<span data-ttu-id="106a3-231">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-231">Yes</span></span>|<span data-ttu-id="106a3-232">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="106a3-232">\<subjectId\></span></span>|
|<span data-ttu-id="106a3-233">assignmentState</span><span class="sxs-lookup"><span data-stu-id="106a3-233">assignmentState</span></span>|<span data-ttu-id="106a3-234">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-234">String</span></span>|<span data-ttu-id="106a3-235">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-235">Yes</span></span>| <span data-ttu-id="106a3-236">Допустимость / Active</span><span class="sxs-lookup"><span data-stu-id="106a3-236">Eligible / Active</span></span>|
|<span data-ttu-id="106a3-237">type</span><span class="sxs-lookup"><span data-stu-id="106a3-237">type</span></span>|<span data-ttu-id="106a3-238">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-238">String</span></span>|<span data-ttu-id="106a3-239">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-239">Yes</span></span>| <span data-ttu-id="106a3-240">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="106a3-240">AdminAdd</span></span>|
|<span data-ttu-id="106a3-241">Причина</span><span class="sxs-lookup"><span data-stu-id="106a3-241">reason</span></span>|<span data-ttu-id="106a3-242">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-242">String</span></span>| <span data-ttu-id="106a3-243">зависит от роли параметров</span><span class="sxs-lookup"><span data-stu-id="106a3-243">depends on role Settings</span></span>||
|<span data-ttu-id="106a3-244">расписание</span><span class="sxs-lookup"><span data-stu-id="106a3-244">schedule</span></span>|[<span data-ttu-id="106a3-245">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="106a3-245">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="106a3-246">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-246">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="106a3-247">Запрос</span><span class="sxs-lookup"><span data-stu-id="106a3-247">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="106a3-248">Отклик</span><span class="sxs-lookup"><span data-stu-id="106a3-248">Response</span></span>
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

### <a name="example-2"></a><span data-ttu-id="106a3-249">Пример 2</span><span class="sxs-lookup"><span data-stu-id="106a3-249">Example 2</span></span>
<span data-ttu-id="106a3-250">В этом примере nawu@fimdev.net пользователь активирует право чтения выставления счетов роли.</span><span class="sxs-lookup"><span data-stu-id="106a3-250">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="106a3-251">Свойство</span><span class="sxs-lookup"><span data-stu-id="106a3-251">Property</span></span>     | <span data-ttu-id="106a3-252">Тип</span><span class="sxs-lookup"><span data-stu-id="106a3-252">Type</span></span>    |<span data-ttu-id="106a3-253">Обязательный</span><span class="sxs-lookup"><span data-stu-id="106a3-253">Required</span></span>|  <span data-ttu-id="106a3-254">Значение</span><span class="sxs-lookup"><span data-stu-id="106a3-254">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="106a3-255">resourceId</span><span class="sxs-lookup"><span data-stu-id="106a3-255">resourceId</span></span>|<span data-ttu-id="106a3-256">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-256">String</span></span>|<span data-ttu-id="106a3-257">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-257">Yes</span></span>|<span data-ttu-id="106a3-258">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="106a3-258">\<resourceId\></span></span>|
|<span data-ttu-id="106a3-259">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="106a3-259">roleDefinitionId</span></span>|<span data-ttu-id="106a3-260">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-260">String</span></span>|<span data-ttu-id="106a3-261">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-261">Yes</span></span>|<span data-ttu-id="106a3-262">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="106a3-262">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="106a3-263">subjectId</span><span class="sxs-lookup"><span data-stu-id="106a3-263">subjectId</span></span>|<span data-ttu-id="106a3-264">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-264">String</span></span>|<span data-ttu-id="106a3-265">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-265">Yes</span></span>|<span data-ttu-id="106a3-266">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="106a3-266">\<subjectId\></span></span>|
|<span data-ttu-id="106a3-267">assignmentState</span><span class="sxs-lookup"><span data-stu-id="106a3-267">assignmentState</span></span>|<span data-ttu-id="106a3-268">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-268">String</span></span>|<span data-ttu-id="106a3-269">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-269">Yes</span></span>| <span data-ttu-id="106a3-270">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="106a3-270">Active</span></span>|
|<span data-ttu-id="106a3-271">type</span><span class="sxs-lookup"><span data-stu-id="106a3-271">type</span></span>|<span data-ttu-id="106a3-272">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-272">String</span></span>|<span data-ttu-id="106a3-273">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-273">Yes</span></span>| <span data-ttu-id="106a3-274">UserAdd</span><span class="sxs-lookup"><span data-stu-id="106a3-274">UserAdd</span></span>|
|<span data-ttu-id="106a3-275">Причина</span><span class="sxs-lookup"><span data-stu-id="106a3-275">reason</span></span>|<span data-ttu-id="106a3-276">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-276">String</span></span>| <span data-ttu-id="106a3-277">зависит от роли параметров</span><span class="sxs-lookup"><span data-stu-id="106a3-277">depends on role Settings</span></span>||
|<span data-ttu-id="106a3-278">расписание</span><span class="sxs-lookup"><span data-stu-id="106a3-278">schedule</span></span>|[<span data-ttu-id="106a3-279">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="106a3-279">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="106a3-280">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-280">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="106a3-281">Запрос</span><span class="sxs-lookup"><span data-stu-id="106a3-281">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="106a3-282">Отклик</span><span class="sxs-lookup"><span data-stu-id="106a3-282">Response</span></span>
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

### <a name="example-3"></a><span data-ttu-id="106a3-283">Пример 3</span><span class="sxs-lookup"><span data-stu-id="106a3-283">Example 3</span></span>
<span data-ttu-id="106a3-284">В этом примере пользователь nawu@fimdev.net деактивирует активная роль чтения выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="106a3-284">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="106a3-285">Свойство</span><span class="sxs-lookup"><span data-stu-id="106a3-285">Property</span></span>     | <span data-ttu-id="106a3-286">Тип</span><span class="sxs-lookup"><span data-stu-id="106a3-286">Type</span></span>    |<span data-ttu-id="106a3-287">Обязательный</span><span class="sxs-lookup"><span data-stu-id="106a3-287">Required</span></span>|  <span data-ttu-id="106a3-288">Значение</span><span class="sxs-lookup"><span data-stu-id="106a3-288">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="106a3-289">resourceId</span><span class="sxs-lookup"><span data-stu-id="106a3-289">resourceId</span></span>|<span data-ttu-id="106a3-290">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-290">String</span></span>|<span data-ttu-id="106a3-291">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-291">Yes</span></span>|<span data-ttu-id="106a3-292">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="106a3-292">\<resourceId\></span></span>|
|<span data-ttu-id="106a3-293">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="106a3-293">roleDefinitionId</span></span>|<span data-ttu-id="106a3-294">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-294">String</span></span>|<span data-ttu-id="106a3-295">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-295">Yes</span></span>|<span data-ttu-id="106a3-296">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="106a3-296">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="106a3-297">subjectId</span><span class="sxs-lookup"><span data-stu-id="106a3-297">subjectId</span></span>|<span data-ttu-id="106a3-298">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-298">String</span></span>|<span data-ttu-id="106a3-299">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-299">Yes</span></span>|<span data-ttu-id="106a3-300">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="106a3-300">\<subjectId\></span></span>|
|<span data-ttu-id="106a3-301">assignmentState</span><span class="sxs-lookup"><span data-stu-id="106a3-301">assignmentState</span></span>|<span data-ttu-id="106a3-302">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-302">String</span></span>|<span data-ttu-id="106a3-303">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-303">Yes</span></span>| <span data-ttu-id="106a3-304">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="106a3-304">Active</span></span>|
|<span data-ttu-id="106a3-305">type</span><span class="sxs-lookup"><span data-stu-id="106a3-305">type</span></span>|<span data-ttu-id="106a3-306">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-306">String</span></span>|<span data-ttu-id="106a3-307">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-307">Yes</span></span>| <span data-ttu-id="106a3-308">UserRemove</span><span class="sxs-lookup"><span data-stu-id="106a3-308">UserRemove</span></span>|
|<span data-ttu-id="106a3-309">Причина</span><span class="sxs-lookup"><span data-stu-id="106a3-309">reason</span></span>|<span data-ttu-id="106a3-310">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-310">String</span></span>| <span data-ttu-id="106a3-311">Нет</span><span class="sxs-lookup"><span data-stu-id="106a3-311">No</span></span>||
|<span data-ttu-id="106a3-312">расписание</span><span class="sxs-lookup"><span data-stu-id="106a3-312">schedule</span></span>|[<span data-ttu-id="106a3-313">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="106a3-313">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="106a3-314">Нет</span><span class="sxs-lookup"><span data-stu-id="106a3-314">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="106a3-315">Запрос</span><span class="sxs-lookup"><span data-stu-id="106a3-315">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="106a3-316">Отклик</span><span class="sxs-lookup"><span data-stu-id="106a3-316">Response</span></span>
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
    "reason": "Evaluate only",
    "schedule": null,
    "status": {
        "status": "Closed",
        "subStatus": "Revoked",
        "statusDetails": []
    }
}
```

### <a name="example-4"></a><span data-ttu-id="106a3-317">Пример 4</span><span class="sxs-lookup"><span data-stu-id="106a3-317">Example 4</span></span>
<span data-ttu-id="106a3-318">В этом примере администраторам удалить nawu@fimdev.net пользователя из роли выставления счетов чтения.</span><span class="sxs-lookup"><span data-stu-id="106a3-318">In this example, administrators remove the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="106a3-319">**Примечание:** В дополнение к разрешение, в этом примере требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="106a3-319">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="106a3-320">Свойство</span><span class="sxs-lookup"><span data-stu-id="106a3-320">Property</span></span>     | <span data-ttu-id="106a3-321">Тип</span><span class="sxs-lookup"><span data-stu-id="106a3-321">Type</span></span>    |<span data-ttu-id="106a3-322">Обязательный</span><span class="sxs-lookup"><span data-stu-id="106a3-322">Required</span></span>|  <span data-ttu-id="106a3-323">Значение</span><span class="sxs-lookup"><span data-stu-id="106a3-323">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="106a3-324">resourceId</span><span class="sxs-lookup"><span data-stu-id="106a3-324">resourceId</span></span>|<span data-ttu-id="106a3-325">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-325">String</span></span>|<span data-ttu-id="106a3-326">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-326">Yes</span></span>|<span data-ttu-id="106a3-327">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="106a3-327">\<resourceId\></span></span>|
|<span data-ttu-id="106a3-328">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="106a3-328">roleDefinitionId</span></span>|<span data-ttu-id="106a3-329">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-329">String</span></span>|<span data-ttu-id="106a3-330">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-330">Yes</span></span>|<span data-ttu-id="106a3-331">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="106a3-331">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="106a3-332">subjectId</span><span class="sxs-lookup"><span data-stu-id="106a3-332">subjectId</span></span>|<span data-ttu-id="106a3-333">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-333">String</span></span>|<span data-ttu-id="106a3-334">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-334">Yes</span></span>|<span data-ttu-id="106a3-335">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="106a3-335">\<subjectId\></span></span>|
|<span data-ttu-id="106a3-336">assignmentState</span><span class="sxs-lookup"><span data-stu-id="106a3-336">assignmentState</span></span>|<span data-ttu-id="106a3-337">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-337">String</span></span>|<span data-ttu-id="106a3-338">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-338">Yes</span></span>| <span data-ttu-id="106a3-339">Допустимость / Active</span><span class="sxs-lookup"><span data-stu-id="106a3-339">Eligible / Active</span></span>|
|<span data-ttu-id="106a3-340">type</span><span class="sxs-lookup"><span data-stu-id="106a3-340">type</span></span>|<span data-ttu-id="106a3-341">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-341">String</span></span>|<span data-ttu-id="106a3-342">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-342">Yes</span></span>| <span data-ttu-id="106a3-343">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="106a3-343">AdminRemove</span></span>|
|<span data-ttu-id="106a3-344">Причина</span><span class="sxs-lookup"><span data-stu-id="106a3-344">reason</span></span>|<span data-ttu-id="106a3-345">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-345">String</span></span>| <span data-ttu-id="106a3-346">Нет</span><span class="sxs-lookup"><span data-stu-id="106a3-346">No</span></span>||
|<span data-ttu-id="106a3-347">расписание</span><span class="sxs-lookup"><span data-stu-id="106a3-347">schedule</span></span>|[<span data-ttu-id="106a3-348">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="106a3-348">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="106a3-349">Нет</span><span class="sxs-lookup"><span data-stu-id="106a3-349">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="106a3-350">Запрос</span><span class="sxs-lookup"><span data-stu-id="106a3-350">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="106a3-351">Отклик</span><span class="sxs-lookup"><span data-stu-id="106a3-351">Response</span></span>
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
  "reason":null,
  "status":{
    "status":"Closed",
    "subStatus":"Revoked",
    "statusDetails":[]
  },
  "schedule":null
}
```

### <a name="example-5"></a><span data-ttu-id="106a3-352">Пример 5</span><span class="sxs-lookup"><span data-stu-id="106a3-352">Example 5</span></span>
<span data-ttu-id="106a3-353">В этом примере Администраторы обновление назначения ролей для пользователя nawu@fimdev.net владельцу.</span><span class="sxs-lookup"><span data-stu-id="106a3-353">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="106a3-354">**Примечание:** В дополнение к разрешение, в этом примере требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="106a3-354">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="106a3-355">Свойство</span><span class="sxs-lookup"><span data-stu-id="106a3-355">Property</span></span>     | <span data-ttu-id="106a3-356">Тип</span><span class="sxs-lookup"><span data-stu-id="106a3-356">Type</span></span>    |<span data-ttu-id="106a3-357">Обязательный</span><span class="sxs-lookup"><span data-stu-id="106a3-357">Required</span></span>|  <span data-ttu-id="106a3-358">Значение</span><span class="sxs-lookup"><span data-stu-id="106a3-358">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="106a3-359">resourceId</span><span class="sxs-lookup"><span data-stu-id="106a3-359">resourceId</span></span>|<span data-ttu-id="106a3-360">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-360">String</span></span>|<span data-ttu-id="106a3-361">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-361">Yes</span></span>|<span data-ttu-id="106a3-362">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="106a3-362">\<resourceId\></span></span>|
|<span data-ttu-id="106a3-363">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="106a3-363">roleDefinitionId</span></span>|<span data-ttu-id="106a3-364">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-364">String</span></span>|<span data-ttu-id="106a3-365">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-365">Yes</span></span>|<span data-ttu-id="106a3-366">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="106a3-366">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="106a3-367">subjectId</span><span class="sxs-lookup"><span data-stu-id="106a3-367">subjectId</span></span>|<span data-ttu-id="106a3-368">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-368">String</span></span>|<span data-ttu-id="106a3-369">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-369">Yes</span></span>|<span data-ttu-id="106a3-370">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="106a3-370">\<subjectId\></span></span>|
|<span data-ttu-id="106a3-371">assignmentState</span><span class="sxs-lookup"><span data-stu-id="106a3-371">assignmentState</span></span>|<span data-ttu-id="106a3-372">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-372">String</span></span>|<span data-ttu-id="106a3-373">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-373">Yes</span></span>| <span data-ttu-id="106a3-374">Допустимость / Active</span><span class="sxs-lookup"><span data-stu-id="106a3-374">Eligible / Active</span></span>|
|<span data-ttu-id="106a3-375">type</span><span class="sxs-lookup"><span data-stu-id="106a3-375">type</span></span>|<span data-ttu-id="106a3-376">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-376">String</span></span>|<span data-ttu-id="106a3-377">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-377">Yes</span></span>| <span data-ttu-id="106a3-378">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="106a3-378">AdminUpdate</span></span>|
|<span data-ttu-id="106a3-379">Причина</span><span class="sxs-lookup"><span data-stu-id="106a3-379">reason</span></span>|<span data-ttu-id="106a3-380">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-380">String</span></span>| <span data-ttu-id="106a3-381">зависит от roleSettings</span><span class="sxs-lookup"><span data-stu-id="106a3-381">depends on roleSettings</span></span>||
|<span data-ttu-id="106a3-382">расписание</span><span class="sxs-lookup"><span data-stu-id="106a3-382">schedule</span></span>|[<span data-ttu-id="106a3-383">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="106a3-383">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="106a3-384">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-384">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="106a3-385">Запрос</span><span class="sxs-lookup"><span data-stu-id="106a3-385">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="106a3-386">Отклик</span><span class="sxs-lookup"><span data-stu-id="106a3-386">Response</span></span>
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

### <a name="example-6"></a><span data-ttu-id="106a3-387">В примере 6</span><span class="sxs-lookup"><span data-stu-id="106a3-387">Example 6</span></span>
<span data-ttu-id="106a3-388">В этом примере расширяет истекающим сроком действия назначения ролей для пользователя ANUJCUSER для участника службы управления API.</span><span class="sxs-lookup"><span data-stu-id="106a3-388">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="106a3-389">**Примечание:** В additon разрешение, в этом примере требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="106a3-389">**Note:** In additon to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="106a3-390">Свойство</span><span class="sxs-lookup"><span data-stu-id="106a3-390">Property</span></span>     | <span data-ttu-id="106a3-391">Тип</span><span class="sxs-lookup"><span data-stu-id="106a3-391">Type</span></span>    |<span data-ttu-id="106a3-392">Обязательный</span><span class="sxs-lookup"><span data-stu-id="106a3-392">Required</span></span>|  <span data-ttu-id="106a3-393">Значение</span><span class="sxs-lookup"><span data-stu-id="106a3-393">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="106a3-394">resourceId</span><span class="sxs-lookup"><span data-stu-id="106a3-394">resourceId</span></span>|<span data-ttu-id="106a3-395">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-395">String</span></span>|<span data-ttu-id="106a3-396">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-396">Yes</span></span>|<span data-ttu-id="106a3-397">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="106a3-397">\<resourceId\></span></span>|
|<span data-ttu-id="106a3-398">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="106a3-398">roleDefinitionId</span></span>|<span data-ttu-id="106a3-399">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-399">String</span></span>|<span data-ttu-id="106a3-400">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-400">Yes</span></span>|<span data-ttu-id="106a3-401">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="106a3-401">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="106a3-402">subjectId</span><span class="sxs-lookup"><span data-stu-id="106a3-402">subjectId</span></span>|<span data-ttu-id="106a3-403">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-403">String</span></span>|<span data-ttu-id="106a3-404">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-404">Yes</span></span>|<span data-ttu-id="106a3-405">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="106a3-405">\<subjectId\></span></span>|
|<span data-ttu-id="106a3-406">assignmentState</span><span class="sxs-lookup"><span data-stu-id="106a3-406">assignmentState</span></span>|<span data-ttu-id="106a3-407">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-407">String</span></span>|<span data-ttu-id="106a3-408">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-408">Yes</span></span>| <span data-ttu-id="106a3-409">Допустимость / Active</span><span class="sxs-lookup"><span data-stu-id="106a3-409">Eligible / Active</span></span> |
|<span data-ttu-id="106a3-410">type</span><span class="sxs-lookup"><span data-stu-id="106a3-410">type</span></span>|<span data-ttu-id="106a3-411">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-411">String</span></span>|<span data-ttu-id="106a3-412">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-412">Yes</span></span>| <span data-ttu-id="106a3-413">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="106a3-413">AdminExtend</span></span>|
|<span data-ttu-id="106a3-414">Причина</span><span class="sxs-lookup"><span data-stu-id="106a3-414">reason</span></span>|<span data-ttu-id="106a3-415">Строка</span><span class="sxs-lookup"><span data-stu-id="106a3-415">String</span></span>| <span data-ttu-id="106a3-416">зависит от roleSettings</span><span class="sxs-lookup"><span data-stu-id="106a3-416">depends on roleSettings</span></span>||
|<span data-ttu-id="106a3-417">расписание</span><span class="sxs-lookup"><span data-stu-id="106a3-417">schedule</span></span>|[<span data-ttu-id="106a3-418">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="106a3-418">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="106a3-419">Да</span><span class="sxs-lookup"><span data-stu-id="106a3-419">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="106a3-420">Запрос</span><span class="sxs-lookup"><span data-stu-id="106a3-420">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="106a3-421">Отклик</span><span class="sxs-lookup"><span data-stu-id="106a3-421">Response</span></span>
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
