---
title: Создание governanceRoleAssignmentRequest
description: Создание роли назначения запроса для представления операции, требуется на назначения ролей. В следующей таблице перечислены операции.
localization_priority: Normal
ms.openlocfilehash: c936a6cd0ba061fc1dd3758533781d7270673939
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523241"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="c5f9d-104">Создание governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="c5f9d-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5f9d-105">Создание роли назначения запроса для представления операции, требуется на назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="c5f9d-106">В следующей таблице перечислены операции.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-106">The following table lists the operations.</span></span>

| <span data-ttu-id="c5f9d-107">Operation</span><span class="sxs-lookup"><span data-stu-id="c5f9d-107">Operation</span></span>       | <span data-ttu-id="c5f9d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c5f9d-108">Type</span></span> | 
|:---------------|:----------|
| <span data-ttu-id="c5f9d-109">Назначение назначения ролей</span><span class="sxs-lookup"><span data-stu-id="c5f9d-109">Assign a role assignment</span></span>| <span data-ttu-id="c5f9d-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="c5f9d-110">AdminAdd</span></span> |
| <span data-ttu-id="c5f9d-111">Активация назначение подходящими роли</span><span class="sxs-lookup"><span data-stu-id="c5f9d-111">Activate an eligible role assignment</span></span>| <span data-ttu-id="c5f9d-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="c5f9d-112">UserAdd</span></span> | 
| <span data-ttu-id="c5f9d-113">Деактивация назначение активированные роли</span><span class="sxs-lookup"><span data-stu-id="c5f9d-113">Deactivate an activated role assignment</span></span>| <span data-ttu-id="c5f9d-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="c5f9d-114">UserRemove</span></span> | 
| <span data-ttu-id="c5f9d-115">Удаление назначения ролей</span><span class="sxs-lookup"><span data-stu-id="c5f9d-115">Remove a role assignment</span></span>| <span data-ttu-id="c5f9d-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="c5f9d-116">AdminRemove</span></span> |
| <span data-ttu-id="c5f9d-117">Обновление назначения ролей</span><span class="sxs-lookup"><span data-stu-id="c5f9d-117">Update a role assignment</span></span>| <span data-ttu-id="c5f9d-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="c5f9d-118">AdminUpdate</span></span> |
| <span data-ttu-id="c5f9d-119">Запрос на расширение my назначения роли</span><span class="sxs-lookup"><span data-stu-id="c5f9d-119">Request to extend my role assignment</span></span>| <span data-ttu-id="c5f9d-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="c5f9d-120">UserExtend</span></span> | 
| <span data-ttu-id="c5f9d-121">Расширение назначения ролей</span><span class="sxs-lookup"><span data-stu-id="c5f9d-121">Extend a role assignment</span></span>| <span data-ttu-id="c5f9d-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="c5f9d-122">AdminExtend</span></span> | 
| <span data-ttu-id="c5f9d-123">Запрос на обновление назначения ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="c5f9d-123">Request to renew my expired role assignment</span></span>| <span data-ttu-id="c5f9d-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="c5f9d-124">UserRenew</span></span> | 
| <span data-ttu-id="c5f9d-125">Обновление назначения ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="c5f9d-125">Renew an expired role assignment</span></span>| <span data-ttu-id="c5f9d-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="c5f9d-126">AdminRenew</span></span> | 

 
## <a name="permissions"></a><span data-ttu-id="c5f9d-127">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5f9d-127">Permissions</span></span>
<span data-ttu-id="c5f9d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5f9d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5f9d-130">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5f9d-130">Permission type</span></span>      | <span data-ttu-id="c5f9d-131">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5f9d-131">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5f9d-132">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5f9d-132">Delegated (work or school account)</span></span> | <span data-ttu-id="c5f9d-133">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="c5f9d-133">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="c5f9d-134">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5f9d-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5f9d-135">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-135">Not supported.</span></span>    |
|<span data-ttu-id="c5f9d-136">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5f9d-136">Application</span></span> | <span data-ttu-id="c5f9d-137">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="c5f9d-137">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5f9d-138">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5f9d-138">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="c5f9d-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5f9d-139">Request headers</span></span>
| <span data-ttu-id="c5f9d-140">Имя</span><span class="sxs-lookup"><span data-stu-id="c5f9d-140">Name</span></span>       | <span data-ttu-id="c5f9d-141">Описание</span><span class="sxs-lookup"><span data-stu-id="c5f9d-141">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c5f9d-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5f9d-142">Authorization</span></span>  | <span data-ttu-id="c5f9d-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c5f9d-143">Bearer {code}</span></span>|
| <span data-ttu-id="c5f9d-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c5f9d-144">Content-type</span></span>  | <span data-ttu-id="c5f9d-145">application/json</span><span class="sxs-lookup"><span data-stu-id="c5f9d-145">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5f9d-146">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5f9d-146">Request body</span></span>
<span data-ttu-id="c5f9d-147">В тексте запроса укажите представление JSON объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="c5f9d-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="c5f9d-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5f9d-148">Property</span></span>     | <span data-ttu-id="c5f9d-149">Тип</span><span class="sxs-lookup"><span data-stu-id="c5f9d-149">Type</span></span>    |<span data-ttu-id="c5f9d-150">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c5f9d-150">Required</span></span>|  <span data-ttu-id="c5f9d-151">Описание</span><span class="sxs-lookup"><span data-stu-id="c5f9d-151">Description</span></span>|
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="c5f9d-152">resourceId</span><span class="sxs-lookup"><span data-stu-id="c5f9d-152">resourceId</span></span>|<span data-ttu-id="c5f9d-153">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-153">String</span></span>|<span data-ttu-id="c5f9d-154">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-154">Yes</span></span>|<span data-ttu-id="c5f9d-155">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-155">The ID of the resource.</span></span>|
|<span data-ttu-id="c5f9d-156">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c5f9d-156">roleDefinitionId</span></span>|<span data-ttu-id="c5f9d-157">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-157">String</span></span>|<span data-ttu-id="c5f9d-158">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-158">Yes</span></span>|<span data-ttu-id="c5f9d-159">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-159">The ID of the role definition.</span></span>|
|<span data-ttu-id="c5f9d-160">subjectId</span><span class="sxs-lookup"><span data-stu-id="c5f9d-160">subjectId</span></span>|<span data-ttu-id="c5f9d-161">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-161">String</span></span>|<span data-ttu-id="c5f9d-162">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-162">Yes</span></span>|<span data-ttu-id="c5f9d-163">Идентификатор субъекта.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-163">The ID of the subject.</span></span>|
|<span data-ttu-id="c5f9d-164">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c5f9d-164">assignmentState</span></span>|<span data-ttu-id="c5f9d-165">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-165">String</span></span>|<span data-ttu-id="c5f9d-166">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-166">Yes</span></span>|<span data-ttu-id="c5f9d-167">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-167">The state of assignment.</span></span> <span data-ttu-id="c5f9d-168">Значение может быть ``Eligible`` и ``Active``.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-168">The value can be ``Eligible`` and ``Active``.</span></span>|
|<span data-ttu-id="c5f9d-169">type</span><span class="sxs-lookup"><span data-stu-id="c5f9d-169">type</span></span>|<span data-ttu-id="c5f9d-170">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-170">String</span></span>|<span data-ttu-id="c5f9d-171">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-171">Yes</span></span>|<span data-ttu-id="c5f9d-172">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-172">The request type.</span></span> <span data-ttu-id="c5f9d-173">Значение может быть `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`и `AdminExtend`.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-173">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span>|
|<span data-ttu-id="c5f9d-174">Reason</span><span class="sxs-lookup"><span data-stu-id="c5f9d-174">reason</span></span>|<span data-ttu-id="c5f9d-175">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-175">String</span></span>| |<span data-ttu-id="c5f9d-176">Причину должно предоставляться для запроса назначений ролей для аудита и предварительный просмотр цели.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-176">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="c5f9d-177">Расписание</span><span class="sxs-lookup"><span data-stu-id="c5f9d-177">schedule</span></span>|[<span data-ttu-id="c5f9d-178">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c5f9d-178">governanceSchedule</span></span>](../resources/governanceschedule.md)| | <span data-ttu-id="c5f9d-179">Расписание для запроса назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-179">The schedule of the role assignment request.</span></span> <span data-ttu-id="c5f9d-180">Для запроса типа `UserAdd`, `AdminAdd`, `AdminUpdate`, и `AdminExtend`, это необходимо.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-180">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span>|

## <a name="response"></a><span data-ttu-id="c5f9d-181">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5f9d-181">Response</span></span>
<span data-ttu-id="c5f9d-182">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-182">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="c5f9d-183">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="c5f9d-183">Error codes</span></span>
<span data-ttu-id="c5f9d-184">Этот интерфейс API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-184">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="c5f9d-185">Кроме того он возвращает коды ошибок, перечисленных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-185">In addition, it also returns the error codes listed in the following table.</span></span>

|<span data-ttu-id="c5f9d-186">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="c5f9d-186">Error code</span></span>     | <span data-ttu-id="c5f9d-187">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="c5f9d-187">Error message</span></span>              | <span data-ttu-id="c5f9d-188">Сведения</span><span class="sxs-lookup"><span data-stu-id="c5f9d-188">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="c5f9d-189">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c5f9d-189">400 BadRequest</span></span> | <span data-ttu-id="c5f9d-190">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="c5f9d-190">RoleNotFound</span></span>    | <span data-ttu-id="c5f9d-191">`roleDefinitionId` Условии, что в запросе не удается найти текст.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-191">The `roleDefinitionId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="c5f9d-192">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c5f9d-192">400 BadRequest</span></span> | <span data-ttu-id="c5f9d-193">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="c5f9d-193">ResourceIsLocked</span></span>    | <span data-ttu-id="c5f9d-194">Ресурс, представленные в тексте запроса находится в состоянии из `Locked` и не могут создавать запросы назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-194">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span>
| <span data-ttu-id="c5f9d-195">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c5f9d-195">400 BadRequest</span></span> | <span data-ttu-id="c5f9d-196">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="c5f9d-196">SubjectNotFound</span></span>    | <span data-ttu-id="c5f9d-197">`subjectId` Условии, что в запросе не удается найти текст.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-197">The `subjectId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="c5f9d-198">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c5f9d-198">400 BadRequest</span></span> | <span data-ttu-id="c5f9d-199">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="c5f9d-199">PendingRoleAssignmentRequest</span></span>    | <span data-ttu-id="c5f9d-200">Уже существует ожидающие [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в системе.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-200">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span>
| <span data-ttu-id="c5f9d-201">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c5f9d-201">400 BadRequest</span></span> | <span data-ttu-id="c5f9d-202">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="c5f9d-202">RoleAssignmentExists</span></span>    | <span data-ttu-id="c5f9d-203">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) запрошено будет создан уже существует в системе.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-203">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span>
| <span data-ttu-id="c5f9d-204">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c5f9d-204">400 BadRequest</span></span> | <span data-ttu-id="c5f9d-205">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="c5f9d-205">RoleAssignmentDoesNotExist</span></span>    | <span data-ttu-id="c5f9d-206">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) запрос на обновление/расширить не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-206">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span>
| <span data-ttu-id="c5f9d-207">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c5f9d-207">400 BadRequest</span></span> | <span data-ttu-id="c5f9d-208">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="c5f9d-208">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="c5f9d-209">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) не соответствует внутренней политик и не может быть создан.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-209">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span>

## <a name="examples"></a><span data-ttu-id="c5f9d-210">Примеры</span><span class="sxs-lookup"><span data-stu-id="c5f9d-210">Examples</span></span>
<span data-ttu-id="c5f9d-211">В приведенных ниже примерах показано, как использовать этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-211">The following examples show how to use this API.</span></span>

### <a name="example-1"></a><span data-ttu-id="c5f9d-212">Пример 1</span><span class="sxs-lookup"><span data-stu-id="c5f9d-212">Example 1</span></span>
<span data-ttu-id="c5f9d-213">В этом примере администраторам назначение роли выставления счетов читатель nawu@fimdev.net пользователя.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-213">In this example, administrators assign user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="c5f9d-214">**Примечание:** В дополнение к разрешение, в этом примере требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-214">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="c5f9d-215">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5f9d-215">Property</span></span>     | <span data-ttu-id="c5f9d-216">Тип</span><span class="sxs-lookup"><span data-stu-id="c5f9d-216">Type</span></span>    |<span data-ttu-id="c5f9d-217">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c5f9d-217">Required</span></span>|  <span data-ttu-id="c5f9d-218">Значение</span><span class="sxs-lookup"><span data-stu-id="c5f9d-218">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="c5f9d-219">resourceId</span><span class="sxs-lookup"><span data-stu-id="c5f9d-219">resourceId</span></span>|<span data-ttu-id="c5f9d-220">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-220">String</span></span>|<span data-ttu-id="c5f9d-221">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-221">Yes</span></span>|<span data-ttu-id="c5f9d-222">\<</span><span class="sxs-lookup"><span data-stu-id="c5f9d-222">\<resourceId\></span></span>|
|<span data-ttu-id="c5f9d-223">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c5f9d-223">roleDefinitionId</span></span>|<span data-ttu-id="c5f9d-224">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-224">String</span></span>|<span data-ttu-id="c5f9d-225">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-225">Yes</span></span>|<span data-ttu-id="c5f9d-226">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="c5f9d-226">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="c5f9d-227">subjectId</span><span class="sxs-lookup"><span data-stu-id="c5f9d-227">subjectId</span></span>|<span data-ttu-id="c5f9d-228">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-228">String</span></span>|<span data-ttu-id="c5f9d-229">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-229">Yes</span></span>|<span data-ttu-id="c5f9d-230">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="c5f9d-230">\<subjectId\></span></span>|
|<span data-ttu-id="c5f9d-231">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c5f9d-231">assignmentState</span></span>|<span data-ttu-id="c5f9d-232">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-232">String</span></span>|<span data-ttu-id="c5f9d-233">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-233">Yes</span></span>| <span data-ttu-id="c5f9d-234">Допустимость / Active</span><span class="sxs-lookup"><span data-stu-id="c5f9d-234">Eligible / Active</span></span>|
|<span data-ttu-id="c5f9d-235">type</span><span class="sxs-lookup"><span data-stu-id="c5f9d-235">type</span></span>|<span data-ttu-id="c5f9d-236">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-236">String</span></span>|<span data-ttu-id="c5f9d-237">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-237">Yes</span></span>| <span data-ttu-id="c5f9d-238">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="c5f9d-238">AdminAdd</span></span>|
|<span data-ttu-id="c5f9d-239">Reason</span><span class="sxs-lookup"><span data-stu-id="c5f9d-239">reason</span></span>|<span data-ttu-id="c5f9d-240">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-240">String</span></span>| <span data-ttu-id="c5f9d-241">зависит от роли параметров</span><span class="sxs-lookup"><span data-stu-id="c5f9d-241">depends on role Settings</span></span>||
|<span data-ttu-id="c5f9d-242">Расписание</span><span class="sxs-lookup"><span data-stu-id="c5f9d-242">schedule</span></span>|[<span data-ttu-id="c5f9d-243">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c5f9d-243">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="c5f9d-244">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-244">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="c5f9d-245">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5f9d-245">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="c5f9d-246">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5f9d-246">Response</span></span>
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

### <a name="example-2"></a><span data-ttu-id="c5f9d-247">Пример 2</span><span class="sxs-lookup"><span data-stu-id="c5f9d-247">Example 2</span></span>
<span data-ttu-id="c5f9d-248">В этом примере nawu@fimdev.net пользователь активирует право чтения выставления счетов роли.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-248">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="c5f9d-249">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5f9d-249">Property</span></span>     | <span data-ttu-id="c5f9d-250">Тип</span><span class="sxs-lookup"><span data-stu-id="c5f9d-250">Type</span></span>    |<span data-ttu-id="c5f9d-251">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c5f9d-251">Required</span></span>|  <span data-ttu-id="c5f9d-252">Значение</span><span class="sxs-lookup"><span data-stu-id="c5f9d-252">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="c5f9d-253">resourceId</span><span class="sxs-lookup"><span data-stu-id="c5f9d-253">resourceId</span></span>|<span data-ttu-id="c5f9d-254">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-254">String</span></span>|<span data-ttu-id="c5f9d-255">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-255">Yes</span></span>|<span data-ttu-id="c5f9d-256">\<</span><span class="sxs-lookup"><span data-stu-id="c5f9d-256">\<resourceId\></span></span>|
|<span data-ttu-id="c5f9d-257">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c5f9d-257">roleDefinitionId</span></span>|<span data-ttu-id="c5f9d-258">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-258">String</span></span>|<span data-ttu-id="c5f9d-259">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-259">Yes</span></span>|<span data-ttu-id="c5f9d-260">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="c5f9d-260">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="c5f9d-261">subjectId</span><span class="sxs-lookup"><span data-stu-id="c5f9d-261">subjectId</span></span>|<span data-ttu-id="c5f9d-262">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-262">String</span></span>|<span data-ttu-id="c5f9d-263">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-263">Yes</span></span>|<span data-ttu-id="c5f9d-264">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="c5f9d-264">\<subjectId\></span></span>|
|<span data-ttu-id="c5f9d-265">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c5f9d-265">assignmentState</span></span>|<span data-ttu-id="c5f9d-266">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-266">String</span></span>|<span data-ttu-id="c5f9d-267">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-267">Yes</span></span>| <span data-ttu-id="c5f9d-268">Активное</span><span class="sxs-lookup"><span data-stu-id="c5f9d-268">Active</span></span>|
|<span data-ttu-id="c5f9d-269">type</span><span class="sxs-lookup"><span data-stu-id="c5f9d-269">type</span></span>|<span data-ttu-id="c5f9d-270">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-270">String</span></span>|<span data-ttu-id="c5f9d-271">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-271">Yes</span></span>| <span data-ttu-id="c5f9d-272">UserAdd</span><span class="sxs-lookup"><span data-stu-id="c5f9d-272">UserAdd</span></span>|
|<span data-ttu-id="c5f9d-273">Reason</span><span class="sxs-lookup"><span data-stu-id="c5f9d-273">reason</span></span>|<span data-ttu-id="c5f9d-274">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-274">String</span></span>| <span data-ttu-id="c5f9d-275">зависит от роли параметров</span><span class="sxs-lookup"><span data-stu-id="c5f9d-275">depends on role Settings</span></span>||
|<span data-ttu-id="c5f9d-276">Расписание</span><span class="sxs-lookup"><span data-stu-id="c5f9d-276">schedule</span></span>|[<span data-ttu-id="c5f9d-277">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c5f9d-277">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="c5f9d-278">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-278">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="c5f9d-279">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5f9d-279">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="c5f9d-280">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5f9d-280">Response</span></span>
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

### <a name="example-3"></a><span data-ttu-id="c5f9d-281">Пример 3</span><span class="sxs-lookup"><span data-stu-id="c5f9d-281">Example 3</span></span>
<span data-ttu-id="c5f9d-282">В этом примере пользователь nawu@fimdev.net деактивирует активная роль чтения выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-282">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="c5f9d-283">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5f9d-283">Property</span></span>     | <span data-ttu-id="c5f9d-284">Тип</span><span class="sxs-lookup"><span data-stu-id="c5f9d-284">Type</span></span>    |<span data-ttu-id="c5f9d-285">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c5f9d-285">Required</span></span>|  <span data-ttu-id="c5f9d-286">Значение</span><span class="sxs-lookup"><span data-stu-id="c5f9d-286">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="c5f9d-287">resourceId</span><span class="sxs-lookup"><span data-stu-id="c5f9d-287">resourceId</span></span>|<span data-ttu-id="c5f9d-288">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-288">String</span></span>|<span data-ttu-id="c5f9d-289">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-289">Yes</span></span>|<span data-ttu-id="c5f9d-290">\<</span><span class="sxs-lookup"><span data-stu-id="c5f9d-290">\<resourceId\></span></span>|
|<span data-ttu-id="c5f9d-291">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c5f9d-291">roleDefinitionId</span></span>|<span data-ttu-id="c5f9d-292">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-292">String</span></span>|<span data-ttu-id="c5f9d-293">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-293">Yes</span></span>|<span data-ttu-id="c5f9d-294">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="c5f9d-294">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="c5f9d-295">subjectId</span><span class="sxs-lookup"><span data-stu-id="c5f9d-295">subjectId</span></span>|<span data-ttu-id="c5f9d-296">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-296">String</span></span>|<span data-ttu-id="c5f9d-297">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-297">Yes</span></span>|<span data-ttu-id="c5f9d-298">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="c5f9d-298">\<subjectId\></span></span>|
|<span data-ttu-id="c5f9d-299">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c5f9d-299">assignmentState</span></span>|<span data-ttu-id="c5f9d-300">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-300">String</span></span>|<span data-ttu-id="c5f9d-301">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-301">Yes</span></span>| <span data-ttu-id="c5f9d-302">Активное</span><span class="sxs-lookup"><span data-stu-id="c5f9d-302">Active</span></span>|
|<span data-ttu-id="c5f9d-303">type</span><span class="sxs-lookup"><span data-stu-id="c5f9d-303">type</span></span>|<span data-ttu-id="c5f9d-304">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-304">String</span></span>|<span data-ttu-id="c5f9d-305">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-305">Yes</span></span>| <span data-ttu-id="c5f9d-306">UserRemove</span><span class="sxs-lookup"><span data-stu-id="c5f9d-306">UserRemove</span></span>|
|<span data-ttu-id="c5f9d-307">Reason</span><span class="sxs-lookup"><span data-stu-id="c5f9d-307">reason</span></span>|<span data-ttu-id="c5f9d-308">Строка</span><span class="sxs-lookup"><span data-stu-id="c5f9d-308">String</span></span>| <span data-ttu-id="c5f9d-309">Нет</span><span class="sxs-lookup"><span data-stu-id="c5f9d-309">No</span></span>||
|<span data-ttu-id="c5f9d-310">Расписание</span><span class="sxs-lookup"><span data-stu-id="c5f9d-310">schedule</span></span>|[<span data-ttu-id="c5f9d-311">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c5f9d-311">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="c5f9d-312">Нет</span><span class="sxs-lookup"><span data-stu-id="c5f9d-312">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="c5f9d-313">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5f9d-313">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="c5f9d-314">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5f9d-314">Response</span></span>
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

### <a name="example-4"></a><span data-ttu-id="c5f9d-315">---------------------ПРИМЕР 4-----------------------</span><span class="sxs-lookup"><span data-stu-id="c5f9d-315">Example 4</span></span>
<span data-ttu-id="c5f9d-316">В этом примере администраторам удалить nawu@fimdev.net пользователя из роли выставления счетов чтения.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-316">In this example, administrators remove the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="c5f9d-317">**Примечание:** В дополнение к разрешение, в этом примере требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-317">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="c5f9d-318">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5f9d-318">Property</span></span>     | <span data-ttu-id="c5f9d-319">Тип</span><span class="sxs-lookup"><span data-stu-id="c5f9d-319">Type</span></span>    |<span data-ttu-id="c5f9d-320">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c5f9d-320">Required</span></span>|  <span data-ttu-id="c5f9d-321">Значение</span><span class="sxs-lookup"><span data-stu-id="c5f9d-321">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="c5f9d-322">resourceId</span><span class="sxs-lookup"><span data-stu-id="c5f9d-322">resourceId</span></span>|<span data-ttu-id="c5f9d-323">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-323">String</span></span>|<span data-ttu-id="c5f9d-324">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-324">Yes</span></span>|<span data-ttu-id="c5f9d-325">\<</span><span class="sxs-lookup"><span data-stu-id="c5f9d-325">\<resourceId\></span></span>|
|<span data-ttu-id="c5f9d-326">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c5f9d-326">roleDefinitionId</span></span>|<span data-ttu-id="c5f9d-327">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-327">String</span></span>|<span data-ttu-id="c5f9d-328">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-328">Yes</span></span>|<span data-ttu-id="c5f9d-329">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="c5f9d-329">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="c5f9d-330">subjectId</span><span class="sxs-lookup"><span data-stu-id="c5f9d-330">subjectId</span></span>|<span data-ttu-id="c5f9d-331">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-331">String</span></span>|<span data-ttu-id="c5f9d-332">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-332">Yes</span></span>|<span data-ttu-id="c5f9d-333">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="c5f9d-333">\<subjectId\></span></span>|
|<span data-ttu-id="c5f9d-334">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c5f9d-334">assignmentState</span></span>|<span data-ttu-id="c5f9d-335">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-335">String</span></span>|<span data-ttu-id="c5f9d-336">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-336">Yes</span></span>| <span data-ttu-id="c5f9d-337">Допустимость / Active</span><span class="sxs-lookup"><span data-stu-id="c5f9d-337">Eligible / Active</span></span>|
|<span data-ttu-id="c5f9d-338">type</span><span class="sxs-lookup"><span data-stu-id="c5f9d-338">type</span></span>|<span data-ttu-id="c5f9d-339">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-339">String</span></span>|<span data-ttu-id="c5f9d-340">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-340">Yes</span></span>| <span data-ttu-id="c5f9d-341">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="c5f9d-341">AdminRemove</span></span>|
|<span data-ttu-id="c5f9d-342">Reason</span><span class="sxs-lookup"><span data-stu-id="c5f9d-342">reason</span></span>|<span data-ttu-id="c5f9d-343">Строка</span><span class="sxs-lookup"><span data-stu-id="c5f9d-343">String</span></span>| <span data-ttu-id="c5f9d-344">Нет</span><span class="sxs-lookup"><span data-stu-id="c5f9d-344">No</span></span>||
|<span data-ttu-id="c5f9d-345">Расписание</span><span class="sxs-lookup"><span data-stu-id="c5f9d-345">schedule</span></span>|[<span data-ttu-id="c5f9d-346">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c5f9d-346">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="c5f9d-347">Нет</span><span class="sxs-lookup"><span data-stu-id="c5f9d-347">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="c5f9d-348">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5f9d-348">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="c5f9d-349">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5f9d-349">Response</span></span>
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

### <a name="example-5"></a><span data-ttu-id="c5f9d-350">Пример 5</span><span class="sxs-lookup"><span data-stu-id="c5f9d-350">Example 5</span></span>
<span data-ttu-id="c5f9d-351">В этом примере Администраторы обновление назначения ролей для пользователя nawu@fimdev.net владельцу.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-351">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="c5f9d-352">**Примечание:** В дополнение к разрешение, в этом примере требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-352">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="c5f9d-353">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5f9d-353">Property</span></span>     | <span data-ttu-id="c5f9d-354">Тип</span><span class="sxs-lookup"><span data-stu-id="c5f9d-354">Type</span></span>    |<span data-ttu-id="c5f9d-355">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c5f9d-355">Required</span></span>|  <span data-ttu-id="c5f9d-356">Значение</span><span class="sxs-lookup"><span data-stu-id="c5f9d-356">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="c5f9d-357">resourceId</span><span class="sxs-lookup"><span data-stu-id="c5f9d-357">resourceId</span></span>|<span data-ttu-id="c5f9d-358">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-358">String</span></span>|<span data-ttu-id="c5f9d-359">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-359">Yes</span></span>|<span data-ttu-id="c5f9d-360">\<</span><span class="sxs-lookup"><span data-stu-id="c5f9d-360">\<resourceId\></span></span>|
|<span data-ttu-id="c5f9d-361">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c5f9d-361">roleDefinitionId</span></span>|<span data-ttu-id="c5f9d-362">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-362">String</span></span>|<span data-ttu-id="c5f9d-363">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-363">Yes</span></span>|<span data-ttu-id="c5f9d-364">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="c5f9d-364">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="c5f9d-365">subjectId</span><span class="sxs-lookup"><span data-stu-id="c5f9d-365">subjectId</span></span>|<span data-ttu-id="c5f9d-366">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-366">String</span></span>|<span data-ttu-id="c5f9d-367">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-367">Yes</span></span>|<span data-ttu-id="c5f9d-368">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="c5f9d-368">\<subjectId\></span></span>|
|<span data-ttu-id="c5f9d-369">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c5f9d-369">assignmentState</span></span>|<span data-ttu-id="c5f9d-370">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-370">String</span></span>|<span data-ttu-id="c5f9d-371">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-371">Yes</span></span>| <span data-ttu-id="c5f9d-372">Допустимость / Active</span><span class="sxs-lookup"><span data-stu-id="c5f9d-372">Eligible / Active</span></span>|
|<span data-ttu-id="c5f9d-373">type</span><span class="sxs-lookup"><span data-stu-id="c5f9d-373">type</span></span>|<span data-ttu-id="c5f9d-374">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-374">String</span></span>|<span data-ttu-id="c5f9d-375">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-375">Yes</span></span>| <span data-ttu-id="c5f9d-376">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="c5f9d-376">AdminUpdate</span></span>|
|<span data-ttu-id="c5f9d-377">Reason</span><span class="sxs-lookup"><span data-stu-id="c5f9d-377">reason</span></span>|<span data-ttu-id="c5f9d-378">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-378">String</span></span>| <span data-ttu-id="c5f9d-379">зависит от roleSettings</span><span class="sxs-lookup"><span data-stu-id="c5f9d-379">depends on roleSettings</span></span>||
|<span data-ttu-id="c5f9d-380">Расписание</span><span class="sxs-lookup"><span data-stu-id="c5f9d-380">schedule</span></span>|[<span data-ttu-id="c5f9d-381">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c5f9d-381">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="c5f9d-382">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-382">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="c5f9d-383">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5f9d-383">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="c5f9d-384">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5f9d-384">Response</span></span>
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

### <a name="example-6"></a><span data-ttu-id="c5f9d-385">В примере 6</span><span class="sxs-lookup"><span data-stu-id="c5f9d-385">Example 6</span></span>
<span data-ttu-id="c5f9d-386">В этом примере расширяет истекающим сроком действия назначения ролей для пользователя ANUJCUSER для участника службы управления API.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-386">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="c5f9d-387">**Примечание:** В additon разрешение, в этом примере требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="c5f9d-387">**Note:** In additon to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="c5f9d-388">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5f9d-388">Property</span></span>     | <span data-ttu-id="c5f9d-389">Тип</span><span class="sxs-lookup"><span data-stu-id="c5f9d-389">Type</span></span>    |<span data-ttu-id="c5f9d-390">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c5f9d-390">Required</span></span>|  <span data-ttu-id="c5f9d-391">Значение</span><span class="sxs-lookup"><span data-stu-id="c5f9d-391">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="c5f9d-392">resourceId</span><span class="sxs-lookup"><span data-stu-id="c5f9d-392">resourceId</span></span>|<span data-ttu-id="c5f9d-393">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-393">String</span></span>|<span data-ttu-id="c5f9d-394">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-394">Yes</span></span>|<span data-ttu-id="c5f9d-395">\<</span><span class="sxs-lookup"><span data-stu-id="c5f9d-395">\<resourceId\></span></span>|
|<span data-ttu-id="c5f9d-396">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c5f9d-396">roleDefinitionId</span></span>|<span data-ttu-id="c5f9d-397">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-397">String</span></span>|<span data-ttu-id="c5f9d-398">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-398">Yes</span></span>|<span data-ttu-id="c5f9d-399">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="c5f9d-399">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="c5f9d-400">subjectId</span><span class="sxs-lookup"><span data-stu-id="c5f9d-400">subjectId</span></span>|<span data-ttu-id="c5f9d-401">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-401">String</span></span>|<span data-ttu-id="c5f9d-402">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-402">Yes</span></span>|<span data-ttu-id="c5f9d-403">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="c5f9d-403">\<subjectId\></span></span>|
|<span data-ttu-id="c5f9d-404">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c5f9d-404">assignmentState</span></span>|<span data-ttu-id="c5f9d-405">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-405">String</span></span>|<span data-ttu-id="c5f9d-406">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-406">Yes</span></span>| <span data-ttu-id="c5f9d-407">Допустимость / Active</span><span class="sxs-lookup"><span data-stu-id="c5f9d-407">Eligible / Active</span></span> |
|<span data-ttu-id="c5f9d-408">type</span><span class="sxs-lookup"><span data-stu-id="c5f9d-408">type</span></span>|<span data-ttu-id="c5f9d-409">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-409">String</span></span>|<span data-ttu-id="c5f9d-410">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-410">Yes</span></span>| <span data-ttu-id="c5f9d-411">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="c5f9d-411">AdminExtend</span></span>|
|<span data-ttu-id="c5f9d-412">Reason</span><span class="sxs-lookup"><span data-stu-id="c5f9d-412">reason</span></span>|<span data-ttu-id="c5f9d-413">String</span><span class="sxs-lookup"><span data-stu-id="c5f9d-413">String</span></span>| <span data-ttu-id="c5f9d-414">зависит от roleSettings</span><span class="sxs-lookup"><span data-stu-id="c5f9d-414">depends on roleSettings</span></span>||
|<span data-ttu-id="c5f9d-415">Расписание</span><span class="sxs-lookup"><span data-stu-id="c5f9d-415">schedule</span></span>|[<span data-ttu-id="c5f9d-416">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c5f9d-416">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="c5f9d-417">Да</span><span class="sxs-lookup"><span data-stu-id="c5f9d-417">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="c5f9d-418">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5f9d-418">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="c5f9d-419">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5f9d-419">Response</span></span>
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
