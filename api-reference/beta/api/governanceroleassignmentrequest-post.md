---
title: Создание governanceRoleAssignmentRequest
description: Создание роли назначения запроса для представления операции, требуется на назначения ролей. В следующей таблице перечислены операции.
localization_priority: Normal
ms.openlocfilehash: 104ab1a0d4909bc2181df70bc4fc895fc4558260
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967223"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="753e6-104">Создание governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="753e6-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="753e6-105">Создание роли назначения запроса для представления операции, требуется на назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="753e6-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="753e6-106">В следующей таблице перечислены операции.</span><span class="sxs-lookup"><span data-stu-id="753e6-106">The following table lists the operations.</span></span>

| <span data-ttu-id="753e6-107">Operation</span><span class="sxs-lookup"><span data-stu-id="753e6-107">Operation</span></span>                                   | <span data-ttu-id="753e6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="753e6-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="753e6-109">Назначение назначения ролей</span><span class="sxs-lookup"><span data-stu-id="753e6-109">Assign a role assignment</span></span>                    | <span data-ttu-id="753e6-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="753e6-110">AdminAdd</span></span>    |
| <span data-ttu-id="753e6-111">Активация назначение подходящими роли</span><span class="sxs-lookup"><span data-stu-id="753e6-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="753e6-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="753e6-112">UserAdd</span></span>     |
| <span data-ttu-id="753e6-113">Деактивация назначение активированные роли</span><span class="sxs-lookup"><span data-stu-id="753e6-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="753e6-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="753e6-114">UserRemove</span></span>  |
| <span data-ttu-id="753e6-115">Удаление назначения ролей</span><span class="sxs-lookup"><span data-stu-id="753e6-115">Remove a role assignment</span></span>                    | <span data-ttu-id="753e6-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="753e6-116">AdminRemove</span></span> |
| <span data-ttu-id="753e6-117">Обновление назначения ролей</span><span class="sxs-lookup"><span data-stu-id="753e6-117">Update a role assignment</span></span>                    | <span data-ttu-id="753e6-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="753e6-118">AdminUpdate</span></span> |
| <span data-ttu-id="753e6-119">Запрос на расширение my назначения роли</span><span class="sxs-lookup"><span data-stu-id="753e6-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="753e6-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="753e6-120">UserExtend</span></span>  |
| <span data-ttu-id="753e6-121">Расширение назначения ролей</span><span class="sxs-lookup"><span data-stu-id="753e6-121">Extend a role assignment</span></span>                    | <span data-ttu-id="753e6-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="753e6-122">AdminExtend</span></span> |
| <span data-ttu-id="753e6-123">Запрос на обновление назначения ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="753e6-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="753e6-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="753e6-124">UserRenew</span></span>   |
| <span data-ttu-id="753e6-125">Обновление назначения ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="753e6-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="753e6-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="753e6-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="753e6-127">Разрешения</span><span class="sxs-lookup"><span data-stu-id="753e6-127">Permissions</span></span>

<span data-ttu-id="753e6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="753e6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="753e6-130">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="753e6-130">Permission type</span></span>                        | <span data-ttu-id="753e6-131">Разрешения</span><span class="sxs-lookup"><span data-stu-id="753e6-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="753e6-132">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="753e6-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="753e6-133">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="753e6-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="753e6-134">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="753e6-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="753e6-135">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="753e6-135">Not supported.</span></span>                            |
| <span data-ttu-id="753e6-136">Для приложений</span><span class="sxs-lookup"><span data-stu-id="753e6-136">Application</span></span>                            | <span data-ttu-id="753e6-137">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="753e6-137">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="753e6-138">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="753e6-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="753e6-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="753e6-139">Request headers</span></span>

| <span data-ttu-id="753e6-140">Имя</span><span class="sxs-lookup"><span data-stu-id="753e6-140">Name</span></span>          | <span data-ttu-id="753e6-141">Описание</span><span class="sxs-lookup"><span data-stu-id="753e6-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="753e6-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="753e6-142">Authorization</span></span> | <span data-ttu-id="753e6-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="753e6-143">Bearer {code}</span></span>    |
| <span data-ttu-id="753e6-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="753e6-144">Content-type</span></span>  | <span data-ttu-id="753e6-145">application/json</span><span class="sxs-lookup"><span data-stu-id="753e6-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="753e6-146">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="753e6-146">Request body</span></span>

<span data-ttu-id="753e6-147">В тексте запроса укажите представление JSON объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="753e6-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="753e6-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="753e6-148">Property</span></span>         | <span data-ttu-id="753e6-149">Тип</span><span class="sxs-lookup"><span data-stu-id="753e6-149">Type</span></span>                                                     | <span data-ttu-id="753e6-150">Описание</span><span class="sxs-lookup"><span data-stu-id="753e6-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="753e6-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="753e6-151">resourceId</span></span>       | <span data-ttu-id="753e6-152">String</span><span class="sxs-lookup"><span data-stu-id="753e6-152">String</span></span>                                                   | <span data-ttu-id="753e6-153">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="753e6-153">The ID of the resource.</span></span> <span data-ttu-id="753e6-154">Обязательно указывать.</span><span class="sxs-lookup"><span data-stu-id="753e6-154">Required.</span></span> |
| <span data-ttu-id="753e6-155">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="753e6-155">roleDefinitionId</span></span> | <span data-ttu-id="753e6-156">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-156">String</span></span>                                                   | <span data-ttu-id="753e6-157">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="753e6-157">The ID of the role definition.</span></span> <span data-ttu-id="753e6-158">Обязательно указывать.</span><span class="sxs-lookup"><span data-stu-id="753e6-158">Required.</span></span> |
| <span data-ttu-id="753e6-159">subjectId</span><span class="sxs-lookup"><span data-stu-id="753e6-159">subjectId</span></span>        | <span data-ttu-id="753e6-160">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-160">String</span></span>                                                   | <span data-ttu-id="753e6-161">Идентификатор субъекта.</span><span class="sxs-lookup"><span data-stu-id="753e6-161">The ID of the subject.</span></span> <span data-ttu-id="753e6-162">Обязательно указывать.</span><span class="sxs-lookup"><span data-stu-id="753e6-162">Required.</span></span> |
| <span data-ttu-id="753e6-163">assignmentState</span><span class="sxs-lookup"><span data-stu-id="753e6-163">assignmentState</span></span>  | <span data-ttu-id="753e6-164">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-164">String</span></span>                                                   | <span data-ttu-id="753e6-165">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="753e6-165">The state of assignment.</span></span> <span data-ttu-id="753e6-166">Значение может быть `Eligible` и `Active`.</span><span class="sxs-lookup"><span data-stu-id="753e6-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="753e6-167">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="753e6-167">Required.</span></span> |
| <span data-ttu-id="753e6-168">type</span><span class="sxs-lookup"><span data-stu-id="753e6-168">type</span></span>             | <span data-ttu-id="753e6-169">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-169">String</span></span>                                                   | <span data-ttu-id="753e6-170">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="753e6-170">The request type.</span></span> <span data-ttu-id="753e6-171">Значение может быть `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`и `AdminExtend`.</span><span class="sxs-lookup"><span data-stu-id="753e6-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="753e6-172">Обязательно указывать.</span><span class="sxs-lookup"><span data-stu-id="753e6-172">Required.</span></span> |
| <span data-ttu-id="753e6-173">Причина</span><span class="sxs-lookup"><span data-stu-id="753e6-173">reason</span></span>           | <span data-ttu-id="753e6-174">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-174">String</span></span>                                                   | <span data-ttu-id="753e6-175">Причину должно предоставляться для запроса назначений ролей для аудита и предварительный просмотр цели.</span><span class="sxs-lookup"><span data-stu-id="753e6-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="753e6-176">расписание</span><span class="sxs-lookup"><span data-stu-id="753e6-176">schedule</span></span>         | [<span data-ttu-id="753e6-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="753e6-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="753e6-178">Расписание для запроса назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="753e6-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="753e6-179">Для запроса типа `UserAdd`, `AdminAdd`, `AdminUpdate`, и `AdminExtend`, это необходимо.</span><span class="sxs-lookup"><span data-stu-id="753e6-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="753e6-180">Ответ</span><span class="sxs-lookup"><span data-stu-id="753e6-180">Response</span></span>

<span data-ttu-id="753e6-181">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="753e6-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="753e6-182">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="753e6-182">Error codes</span></span>

<span data-ttu-id="753e6-183">Этот интерфейс API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="753e6-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="753e6-184">Кроме того он возвращает коды ошибок, перечисленных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="753e6-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="753e6-185">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="753e6-185">Error code</span></span>     | <span data-ttu-id="753e6-186">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="753e6-186">Error message</span></span>                               | <span data-ttu-id="753e6-187">Сведения</span><span class="sxs-lookup"><span data-stu-id="753e6-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="753e6-188">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="753e6-188">400 BadRequest</span></span> | <span data-ttu-id="753e6-189">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="753e6-189">RoleNotFound</span></span>                                | <span data-ttu-id="753e6-190">`roleDefinitionId` Условии, что в запросе не удается найти текст.</span><span class="sxs-lookup"><span data-stu-id="753e6-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="753e6-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="753e6-191">400 BadRequest</span></span> | <span data-ttu-id="753e6-192">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="753e6-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="753e6-193">Ресурс, представленные в тексте запроса находится в состоянии из `Locked` и не могут создавать запросы назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="753e6-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="753e6-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="753e6-194">400 BadRequest</span></span> | <span data-ttu-id="753e6-195">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="753e6-195">SubjectNotFound</span></span>                             | <span data-ttu-id="753e6-196">`subjectId` Условии, что в запросе не удается найти текст.</span><span class="sxs-lookup"><span data-stu-id="753e6-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="753e6-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="753e6-197">400 BadRequest</span></span> | <span data-ttu-id="753e6-198">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="753e6-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="753e6-199">Уже существует ожидающие [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в системе.</span><span class="sxs-lookup"><span data-stu-id="753e6-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="753e6-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="753e6-200">400 BadRequest</span></span> | <span data-ttu-id="753e6-201">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="753e6-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="753e6-202">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) запрошено будет создан уже существует в системе.</span><span class="sxs-lookup"><span data-stu-id="753e6-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="753e6-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="753e6-203">400 BadRequest</span></span> | <span data-ttu-id="753e6-204">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="753e6-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="753e6-205">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) запрос на обновление/расширить не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="753e6-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="753e6-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="753e6-206">400 BadRequest</span></span> | <span data-ttu-id="753e6-207">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="753e6-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="753e6-208">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) не соответствует внутренней политик и не может быть создан.</span><span class="sxs-lookup"><span data-stu-id="753e6-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="753e6-209">Примеры</span><span class="sxs-lookup"><span data-stu-id="753e6-209">Examples</span></span>

<span data-ttu-id="753e6-210">В приведенных ниже примерах показано, как использовать этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="753e6-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="753e6-211">В примере 1: Администратор назначает пользователя к роли</span><span class="sxs-lookup"><span data-stu-id="753e6-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="753e6-212">В этом примере администратор назначает nawu@fimdev.net пользователя по выставлению счетов новую роль.</span><span class="sxs-lookup"><span data-stu-id="753e6-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="753e6-213">**Примечание:** В дополнение к разрешение, в этом примере требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="753e6-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="753e6-214">Свойство</span><span class="sxs-lookup"><span data-stu-id="753e6-214">Property</span></span>         | <span data-ttu-id="753e6-215">Тип</span><span class="sxs-lookup"><span data-stu-id="753e6-215">Type</span></span>                                                     | <span data-ttu-id="753e6-216">Обязательный</span><span class="sxs-lookup"><span data-stu-id="753e6-216">Required</span></span>                 | <span data-ttu-id="753e6-217">Значение</span><span class="sxs-lookup"><span data-stu-id="753e6-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="753e6-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="753e6-218">resourceId</span></span>       | <span data-ttu-id="753e6-219">String</span><span class="sxs-lookup"><span data-stu-id="753e6-219">String</span></span>                                                   | <span data-ttu-id="753e6-220">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-220">Yes</span></span>                      | <span data-ttu-id="753e6-221">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="753e6-221">\<resourceId\></span></span> |
| <span data-ttu-id="753e6-222">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="753e6-222">roleDefinitionId</span></span> | <span data-ttu-id="753e6-223">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-223">String</span></span>                                                   | <span data-ttu-id="753e6-224">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-224">Yes</span></span>                      | <span data-ttu-id="753e6-225">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="753e6-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="753e6-226">subjectId</span><span class="sxs-lookup"><span data-stu-id="753e6-226">subjectId</span></span>        | <span data-ttu-id="753e6-227">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-227">String</span></span>                                                   | <span data-ttu-id="753e6-228">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-228">Yes</span></span>                      | <span data-ttu-id="753e6-229">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="753e6-229">\<subjectId\></span></span> |
| <span data-ttu-id="753e6-230">assignmentState</span><span class="sxs-lookup"><span data-stu-id="753e6-230">assignmentState</span></span>  | <span data-ttu-id="753e6-231">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-231">String</span></span>                                                   | <span data-ttu-id="753e6-232">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-232">Yes</span></span>                      | <span data-ttu-id="753e6-233">Допустимость / Active</span><span class="sxs-lookup"><span data-stu-id="753e6-233">Eligible / Active</span></span> |
| <span data-ttu-id="753e6-234">type</span><span class="sxs-lookup"><span data-stu-id="753e6-234">type</span></span>             | <span data-ttu-id="753e6-235">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-235">String</span></span>                                                   | <span data-ttu-id="753e6-236">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-236">Yes</span></span>                      | <span data-ttu-id="753e6-237">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="753e6-237">AdminAdd</span></span> |
| <span data-ttu-id="753e6-238">Причина</span><span class="sxs-lookup"><span data-stu-id="753e6-238">reason</span></span>           | <span data-ttu-id="753e6-239">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-239">String</span></span>                                                   | <span data-ttu-id="753e6-240">зависит от роли параметров</span><span class="sxs-lookup"><span data-stu-id="753e6-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="753e6-241">расписание</span><span class="sxs-lookup"><span data-stu-id="753e6-241">schedule</span></span>         | [<span data-ttu-id="753e6-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="753e6-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="753e6-243">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="753e6-244">Запрос</span><span class="sxs-lookup"><span data-stu-id="753e6-244">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Eligible",
  "type": "AdminAdd",
  "reason": "Assign an eligible role",
  "schedule": {
    "startDateTime": "2018-05-12T23:37:43.356Z",
    "endDateTime": "2018-11-08T23:37:43.356Z",
    "type": "Once"
  }
}
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="753e6-245">Ответ</span><span class="sxs-lookup"><span data-stu-id="753e6-245">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="753e6-246">Пример 2: Пользователь активирует подходящими роли</span><span class="sxs-lookup"><span data-stu-id="753e6-246">Example 2: User activates eligible role</span></span>

<span data-ttu-id="753e6-247">В этом примере nawu@fimdev.net пользователь активирует право чтения выставления счетов роли.</span><span class="sxs-lookup"><span data-stu-id="753e6-247">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="753e6-248">Свойство</span><span class="sxs-lookup"><span data-stu-id="753e6-248">Property</span></span>         | <span data-ttu-id="753e6-249">Тип</span><span class="sxs-lookup"><span data-stu-id="753e6-249">Type</span></span>                                                     | <span data-ttu-id="753e6-250">Обязательный</span><span class="sxs-lookup"><span data-stu-id="753e6-250">Required</span></span>                 | <span data-ttu-id="753e6-251">Значение</span><span class="sxs-lookup"><span data-stu-id="753e6-251">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="753e6-252">resourceId</span><span class="sxs-lookup"><span data-stu-id="753e6-252">resourceId</span></span>       | <span data-ttu-id="753e6-253">String</span><span class="sxs-lookup"><span data-stu-id="753e6-253">String</span></span>                                                   | <span data-ttu-id="753e6-254">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-254">Yes</span></span>                      | <span data-ttu-id="753e6-255">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="753e6-255">\<resourceId\></span></span> |
| <span data-ttu-id="753e6-256">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="753e6-256">roleDefinitionId</span></span> | <span data-ttu-id="753e6-257">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-257">String</span></span>                                                   | <span data-ttu-id="753e6-258">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-258">Yes</span></span>                      | <span data-ttu-id="753e6-259">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="753e6-259">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="753e6-260">subjectId</span><span class="sxs-lookup"><span data-stu-id="753e6-260">subjectId</span></span>        | <span data-ttu-id="753e6-261">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-261">String</span></span>                                                   | <span data-ttu-id="753e6-262">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-262">Yes</span></span>                      | <span data-ttu-id="753e6-263">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="753e6-263">\<subjectId\></span></span> |
| <span data-ttu-id="753e6-264">assignmentState</span><span class="sxs-lookup"><span data-stu-id="753e6-264">assignmentState</span></span>  | <span data-ttu-id="753e6-265">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-265">String</span></span>                                                   | <span data-ttu-id="753e6-266">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-266">Yes</span></span>                      | <span data-ttu-id="753e6-267">Активное</span><span class="sxs-lookup"><span data-stu-id="753e6-267">Active</span></span> |
| <span data-ttu-id="753e6-268">type</span><span class="sxs-lookup"><span data-stu-id="753e6-268">type</span></span>             | <span data-ttu-id="753e6-269">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-269">String</span></span>                                                   | <span data-ttu-id="753e6-270">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-270">Yes</span></span>                      | <span data-ttu-id="753e6-271">UserAdd</span><span class="sxs-lookup"><span data-stu-id="753e6-271">UserAdd</span></span> |
| <span data-ttu-id="753e6-272">Причина</span><span class="sxs-lookup"><span data-stu-id="753e6-272">reason</span></span>           | <span data-ttu-id="753e6-273">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-273">String</span></span>                                                   | <span data-ttu-id="753e6-274">зависит от роли параметров</span><span class="sxs-lookup"><span data-stu-id="753e6-274">depends on role Settings</span></span> |   |
| <span data-ttu-id="753e6-275">расписание</span><span class="sxs-lookup"><span data-stu-id="753e6-275">schedule</span></span>         | [<span data-ttu-id="753e6-276">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="753e6-276">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="753e6-277">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-277">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="753e6-278">Запрос</span><span class="sxs-lookup"><span data-stu-id="753e6-278">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Active",
  "type": "UserAdd",
  "reason": "Activate the owner role",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:28:43.537Z",
    "duration": "PT9H"
  },
  "linkedEligibleRoleAssignmentId": "e327f4be-42a0-47a2-8579-0a39b025b394"
}
```

#### <a name="response"></a><span data-ttu-id="753e6-279">Ответ</span><span class="sxs-lookup"><span data-stu-id="753e6-279">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="753e6-280">В примере 3: Пользователь деактивирует назначенной роли</span><span class="sxs-lookup"><span data-stu-id="753e6-280">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="753e6-281">В этом примере пользователь nawu@fimdev.net деактивирует активная роль чтения выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="753e6-281">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="753e6-282">Свойство</span><span class="sxs-lookup"><span data-stu-id="753e6-282">Property</span></span>         | <span data-ttu-id="753e6-283">Тип</span><span class="sxs-lookup"><span data-stu-id="753e6-283">Type</span></span>                                                     | <span data-ttu-id="753e6-284">Обязательный</span><span class="sxs-lookup"><span data-stu-id="753e6-284">Required</span></span> | <span data-ttu-id="753e6-285">Значение</span><span class="sxs-lookup"><span data-stu-id="753e6-285">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="753e6-286">resourceId</span><span class="sxs-lookup"><span data-stu-id="753e6-286">resourceId</span></span>       | <span data-ttu-id="753e6-287">String</span><span class="sxs-lookup"><span data-stu-id="753e6-287">String</span></span>                                                   | <span data-ttu-id="753e6-288">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-288">Yes</span></span>      | <span data-ttu-id="753e6-289">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="753e6-289">\<resourceId\></span></span> |
| <span data-ttu-id="753e6-290">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="753e6-290">roleDefinitionId</span></span> | <span data-ttu-id="753e6-291">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-291">String</span></span>                                                   | <span data-ttu-id="753e6-292">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-292">Yes</span></span>      | <span data-ttu-id="753e6-293">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="753e6-293">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="753e6-294">subjectId</span><span class="sxs-lookup"><span data-stu-id="753e6-294">subjectId</span></span>        | <span data-ttu-id="753e6-295">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-295">String</span></span>                                                   | <span data-ttu-id="753e6-296">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-296">Yes</span></span>      | <span data-ttu-id="753e6-297">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="753e6-297">\<subjectId\></span></span> |
| <span data-ttu-id="753e6-298">assignmentState</span><span class="sxs-lookup"><span data-stu-id="753e6-298">assignmentState</span></span>  | <span data-ttu-id="753e6-299">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-299">String</span></span>                                                   | <span data-ttu-id="753e6-300">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-300">Yes</span></span>      | <span data-ttu-id="753e6-301">Активное</span><span class="sxs-lookup"><span data-stu-id="753e6-301">Active</span></span> |
| <span data-ttu-id="753e6-302">type</span><span class="sxs-lookup"><span data-stu-id="753e6-302">type</span></span>             | <span data-ttu-id="753e6-303">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-303">String</span></span>                                                   | <span data-ttu-id="753e6-304">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-304">Yes</span></span>      | <span data-ttu-id="753e6-305">UserRemove</span><span class="sxs-lookup"><span data-stu-id="753e6-305">UserRemove</span></span> |
| <span data-ttu-id="753e6-306">Причина</span><span class="sxs-lookup"><span data-stu-id="753e6-306">reason</span></span>           | <span data-ttu-id="753e6-307">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-307">String</span></span>                                                   | <span data-ttu-id="753e6-308">Нет</span><span class="sxs-lookup"><span data-stu-id="753e6-308">No</span></span>       |   |
| <span data-ttu-id="753e6-309">расписание</span><span class="sxs-lookup"><span data-stu-id="753e6-309">schedule</span></span>         | [<span data-ttu-id="753e6-310">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="753e6-310">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="753e6-311">Нет</span><span class="sxs-lookup"><span data-stu-id="753e6-311">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="753e6-312">Запрос</span><span class="sxs-lookup"><span data-stu-id="753e6-312">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
  "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Active",
  "type": "UserRemove",
  "reason": "Deactivate the role",
  "linkedEligibleRoleAssignmentId": "cb8a533e-02d5-42ad-8499-916b1e4822ec"
}
```

#### <a name="response"></a><span data-ttu-id="753e6-313">Ответ</span><span class="sxs-lookup"><span data-stu-id="753e6-313">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="753e6-314">Пример 4: Администратор удаляет пользователя из роли</span><span class="sxs-lookup"><span data-stu-id="753e6-314">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="753e6-315">В этом примере администратор удаляет nawu@fimdev.net пользователя из роли выставления счетов чтения.</span><span class="sxs-lookup"><span data-stu-id="753e6-315">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="753e6-316">**Примечание:** В дополнение к разрешение, в этом примере требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="753e6-316">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="753e6-317">Свойство</span><span class="sxs-lookup"><span data-stu-id="753e6-317">Property</span></span>         | <span data-ttu-id="753e6-318">Тип</span><span class="sxs-lookup"><span data-stu-id="753e6-318">Type</span></span>                                                     | <span data-ttu-id="753e6-319">Обязательный</span><span class="sxs-lookup"><span data-stu-id="753e6-319">Required</span></span> | <span data-ttu-id="753e6-320">Значение</span><span class="sxs-lookup"><span data-stu-id="753e6-320">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="753e6-321">resourceId</span><span class="sxs-lookup"><span data-stu-id="753e6-321">resourceId</span></span>       | <span data-ttu-id="753e6-322">String</span><span class="sxs-lookup"><span data-stu-id="753e6-322">String</span></span>                                                   | <span data-ttu-id="753e6-323">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-323">Yes</span></span>      | <span data-ttu-id="753e6-324">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="753e6-324">\<resourceId\></span></span> |
| <span data-ttu-id="753e6-325">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="753e6-325">roleDefinitionId</span></span> | <span data-ttu-id="753e6-326">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-326">String</span></span>                                                   | <span data-ttu-id="753e6-327">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-327">Yes</span></span>      | <span data-ttu-id="753e6-328">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="753e6-328">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="753e6-329">subjectId</span><span class="sxs-lookup"><span data-stu-id="753e6-329">subjectId</span></span>        | <span data-ttu-id="753e6-330">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-330">String</span></span>                                                   | <span data-ttu-id="753e6-331">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-331">Yes</span></span>      | <span data-ttu-id="753e6-332">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="753e6-332">\<subjectId\></span></span> |
| <span data-ttu-id="753e6-333">assignmentState</span><span class="sxs-lookup"><span data-stu-id="753e6-333">assignmentState</span></span>  | <span data-ttu-id="753e6-334">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-334">String</span></span>                                                   | <span data-ttu-id="753e6-335">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-335">Yes</span></span>      | <span data-ttu-id="753e6-336">Допустимость / Active</span><span class="sxs-lookup"><span data-stu-id="753e6-336">Eligible / Active</span></span> |
| <span data-ttu-id="753e6-337">type</span><span class="sxs-lookup"><span data-stu-id="753e6-337">type</span></span>             | <span data-ttu-id="753e6-338">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-338">String</span></span>                                                   | <span data-ttu-id="753e6-339">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-339">Yes</span></span>      | <span data-ttu-id="753e6-340">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="753e6-340">AdminRemove</span></span> |
| <span data-ttu-id="753e6-341">Причина</span><span class="sxs-lookup"><span data-stu-id="753e6-341">reason</span></span>           | <span data-ttu-id="753e6-342">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-342">String</span></span>                                                   | <span data-ttu-id="753e6-343">Нет</span><span class="sxs-lookup"><span data-stu-id="753e6-343">No</span></span>       |   |
| <span data-ttu-id="753e6-344">расписание</span><span class="sxs-lookup"><span data-stu-id="753e6-344">schedule</span></span>         | [<span data-ttu-id="753e6-345">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="753e6-345">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="753e6-346">Нет</span><span class="sxs-lookup"><span data-stu-id="753e6-346">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="753e6-347">Запрос</span><span class="sxs-lookup"><span data-stu-id="753e6-347">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState": "Eligible",
  "type": "AdminRemove"
}
```

#### <a name="response"></a><span data-ttu-id="753e6-348">Ответ</span><span class="sxs-lookup"><span data-stu-id="753e6-348">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "c934fcb9-cf53-42ac-a8b4-6246f6726299",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminRemove",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": null,
  "status": {
    "status": "Closed",
    "subStatus": "Revoked",
    "statusDetails": []
  },
  "schedule": null
}
```

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="753e6-349">Пример 5: Администратор обновляет назначения роли</span><span class="sxs-lookup"><span data-stu-id="753e6-349">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="753e6-350">В этом примере Администраторы обновление назначения ролей для пользователя nawu@fimdev.net владельцу.</span><span class="sxs-lookup"><span data-stu-id="753e6-350">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="753e6-351">**Примечание:** В дополнение к разрешение, в этом примере требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="753e6-351">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="753e6-352">Свойство</span><span class="sxs-lookup"><span data-stu-id="753e6-352">Property</span></span>         | <span data-ttu-id="753e6-353">Тип</span><span class="sxs-lookup"><span data-stu-id="753e6-353">Type</span></span>                                                     | <span data-ttu-id="753e6-354">Обязательный</span><span class="sxs-lookup"><span data-stu-id="753e6-354">Required</span></span>                | <span data-ttu-id="753e6-355">Значение</span><span class="sxs-lookup"><span data-stu-id="753e6-355">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="753e6-356">resourceId</span><span class="sxs-lookup"><span data-stu-id="753e6-356">resourceId</span></span>       | <span data-ttu-id="753e6-357">String</span><span class="sxs-lookup"><span data-stu-id="753e6-357">String</span></span>                                                   | <span data-ttu-id="753e6-358">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-358">Yes</span></span>                     | <span data-ttu-id="753e6-359">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="753e6-359">\<resourceId\></span></span> |
| <span data-ttu-id="753e6-360">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="753e6-360">roleDefinitionId</span></span> | <span data-ttu-id="753e6-361">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-361">String</span></span>                                                   | <span data-ttu-id="753e6-362">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-362">Yes</span></span>                     | <span data-ttu-id="753e6-363">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="753e6-363">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="753e6-364">subjectId</span><span class="sxs-lookup"><span data-stu-id="753e6-364">subjectId</span></span>        | <span data-ttu-id="753e6-365">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-365">String</span></span>                                                   | <span data-ttu-id="753e6-366">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-366">Yes</span></span>                     | <span data-ttu-id="753e6-367">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="753e6-367">\<subjectId\></span></span> |
| <span data-ttu-id="753e6-368">assignmentState</span><span class="sxs-lookup"><span data-stu-id="753e6-368">assignmentState</span></span>  | <span data-ttu-id="753e6-369">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-369">String</span></span>                                                   | <span data-ttu-id="753e6-370">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-370">Yes</span></span>                     | <span data-ttu-id="753e6-371">Допустимость / Active</span><span class="sxs-lookup"><span data-stu-id="753e6-371">Eligible / Active</span></span> |
| <span data-ttu-id="753e6-372">type</span><span class="sxs-lookup"><span data-stu-id="753e6-372">type</span></span>             | <span data-ttu-id="753e6-373">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-373">String</span></span>                                                   | <span data-ttu-id="753e6-374">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-374">Yes</span></span>                     | <span data-ttu-id="753e6-375">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="753e6-375">AdminUpdate</span></span> |
| <span data-ttu-id="753e6-376">Причина</span><span class="sxs-lookup"><span data-stu-id="753e6-376">reason</span></span>           | <span data-ttu-id="753e6-377">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-377">String</span></span>                                                   | <span data-ttu-id="753e6-378">зависит от roleSettings</span><span class="sxs-lookup"><span data-stu-id="753e6-378">depends on roleSettings</span></span> |   |
| <span data-ttu-id="753e6-379">расписание</span><span class="sxs-lookup"><span data-stu-id="753e6-379">schedule</span></span>         | [<span data-ttu-id="753e6-380">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="753e6-380">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="753e6-381">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-381">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="753e6-382">Запрос</span><span class="sxs-lookup"><span data-stu-id="753e6-382">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "1566d11d-d2b6-444a-a8de-28698682c445",
  "assignmentState": "Eligible",
  "type": "AdminUpdate",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-03-08T05:42:45.317Z",
    "endDateTime": "2018-06-05T05:42:31.000Z"
  }
}
```

#### <a name="response"></a><span data-ttu-id="753e6-383">Ответ</span><span class="sxs-lookup"><span data-stu-id="753e6-383">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "4f6d4802-b3ac-4f5a-86d7-a6a4edd7d383",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "subjectId": "1566d11d-d2b6-444a-a8de-28698682c445",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminUpdate",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": null,
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
    "startDateTime": "2018-03-08T05:42:45.317Z",
    "endDateTime": "2018-06-05T05:42:31Z",
    "duration": "PT0S"
  }
}
```

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="753e6-384">В примере 6: Администратор расширяет истекающим сроком действия назначения роли</span><span class="sxs-lookup"><span data-stu-id="753e6-384">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="753e6-385">В этом примере расширяет истекающим сроком действия назначения ролей для пользователя ANUJCUSER для участника службы управления API.</span><span class="sxs-lookup"><span data-stu-id="753e6-385">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="753e6-386">**Примечание:** В дополнение к разрешение, в этом примере требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="753e6-386">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="753e6-387">Свойство</span><span class="sxs-lookup"><span data-stu-id="753e6-387">Property</span></span>         | <span data-ttu-id="753e6-388">Тип</span><span class="sxs-lookup"><span data-stu-id="753e6-388">Type</span></span>                                                     | <span data-ttu-id="753e6-389">Обязательный</span><span class="sxs-lookup"><span data-stu-id="753e6-389">Required</span></span>                | <span data-ttu-id="753e6-390">Значение</span><span class="sxs-lookup"><span data-stu-id="753e6-390">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="753e6-391">resourceId</span><span class="sxs-lookup"><span data-stu-id="753e6-391">resourceId</span></span>       | <span data-ttu-id="753e6-392">String</span><span class="sxs-lookup"><span data-stu-id="753e6-392">String</span></span>                                                   | <span data-ttu-id="753e6-393">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-393">Yes</span></span>                     | <span data-ttu-id="753e6-394">\<Ид_ресурса\></span><span class="sxs-lookup"><span data-stu-id="753e6-394">\<resourceId\></span></span> |
| <span data-ttu-id="753e6-395">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="753e6-395">roleDefinitionId</span></span> | <span data-ttu-id="753e6-396">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-396">String</span></span>                                                   | <span data-ttu-id="753e6-397">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-397">Yes</span></span>                     | <span data-ttu-id="753e6-398">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="753e6-398">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="753e6-399">subjectId</span><span class="sxs-lookup"><span data-stu-id="753e6-399">subjectId</span></span>        | <span data-ttu-id="753e6-400">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-400">String</span></span>                                                   | <span data-ttu-id="753e6-401">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-401">Yes</span></span>                     | <span data-ttu-id="753e6-402">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="753e6-402">\<subjectId\></span></span> |
| <span data-ttu-id="753e6-403">assignmentState</span><span class="sxs-lookup"><span data-stu-id="753e6-403">assignmentState</span></span>  | <span data-ttu-id="753e6-404">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-404">String</span></span>                                                   | <span data-ttu-id="753e6-405">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-405">Yes</span></span>                     | <span data-ttu-id="753e6-406">Допустимость / Active</span><span class="sxs-lookup"><span data-stu-id="753e6-406">Eligible / Active</span></span> |
| <span data-ttu-id="753e6-407">type</span><span class="sxs-lookup"><span data-stu-id="753e6-407">type</span></span>             | <span data-ttu-id="753e6-408">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-408">String</span></span>                                                   | <span data-ttu-id="753e6-409">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-409">Yes</span></span>                     | <span data-ttu-id="753e6-410">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="753e6-410">AdminExtend</span></span> |
| <span data-ttu-id="753e6-411">Причина</span><span class="sxs-lookup"><span data-stu-id="753e6-411">reason</span></span>           | <span data-ttu-id="753e6-412">Строка</span><span class="sxs-lookup"><span data-stu-id="753e6-412">String</span></span>                                                   | <span data-ttu-id="753e6-413">зависит от roleSettings</span><span class="sxs-lookup"><span data-stu-id="753e6-413">depends on roleSettings</span></span> |   |
| <span data-ttu-id="753e6-414">расписание</span><span class="sxs-lookup"><span data-stu-id="753e6-414">schedule</span></span>         | [<span data-ttu-id="753e6-415">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="753e6-415">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="753e6-416">Да</span><span class="sxs-lookup"><span data-stu-id="753e6-416">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="753e6-417">Запрос</span><span class="sxs-lookup"><span data-stu-id="753e6-417">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState": "Eligible",
  "type": "AdminExtend",
  "reason": "extend role assignment",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:53:55.327Z",
    "endDateTime": "2018-08-10T23:53:55.327Z"
  }
}
```

#### <a name="response"></a><span data-ttu-id="753e6-418">Отклик</span><span class="sxs-lookup"><span data-stu-id="753e6-418">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "486f0c05-47c8-4498-9c06-086a78c83004",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminExtend",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": "extend role assignment",
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
    "startDateTime": "2018-05-12T23:53:55.327Z",
    "endDateTime": "2018-08-10T23:53:55.327Z",
    "duration": "PT0S"
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
