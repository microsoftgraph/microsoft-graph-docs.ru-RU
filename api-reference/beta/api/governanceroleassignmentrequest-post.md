---
title: Создание governanceRoleAssignmentRequest
description: Создание роли назначения запроса для представления операции, требуется на назначения ролей. В следующей таблице перечислены операции.
localization_priority: Normal
ms.openlocfilehash: 0fc8d96585daf63f53bc6b33985a289e8f810d6b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572369"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="00840-104">Создание governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="00840-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00840-105">Создание роли назначения запроса для представления операции, требуется на назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="00840-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="00840-106">В следующей таблице перечислены операции.</span><span class="sxs-lookup"><span data-stu-id="00840-106">The following table lists the operations.</span></span>

| <span data-ttu-id="00840-107">Operation</span><span class="sxs-lookup"><span data-stu-id="00840-107">Operation</span></span>       | <span data-ttu-id="00840-108">Тип</span><span class="sxs-lookup"><span data-stu-id="00840-108">Type</span></span> | 
|:---------------|:----------|
| <span data-ttu-id="00840-109">Назначение назначения ролей</span><span class="sxs-lookup"><span data-stu-id="00840-109">Assign a role assignment</span></span>| <span data-ttu-id="00840-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="00840-110">AdminAdd</span></span> |
| <span data-ttu-id="00840-111">Активация назначение подходящими роли</span><span class="sxs-lookup"><span data-stu-id="00840-111">Activate an eligible role assignment</span></span>| <span data-ttu-id="00840-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="00840-112">UserAdd</span></span> | 
| <span data-ttu-id="00840-113">Деактивация назначение активированные роли</span><span class="sxs-lookup"><span data-stu-id="00840-113">Deactivate an activated role assignment</span></span>| <span data-ttu-id="00840-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="00840-114">UserRemove</span></span> | 
| <span data-ttu-id="00840-115">Удаление назначения ролей</span><span class="sxs-lookup"><span data-stu-id="00840-115">Remove a role assignment</span></span>| <span data-ttu-id="00840-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="00840-116">AdminRemove</span></span> |
| <span data-ttu-id="00840-117">Обновление назначения ролей</span><span class="sxs-lookup"><span data-stu-id="00840-117">Update a role assignment</span></span>| <span data-ttu-id="00840-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="00840-118">AdminUpdate</span></span> |
| <span data-ttu-id="00840-119">Запрос на расширение my назначения роли</span><span class="sxs-lookup"><span data-stu-id="00840-119">Request to extend my role assignment</span></span>| <span data-ttu-id="00840-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="00840-120">UserExtend</span></span> | 
| <span data-ttu-id="00840-121">Расширение назначения ролей</span><span class="sxs-lookup"><span data-stu-id="00840-121">Extend a role assignment</span></span>| <span data-ttu-id="00840-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="00840-122">AdminExtend</span></span> | 
| <span data-ttu-id="00840-123">Запрос на обновление назначения ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="00840-123">Request to renew my expired role assignment</span></span>| <span data-ttu-id="00840-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="00840-124">UserRenew</span></span> | 
| <span data-ttu-id="00840-125">Обновление назначения ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="00840-125">Renew an expired role assignment</span></span>| <span data-ttu-id="00840-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="00840-126">AdminRenew</span></span> | 

 
## <a name="permissions"></a><span data-ttu-id="00840-127">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00840-127">Permissions</span></span>
<span data-ttu-id="00840-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00840-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00840-130">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00840-130">Permission type</span></span>      | <span data-ttu-id="00840-131">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00840-131">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00840-132">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00840-132">Delegated (work or school account)</span></span> | <span data-ttu-id="00840-133">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="00840-133">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="00840-134">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00840-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00840-135">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00840-135">Not supported.</span></span>    |
|<span data-ttu-id="00840-136">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00840-136">Application</span></span> | <span data-ttu-id="00840-137">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="00840-137">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="00840-138">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00840-138">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="00840-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00840-139">Request headers</span></span>
| <span data-ttu-id="00840-140">Имя</span><span class="sxs-lookup"><span data-stu-id="00840-140">Name</span></span>       | <span data-ttu-id="00840-141">Описание</span><span class="sxs-lookup"><span data-stu-id="00840-141">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="00840-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="00840-142">Authorization</span></span>  | <span data-ttu-id="00840-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="00840-143">Bearer {code}</span></span>|
| <span data-ttu-id="00840-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="00840-144">Content-type</span></span>  | <span data-ttu-id="00840-145">application/json</span><span class="sxs-lookup"><span data-stu-id="00840-145">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00840-146">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00840-146">Request body</span></span>
<span data-ttu-id="00840-147">В тексте запроса укажите представление JSON объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="00840-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="00840-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="00840-148">Property</span></span>     | <span data-ttu-id="00840-149">Тип</span><span class="sxs-lookup"><span data-stu-id="00840-149">Type</span></span>    |<span data-ttu-id="00840-150">Обязательный</span><span class="sxs-lookup"><span data-stu-id="00840-150">Required</span></span>|  <span data-ttu-id="00840-151">Описание</span><span class="sxs-lookup"><span data-stu-id="00840-151">Description</span></span>|
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="00840-152">resourceId</span><span class="sxs-lookup"><span data-stu-id="00840-152">resourceId</span></span>|<span data-ttu-id="00840-153">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-153">String</span></span>|<span data-ttu-id="00840-154">Да</span><span class="sxs-lookup"><span data-stu-id="00840-154">Yes</span></span>|<span data-ttu-id="00840-155">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="00840-155">The ID of the resource.</span></span>|
|<span data-ttu-id="00840-156">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="00840-156">roleDefinitionId</span></span>|<span data-ttu-id="00840-157">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-157">String</span></span>|<span data-ttu-id="00840-158">Да</span><span class="sxs-lookup"><span data-stu-id="00840-158">Yes</span></span>|<span data-ttu-id="00840-159">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="00840-159">The ID of the role definition.</span></span>|
|<span data-ttu-id="00840-160">subjectId</span><span class="sxs-lookup"><span data-stu-id="00840-160">subjectId</span></span>|<span data-ttu-id="00840-161">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-161">String</span></span>|<span data-ttu-id="00840-162">Да</span><span class="sxs-lookup"><span data-stu-id="00840-162">Yes</span></span>|<span data-ttu-id="00840-163">Идентификатор субъекта.</span><span class="sxs-lookup"><span data-stu-id="00840-163">The ID of the subject.</span></span>|
|<span data-ttu-id="00840-164">assignmentState</span><span class="sxs-lookup"><span data-stu-id="00840-164">assignmentState</span></span>|<span data-ttu-id="00840-165">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-165">String</span></span>|<span data-ttu-id="00840-166">Да</span><span class="sxs-lookup"><span data-stu-id="00840-166">Yes</span></span>|<span data-ttu-id="00840-167">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="00840-167">The state of assignment.</span></span> <span data-ttu-id="00840-168">Значение может быть ``Eligible`` и ``Active``.</span><span class="sxs-lookup"><span data-stu-id="00840-168">The value can be ``Eligible`` and ``Active``.</span></span>|
|<span data-ttu-id="00840-169">type</span><span class="sxs-lookup"><span data-stu-id="00840-169">type</span></span>|<span data-ttu-id="00840-170">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-170">String</span></span>|<span data-ttu-id="00840-171">Да</span><span class="sxs-lookup"><span data-stu-id="00840-171">Yes</span></span>|<span data-ttu-id="00840-172">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="00840-172">The request type.</span></span> <span data-ttu-id="00840-173">Значение может быть `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`и `AdminExtend`.</span><span class="sxs-lookup"><span data-stu-id="00840-173">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span>|
|<span data-ttu-id="00840-174">Причина</span><span class="sxs-lookup"><span data-stu-id="00840-174">reason</span></span>|<span data-ttu-id="00840-175">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-175">String</span></span>| |<span data-ttu-id="00840-176">Причину должно предоставляться для запроса назначений ролей для аудита и предварительный просмотр цели.</span><span class="sxs-lookup"><span data-stu-id="00840-176">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="00840-177">расписание</span><span class="sxs-lookup"><span data-stu-id="00840-177">schedule</span></span>|[<span data-ttu-id="00840-178">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="00840-178">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)| | <span data-ttu-id="00840-179">Расписание для запроса назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="00840-179">The schedule of the role assignment request.</span></span> <span data-ttu-id="00840-180">Для запроса типа `UserAdd`, `AdminAdd`, `AdminUpdate`, и `AdminExtend`, это необходимо.</span><span class="sxs-lookup"><span data-stu-id="00840-180">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span>|

## <a name="response"></a><span data-ttu-id="00840-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="00840-181">Response</span></span>
<span data-ttu-id="00840-182">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="00840-182">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="00840-183">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="00840-183">Error codes</span></span>
<span data-ttu-id="00840-184">Этот интерфейс API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="00840-184">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="00840-185">Кроме того он возвращает коды ошибок, перечисленных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="00840-185">In addition, it also returns the error codes listed in the following table.</span></span>

|<span data-ttu-id="00840-186">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="00840-186">Error code</span></span>     | <span data-ttu-id="00840-187">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="00840-187">Error message</span></span>              | <span data-ttu-id="00840-188">Сведения</span><span class="sxs-lookup"><span data-stu-id="00840-188">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="00840-189">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="00840-189">400 BadRequest</span></span> | <span data-ttu-id="00840-190">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="00840-190">RoleNotFound</span></span>    | <span data-ttu-id="00840-191">`roleDefinitionId` Условии, что в запросе не удается найти текст.</span><span class="sxs-lookup"><span data-stu-id="00840-191">The `roleDefinitionId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="00840-192">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="00840-192">400 BadRequest</span></span> | <span data-ttu-id="00840-193">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="00840-193">ResourceIsLocked</span></span>    | <span data-ttu-id="00840-194">Ресурс, представленные в тексте запроса находится в состоянии из `Locked` и не могут создавать запросы назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="00840-194">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span>
| <span data-ttu-id="00840-195">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="00840-195">400 BadRequest</span></span> | <span data-ttu-id="00840-196">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="00840-196">SubjectNotFound</span></span>    | <span data-ttu-id="00840-197">`subjectId` Условии, что в запросе не удается найти текст.</span><span class="sxs-lookup"><span data-stu-id="00840-197">The `subjectId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="00840-198">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="00840-198">400 BadRequest</span></span> | <span data-ttu-id="00840-199">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="00840-199">PendingRoleAssignmentRequest</span></span>    | <span data-ttu-id="00840-200">Уже существует ожидающие [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в системе.</span><span class="sxs-lookup"><span data-stu-id="00840-200">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span>
| <span data-ttu-id="00840-201">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="00840-201">400 BadRequest</span></span> | <span data-ttu-id="00840-202">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="00840-202">RoleAssignmentExists</span></span>    | <span data-ttu-id="00840-203">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) запрошено будет создан уже существует в системе.</span><span class="sxs-lookup"><span data-stu-id="00840-203">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span>
| <span data-ttu-id="00840-204">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="00840-204">400 BadRequest</span></span> | <span data-ttu-id="00840-205">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="00840-205">RoleAssignmentDoesNotExist</span></span>    | <span data-ttu-id="00840-206">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) запрос на обновление/расширить не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="00840-206">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span>
| <span data-ttu-id="00840-207">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="00840-207">400 BadRequest</span></span> | <span data-ttu-id="00840-208">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="00840-208">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="00840-209">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) не соответствует внутренней политик и не может быть создан.</span><span class="sxs-lookup"><span data-stu-id="00840-209">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span>

## <a name="examples"></a><span data-ttu-id="00840-210">Примеры</span><span class="sxs-lookup"><span data-stu-id="00840-210">Examples</span></span>
<span data-ttu-id="00840-211">В приведенных ниже примерах показано, как использовать этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="00840-211">The following examples show how to use this API.</span></span>

### <a name="example-1"></a><span data-ttu-id="00840-212">Пример 1</span><span class="sxs-lookup"><span data-stu-id="00840-212">Example 1</span></span>
<span data-ttu-id="00840-213">В этом примере администраторам назначение роли выставления счетов читатель nawu@fimdev.net пользователя.</span><span class="sxs-lookup"><span data-stu-id="00840-213">In this example, administrators assign user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="00840-214">**Примечание:** В дополнение к разрешение, в этом примере требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="00840-214">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="00840-215">Свойство</span><span class="sxs-lookup"><span data-stu-id="00840-215">Property</span></span>     | <span data-ttu-id="00840-216">Тип</span><span class="sxs-lookup"><span data-stu-id="00840-216">Type</span></span>    |<span data-ttu-id="00840-217">Обязательный</span><span class="sxs-lookup"><span data-stu-id="00840-217">Required</span></span>|  <span data-ttu-id="00840-218">Значение</span><span class="sxs-lookup"><span data-stu-id="00840-218">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="00840-219">resourceId</span><span class="sxs-lookup"><span data-stu-id="00840-219">resourceId</span></span>|<span data-ttu-id="00840-220">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-220">String</span></span>|<span data-ttu-id="00840-221">Да</span><span class="sxs-lookup"><span data-stu-id="00840-221">Yes</span></span>|<span data-ttu-id="00840-222">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="00840-222">\<resourceId\></span></span>|
|<span data-ttu-id="00840-223">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="00840-223">roleDefinitionId</span></span>|<span data-ttu-id="00840-224">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-224">String</span></span>|<span data-ttu-id="00840-225">Да</span><span class="sxs-lookup"><span data-stu-id="00840-225">Yes</span></span>|<span data-ttu-id="00840-226">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="00840-226">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="00840-227">subjectId</span><span class="sxs-lookup"><span data-stu-id="00840-227">subjectId</span></span>|<span data-ttu-id="00840-228">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-228">String</span></span>|<span data-ttu-id="00840-229">Да</span><span class="sxs-lookup"><span data-stu-id="00840-229">Yes</span></span>|<span data-ttu-id="00840-230">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="00840-230">\<subjectId\></span></span>|
|<span data-ttu-id="00840-231">assignmentState</span><span class="sxs-lookup"><span data-stu-id="00840-231">assignmentState</span></span>|<span data-ttu-id="00840-232">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-232">String</span></span>|<span data-ttu-id="00840-233">Да</span><span class="sxs-lookup"><span data-stu-id="00840-233">Yes</span></span>| <span data-ttu-id="00840-234">Допустимость / Active</span><span class="sxs-lookup"><span data-stu-id="00840-234">Eligible / Active</span></span>|
|<span data-ttu-id="00840-235">type</span><span class="sxs-lookup"><span data-stu-id="00840-235">type</span></span>|<span data-ttu-id="00840-236">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-236">String</span></span>|<span data-ttu-id="00840-237">Да</span><span class="sxs-lookup"><span data-stu-id="00840-237">Yes</span></span>| <span data-ttu-id="00840-238">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="00840-238">AdminAdd</span></span>|
|<span data-ttu-id="00840-239">Причина</span><span class="sxs-lookup"><span data-stu-id="00840-239">reason</span></span>|<span data-ttu-id="00840-240">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-240">String</span></span>| <span data-ttu-id="00840-241">зависит от роли параметров</span><span class="sxs-lookup"><span data-stu-id="00840-241">depends on role Settings</span></span>||
|<span data-ttu-id="00840-242">расписание</span><span class="sxs-lookup"><span data-stu-id="00840-242">schedule</span></span>|[<span data-ttu-id="00840-243">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="00840-243">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="00840-244">Да</span><span class="sxs-lookup"><span data-stu-id="00840-244">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="00840-245">Запрос</span><span class="sxs-lookup"><span data-stu-id="00840-245">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="00840-246">Отклик</span><span class="sxs-lookup"><span data-stu-id="00840-246">Response</span></span>
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

### <a name="example-2"></a><span data-ttu-id="00840-247">Пример 2</span><span class="sxs-lookup"><span data-stu-id="00840-247">Example 2</span></span>
<span data-ttu-id="00840-248">В этом примере nawu@fimdev.net пользователь активирует право чтения выставления счетов роли.</span><span class="sxs-lookup"><span data-stu-id="00840-248">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="00840-249">Свойство</span><span class="sxs-lookup"><span data-stu-id="00840-249">Property</span></span>     | <span data-ttu-id="00840-250">Тип</span><span class="sxs-lookup"><span data-stu-id="00840-250">Type</span></span>    |<span data-ttu-id="00840-251">Обязательный</span><span class="sxs-lookup"><span data-stu-id="00840-251">Required</span></span>|  <span data-ttu-id="00840-252">Значение</span><span class="sxs-lookup"><span data-stu-id="00840-252">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="00840-253">resourceId</span><span class="sxs-lookup"><span data-stu-id="00840-253">resourceId</span></span>|<span data-ttu-id="00840-254">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-254">String</span></span>|<span data-ttu-id="00840-255">Да</span><span class="sxs-lookup"><span data-stu-id="00840-255">Yes</span></span>|<span data-ttu-id="00840-256">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="00840-256">\<resourceId\></span></span>|
|<span data-ttu-id="00840-257">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="00840-257">roleDefinitionId</span></span>|<span data-ttu-id="00840-258">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-258">String</span></span>|<span data-ttu-id="00840-259">Да</span><span class="sxs-lookup"><span data-stu-id="00840-259">Yes</span></span>|<span data-ttu-id="00840-260">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="00840-260">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="00840-261">subjectId</span><span class="sxs-lookup"><span data-stu-id="00840-261">subjectId</span></span>|<span data-ttu-id="00840-262">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-262">String</span></span>|<span data-ttu-id="00840-263">Да</span><span class="sxs-lookup"><span data-stu-id="00840-263">Yes</span></span>|<span data-ttu-id="00840-264">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="00840-264">\<subjectId\></span></span>|
|<span data-ttu-id="00840-265">assignmentState</span><span class="sxs-lookup"><span data-stu-id="00840-265">assignmentState</span></span>|<span data-ttu-id="00840-266">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-266">String</span></span>|<span data-ttu-id="00840-267">Да</span><span class="sxs-lookup"><span data-stu-id="00840-267">Yes</span></span>| <span data-ttu-id="00840-268">Активное</span><span class="sxs-lookup"><span data-stu-id="00840-268">Active</span></span>|
|<span data-ttu-id="00840-269">type</span><span class="sxs-lookup"><span data-stu-id="00840-269">type</span></span>|<span data-ttu-id="00840-270">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-270">String</span></span>|<span data-ttu-id="00840-271">Да</span><span class="sxs-lookup"><span data-stu-id="00840-271">Yes</span></span>| <span data-ttu-id="00840-272">UserAdd</span><span class="sxs-lookup"><span data-stu-id="00840-272">UserAdd</span></span>|
|<span data-ttu-id="00840-273">Причина</span><span class="sxs-lookup"><span data-stu-id="00840-273">reason</span></span>|<span data-ttu-id="00840-274">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-274">String</span></span>| <span data-ttu-id="00840-275">зависит от роли параметров</span><span class="sxs-lookup"><span data-stu-id="00840-275">depends on role Settings</span></span>||
|<span data-ttu-id="00840-276">расписание</span><span class="sxs-lookup"><span data-stu-id="00840-276">schedule</span></span>|[<span data-ttu-id="00840-277">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="00840-277">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="00840-278">Да</span><span class="sxs-lookup"><span data-stu-id="00840-278">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="00840-279">Запрос</span><span class="sxs-lookup"><span data-stu-id="00840-279">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="00840-280">Отклик</span><span class="sxs-lookup"><span data-stu-id="00840-280">Response</span></span>
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

### <a name="example-3"></a><span data-ttu-id="00840-281">Пример 3</span><span class="sxs-lookup"><span data-stu-id="00840-281">Example 3</span></span>
<span data-ttu-id="00840-282">В этом примере пользователь nawu@fimdev.net деактивирует активная роль чтения выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="00840-282">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="00840-283">Свойство</span><span class="sxs-lookup"><span data-stu-id="00840-283">Property</span></span>     | <span data-ttu-id="00840-284">Тип</span><span class="sxs-lookup"><span data-stu-id="00840-284">Type</span></span>    |<span data-ttu-id="00840-285">Обязательный</span><span class="sxs-lookup"><span data-stu-id="00840-285">Required</span></span>|  <span data-ttu-id="00840-286">Значение</span><span class="sxs-lookup"><span data-stu-id="00840-286">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="00840-287">resourceId</span><span class="sxs-lookup"><span data-stu-id="00840-287">resourceId</span></span>|<span data-ttu-id="00840-288">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-288">String</span></span>|<span data-ttu-id="00840-289">Да</span><span class="sxs-lookup"><span data-stu-id="00840-289">Yes</span></span>|<span data-ttu-id="00840-290">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="00840-290">\<resourceId\></span></span>|
|<span data-ttu-id="00840-291">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="00840-291">roleDefinitionId</span></span>|<span data-ttu-id="00840-292">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-292">String</span></span>|<span data-ttu-id="00840-293">Да</span><span class="sxs-lookup"><span data-stu-id="00840-293">Yes</span></span>|<span data-ttu-id="00840-294">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="00840-294">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="00840-295">subjectId</span><span class="sxs-lookup"><span data-stu-id="00840-295">subjectId</span></span>|<span data-ttu-id="00840-296">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-296">String</span></span>|<span data-ttu-id="00840-297">Да</span><span class="sxs-lookup"><span data-stu-id="00840-297">Yes</span></span>|<span data-ttu-id="00840-298">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="00840-298">\<subjectId\></span></span>|
|<span data-ttu-id="00840-299">assignmentState</span><span class="sxs-lookup"><span data-stu-id="00840-299">assignmentState</span></span>|<span data-ttu-id="00840-300">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-300">String</span></span>|<span data-ttu-id="00840-301">Да</span><span class="sxs-lookup"><span data-stu-id="00840-301">Yes</span></span>| <span data-ttu-id="00840-302">Активное</span><span class="sxs-lookup"><span data-stu-id="00840-302">Active</span></span>|
|<span data-ttu-id="00840-303">type</span><span class="sxs-lookup"><span data-stu-id="00840-303">type</span></span>|<span data-ttu-id="00840-304">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-304">String</span></span>|<span data-ttu-id="00840-305">Да</span><span class="sxs-lookup"><span data-stu-id="00840-305">Yes</span></span>| <span data-ttu-id="00840-306">UserRemove</span><span class="sxs-lookup"><span data-stu-id="00840-306">UserRemove</span></span>|
|<span data-ttu-id="00840-307">Причина</span><span class="sxs-lookup"><span data-stu-id="00840-307">reason</span></span>|<span data-ttu-id="00840-308">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-308">String</span></span>| <span data-ttu-id="00840-309">Нет</span><span class="sxs-lookup"><span data-stu-id="00840-309">No</span></span>||
|<span data-ttu-id="00840-310">расписание</span><span class="sxs-lookup"><span data-stu-id="00840-310">schedule</span></span>|[<span data-ttu-id="00840-311">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="00840-311">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="00840-312">Нет</span><span class="sxs-lookup"><span data-stu-id="00840-312">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="00840-313">Запрос</span><span class="sxs-lookup"><span data-stu-id="00840-313">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="00840-314">Отклик</span><span class="sxs-lookup"><span data-stu-id="00840-314">Response</span></span>
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

### <a name="example-4"></a><span data-ttu-id="00840-315">Пример 4</span><span class="sxs-lookup"><span data-stu-id="00840-315">Example 4</span></span>
<span data-ttu-id="00840-316">В этом примере администраторам удалить nawu@fimdev.net пользователя из роли выставления счетов чтения.</span><span class="sxs-lookup"><span data-stu-id="00840-316">In this example, administrators remove the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="00840-317">**Примечание:** В дополнение к разрешение, в этом примере требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="00840-317">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="00840-318">Свойство</span><span class="sxs-lookup"><span data-stu-id="00840-318">Property</span></span>     | <span data-ttu-id="00840-319">Тип</span><span class="sxs-lookup"><span data-stu-id="00840-319">Type</span></span>    |<span data-ttu-id="00840-320">Обязательный</span><span class="sxs-lookup"><span data-stu-id="00840-320">Required</span></span>|  <span data-ttu-id="00840-321">Значение</span><span class="sxs-lookup"><span data-stu-id="00840-321">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="00840-322">resourceId</span><span class="sxs-lookup"><span data-stu-id="00840-322">resourceId</span></span>|<span data-ttu-id="00840-323">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-323">String</span></span>|<span data-ttu-id="00840-324">Да</span><span class="sxs-lookup"><span data-stu-id="00840-324">Yes</span></span>|<span data-ttu-id="00840-325">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="00840-325">\<resourceId\></span></span>|
|<span data-ttu-id="00840-326">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="00840-326">roleDefinitionId</span></span>|<span data-ttu-id="00840-327">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-327">String</span></span>|<span data-ttu-id="00840-328">Да</span><span class="sxs-lookup"><span data-stu-id="00840-328">Yes</span></span>|<span data-ttu-id="00840-329">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="00840-329">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="00840-330">subjectId</span><span class="sxs-lookup"><span data-stu-id="00840-330">subjectId</span></span>|<span data-ttu-id="00840-331">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-331">String</span></span>|<span data-ttu-id="00840-332">Да</span><span class="sxs-lookup"><span data-stu-id="00840-332">Yes</span></span>|<span data-ttu-id="00840-333">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="00840-333">\<subjectId\></span></span>|
|<span data-ttu-id="00840-334">assignmentState</span><span class="sxs-lookup"><span data-stu-id="00840-334">assignmentState</span></span>|<span data-ttu-id="00840-335">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-335">String</span></span>|<span data-ttu-id="00840-336">Да</span><span class="sxs-lookup"><span data-stu-id="00840-336">Yes</span></span>| <span data-ttu-id="00840-337">Допустимость / Active</span><span class="sxs-lookup"><span data-stu-id="00840-337">Eligible / Active</span></span>|
|<span data-ttu-id="00840-338">type</span><span class="sxs-lookup"><span data-stu-id="00840-338">type</span></span>|<span data-ttu-id="00840-339">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-339">String</span></span>|<span data-ttu-id="00840-340">Да</span><span class="sxs-lookup"><span data-stu-id="00840-340">Yes</span></span>| <span data-ttu-id="00840-341">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="00840-341">AdminRemove</span></span>|
|<span data-ttu-id="00840-342">Причина</span><span class="sxs-lookup"><span data-stu-id="00840-342">reason</span></span>|<span data-ttu-id="00840-343">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-343">String</span></span>| <span data-ttu-id="00840-344">Нет</span><span class="sxs-lookup"><span data-stu-id="00840-344">No</span></span>||
|<span data-ttu-id="00840-345">расписание</span><span class="sxs-lookup"><span data-stu-id="00840-345">schedule</span></span>|[<span data-ttu-id="00840-346">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="00840-346">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="00840-347">Нет</span><span class="sxs-lookup"><span data-stu-id="00840-347">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="00840-348">Запрос</span><span class="sxs-lookup"><span data-stu-id="00840-348">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="00840-349">Отклик</span><span class="sxs-lookup"><span data-stu-id="00840-349">Response</span></span>
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

### <a name="example-5"></a><span data-ttu-id="00840-350">Пример 5</span><span class="sxs-lookup"><span data-stu-id="00840-350">Example 5</span></span>
<span data-ttu-id="00840-351">В этом примере Администраторы обновление назначения ролей для пользователя nawu@fimdev.net владельцу.</span><span class="sxs-lookup"><span data-stu-id="00840-351">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="00840-352">**Примечание:** В дополнение к разрешение, в этом примере требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="00840-352">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="00840-353">Свойство</span><span class="sxs-lookup"><span data-stu-id="00840-353">Property</span></span>     | <span data-ttu-id="00840-354">Тип</span><span class="sxs-lookup"><span data-stu-id="00840-354">Type</span></span>    |<span data-ttu-id="00840-355">Обязательный</span><span class="sxs-lookup"><span data-stu-id="00840-355">Required</span></span>|  <span data-ttu-id="00840-356">Значение</span><span class="sxs-lookup"><span data-stu-id="00840-356">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="00840-357">resourceId</span><span class="sxs-lookup"><span data-stu-id="00840-357">resourceId</span></span>|<span data-ttu-id="00840-358">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-358">String</span></span>|<span data-ttu-id="00840-359">Да</span><span class="sxs-lookup"><span data-stu-id="00840-359">Yes</span></span>|<span data-ttu-id="00840-360">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="00840-360">\<resourceId\></span></span>|
|<span data-ttu-id="00840-361">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="00840-361">roleDefinitionId</span></span>|<span data-ttu-id="00840-362">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-362">String</span></span>|<span data-ttu-id="00840-363">Да</span><span class="sxs-lookup"><span data-stu-id="00840-363">Yes</span></span>|<span data-ttu-id="00840-364">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="00840-364">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="00840-365">subjectId</span><span class="sxs-lookup"><span data-stu-id="00840-365">subjectId</span></span>|<span data-ttu-id="00840-366">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-366">String</span></span>|<span data-ttu-id="00840-367">Да</span><span class="sxs-lookup"><span data-stu-id="00840-367">Yes</span></span>|<span data-ttu-id="00840-368">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="00840-368">\<subjectId\></span></span>|
|<span data-ttu-id="00840-369">assignmentState</span><span class="sxs-lookup"><span data-stu-id="00840-369">assignmentState</span></span>|<span data-ttu-id="00840-370">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-370">String</span></span>|<span data-ttu-id="00840-371">Да</span><span class="sxs-lookup"><span data-stu-id="00840-371">Yes</span></span>| <span data-ttu-id="00840-372">Допустимость / Active</span><span class="sxs-lookup"><span data-stu-id="00840-372">Eligible / Active</span></span>|
|<span data-ttu-id="00840-373">type</span><span class="sxs-lookup"><span data-stu-id="00840-373">type</span></span>|<span data-ttu-id="00840-374">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-374">String</span></span>|<span data-ttu-id="00840-375">Да</span><span class="sxs-lookup"><span data-stu-id="00840-375">Yes</span></span>| <span data-ttu-id="00840-376">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="00840-376">AdminUpdate</span></span>|
|<span data-ttu-id="00840-377">Причина</span><span class="sxs-lookup"><span data-stu-id="00840-377">reason</span></span>|<span data-ttu-id="00840-378">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-378">String</span></span>| <span data-ttu-id="00840-379">зависит от roleSettings</span><span class="sxs-lookup"><span data-stu-id="00840-379">depends on roleSettings</span></span>||
|<span data-ttu-id="00840-380">расписание</span><span class="sxs-lookup"><span data-stu-id="00840-380">schedule</span></span>|[<span data-ttu-id="00840-381">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="00840-381">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="00840-382">Да</span><span class="sxs-lookup"><span data-stu-id="00840-382">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="00840-383">Запрос</span><span class="sxs-lookup"><span data-stu-id="00840-383">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="00840-384">Отклик</span><span class="sxs-lookup"><span data-stu-id="00840-384">Response</span></span>
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

### <a name="example-6"></a><span data-ttu-id="00840-385">В примере 6</span><span class="sxs-lookup"><span data-stu-id="00840-385">Example 6</span></span>
<span data-ttu-id="00840-386">В этом примере расширяет истекающим сроком действия назначения ролей для пользователя ANUJCUSER для участника службы управления API.</span><span class="sxs-lookup"><span data-stu-id="00840-386">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="00840-387">**Примечание:** В additon разрешение, в этом примере требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="00840-387">**Note:** In additon to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="00840-388">Свойство</span><span class="sxs-lookup"><span data-stu-id="00840-388">Property</span></span>     | <span data-ttu-id="00840-389">Тип</span><span class="sxs-lookup"><span data-stu-id="00840-389">Type</span></span>    |<span data-ttu-id="00840-390">Обязательный</span><span class="sxs-lookup"><span data-stu-id="00840-390">Required</span></span>|  <span data-ttu-id="00840-391">Значение</span><span class="sxs-lookup"><span data-stu-id="00840-391">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="00840-392">resourceId</span><span class="sxs-lookup"><span data-stu-id="00840-392">resourceId</span></span>|<span data-ttu-id="00840-393">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-393">String</span></span>|<span data-ttu-id="00840-394">Да</span><span class="sxs-lookup"><span data-stu-id="00840-394">Yes</span></span>|<span data-ttu-id="00840-395">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="00840-395">\<resourceId\></span></span>|
|<span data-ttu-id="00840-396">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="00840-396">roleDefinitionId</span></span>|<span data-ttu-id="00840-397">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-397">String</span></span>|<span data-ttu-id="00840-398">Да</span><span class="sxs-lookup"><span data-stu-id="00840-398">Yes</span></span>|<span data-ttu-id="00840-399">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="00840-399">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="00840-400">subjectId</span><span class="sxs-lookup"><span data-stu-id="00840-400">subjectId</span></span>|<span data-ttu-id="00840-401">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-401">String</span></span>|<span data-ttu-id="00840-402">Да</span><span class="sxs-lookup"><span data-stu-id="00840-402">Yes</span></span>|<span data-ttu-id="00840-403">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="00840-403">\<subjectId\></span></span>|
|<span data-ttu-id="00840-404">assignmentState</span><span class="sxs-lookup"><span data-stu-id="00840-404">assignmentState</span></span>|<span data-ttu-id="00840-405">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-405">String</span></span>|<span data-ttu-id="00840-406">Да</span><span class="sxs-lookup"><span data-stu-id="00840-406">Yes</span></span>| <span data-ttu-id="00840-407">Допустимость / Active</span><span class="sxs-lookup"><span data-stu-id="00840-407">Eligible / Active</span></span> |
|<span data-ttu-id="00840-408">type</span><span class="sxs-lookup"><span data-stu-id="00840-408">type</span></span>|<span data-ttu-id="00840-409">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-409">String</span></span>|<span data-ttu-id="00840-410">Да</span><span class="sxs-lookup"><span data-stu-id="00840-410">Yes</span></span>| <span data-ttu-id="00840-411">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="00840-411">AdminExtend</span></span>|
|<span data-ttu-id="00840-412">Причина</span><span class="sxs-lookup"><span data-stu-id="00840-412">reason</span></span>|<span data-ttu-id="00840-413">Строка</span><span class="sxs-lookup"><span data-stu-id="00840-413">String</span></span>| <span data-ttu-id="00840-414">зависит от roleSettings</span><span class="sxs-lookup"><span data-stu-id="00840-414">depends on roleSettings</span></span>||
|<span data-ttu-id="00840-415">расписание</span><span class="sxs-lookup"><span data-stu-id="00840-415">schedule</span></span>|[<span data-ttu-id="00840-416">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="00840-416">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="00840-417">Да</span><span class="sxs-lookup"><span data-stu-id="00840-417">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="00840-418">Запрос</span><span class="sxs-lookup"><span data-stu-id="00840-418">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="00840-419">Отклик</span><span class="sxs-lookup"><span data-stu-id="00840-419">Response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Post roleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
