---
title: Создание governanceRoleAssignmentRequest
description: Создание роли назначения запроса для представления операции, требуется на назначения ролей. В следующей таблице перечислены операции.
localization_priority: Normal
ms.openlocfilehash: 09adb824147dba745649efc7589ca763f815278d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823774"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="dd7c7-104">Создание governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="dd7c7-104">Create governanceRoleAssignmentRequest</span></span>

> <span data-ttu-id="dd7c7-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd7c7-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dd7c7-107">Создание роли назначения запроса для представления операции, требуется на назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-107">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="dd7c7-108">В следующей таблице перечислены операции.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-108">The following table lists the operations.</span></span>

| <span data-ttu-id="dd7c7-109">Операция</span><span class="sxs-lookup"><span data-stu-id="dd7c7-109">Operation</span></span>       | <span data-ttu-id="dd7c7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="dd7c7-110">Type</span></span> | 
|:---------------|:----------|
| <span data-ttu-id="dd7c7-111">Назначение назначения ролей</span><span class="sxs-lookup"><span data-stu-id="dd7c7-111">Assign a role assignment</span></span>| <span data-ttu-id="dd7c7-112">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="dd7c7-112">AdminAdd</span></span> |
| <span data-ttu-id="dd7c7-113">Активация назначение подходящими роли</span><span class="sxs-lookup"><span data-stu-id="dd7c7-113">Activate an eligible role assignment</span></span>| <span data-ttu-id="dd7c7-114">UserAdd</span><span class="sxs-lookup"><span data-stu-id="dd7c7-114">UserAdd</span></span> | 
| <span data-ttu-id="dd7c7-115">Деактивация назначение активированные роли</span><span class="sxs-lookup"><span data-stu-id="dd7c7-115">Deactivate an activated role assignment</span></span>| <span data-ttu-id="dd7c7-116">UserRemove</span><span class="sxs-lookup"><span data-stu-id="dd7c7-116">UserRemove</span></span> | 
| <span data-ttu-id="dd7c7-117">Удаление назначения ролей</span><span class="sxs-lookup"><span data-stu-id="dd7c7-117">Remove a role assignment</span></span>| <span data-ttu-id="dd7c7-118">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="dd7c7-118">AdminRemove</span></span> |
| <span data-ttu-id="dd7c7-119">Обновление назначения ролей</span><span class="sxs-lookup"><span data-stu-id="dd7c7-119">Update a role assignment</span></span>| <span data-ttu-id="dd7c7-120">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="dd7c7-120">AdminUpdate</span></span> |
| <span data-ttu-id="dd7c7-121">Запрос на расширение my назначения роли</span><span class="sxs-lookup"><span data-stu-id="dd7c7-121">Request to extend my role assignment</span></span>| <span data-ttu-id="dd7c7-122">UserExtend</span><span class="sxs-lookup"><span data-stu-id="dd7c7-122">UserExtend</span></span> | 
| <span data-ttu-id="dd7c7-123">Расширение назначения ролей</span><span class="sxs-lookup"><span data-stu-id="dd7c7-123">Extend a role assignment</span></span>| <span data-ttu-id="dd7c7-124">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="dd7c7-124">AdminExtend</span></span> | 
| <span data-ttu-id="dd7c7-125">Запрос на обновление назначения ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="dd7c7-125">Request to renew my expired role assignment</span></span>| <span data-ttu-id="dd7c7-126">UserRenew</span><span class="sxs-lookup"><span data-stu-id="dd7c7-126">UserRenew</span></span> | 
| <span data-ttu-id="dd7c7-127">Обновление назначения ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="dd7c7-127">Renew an expired role assignment</span></span>| <span data-ttu-id="dd7c7-128">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="dd7c7-128">AdminRenew</span></span> | 

 
## <a name="permissions"></a><span data-ttu-id="dd7c7-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd7c7-129">Permissions</span></span>
<span data-ttu-id="dd7c7-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd7c7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd7c7-132">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd7c7-132">Permission type</span></span>      | <span data-ttu-id="dd7c7-133">Permissions</span><span class="sxs-lookup"><span data-stu-id="dd7c7-133">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd7c7-134">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd7c7-134">Delegated (work or school account)</span></span> | <span data-ttu-id="dd7c7-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="dd7c7-135">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="dd7c7-136">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd7c7-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd7c7-137">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-137">Not supported.</span></span>    |
|<span data-ttu-id="dd7c7-138">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd7c7-138">Application</span></span> | <span data-ttu-id="dd7c7-139">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="dd7c7-139">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd7c7-140">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd7c7-140">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="dd7c7-141">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd7c7-141">Request headers</span></span>
| <span data-ttu-id="dd7c7-142">Имя</span><span class="sxs-lookup"><span data-stu-id="dd7c7-142">Name</span></span>       | <span data-ttu-id="dd7c7-143">Описание</span><span class="sxs-lookup"><span data-stu-id="dd7c7-143">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dd7c7-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd7c7-144">Authorization</span></span>  | <span data-ttu-id="dd7c7-145">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="dd7c7-145">Bearer {code}</span></span>|
| <span data-ttu-id="dd7c7-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dd7c7-146">Content-type</span></span>  | <span data-ttu-id="dd7c7-147">application/json</span><span class="sxs-lookup"><span data-stu-id="dd7c7-147">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd7c7-148">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dd7c7-148">Request body</span></span>
<span data-ttu-id="dd7c7-149">В тексте запроса укажите представление JSON объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="dd7c7-149">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="dd7c7-150">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd7c7-150">Property</span></span>     | <span data-ttu-id="dd7c7-151">Тип</span><span class="sxs-lookup"><span data-stu-id="dd7c7-151">Type</span></span>    |<span data-ttu-id="dd7c7-152">Обязательный</span><span class="sxs-lookup"><span data-stu-id="dd7c7-152">Required</span></span>|  <span data-ttu-id="dd7c7-153">Описание</span><span class="sxs-lookup"><span data-stu-id="dd7c7-153">Description</span></span>|
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="dd7c7-154">resourceId</span><span class="sxs-lookup"><span data-stu-id="dd7c7-154">resourceId</span></span>|<span data-ttu-id="dd7c7-155">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-155">String</span></span>|<span data-ttu-id="dd7c7-156">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-156">Yes</span></span>|<span data-ttu-id="dd7c7-157">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-157">The ID of the resource.</span></span>|
|<span data-ttu-id="dd7c7-158">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="dd7c7-158">roleDefinitionId</span></span>|<span data-ttu-id="dd7c7-159">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-159">String</span></span>|<span data-ttu-id="dd7c7-160">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-160">Yes</span></span>|<span data-ttu-id="dd7c7-161">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-161">The ID of the role definition.</span></span>|
|<span data-ttu-id="dd7c7-162">subjectId</span><span class="sxs-lookup"><span data-stu-id="dd7c7-162">subjectId</span></span>|<span data-ttu-id="dd7c7-163">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-163">String</span></span>|<span data-ttu-id="dd7c7-164">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-164">Yes</span></span>|<span data-ttu-id="dd7c7-165">Идентификатор субъекта.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-165">The ID of the subject.</span></span>|
|<span data-ttu-id="dd7c7-166">assignmentState</span><span class="sxs-lookup"><span data-stu-id="dd7c7-166">assignmentState</span></span>|<span data-ttu-id="dd7c7-167">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-167">String</span></span>|<span data-ttu-id="dd7c7-168">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-168">Yes</span></span>|<span data-ttu-id="dd7c7-169">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-169">The state of assignment.</span></span> <span data-ttu-id="dd7c7-170">Значение может быть ``Eligible`` и ``Active``.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-170">The value can be ``Eligible`` and ``Active``.</span></span>|
|<span data-ttu-id="dd7c7-171">type</span><span class="sxs-lookup"><span data-stu-id="dd7c7-171">type</span></span>|<span data-ttu-id="dd7c7-172">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-172">String</span></span>|<span data-ttu-id="dd7c7-173">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-173">Yes</span></span>|<span data-ttu-id="dd7c7-174">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-174">The request type.</span></span> <span data-ttu-id="dd7c7-175">Значение может быть `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`и `AdminExtend`.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-175">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span>|
|<span data-ttu-id="dd7c7-176">Причина</span><span class="sxs-lookup"><span data-stu-id="dd7c7-176">reason</span></span>|<span data-ttu-id="dd7c7-177">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-177">String</span></span>| |<span data-ttu-id="dd7c7-178">Причину должно предоставляться для запроса назначений ролей для аудита и предварительный просмотр цели.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-178">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="dd7c7-179">расписание</span><span class="sxs-lookup"><span data-stu-id="dd7c7-179">schedule</span></span>|[<span data-ttu-id="dd7c7-180">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="dd7c7-180">governanceSchedule</span></span>](../resources/governanceschedule.md)| | <span data-ttu-id="dd7c7-181">Расписание для запроса назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-181">The schedule of the role assignment request.</span></span> <span data-ttu-id="dd7c7-182">Для запроса типа `UserAdd`, `AdminAdd`, `AdminUpdate`, и `AdminExtend`, это необходимо.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-182">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span>|

## <a name="response"></a><span data-ttu-id="dd7c7-183">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd7c7-183">Response</span></span>
<span data-ttu-id="dd7c7-184">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-184">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="dd7c7-185">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="dd7c7-185">Error codes</span></span>
<span data-ttu-id="dd7c7-186">Этот интерфейс API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-186">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="dd7c7-187">Кроме того он возвращает коды ошибок, перечисленных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-187">In addition, it also returns the error codes listed in the following table.</span></span>

|<span data-ttu-id="dd7c7-188">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="dd7c7-188">Error code</span></span>     | <span data-ttu-id="dd7c7-189">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="dd7c7-189">Error message</span></span>              | <span data-ttu-id="dd7c7-190">Сведения</span><span class="sxs-lookup"><span data-stu-id="dd7c7-190">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="dd7c7-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="dd7c7-191">400 BadRequest</span></span> | <span data-ttu-id="dd7c7-192">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="dd7c7-192">RoleNotFound</span></span>    | <span data-ttu-id="dd7c7-193">`roleDefinitionId` Условии, что в запросе не удается найти текст.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-193">The `roleDefinitionId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="dd7c7-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="dd7c7-194">400 BadRequest</span></span> | <span data-ttu-id="dd7c7-195">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="dd7c7-195">ResourceIsLocked</span></span>    | <span data-ttu-id="dd7c7-196">Ресурс, представленные в тексте запроса находится в состоянии из `Locked` и не могут создавать запросы назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-196">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span>
| <span data-ttu-id="dd7c7-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="dd7c7-197">400 BadRequest</span></span> | <span data-ttu-id="dd7c7-198">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="dd7c7-198">SubjectNotFound</span></span>    | <span data-ttu-id="dd7c7-199">`subjectId` Условии, что в запросе не удается найти текст.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-199">The `subjectId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="dd7c7-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="dd7c7-200">400 BadRequest</span></span> | <span data-ttu-id="dd7c7-201">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="dd7c7-201">PendingRoleAssignmentRequest</span></span>    | <span data-ttu-id="dd7c7-202">Уже существует ожидающие [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в системе.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-202">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span>
| <span data-ttu-id="dd7c7-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="dd7c7-203">400 BadRequest</span></span> | <span data-ttu-id="dd7c7-204">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="dd7c7-204">RoleAssignmentExists</span></span>    | <span data-ttu-id="dd7c7-205">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) запрошено будет создан уже существует в системе.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span>
| <span data-ttu-id="dd7c7-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="dd7c7-206">400 BadRequest</span></span> | <span data-ttu-id="dd7c7-207">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="dd7c7-207">RoleAssignmentDoesNotExist</span></span>    | <span data-ttu-id="dd7c7-208">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) запрос на обновление/расширить не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-208">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span>
| <span data-ttu-id="dd7c7-209">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="dd7c7-209">400 BadRequest</span></span> | <span data-ttu-id="dd7c7-210">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="dd7c7-210">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="dd7c7-211">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) не соответствует внутренней политик и не может быть создан.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-211">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span>

## <a name="examples"></a><span data-ttu-id="dd7c7-212">Примеры</span><span class="sxs-lookup"><span data-stu-id="dd7c7-212">Examples</span></span>
<span data-ttu-id="dd7c7-213">В приведенных ниже примерах показано, как использовать этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-213">The following examples show how to use this API.</span></span>

### <a name="example-1"></a><span data-ttu-id="dd7c7-214">Пример 1</span><span class="sxs-lookup"><span data-stu-id="dd7c7-214">Example 1</span></span>
<span data-ttu-id="dd7c7-215">В этом примере администраторам назначение роли выставления счетов читатель nawu@fimdev.net пользователя.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-215">In this example, administrators assign user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="dd7c7-216">**Примечание:** В дополнение к разрешение, в этом примере требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-216">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="dd7c7-217">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd7c7-217">Property</span></span>     | <span data-ttu-id="dd7c7-218">Тип</span><span class="sxs-lookup"><span data-stu-id="dd7c7-218">Type</span></span>    |<span data-ttu-id="dd7c7-219">Обязательный</span><span class="sxs-lookup"><span data-stu-id="dd7c7-219">Required</span></span>|  <span data-ttu-id="dd7c7-220">Значение</span><span class="sxs-lookup"><span data-stu-id="dd7c7-220">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="dd7c7-221">resourceId</span><span class="sxs-lookup"><span data-stu-id="dd7c7-221">resourceId</span></span>|<span data-ttu-id="dd7c7-222">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-222">String</span></span>|<span data-ttu-id="dd7c7-223">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-223">Yes</span></span>|<span data-ttu-id="dd7c7-224">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="dd7c7-224">\<resourceId\></span></span>|
|<span data-ttu-id="dd7c7-225">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="dd7c7-225">roleDefinitionId</span></span>|<span data-ttu-id="dd7c7-226">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-226">String</span></span>|<span data-ttu-id="dd7c7-227">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-227">Yes</span></span>|<span data-ttu-id="dd7c7-228">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="dd7c7-228">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="dd7c7-229">subjectId</span><span class="sxs-lookup"><span data-stu-id="dd7c7-229">subjectId</span></span>|<span data-ttu-id="dd7c7-230">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-230">String</span></span>|<span data-ttu-id="dd7c7-231">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-231">Yes</span></span>|<span data-ttu-id="dd7c7-232">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="dd7c7-232">\<subjectId\></span></span>|
|<span data-ttu-id="dd7c7-233">assignmentState</span><span class="sxs-lookup"><span data-stu-id="dd7c7-233">assignmentState</span></span>|<span data-ttu-id="dd7c7-234">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-234">String</span></span>|<span data-ttu-id="dd7c7-235">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-235">Yes</span></span>| <span data-ttu-id="dd7c7-236">Допустимость / Active</span><span class="sxs-lookup"><span data-stu-id="dd7c7-236">Eligible / Active</span></span>|
|<span data-ttu-id="dd7c7-237">type</span><span class="sxs-lookup"><span data-stu-id="dd7c7-237">type</span></span>|<span data-ttu-id="dd7c7-238">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-238">String</span></span>|<span data-ttu-id="dd7c7-239">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-239">Yes</span></span>| <span data-ttu-id="dd7c7-240">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="dd7c7-240">AdminAdd</span></span>|
|<span data-ttu-id="dd7c7-241">Причина</span><span class="sxs-lookup"><span data-stu-id="dd7c7-241">reason</span></span>|<span data-ttu-id="dd7c7-242">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-242">String</span></span>| <span data-ttu-id="dd7c7-243">зависит от роли параметров</span><span class="sxs-lookup"><span data-stu-id="dd7c7-243">depends on role Settings</span></span>||
|<span data-ttu-id="dd7c7-244">расписание</span><span class="sxs-lookup"><span data-stu-id="dd7c7-244">schedule</span></span>|[<span data-ttu-id="dd7c7-245">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="dd7c7-245">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="dd7c7-246">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-246">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="dd7c7-247">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd7c7-247">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="dd7c7-248">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd7c7-248">Response</span></span>
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

### <a name="example-2"></a><span data-ttu-id="dd7c7-249">Пример 2</span><span class="sxs-lookup"><span data-stu-id="dd7c7-249">Example 2</span></span>
<span data-ttu-id="dd7c7-250">В этом примере nawu@fimdev.net пользователь активирует право чтения выставления счетов роли.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-250">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="dd7c7-251">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd7c7-251">Property</span></span>     | <span data-ttu-id="dd7c7-252">Тип</span><span class="sxs-lookup"><span data-stu-id="dd7c7-252">Type</span></span>    |<span data-ttu-id="dd7c7-253">Обязательный</span><span class="sxs-lookup"><span data-stu-id="dd7c7-253">Required</span></span>|  <span data-ttu-id="dd7c7-254">Значение</span><span class="sxs-lookup"><span data-stu-id="dd7c7-254">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="dd7c7-255">resourceId</span><span class="sxs-lookup"><span data-stu-id="dd7c7-255">resourceId</span></span>|<span data-ttu-id="dd7c7-256">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-256">String</span></span>|<span data-ttu-id="dd7c7-257">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-257">Yes</span></span>|<span data-ttu-id="dd7c7-258">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="dd7c7-258">\<resourceId\></span></span>|
|<span data-ttu-id="dd7c7-259">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="dd7c7-259">roleDefinitionId</span></span>|<span data-ttu-id="dd7c7-260">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-260">String</span></span>|<span data-ttu-id="dd7c7-261">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-261">Yes</span></span>|<span data-ttu-id="dd7c7-262">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="dd7c7-262">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="dd7c7-263">subjectId</span><span class="sxs-lookup"><span data-stu-id="dd7c7-263">subjectId</span></span>|<span data-ttu-id="dd7c7-264">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-264">String</span></span>|<span data-ttu-id="dd7c7-265">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-265">Yes</span></span>|<span data-ttu-id="dd7c7-266">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="dd7c7-266">\<subjectId\></span></span>|
|<span data-ttu-id="dd7c7-267">assignmentState</span><span class="sxs-lookup"><span data-stu-id="dd7c7-267">assignmentState</span></span>|<span data-ttu-id="dd7c7-268">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-268">String</span></span>|<span data-ttu-id="dd7c7-269">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-269">Yes</span></span>| <span data-ttu-id="dd7c7-270">Активное</span><span class="sxs-lookup"><span data-stu-id="dd7c7-270">Active</span></span>|
|<span data-ttu-id="dd7c7-271">type</span><span class="sxs-lookup"><span data-stu-id="dd7c7-271">type</span></span>|<span data-ttu-id="dd7c7-272">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-272">String</span></span>|<span data-ttu-id="dd7c7-273">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-273">Yes</span></span>| <span data-ttu-id="dd7c7-274">UserAdd</span><span class="sxs-lookup"><span data-stu-id="dd7c7-274">UserAdd</span></span>|
|<span data-ttu-id="dd7c7-275">Причина</span><span class="sxs-lookup"><span data-stu-id="dd7c7-275">reason</span></span>|<span data-ttu-id="dd7c7-276">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-276">String</span></span>| <span data-ttu-id="dd7c7-277">зависит от роли параметров</span><span class="sxs-lookup"><span data-stu-id="dd7c7-277">depends on role Settings</span></span>||
|<span data-ttu-id="dd7c7-278">расписание</span><span class="sxs-lookup"><span data-stu-id="dd7c7-278">schedule</span></span>|[<span data-ttu-id="dd7c7-279">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="dd7c7-279">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="dd7c7-280">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-280">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="dd7c7-281">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd7c7-281">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="dd7c7-282">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd7c7-282">Response</span></span>
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

### <a name="example-3"></a><span data-ttu-id="dd7c7-283">Пример 3</span><span class="sxs-lookup"><span data-stu-id="dd7c7-283">Example 3</span></span>
<span data-ttu-id="dd7c7-284">В этом примере пользователь nawu@fimdev.net деактивирует активная роль чтения выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-284">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="dd7c7-285">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd7c7-285">Property</span></span>     | <span data-ttu-id="dd7c7-286">Тип</span><span class="sxs-lookup"><span data-stu-id="dd7c7-286">Type</span></span>    |<span data-ttu-id="dd7c7-287">Обязательный</span><span class="sxs-lookup"><span data-stu-id="dd7c7-287">Required</span></span>|  <span data-ttu-id="dd7c7-288">Значение</span><span class="sxs-lookup"><span data-stu-id="dd7c7-288">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="dd7c7-289">resourceId</span><span class="sxs-lookup"><span data-stu-id="dd7c7-289">resourceId</span></span>|<span data-ttu-id="dd7c7-290">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-290">String</span></span>|<span data-ttu-id="dd7c7-291">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-291">Yes</span></span>|<span data-ttu-id="dd7c7-292">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="dd7c7-292">\<resourceId\></span></span>|
|<span data-ttu-id="dd7c7-293">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="dd7c7-293">roleDefinitionId</span></span>|<span data-ttu-id="dd7c7-294">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-294">String</span></span>|<span data-ttu-id="dd7c7-295">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-295">Yes</span></span>|<span data-ttu-id="dd7c7-296">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="dd7c7-296">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="dd7c7-297">subjectId</span><span class="sxs-lookup"><span data-stu-id="dd7c7-297">subjectId</span></span>|<span data-ttu-id="dd7c7-298">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-298">String</span></span>|<span data-ttu-id="dd7c7-299">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-299">Yes</span></span>|<span data-ttu-id="dd7c7-300">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="dd7c7-300">\<subjectId\></span></span>|
|<span data-ttu-id="dd7c7-301">assignmentState</span><span class="sxs-lookup"><span data-stu-id="dd7c7-301">assignmentState</span></span>|<span data-ttu-id="dd7c7-302">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-302">String</span></span>|<span data-ttu-id="dd7c7-303">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-303">Yes</span></span>| <span data-ttu-id="dd7c7-304">Активное</span><span class="sxs-lookup"><span data-stu-id="dd7c7-304">Active</span></span>|
|<span data-ttu-id="dd7c7-305">type</span><span class="sxs-lookup"><span data-stu-id="dd7c7-305">type</span></span>|<span data-ttu-id="dd7c7-306">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-306">String</span></span>|<span data-ttu-id="dd7c7-307">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-307">Yes</span></span>| <span data-ttu-id="dd7c7-308">UserRemove</span><span class="sxs-lookup"><span data-stu-id="dd7c7-308">UserRemove</span></span>|
|<span data-ttu-id="dd7c7-309">Причина</span><span class="sxs-lookup"><span data-stu-id="dd7c7-309">reason</span></span>|<span data-ttu-id="dd7c7-310">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-310">String</span></span>| <span data-ttu-id="dd7c7-311">Нет</span><span class="sxs-lookup"><span data-stu-id="dd7c7-311">No</span></span>||
|<span data-ttu-id="dd7c7-312">расписание</span><span class="sxs-lookup"><span data-stu-id="dd7c7-312">schedule</span></span>|[<span data-ttu-id="dd7c7-313">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="dd7c7-313">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="dd7c7-314">Нет</span><span class="sxs-lookup"><span data-stu-id="dd7c7-314">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="dd7c7-315">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd7c7-315">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="dd7c7-316">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd7c7-316">Response</span></span>
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

### <a name="example-4"></a><span data-ttu-id="dd7c7-317">Пример 4</span><span class="sxs-lookup"><span data-stu-id="dd7c7-317">Example 4</span></span>
<span data-ttu-id="dd7c7-318">В этом примере администраторам удалить nawu@fimdev.net пользователя из роли выставления счетов чтения.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-318">In this example, administrators remove the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="dd7c7-319">**Примечание:** В дополнение к разрешение, в этом примере требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-319">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="dd7c7-320">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd7c7-320">Property</span></span>     | <span data-ttu-id="dd7c7-321">Тип</span><span class="sxs-lookup"><span data-stu-id="dd7c7-321">Type</span></span>    |<span data-ttu-id="dd7c7-322">Обязательный</span><span class="sxs-lookup"><span data-stu-id="dd7c7-322">Required</span></span>|  <span data-ttu-id="dd7c7-323">Значение</span><span class="sxs-lookup"><span data-stu-id="dd7c7-323">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="dd7c7-324">resourceId</span><span class="sxs-lookup"><span data-stu-id="dd7c7-324">resourceId</span></span>|<span data-ttu-id="dd7c7-325">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-325">String</span></span>|<span data-ttu-id="dd7c7-326">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-326">Yes</span></span>|<span data-ttu-id="dd7c7-327">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="dd7c7-327">\<resourceId\></span></span>|
|<span data-ttu-id="dd7c7-328">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="dd7c7-328">roleDefinitionId</span></span>|<span data-ttu-id="dd7c7-329">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-329">String</span></span>|<span data-ttu-id="dd7c7-330">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-330">Yes</span></span>|<span data-ttu-id="dd7c7-331">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="dd7c7-331">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="dd7c7-332">subjectId</span><span class="sxs-lookup"><span data-stu-id="dd7c7-332">subjectId</span></span>|<span data-ttu-id="dd7c7-333">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-333">String</span></span>|<span data-ttu-id="dd7c7-334">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-334">Yes</span></span>|<span data-ttu-id="dd7c7-335">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="dd7c7-335">\<subjectId\></span></span>|
|<span data-ttu-id="dd7c7-336">assignmentState</span><span class="sxs-lookup"><span data-stu-id="dd7c7-336">assignmentState</span></span>|<span data-ttu-id="dd7c7-337">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-337">String</span></span>|<span data-ttu-id="dd7c7-338">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-338">Yes</span></span>| <span data-ttu-id="dd7c7-339">Допустимость / Active</span><span class="sxs-lookup"><span data-stu-id="dd7c7-339">Eligible / Active</span></span>|
|<span data-ttu-id="dd7c7-340">type</span><span class="sxs-lookup"><span data-stu-id="dd7c7-340">type</span></span>|<span data-ttu-id="dd7c7-341">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-341">String</span></span>|<span data-ttu-id="dd7c7-342">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-342">Yes</span></span>| <span data-ttu-id="dd7c7-343">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="dd7c7-343">AdminRemove</span></span>|
|<span data-ttu-id="dd7c7-344">Причина</span><span class="sxs-lookup"><span data-stu-id="dd7c7-344">reason</span></span>|<span data-ttu-id="dd7c7-345">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-345">String</span></span>| <span data-ttu-id="dd7c7-346">Нет</span><span class="sxs-lookup"><span data-stu-id="dd7c7-346">No</span></span>||
|<span data-ttu-id="dd7c7-347">расписание</span><span class="sxs-lookup"><span data-stu-id="dd7c7-347">schedule</span></span>|[<span data-ttu-id="dd7c7-348">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="dd7c7-348">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="dd7c7-349">Нет</span><span class="sxs-lookup"><span data-stu-id="dd7c7-349">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="dd7c7-350">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd7c7-350">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="dd7c7-351">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd7c7-351">Response</span></span>
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

### <a name="example-5"></a><span data-ttu-id="dd7c7-352">Пример 5</span><span class="sxs-lookup"><span data-stu-id="dd7c7-352">Example 5</span></span>
<span data-ttu-id="dd7c7-353">В этом примере Администраторы обновление назначения ролей для пользователя nawu@fimdev.net владельцу.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-353">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="dd7c7-354">**Примечание:** В дополнение к разрешение, в этом примере требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-354">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="dd7c7-355">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd7c7-355">Property</span></span>     | <span data-ttu-id="dd7c7-356">Тип</span><span class="sxs-lookup"><span data-stu-id="dd7c7-356">Type</span></span>    |<span data-ttu-id="dd7c7-357">Обязательный</span><span class="sxs-lookup"><span data-stu-id="dd7c7-357">Required</span></span>|  <span data-ttu-id="dd7c7-358">Значение</span><span class="sxs-lookup"><span data-stu-id="dd7c7-358">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="dd7c7-359">resourceId</span><span class="sxs-lookup"><span data-stu-id="dd7c7-359">resourceId</span></span>|<span data-ttu-id="dd7c7-360">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-360">String</span></span>|<span data-ttu-id="dd7c7-361">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-361">Yes</span></span>|<span data-ttu-id="dd7c7-362">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="dd7c7-362">\<resourceId\></span></span>|
|<span data-ttu-id="dd7c7-363">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="dd7c7-363">roleDefinitionId</span></span>|<span data-ttu-id="dd7c7-364">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-364">String</span></span>|<span data-ttu-id="dd7c7-365">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-365">Yes</span></span>|<span data-ttu-id="dd7c7-366">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="dd7c7-366">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="dd7c7-367">subjectId</span><span class="sxs-lookup"><span data-stu-id="dd7c7-367">subjectId</span></span>|<span data-ttu-id="dd7c7-368">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-368">String</span></span>|<span data-ttu-id="dd7c7-369">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-369">Yes</span></span>|<span data-ttu-id="dd7c7-370">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="dd7c7-370">\<subjectId\></span></span>|
|<span data-ttu-id="dd7c7-371">assignmentState</span><span class="sxs-lookup"><span data-stu-id="dd7c7-371">assignmentState</span></span>|<span data-ttu-id="dd7c7-372">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-372">String</span></span>|<span data-ttu-id="dd7c7-373">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-373">Yes</span></span>| <span data-ttu-id="dd7c7-374">Допустимость / Active</span><span class="sxs-lookup"><span data-stu-id="dd7c7-374">Eligible / Active</span></span>|
|<span data-ttu-id="dd7c7-375">type</span><span class="sxs-lookup"><span data-stu-id="dd7c7-375">type</span></span>|<span data-ttu-id="dd7c7-376">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-376">String</span></span>|<span data-ttu-id="dd7c7-377">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-377">Yes</span></span>| <span data-ttu-id="dd7c7-378">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="dd7c7-378">AdminUpdate</span></span>|
|<span data-ttu-id="dd7c7-379">Причина</span><span class="sxs-lookup"><span data-stu-id="dd7c7-379">reason</span></span>|<span data-ttu-id="dd7c7-380">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-380">String</span></span>| <span data-ttu-id="dd7c7-381">зависит от roleSettings</span><span class="sxs-lookup"><span data-stu-id="dd7c7-381">depends on roleSettings</span></span>||
|<span data-ttu-id="dd7c7-382">расписание</span><span class="sxs-lookup"><span data-stu-id="dd7c7-382">schedule</span></span>|[<span data-ttu-id="dd7c7-383">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="dd7c7-383">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="dd7c7-384">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-384">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="dd7c7-385">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd7c7-385">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="dd7c7-386">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd7c7-386">Response</span></span>
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

### <a name="example-6"></a><span data-ttu-id="dd7c7-387">В примере 6</span><span class="sxs-lookup"><span data-stu-id="dd7c7-387">Example 6</span></span>
<span data-ttu-id="dd7c7-388">В этом примере расширяет истекающим сроком действия назначения ролей для пользователя ANUJCUSER для участника службы управления API.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-388">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="dd7c7-389">**Примечание:** В additon разрешение, в этом примере требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="dd7c7-389">**Note:** In additon to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="dd7c7-390">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd7c7-390">Property</span></span>     | <span data-ttu-id="dd7c7-391">Тип</span><span class="sxs-lookup"><span data-stu-id="dd7c7-391">Type</span></span>    |<span data-ttu-id="dd7c7-392">Обязательный</span><span class="sxs-lookup"><span data-stu-id="dd7c7-392">Required</span></span>|  <span data-ttu-id="dd7c7-393">Значение</span><span class="sxs-lookup"><span data-stu-id="dd7c7-393">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="dd7c7-394">resourceId</span><span class="sxs-lookup"><span data-stu-id="dd7c7-394">resourceId</span></span>|<span data-ttu-id="dd7c7-395">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-395">String</span></span>|<span data-ttu-id="dd7c7-396">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-396">Yes</span></span>|<span data-ttu-id="dd7c7-397">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="dd7c7-397">\<resourceId\></span></span>|
|<span data-ttu-id="dd7c7-398">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="dd7c7-398">roleDefinitionId</span></span>|<span data-ttu-id="dd7c7-399">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-399">String</span></span>|<span data-ttu-id="dd7c7-400">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-400">Yes</span></span>|<span data-ttu-id="dd7c7-401">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="dd7c7-401">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="dd7c7-402">subjectId</span><span class="sxs-lookup"><span data-stu-id="dd7c7-402">subjectId</span></span>|<span data-ttu-id="dd7c7-403">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-403">String</span></span>|<span data-ttu-id="dd7c7-404">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-404">Yes</span></span>|<span data-ttu-id="dd7c7-405">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="dd7c7-405">\<subjectId\></span></span>|
|<span data-ttu-id="dd7c7-406">assignmentState</span><span class="sxs-lookup"><span data-stu-id="dd7c7-406">assignmentState</span></span>|<span data-ttu-id="dd7c7-407">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-407">String</span></span>|<span data-ttu-id="dd7c7-408">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-408">Yes</span></span>| <span data-ttu-id="dd7c7-409">Допустимость / Active</span><span class="sxs-lookup"><span data-stu-id="dd7c7-409">Eligible / Active</span></span> |
|<span data-ttu-id="dd7c7-410">type</span><span class="sxs-lookup"><span data-stu-id="dd7c7-410">type</span></span>|<span data-ttu-id="dd7c7-411">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-411">String</span></span>|<span data-ttu-id="dd7c7-412">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-412">Yes</span></span>| <span data-ttu-id="dd7c7-413">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="dd7c7-413">AdminExtend</span></span>|
|<span data-ttu-id="dd7c7-414">Причина</span><span class="sxs-lookup"><span data-stu-id="dd7c7-414">reason</span></span>|<span data-ttu-id="dd7c7-415">Строка</span><span class="sxs-lookup"><span data-stu-id="dd7c7-415">String</span></span>| <span data-ttu-id="dd7c7-416">зависит от roleSettings</span><span class="sxs-lookup"><span data-stu-id="dd7c7-416">depends on roleSettings</span></span>||
|<span data-ttu-id="dd7c7-417">расписание</span><span class="sxs-lookup"><span data-stu-id="dd7c7-417">schedule</span></span>|[<span data-ttu-id="dd7c7-418">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="dd7c7-418">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="dd7c7-419">Да</span><span class="sxs-lookup"><span data-stu-id="dd7c7-419">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="dd7c7-420">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd7c7-420">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="dd7c7-421">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd7c7-421">Response</span></span>
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
