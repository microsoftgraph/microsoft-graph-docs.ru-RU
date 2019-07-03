---
title: Создание governanceRoleAssignmentRequest
description: Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли. В приведенной ниже таблице перечислены операции.
localization_priority: Normal
ms.openlocfilehash: 614d5a90bbf71f8cb5794923ae4f56d85d06415e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440780"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="d872c-104">Создание governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="d872c-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d872c-105">Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="d872c-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="d872c-106">В приведенной ниже таблице перечислены операции.</span><span class="sxs-lookup"><span data-stu-id="d872c-106">The following table lists the operations.</span></span>

| <span data-ttu-id="d872c-107">Operation</span><span class="sxs-lookup"><span data-stu-id="d872c-107">Operation</span></span>                                   | <span data-ttu-id="d872c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d872c-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="d872c-109">Назначение роли</span><span class="sxs-lookup"><span data-stu-id="d872c-109">Assign a role assignment</span></span>                    | <span data-ttu-id="d872c-110">Админадд</span><span class="sxs-lookup"><span data-stu-id="d872c-110">AdminAdd</span></span>    |
| <span data-ttu-id="d872c-111">Активация подходящего назначения роли</span><span class="sxs-lookup"><span data-stu-id="d872c-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="d872c-112">Усерадд</span><span class="sxs-lookup"><span data-stu-id="d872c-112">UserAdd</span></span>     |
| <span data-ttu-id="d872c-113">Деактивация активированного назначения роли</span><span class="sxs-lookup"><span data-stu-id="d872c-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="d872c-114">Усерремове</span><span class="sxs-lookup"><span data-stu-id="d872c-114">UserRemove</span></span>  |
| <span data-ttu-id="d872c-115">Удаление назначения роли</span><span class="sxs-lookup"><span data-stu-id="d872c-115">Remove a role assignment</span></span>                    | <span data-ttu-id="d872c-116">Админремове</span><span class="sxs-lookup"><span data-stu-id="d872c-116">AdminRemove</span></span> |
| <span data-ttu-id="d872c-117">Обновление назначения роли</span><span class="sxs-lookup"><span data-stu-id="d872c-117">Update a role assignment</span></span>                    | <span data-ttu-id="d872c-118">Админупдате</span><span class="sxs-lookup"><span data-stu-id="d872c-118">AdminUpdate</span></span> |
| <span data-ttu-id="d872c-119">Запрос на расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="d872c-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="d872c-120">Усерекстенд</span><span class="sxs-lookup"><span data-stu-id="d872c-120">UserExtend</span></span>  |
| <span data-ttu-id="d872c-121">Расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="d872c-121">Extend a role assignment</span></span>                    | <span data-ttu-id="d872c-122">Админекстенд</span><span class="sxs-lookup"><span data-stu-id="d872c-122">AdminExtend</span></span> |
| <span data-ttu-id="d872c-123">Запрос на продление назначения роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="d872c-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="d872c-124">Усерренев</span><span class="sxs-lookup"><span data-stu-id="d872c-124">UserRenew</span></span>   |
| <span data-ttu-id="d872c-125">Продление назначенной роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="d872c-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="d872c-126">Админренев</span><span class="sxs-lookup"><span data-stu-id="d872c-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="d872c-127">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d872c-127">Permissions</span></span>

<span data-ttu-id="d872c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d872c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d872c-130">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d872c-130">Permission type</span></span>                        | <span data-ttu-id="d872c-131">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d872c-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="d872c-132">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d872c-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="d872c-133">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="d872c-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="d872c-134">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d872c-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d872c-135">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d872c-135">Not supported.</span></span>                            |
| <span data-ttu-id="d872c-136">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d872c-136">Application</span></span>                            | <span data-ttu-id="d872c-137">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d872c-137">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d872c-138">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d872c-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="d872c-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d872c-139">Request headers</span></span>

| <span data-ttu-id="d872c-140">Имя</span><span class="sxs-lookup"><span data-stu-id="d872c-140">Name</span></span>          | <span data-ttu-id="d872c-141">Описание</span><span class="sxs-lookup"><span data-stu-id="d872c-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="d872c-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d872c-142">Authorization</span></span> | <span data-ttu-id="d872c-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d872c-143">Bearer {code}</span></span>    |
| <span data-ttu-id="d872c-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d872c-144">Content-type</span></span>  | <span data-ttu-id="d872c-145">application/json</span><span class="sxs-lookup"><span data-stu-id="d872c-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d872c-146">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d872c-146">Request body</span></span>

<span data-ttu-id="d872c-147">В тексте запроса добавьте представление объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d872c-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="d872c-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="d872c-148">Property</span></span>         | <span data-ttu-id="d872c-149">Тип</span><span class="sxs-lookup"><span data-stu-id="d872c-149">Type</span></span>                                                     | <span data-ttu-id="d872c-150">Описание</span><span class="sxs-lookup"><span data-stu-id="d872c-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="d872c-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="d872c-151">resourceId</span></span>       | <span data-ttu-id="d872c-152">String</span><span class="sxs-lookup"><span data-stu-id="d872c-152">String</span></span>                                                   | <span data-ttu-id="d872c-153">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="d872c-153">The ID of the resource.</span></span> <span data-ttu-id="d872c-154">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="d872c-154">Required.</span></span> |
| <span data-ttu-id="d872c-155">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="d872c-155">roleDefinitionId</span></span> | <span data-ttu-id="d872c-156">String</span><span class="sxs-lookup"><span data-stu-id="d872c-156">String</span></span>                                                   | <span data-ttu-id="d872c-157">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="d872c-157">The ID of the role definition.</span></span> <span data-ttu-id="d872c-158">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="d872c-158">Required.</span></span> |
| <span data-ttu-id="d872c-159">Субжектид</span><span class="sxs-lookup"><span data-stu-id="d872c-159">subjectId</span></span>        | <span data-ttu-id="d872c-160">String</span><span class="sxs-lookup"><span data-stu-id="d872c-160">String</span></span>                                                   | <span data-ttu-id="d872c-161">ИДЕНТИФИКАТОР субъекта.</span><span class="sxs-lookup"><span data-stu-id="d872c-161">The ID of the subject.</span></span> <span data-ttu-id="d872c-162">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="d872c-162">Required.</span></span> |
| <span data-ttu-id="d872c-163">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="d872c-163">assignmentState</span></span>  | <span data-ttu-id="d872c-164">String</span><span class="sxs-lookup"><span data-stu-id="d872c-164">String</span></span>                                                   | <span data-ttu-id="d872c-165">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="d872c-165">The state of assignment.</span></span> <span data-ttu-id="d872c-166">Значение может быть `Eligible` и `Active`.</span><span class="sxs-lookup"><span data-stu-id="d872c-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="d872c-167">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="d872c-167">Required.</span></span> |
| <span data-ttu-id="d872c-168">type</span><span class="sxs-lookup"><span data-stu-id="d872c-168">type</span></span>             | <span data-ttu-id="d872c-169">String</span><span class="sxs-lookup"><span data-stu-id="d872c-169">String</span></span>                                                   | <span data-ttu-id="d872c-170">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="d872c-170">The request type.</span></span> <span data-ttu-id="d872c-171">Возможные значения: `AdminAdd`, `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `AdminRenew` `AdminExtend`,,,,, и. `UserExtend` `UserRenew`</span><span class="sxs-lookup"><span data-stu-id="d872c-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="d872c-172">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="d872c-172">Required.</span></span> |
| <span data-ttu-id="d872c-173">причиной</span><span class="sxs-lookup"><span data-stu-id="d872c-173">reason</span></span>           | <span data-ttu-id="d872c-174">String</span><span class="sxs-lookup"><span data-stu-id="d872c-174">String</span></span>                                                   | <span data-ttu-id="d872c-175">Необходимо указать причину для запроса на назначение роли для аудита и проверки.</span><span class="sxs-lookup"><span data-stu-id="d872c-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="d872c-176">schedule</span><span class="sxs-lookup"><span data-stu-id="d872c-176">schedule</span></span>         | [<span data-ttu-id="d872c-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="d872c-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="d872c-178">Расписание запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="d872c-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="d872c-179">`UserAdd`Для типа запроса `AdminAdd`,, `AdminUpdate`, и `AdminExtend`, он необходим.</span><span class="sxs-lookup"><span data-stu-id="d872c-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="d872c-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="d872c-180">Response</span></span>

<span data-ttu-id="d872c-181">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d872c-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="d872c-182">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="d872c-182">Error codes</span></span>

<span data-ttu-id="d872c-183">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="d872c-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="d872c-184">Кроме того, он возвращает коды ошибок, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="d872c-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="d872c-185">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="d872c-185">Error code</span></span>     | <span data-ttu-id="d872c-186">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="d872c-186">Error message</span></span>                               | <span data-ttu-id="d872c-187">Сведения</span><span class="sxs-lookup"><span data-stu-id="d872c-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="d872c-188">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="d872c-188">400 BadRequest</span></span> | <span data-ttu-id="d872c-189">Роленотфаунд</span><span class="sxs-lookup"><span data-stu-id="d872c-189">RoleNotFound</span></span>                                | <span data-ttu-id="d872c-190">Не `roleDefinitionId` удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="d872c-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="d872c-191">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="d872c-191">400 BadRequest</span></span> | <span data-ttu-id="d872c-192">Ресаурцеислоккед</span><span class="sxs-lookup"><span data-stu-id="d872c-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="d872c-193">Ресурс, указанный в теле запроса, находится в состоянии `Locked` и не может создавать запросы на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="d872c-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="d872c-194">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="d872c-194">400 BadRequest</span></span> | <span data-ttu-id="d872c-195">Субжектнотфаунд</span><span class="sxs-lookup"><span data-stu-id="d872c-195">SubjectNotFound</span></span>                             | <span data-ttu-id="d872c-196">Не `subjectId` удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="d872c-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="d872c-197">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="d872c-197">400 BadRequest</span></span> | <span data-ttu-id="d872c-198">Пендингролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="d872c-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="d872c-199">В системе уже существует ожидающий [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="d872c-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="d872c-200">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="d872c-200">400 BadRequest</span></span> | <span data-ttu-id="d872c-201">Ролеассигнментексистс</span><span class="sxs-lookup"><span data-stu-id="d872c-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="d872c-202">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , который требуется создать, уже существует в системе.</span><span class="sxs-lookup"><span data-stu-id="d872c-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="d872c-203">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="d872c-203">400 BadRequest</span></span> | <span data-ttu-id="d872c-204">Ролеассигнментдоеснотексист</span><span class="sxs-lookup"><span data-stu-id="d872c-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="d872c-205">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , запрошенный для обновления или расширения, не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="d872c-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="d872c-206">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="d872c-206">400 BadRequest</span></span> | <span data-ttu-id="d872c-207">Ролеассигнментрекуестполицивалидатионфаилед</span><span class="sxs-lookup"><span data-stu-id="d872c-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="d872c-208">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) не отвечает внутренним политикам и не может быть создан.</span><span class="sxs-lookup"><span data-stu-id="d872c-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="d872c-209">Примеры</span><span class="sxs-lookup"><span data-stu-id="d872c-209">Examples</span></span>

<span data-ttu-id="d872c-210">В следующих примерах показано, как использовать этот API.</span><span class="sxs-lookup"><span data-stu-id="d872c-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="d872c-211">Пример 1: Администратор назначает пользователю роль</span><span class="sxs-lookup"><span data-stu-id="d872c-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="d872c-212">В этом примере администратор назначает пользователю nawu@fimdev.net роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="d872c-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="d872c-213">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="d872c-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="d872c-214">Свойство</span><span class="sxs-lookup"><span data-stu-id="d872c-214">Property</span></span>         | <span data-ttu-id="d872c-215">Тип</span><span class="sxs-lookup"><span data-stu-id="d872c-215">Type</span></span>                                                     | <span data-ttu-id="d872c-216">Обязательный</span><span class="sxs-lookup"><span data-stu-id="d872c-216">Required</span></span>                 | <span data-ttu-id="d872c-217">Значение</span><span class="sxs-lookup"><span data-stu-id="d872c-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="d872c-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="d872c-218">resourceId</span></span>       | <span data-ttu-id="d872c-219">String</span><span class="sxs-lookup"><span data-stu-id="d872c-219">String</span></span>                                                   | <span data-ttu-id="d872c-220">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-220">Yes</span></span>                      | <span data-ttu-id="d872c-221">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="d872c-221">\<resourceId\></span></span> |
| <span data-ttu-id="d872c-222">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="d872c-222">roleDefinitionId</span></span> | <span data-ttu-id="d872c-223">String</span><span class="sxs-lookup"><span data-stu-id="d872c-223">String</span></span>                                                   | <span data-ttu-id="d872c-224">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-224">Yes</span></span>                      | <span data-ttu-id="d872c-225">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="d872c-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="d872c-226">Субжектид</span><span class="sxs-lookup"><span data-stu-id="d872c-226">subjectId</span></span>        | <span data-ttu-id="d872c-227">String</span><span class="sxs-lookup"><span data-stu-id="d872c-227">String</span></span>                                                   | <span data-ttu-id="d872c-228">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-228">Yes</span></span>                      | <span data-ttu-id="d872c-229">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="d872c-229">\<subjectId\></span></span> |
| <span data-ttu-id="d872c-230">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="d872c-230">assignmentState</span></span>  | <span data-ttu-id="d872c-231">String</span><span class="sxs-lookup"><span data-stu-id="d872c-231">String</span></span>                                                   | <span data-ttu-id="d872c-232">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-232">Yes</span></span>                      | <span data-ttu-id="d872c-233">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="d872c-233">Eligible / Active</span></span> |
| <span data-ttu-id="d872c-234">type</span><span class="sxs-lookup"><span data-stu-id="d872c-234">type</span></span>             | <span data-ttu-id="d872c-235">String</span><span class="sxs-lookup"><span data-stu-id="d872c-235">String</span></span>                                                   | <span data-ttu-id="d872c-236">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-236">Yes</span></span>                      | <span data-ttu-id="d872c-237">Админадд</span><span class="sxs-lookup"><span data-stu-id="d872c-237">AdminAdd</span></span> |
| <span data-ttu-id="d872c-238">причиной</span><span class="sxs-lookup"><span data-stu-id="d872c-238">reason</span></span>           | <span data-ttu-id="d872c-239">String</span><span class="sxs-lookup"><span data-stu-id="d872c-239">String</span></span>                                                   | <span data-ttu-id="d872c-240">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="d872c-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="d872c-241">schedule</span><span class="sxs-lookup"><span data-stu-id="d872c-241">schedule</span></span>         | [<span data-ttu-id="d872c-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="d872c-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="d872c-243">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="d872c-244">Запрос</span><span class="sxs-lookup"><span data-stu-id="d872c-244">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d872c-245">HTTP</span><span class="sxs-lookup"><span data-stu-id="d872c-245">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d872c-246">C#</span><span class="sxs-lookup"><span data-stu-id="d872c-246">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d872c-247">Javascript</span><span class="sxs-lookup"><span data-stu-id="d872c-247">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d872c-248">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d872c-248">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="d872c-249">Отклик</span><span class="sxs-lookup"><span data-stu-id="d872c-249">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="d872c-250">Пример 2: пользователь активирует подходящие роли</span><span class="sxs-lookup"><span data-stu-id="d872c-250">Example 2: User activates eligible role</span></span>

<span data-ttu-id="d872c-251">В этом примере пользователь nawu@fimdev.net активирует соответствующую роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="d872c-251">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="d872c-252">Свойство</span><span class="sxs-lookup"><span data-stu-id="d872c-252">Property</span></span>         | <span data-ttu-id="d872c-253">Тип</span><span class="sxs-lookup"><span data-stu-id="d872c-253">Type</span></span>                                                     | <span data-ttu-id="d872c-254">Обязательный</span><span class="sxs-lookup"><span data-stu-id="d872c-254">Required</span></span>                 | <span data-ttu-id="d872c-255">Значение</span><span class="sxs-lookup"><span data-stu-id="d872c-255">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="d872c-256">resourceId</span><span class="sxs-lookup"><span data-stu-id="d872c-256">resourceId</span></span>       | <span data-ttu-id="d872c-257">String</span><span class="sxs-lookup"><span data-stu-id="d872c-257">String</span></span>                                                   | <span data-ttu-id="d872c-258">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-258">Yes</span></span>                      | <span data-ttu-id="d872c-259">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="d872c-259">\<resourceId\></span></span> |
| <span data-ttu-id="d872c-260">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="d872c-260">roleDefinitionId</span></span> | <span data-ttu-id="d872c-261">String</span><span class="sxs-lookup"><span data-stu-id="d872c-261">String</span></span>                                                   | <span data-ttu-id="d872c-262">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-262">Yes</span></span>                      | <span data-ttu-id="d872c-263">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="d872c-263">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="d872c-264">Субжектид</span><span class="sxs-lookup"><span data-stu-id="d872c-264">subjectId</span></span>        | <span data-ttu-id="d872c-265">String</span><span class="sxs-lookup"><span data-stu-id="d872c-265">String</span></span>                                                   | <span data-ttu-id="d872c-266">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-266">Yes</span></span>                      | <span data-ttu-id="d872c-267">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="d872c-267">\<subjectId\></span></span> |
| <span data-ttu-id="d872c-268">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="d872c-268">assignmentState</span></span>  | <span data-ttu-id="d872c-269">String</span><span class="sxs-lookup"><span data-stu-id="d872c-269">String</span></span>                                                   | <span data-ttu-id="d872c-270">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-270">Yes</span></span>                      | <span data-ttu-id="d872c-271">Активное</span><span class="sxs-lookup"><span data-stu-id="d872c-271">Active</span></span> |
| <span data-ttu-id="d872c-272">type</span><span class="sxs-lookup"><span data-stu-id="d872c-272">type</span></span>             | <span data-ttu-id="d872c-273">String</span><span class="sxs-lookup"><span data-stu-id="d872c-273">String</span></span>                                                   | <span data-ttu-id="d872c-274">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-274">Yes</span></span>                      | <span data-ttu-id="d872c-275">Усерадд</span><span class="sxs-lookup"><span data-stu-id="d872c-275">UserAdd</span></span> |
| <span data-ttu-id="d872c-276">причиной</span><span class="sxs-lookup"><span data-stu-id="d872c-276">reason</span></span>           | <span data-ttu-id="d872c-277">String</span><span class="sxs-lookup"><span data-stu-id="d872c-277">String</span></span>                                                   | <span data-ttu-id="d872c-278">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="d872c-278">depends on role Settings</span></span> |   |
| <span data-ttu-id="d872c-279">schedule</span><span class="sxs-lookup"><span data-stu-id="d872c-279">schedule</span></span>         | [<span data-ttu-id="d872c-280">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="d872c-280">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="d872c-281">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-281">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="d872c-282">Запрос</span><span class="sxs-lookup"><span data-stu-id="d872c-282">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="d872c-283">Отклик</span><span class="sxs-lookup"><span data-stu-id="d872c-283">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="d872c-284">Пример 3: пользователь отключает назначенную роль</span><span class="sxs-lookup"><span data-stu-id="d872c-284">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="d872c-285">В этом примере пользователь nawu@fimdev.net отключает активную роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="d872c-285">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="d872c-286">Свойство</span><span class="sxs-lookup"><span data-stu-id="d872c-286">Property</span></span>         | <span data-ttu-id="d872c-287">Тип</span><span class="sxs-lookup"><span data-stu-id="d872c-287">Type</span></span>                                                     | <span data-ttu-id="d872c-288">Обязательный</span><span class="sxs-lookup"><span data-stu-id="d872c-288">Required</span></span> | <span data-ttu-id="d872c-289">Значение</span><span class="sxs-lookup"><span data-stu-id="d872c-289">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="d872c-290">resourceId</span><span class="sxs-lookup"><span data-stu-id="d872c-290">resourceId</span></span>       | <span data-ttu-id="d872c-291">String</span><span class="sxs-lookup"><span data-stu-id="d872c-291">String</span></span>                                                   | <span data-ttu-id="d872c-292">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-292">Yes</span></span>      | <span data-ttu-id="d872c-293">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="d872c-293">\<resourceId\></span></span> |
| <span data-ttu-id="d872c-294">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="d872c-294">roleDefinitionId</span></span> | <span data-ttu-id="d872c-295">String</span><span class="sxs-lookup"><span data-stu-id="d872c-295">String</span></span>                                                   | <span data-ttu-id="d872c-296">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-296">Yes</span></span>      | <span data-ttu-id="d872c-297">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="d872c-297">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="d872c-298">Субжектид</span><span class="sxs-lookup"><span data-stu-id="d872c-298">subjectId</span></span>        | <span data-ttu-id="d872c-299">String</span><span class="sxs-lookup"><span data-stu-id="d872c-299">String</span></span>                                                   | <span data-ttu-id="d872c-300">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-300">Yes</span></span>      | <span data-ttu-id="d872c-301">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="d872c-301">\<subjectId\></span></span> |
| <span data-ttu-id="d872c-302">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="d872c-302">assignmentState</span></span>  | <span data-ttu-id="d872c-303">Строка</span><span class="sxs-lookup"><span data-stu-id="d872c-303">String</span></span>                                                   | <span data-ttu-id="d872c-304">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-304">Yes</span></span>      | <span data-ttu-id="d872c-305">Активное</span><span class="sxs-lookup"><span data-stu-id="d872c-305">Active</span></span> |
| <span data-ttu-id="d872c-306">type</span><span class="sxs-lookup"><span data-stu-id="d872c-306">type</span></span>             | <span data-ttu-id="d872c-307">Строка</span><span class="sxs-lookup"><span data-stu-id="d872c-307">String</span></span>                                                   | <span data-ttu-id="d872c-308">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-308">Yes</span></span>      | <span data-ttu-id="d872c-309">Усерремове</span><span class="sxs-lookup"><span data-stu-id="d872c-309">UserRemove</span></span> |
| <span data-ttu-id="d872c-310">причиной</span><span class="sxs-lookup"><span data-stu-id="d872c-310">reason</span></span>           | <span data-ttu-id="d872c-311">String</span><span class="sxs-lookup"><span data-stu-id="d872c-311">String</span></span>                                                   | <span data-ttu-id="d872c-312">Нет</span><span class="sxs-lookup"><span data-stu-id="d872c-312">No</span></span>       |   |
| <span data-ttu-id="d872c-313">schedule</span><span class="sxs-lookup"><span data-stu-id="d872c-313">schedule</span></span>         | [<span data-ttu-id="d872c-314">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="d872c-314">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="d872c-315">Нет</span><span class="sxs-lookup"><span data-stu-id="d872c-315">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="d872c-316">Запрос</span><span class="sxs-lookup"><span data-stu-id="d872c-316">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="d872c-317">Отклик</span><span class="sxs-lookup"><span data-stu-id="d872c-317">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="d872c-318">Пример 4: Администратор удаляет пользователя из роли</span><span class="sxs-lookup"><span data-stu-id="d872c-318">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="d872c-319">В этом примере администратор удаляет пользователя nawu@fimdev.net из роли читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="d872c-319">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="d872c-320">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="d872c-320">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="d872c-321">Свойство</span><span class="sxs-lookup"><span data-stu-id="d872c-321">Property</span></span>         | <span data-ttu-id="d872c-322">Тип</span><span class="sxs-lookup"><span data-stu-id="d872c-322">Type</span></span>                                                     | <span data-ttu-id="d872c-323">Обязательный</span><span class="sxs-lookup"><span data-stu-id="d872c-323">Required</span></span> | <span data-ttu-id="d872c-324">Значение</span><span class="sxs-lookup"><span data-stu-id="d872c-324">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="d872c-325">resourceId</span><span class="sxs-lookup"><span data-stu-id="d872c-325">resourceId</span></span>       | <span data-ttu-id="d872c-326">String</span><span class="sxs-lookup"><span data-stu-id="d872c-326">String</span></span>                                                   | <span data-ttu-id="d872c-327">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-327">Yes</span></span>      | <span data-ttu-id="d872c-328">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="d872c-328">\<resourceId\></span></span> |
| <span data-ttu-id="d872c-329">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="d872c-329">roleDefinitionId</span></span> | <span data-ttu-id="d872c-330">Строка</span><span class="sxs-lookup"><span data-stu-id="d872c-330">String</span></span>                                                   | <span data-ttu-id="d872c-331">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-331">Yes</span></span>      | <span data-ttu-id="d872c-332">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="d872c-332">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="d872c-333">Субжектид</span><span class="sxs-lookup"><span data-stu-id="d872c-333">subjectId</span></span>        | <span data-ttu-id="d872c-334">Строка</span><span class="sxs-lookup"><span data-stu-id="d872c-334">String</span></span>                                                   | <span data-ttu-id="d872c-335">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-335">Yes</span></span>      | <span data-ttu-id="d872c-336">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="d872c-336">\<subjectId\></span></span> |
| <span data-ttu-id="d872c-337">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="d872c-337">assignmentState</span></span>  | <span data-ttu-id="d872c-338">Строка</span><span class="sxs-lookup"><span data-stu-id="d872c-338">String</span></span>                                                   | <span data-ttu-id="d872c-339">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-339">Yes</span></span>      | <span data-ttu-id="d872c-340">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="d872c-340">Eligible / Active</span></span> |
| <span data-ttu-id="d872c-341">type</span><span class="sxs-lookup"><span data-stu-id="d872c-341">type</span></span>             | <span data-ttu-id="d872c-342">Строка</span><span class="sxs-lookup"><span data-stu-id="d872c-342">String</span></span>                                                   | <span data-ttu-id="d872c-343">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-343">Yes</span></span>      | <span data-ttu-id="d872c-344">Админремове</span><span class="sxs-lookup"><span data-stu-id="d872c-344">AdminRemove</span></span> |
| <span data-ttu-id="d872c-345">причиной</span><span class="sxs-lookup"><span data-stu-id="d872c-345">reason</span></span>           | <span data-ttu-id="d872c-346">String</span><span class="sxs-lookup"><span data-stu-id="d872c-346">String</span></span>                                                   | <span data-ttu-id="d872c-347">Нет</span><span class="sxs-lookup"><span data-stu-id="d872c-347">No</span></span>       |   |
| <span data-ttu-id="d872c-348">schedule</span><span class="sxs-lookup"><span data-stu-id="d872c-348">schedule</span></span>         | [<span data-ttu-id="d872c-349">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="d872c-349">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="d872c-350">Нет</span><span class="sxs-lookup"><span data-stu-id="d872c-350">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="d872c-351">Запрос</span><span class="sxs-lookup"><span data-stu-id="d872c-351">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="d872c-352">Отклик</span><span class="sxs-lookup"><span data-stu-id="d872c-352">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="d872c-353">Пример 5: "Администратор обновляет назначение ролей"</span><span class="sxs-lookup"><span data-stu-id="d872c-353">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="d872c-354">В этом примере администраторы обновляют назначение роли пользователя nawu@fimdev.net владельцу.</span><span class="sxs-lookup"><span data-stu-id="d872c-354">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="d872c-355">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="d872c-355">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="d872c-356">Свойство</span><span class="sxs-lookup"><span data-stu-id="d872c-356">Property</span></span>         | <span data-ttu-id="d872c-357">Тип</span><span class="sxs-lookup"><span data-stu-id="d872c-357">Type</span></span>                                                     | <span data-ttu-id="d872c-358">Обязательный</span><span class="sxs-lookup"><span data-stu-id="d872c-358">Required</span></span>                | <span data-ttu-id="d872c-359">Значение</span><span class="sxs-lookup"><span data-stu-id="d872c-359">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="d872c-360">resourceId</span><span class="sxs-lookup"><span data-stu-id="d872c-360">resourceId</span></span>       | <span data-ttu-id="d872c-361">String</span><span class="sxs-lookup"><span data-stu-id="d872c-361">String</span></span>                                                   | <span data-ttu-id="d872c-362">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-362">Yes</span></span>                     | <span data-ttu-id="d872c-363">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="d872c-363">\<resourceId\></span></span> |
| <span data-ttu-id="d872c-364">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="d872c-364">roleDefinitionId</span></span> | <span data-ttu-id="d872c-365">Строка</span><span class="sxs-lookup"><span data-stu-id="d872c-365">String</span></span>                                                   | <span data-ttu-id="d872c-366">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-366">Yes</span></span>                     | <span data-ttu-id="d872c-367">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="d872c-367">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="d872c-368">Субжектид</span><span class="sxs-lookup"><span data-stu-id="d872c-368">subjectId</span></span>        | <span data-ttu-id="d872c-369">Строка</span><span class="sxs-lookup"><span data-stu-id="d872c-369">String</span></span>                                                   | <span data-ttu-id="d872c-370">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-370">Yes</span></span>                     | <span data-ttu-id="d872c-371">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="d872c-371">\<subjectId\></span></span> |
| <span data-ttu-id="d872c-372">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="d872c-372">assignmentState</span></span>  | <span data-ttu-id="d872c-373">Строка</span><span class="sxs-lookup"><span data-stu-id="d872c-373">String</span></span>                                                   | <span data-ttu-id="d872c-374">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-374">Yes</span></span>                     | <span data-ttu-id="d872c-375">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="d872c-375">Eligible / Active</span></span> |
| <span data-ttu-id="d872c-376">type</span><span class="sxs-lookup"><span data-stu-id="d872c-376">type</span></span>             | <span data-ttu-id="d872c-377">Строка</span><span class="sxs-lookup"><span data-stu-id="d872c-377">String</span></span>                                                   | <span data-ttu-id="d872c-378">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-378">Yes</span></span>                     | <span data-ttu-id="d872c-379">Админупдате</span><span class="sxs-lookup"><span data-stu-id="d872c-379">AdminUpdate</span></span> |
| <span data-ttu-id="d872c-380">причиной</span><span class="sxs-lookup"><span data-stu-id="d872c-380">reason</span></span>           | <span data-ttu-id="d872c-381">String</span><span class="sxs-lookup"><span data-stu-id="d872c-381">String</span></span>                                                   | <span data-ttu-id="d872c-382">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="d872c-382">depends on roleSettings</span></span> |   |
| <span data-ttu-id="d872c-383">schedule</span><span class="sxs-lookup"><span data-stu-id="d872c-383">schedule</span></span>         | [<span data-ttu-id="d872c-384">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="d872c-384">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="d872c-385">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-385">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="d872c-386">Запрос</span><span class="sxs-lookup"><span data-stu-id="d872c-386">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="d872c-387">Отклик</span><span class="sxs-lookup"><span data-stu-id="d872c-387">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="d872c-388">Пример 6: администратор расширяет назначение ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="d872c-388">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="d872c-389">В этом примере показано, как расширить назначение роли истечения срока действия для пользователя АНУЖКУСЕР участнику службы управления API.</span><span class="sxs-lookup"><span data-stu-id="d872c-389">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="d872c-390">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="d872c-390">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="d872c-391">Свойство</span><span class="sxs-lookup"><span data-stu-id="d872c-391">Property</span></span>         | <span data-ttu-id="d872c-392">Тип</span><span class="sxs-lookup"><span data-stu-id="d872c-392">Type</span></span>                                                     | <span data-ttu-id="d872c-393">Обязательный</span><span class="sxs-lookup"><span data-stu-id="d872c-393">Required</span></span>                | <span data-ttu-id="d872c-394">Значение</span><span class="sxs-lookup"><span data-stu-id="d872c-394">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="d872c-395">resourceId</span><span class="sxs-lookup"><span data-stu-id="d872c-395">resourceId</span></span>       | <span data-ttu-id="d872c-396">String</span><span class="sxs-lookup"><span data-stu-id="d872c-396">String</span></span>                                                   | <span data-ttu-id="d872c-397">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-397">Yes</span></span>                     | <span data-ttu-id="d872c-398">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="d872c-398">\<resourceId\></span></span> |
| <span data-ttu-id="d872c-399">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="d872c-399">roleDefinitionId</span></span> | <span data-ttu-id="d872c-400">Строка</span><span class="sxs-lookup"><span data-stu-id="d872c-400">String</span></span>                                                   | <span data-ttu-id="d872c-401">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-401">Yes</span></span>                     | <span data-ttu-id="d872c-402">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="d872c-402">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="d872c-403">Субжектид</span><span class="sxs-lookup"><span data-stu-id="d872c-403">subjectId</span></span>        | <span data-ttu-id="d872c-404">String</span><span class="sxs-lookup"><span data-stu-id="d872c-404">String</span></span>                                                   | <span data-ttu-id="d872c-405">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-405">Yes</span></span>                     | <span data-ttu-id="d872c-406">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="d872c-406">\<subjectId\></span></span> |
| <span data-ttu-id="d872c-407">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="d872c-407">assignmentState</span></span>  | <span data-ttu-id="d872c-408">String</span><span class="sxs-lookup"><span data-stu-id="d872c-408">String</span></span>                                                   | <span data-ttu-id="d872c-409">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-409">Yes</span></span>                     | <span data-ttu-id="d872c-410">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="d872c-410">Eligible / Active</span></span> |
| <span data-ttu-id="d872c-411">type</span><span class="sxs-lookup"><span data-stu-id="d872c-411">type</span></span>             | <span data-ttu-id="d872c-412">String</span><span class="sxs-lookup"><span data-stu-id="d872c-412">String</span></span>                                                   | <span data-ttu-id="d872c-413">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-413">Yes</span></span>                     | <span data-ttu-id="d872c-414">Админекстенд</span><span class="sxs-lookup"><span data-stu-id="d872c-414">AdminExtend</span></span> |
| <span data-ttu-id="d872c-415">причиной</span><span class="sxs-lookup"><span data-stu-id="d872c-415">reason</span></span>           | <span data-ttu-id="d872c-416">String</span><span class="sxs-lookup"><span data-stu-id="d872c-416">String</span></span>                                                   | <span data-ttu-id="d872c-417">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="d872c-417">depends on roleSettings</span></span> |   |
| <span data-ttu-id="d872c-418">schedule</span><span class="sxs-lookup"><span data-stu-id="d872c-418">schedule</span></span>         | [<span data-ttu-id="d872c-419">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="d872c-419">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="d872c-420">Да</span><span class="sxs-lookup"><span data-stu-id="d872c-420">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="d872c-421">Запрос</span><span class="sxs-lookup"><span data-stu-id="d872c-421">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="d872c-422">Отклик</span><span class="sxs-lookup"><span data-stu-id="d872c-422">Response</span></span>

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
  ]
}
-->
