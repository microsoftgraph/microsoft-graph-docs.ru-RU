---
title: Создание governanceRoleAssignmentRequest
description: Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли. В приведенной ниже таблице перечислены операции.
localization_priority: Normal
ms.openlocfilehash: 2765018430f4747815fc18428750cdfae4983765
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263541"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="b40c3-104">Создание governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="b40c3-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b40c3-105">Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="b40c3-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="b40c3-106">В приведенной ниже таблице перечислены операции.</span><span class="sxs-lookup"><span data-stu-id="b40c3-106">The following table lists the operations.</span></span>

| <span data-ttu-id="b40c3-107">Operation</span><span class="sxs-lookup"><span data-stu-id="b40c3-107">Operation</span></span>                                   | <span data-ttu-id="b40c3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b40c3-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="b40c3-109">Назначение роли</span><span class="sxs-lookup"><span data-stu-id="b40c3-109">Assign a role assignment</span></span>                    | <span data-ttu-id="b40c3-110">Админадд</span><span class="sxs-lookup"><span data-stu-id="b40c3-110">AdminAdd</span></span>    |
| <span data-ttu-id="b40c3-111">Активация подходящего назначения роли</span><span class="sxs-lookup"><span data-stu-id="b40c3-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="b40c3-112">Усерадд</span><span class="sxs-lookup"><span data-stu-id="b40c3-112">UserAdd</span></span>     |
| <span data-ttu-id="b40c3-113">Деактивация активированного назначения роли</span><span class="sxs-lookup"><span data-stu-id="b40c3-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="b40c3-114">Усерремове</span><span class="sxs-lookup"><span data-stu-id="b40c3-114">UserRemove</span></span>  |
| <span data-ttu-id="b40c3-115">Удаление назначения роли</span><span class="sxs-lookup"><span data-stu-id="b40c3-115">Remove a role assignment</span></span>                    | <span data-ttu-id="b40c3-116">Админремове</span><span class="sxs-lookup"><span data-stu-id="b40c3-116">AdminRemove</span></span> |
| <span data-ttu-id="b40c3-117">Обновление назначения роли</span><span class="sxs-lookup"><span data-stu-id="b40c3-117">Update a role assignment</span></span>                    | <span data-ttu-id="b40c3-118">Админупдате</span><span class="sxs-lookup"><span data-stu-id="b40c3-118">AdminUpdate</span></span> |
| <span data-ttu-id="b40c3-119">Запрос на расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="b40c3-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="b40c3-120">Усерекстенд</span><span class="sxs-lookup"><span data-stu-id="b40c3-120">UserExtend</span></span>  |
| <span data-ttu-id="b40c3-121">Расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="b40c3-121">Extend a role assignment</span></span>                    | <span data-ttu-id="b40c3-122">Админекстенд</span><span class="sxs-lookup"><span data-stu-id="b40c3-122">AdminExtend</span></span> |
| <span data-ttu-id="b40c3-123">Запрос на продление назначения роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="b40c3-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="b40c3-124">Усерренев</span><span class="sxs-lookup"><span data-stu-id="b40c3-124">UserRenew</span></span>   |
| <span data-ttu-id="b40c3-125">Продление назначенной роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="b40c3-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="b40c3-126">Админренев</span><span class="sxs-lookup"><span data-stu-id="b40c3-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="b40c3-127">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b40c3-127">Permissions</span></span>

<span data-ttu-id="b40c3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b40c3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b40c3-130">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b40c3-130">Permission type</span></span>                        | <span data-ttu-id="b40c3-131">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b40c3-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="b40c3-132">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b40c3-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="b40c3-133">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="b40c3-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="b40c3-134">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b40c3-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b40c3-135">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b40c3-135">Not supported.</span></span>                            |
| <span data-ttu-id="b40c3-136">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b40c3-136">Application</span></span>                            | <span data-ttu-id="b40c3-137">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b40c3-137">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b40c3-138">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b40c3-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="b40c3-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b40c3-139">Request headers</span></span>

| <span data-ttu-id="b40c3-140">Имя</span><span class="sxs-lookup"><span data-stu-id="b40c3-140">Name</span></span>          | <span data-ttu-id="b40c3-141">Описание</span><span class="sxs-lookup"><span data-stu-id="b40c3-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="b40c3-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b40c3-142">Authorization</span></span> | <span data-ttu-id="b40c3-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b40c3-143">Bearer {code}</span></span>    |
| <span data-ttu-id="b40c3-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b40c3-144">Content-type</span></span>  | <span data-ttu-id="b40c3-145">application/json</span><span class="sxs-lookup"><span data-stu-id="b40c3-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b40c3-146">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b40c3-146">Request body</span></span>

<span data-ttu-id="b40c3-147">В тексте запроса добавьте представление объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b40c3-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="b40c3-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="b40c3-148">Property</span></span>         | <span data-ttu-id="b40c3-149">Тип</span><span class="sxs-lookup"><span data-stu-id="b40c3-149">Type</span></span>                                                     | <span data-ttu-id="b40c3-150">Описание</span><span class="sxs-lookup"><span data-stu-id="b40c3-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="b40c3-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="b40c3-151">resourceId</span></span>       | <span data-ttu-id="b40c3-152">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-152">String</span></span>                                                   | <span data-ttu-id="b40c3-153">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="b40c3-153">The ID of the resource.</span></span> <span data-ttu-id="b40c3-154">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="b40c3-154">Required.</span></span> |
| <span data-ttu-id="b40c3-155">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="b40c3-155">roleDefinitionId</span></span> | <span data-ttu-id="b40c3-156">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-156">String</span></span>                                                   | <span data-ttu-id="b40c3-157">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="b40c3-157">The ID of the role definition.</span></span> <span data-ttu-id="b40c3-158">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="b40c3-158">Required.</span></span> |
| <span data-ttu-id="b40c3-159">Субжектид</span><span class="sxs-lookup"><span data-stu-id="b40c3-159">subjectId</span></span>        | <span data-ttu-id="b40c3-160">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-160">String</span></span>                                                   | <span data-ttu-id="b40c3-161">ИДЕНТИФИКАТОР субъекта.</span><span class="sxs-lookup"><span data-stu-id="b40c3-161">The ID of the subject.</span></span> <span data-ttu-id="b40c3-162">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="b40c3-162">Required.</span></span> |
| <span data-ttu-id="b40c3-163">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="b40c3-163">assignmentState</span></span>  | <span data-ttu-id="b40c3-164">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-164">String</span></span>                                                   | <span data-ttu-id="b40c3-165">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="b40c3-165">The state of assignment.</span></span> <span data-ttu-id="b40c3-166">Значение может быть `Eligible` и `Active`.</span><span class="sxs-lookup"><span data-stu-id="b40c3-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="b40c3-167">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="b40c3-167">Required.</span></span> |
| <span data-ttu-id="b40c3-168">type</span><span class="sxs-lookup"><span data-stu-id="b40c3-168">type</span></span>             | <span data-ttu-id="b40c3-169">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-169">String</span></span>                                                   | <span data-ttu-id="b40c3-170">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="b40c3-170">The request type.</span></span> <span data-ttu-id="b40c3-171">Возможные значения: `AdminAdd`, `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `AdminRenew` `AdminExtend`,,,,, и. `UserExtend` `UserRenew`</span><span class="sxs-lookup"><span data-stu-id="b40c3-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="b40c3-172">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="b40c3-172">Required.</span></span> |
| <span data-ttu-id="b40c3-173">причиной</span><span class="sxs-lookup"><span data-stu-id="b40c3-173">reason</span></span>           | <span data-ttu-id="b40c3-174">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-174">String</span></span>                                                   | <span data-ttu-id="b40c3-175">Необходимо указать причину для запроса на назначение роли для аудита и проверки.</span><span class="sxs-lookup"><span data-stu-id="b40c3-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="b40c3-176">schedule</span><span class="sxs-lookup"><span data-stu-id="b40c3-176">schedule</span></span>         | [<span data-ttu-id="b40c3-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="b40c3-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="b40c3-178">Расписание запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="b40c3-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="b40c3-179">`UserAdd`Для типа запроса `AdminAdd`,, `AdminUpdate`, и `AdminExtend`, он необходим.</span><span class="sxs-lookup"><span data-stu-id="b40c3-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="b40c3-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="b40c3-180">Response</span></span>

<span data-ttu-id="b40c3-181">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b40c3-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="b40c3-182">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="b40c3-182">Error codes</span></span>

<span data-ttu-id="b40c3-183">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="b40c3-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="b40c3-184">Кроме того, он возвращает коды ошибок, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="b40c3-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="b40c3-185">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="b40c3-185">Error code</span></span>     | <span data-ttu-id="b40c3-186">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="b40c3-186">Error message</span></span>                               | <span data-ttu-id="b40c3-187">Сведения</span><span class="sxs-lookup"><span data-stu-id="b40c3-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="b40c3-188">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="b40c3-188">400 BadRequest</span></span> | <span data-ttu-id="b40c3-189">Роленотфаунд</span><span class="sxs-lookup"><span data-stu-id="b40c3-189">RoleNotFound</span></span>                                | <span data-ttu-id="b40c3-190">Не `roleDefinitionId` удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="b40c3-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="b40c3-191">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="b40c3-191">400 BadRequest</span></span> | <span data-ttu-id="b40c3-192">Ресаурцеислоккед</span><span class="sxs-lookup"><span data-stu-id="b40c3-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="b40c3-193">Ресурс, указанный в теле запроса, находится в состоянии `Locked` и не может создавать запросы на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="b40c3-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="b40c3-194">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="b40c3-194">400 BadRequest</span></span> | <span data-ttu-id="b40c3-195">Субжектнотфаунд</span><span class="sxs-lookup"><span data-stu-id="b40c3-195">SubjectNotFound</span></span>                             | <span data-ttu-id="b40c3-196">Не `subjectId` удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="b40c3-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="b40c3-197">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="b40c3-197">400 BadRequest</span></span> | <span data-ttu-id="b40c3-198">Пендингролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="b40c3-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="b40c3-199">В системе уже существует ожидающий [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="b40c3-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="b40c3-200">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="b40c3-200">400 BadRequest</span></span> | <span data-ttu-id="b40c3-201">Ролеассигнментексистс</span><span class="sxs-lookup"><span data-stu-id="b40c3-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="b40c3-202">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , который требуется создать, уже существует в системе.</span><span class="sxs-lookup"><span data-stu-id="b40c3-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="b40c3-203">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="b40c3-203">400 BadRequest</span></span> | <span data-ttu-id="b40c3-204">Ролеассигнментдоеснотексист</span><span class="sxs-lookup"><span data-stu-id="b40c3-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="b40c3-205">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , запрошенный для обновления или расширения, не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="b40c3-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="b40c3-206">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="b40c3-206">400 BadRequest</span></span> | <span data-ttu-id="b40c3-207">Ролеассигнментрекуестполицивалидатионфаилед</span><span class="sxs-lookup"><span data-stu-id="b40c3-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="b40c3-208">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) не отвечает внутренним политикам и не может быть создан.</span><span class="sxs-lookup"><span data-stu-id="b40c3-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="b40c3-209">Примеры</span><span class="sxs-lookup"><span data-stu-id="b40c3-209">Examples</span></span>

<span data-ttu-id="b40c3-210">В следующих примерах показано, как использовать этот API.</span><span class="sxs-lookup"><span data-stu-id="b40c3-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="b40c3-211">Пример 1: Администратор назначает пользователю роль</span><span class="sxs-lookup"><span data-stu-id="b40c3-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="b40c3-212">В этом примере администратор назначает пользователю nawu@fimdev.net роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="b40c3-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="b40c3-213">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="b40c3-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="b40c3-214">Свойство</span><span class="sxs-lookup"><span data-stu-id="b40c3-214">Property</span></span>         | <span data-ttu-id="b40c3-215">Тип</span><span class="sxs-lookup"><span data-stu-id="b40c3-215">Type</span></span>                                                     | <span data-ttu-id="b40c3-216">Обязательный</span><span class="sxs-lookup"><span data-stu-id="b40c3-216">Required</span></span>                 | <span data-ttu-id="b40c3-217">Значение</span><span class="sxs-lookup"><span data-stu-id="b40c3-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="b40c3-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="b40c3-218">resourceId</span></span>       | <span data-ttu-id="b40c3-219">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-219">String</span></span>                                                   | <span data-ttu-id="b40c3-220">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-220">Yes</span></span>                      | <span data-ttu-id="b40c3-221">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="b40c3-221">\<resourceId\></span></span> |
| <span data-ttu-id="b40c3-222">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="b40c3-222">roleDefinitionId</span></span> | <span data-ttu-id="b40c3-223">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-223">String</span></span>                                                   | <span data-ttu-id="b40c3-224">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-224">Yes</span></span>                      | <span data-ttu-id="b40c3-225">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="b40c3-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="b40c3-226">Субжектид</span><span class="sxs-lookup"><span data-stu-id="b40c3-226">subjectId</span></span>        | <span data-ttu-id="b40c3-227">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-227">String</span></span>                                                   | <span data-ttu-id="b40c3-228">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-228">Yes</span></span>                      | <span data-ttu-id="b40c3-229">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="b40c3-229">\<subjectId\></span></span> |
| <span data-ttu-id="b40c3-230">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="b40c3-230">assignmentState</span></span>  | <span data-ttu-id="b40c3-231">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-231">String</span></span>                                                   | <span data-ttu-id="b40c3-232">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-232">Yes</span></span>                      | <span data-ttu-id="b40c3-233">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="b40c3-233">Eligible / Active</span></span> |
| <span data-ttu-id="b40c3-234">type</span><span class="sxs-lookup"><span data-stu-id="b40c3-234">type</span></span>             | <span data-ttu-id="b40c3-235">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-235">String</span></span>                                                   | <span data-ttu-id="b40c3-236">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-236">Yes</span></span>                      | <span data-ttu-id="b40c3-237">Админадд</span><span class="sxs-lookup"><span data-stu-id="b40c3-237">AdminAdd</span></span> |
| <span data-ttu-id="b40c3-238">причиной</span><span class="sxs-lookup"><span data-stu-id="b40c3-238">reason</span></span>           | <span data-ttu-id="b40c3-239">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-239">String</span></span>                                                   | <span data-ttu-id="b40c3-240">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="b40c3-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="b40c3-241">schedule</span><span class="sxs-lookup"><span data-stu-id="b40c3-241">schedule</span></span>         | [<span data-ttu-id="b40c3-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="b40c3-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="b40c3-243">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="b40c3-244">Запрос</span><span class="sxs-lookup"><span data-stu-id="b40c3-244">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="b40c3-245">Отклик</span><span class="sxs-lookup"><span data-stu-id="b40c3-245">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b40c3-246">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="b40c3-246">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b40c3-247">C#</span><span class="sxs-lookup"><span data-stu-id="b40c3-247">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/governanceroleassignmentrequest_post-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b40c3-248">Javascript</span><span class="sxs-lookup"><span data-stu-id="b40c3-248">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/governanceroleassignmentrequest_post-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b40c3-249">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b40c3-249">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/governanceroleassignmentrequest_post-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="b40c3-250">Пример 2: пользователь активирует подходящие роли</span><span class="sxs-lookup"><span data-stu-id="b40c3-250">Example 2: User activates eligible role</span></span>

<span data-ttu-id="b40c3-251">В этом примере пользователь nawu@fimdev.net активирует соответствующую роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="b40c3-251">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="b40c3-252">Свойство</span><span class="sxs-lookup"><span data-stu-id="b40c3-252">Property</span></span>         | <span data-ttu-id="b40c3-253">Тип</span><span class="sxs-lookup"><span data-stu-id="b40c3-253">Type</span></span>                                                     | <span data-ttu-id="b40c3-254">Обязательный</span><span class="sxs-lookup"><span data-stu-id="b40c3-254">Required</span></span>                 | <span data-ttu-id="b40c3-255">Значение</span><span class="sxs-lookup"><span data-stu-id="b40c3-255">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="b40c3-256">resourceId</span><span class="sxs-lookup"><span data-stu-id="b40c3-256">resourceId</span></span>       | <span data-ttu-id="b40c3-257">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-257">String</span></span>                                                   | <span data-ttu-id="b40c3-258">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-258">Yes</span></span>                      | <span data-ttu-id="b40c3-259">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="b40c3-259">\<resourceId\></span></span> |
| <span data-ttu-id="b40c3-260">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="b40c3-260">roleDefinitionId</span></span> | <span data-ttu-id="b40c3-261">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-261">String</span></span>                                                   | <span data-ttu-id="b40c3-262">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-262">Yes</span></span>                      | <span data-ttu-id="b40c3-263">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="b40c3-263">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="b40c3-264">Субжектид</span><span class="sxs-lookup"><span data-stu-id="b40c3-264">subjectId</span></span>        | <span data-ttu-id="b40c3-265">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-265">String</span></span>                                                   | <span data-ttu-id="b40c3-266">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-266">Yes</span></span>                      | <span data-ttu-id="b40c3-267">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="b40c3-267">\<subjectId\></span></span> |
| <span data-ttu-id="b40c3-268">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="b40c3-268">assignmentState</span></span>  | <span data-ttu-id="b40c3-269">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-269">String</span></span>                                                   | <span data-ttu-id="b40c3-270">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-270">Yes</span></span>                      | <span data-ttu-id="b40c3-271">Активное</span><span class="sxs-lookup"><span data-stu-id="b40c3-271">Active</span></span> |
| <span data-ttu-id="b40c3-272">type</span><span class="sxs-lookup"><span data-stu-id="b40c3-272">type</span></span>             | <span data-ttu-id="b40c3-273">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-273">String</span></span>                                                   | <span data-ttu-id="b40c3-274">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-274">Yes</span></span>                      | <span data-ttu-id="b40c3-275">Усерадд</span><span class="sxs-lookup"><span data-stu-id="b40c3-275">UserAdd</span></span> |
| <span data-ttu-id="b40c3-276">причиной</span><span class="sxs-lookup"><span data-stu-id="b40c3-276">reason</span></span>           | <span data-ttu-id="b40c3-277">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-277">String</span></span>                                                   | <span data-ttu-id="b40c3-278">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="b40c3-278">depends on role Settings</span></span> |   |
| <span data-ttu-id="b40c3-279">schedule</span><span class="sxs-lookup"><span data-stu-id="b40c3-279">schedule</span></span>         | [<span data-ttu-id="b40c3-280">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="b40c3-280">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="b40c3-281">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-281">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="b40c3-282">Запрос</span><span class="sxs-lookup"><span data-stu-id="b40c3-282">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="b40c3-283">Отклик</span><span class="sxs-lookup"><span data-stu-id="b40c3-283">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="b40c3-284">Пример 3: пользователь отключает назначенную роль</span><span class="sxs-lookup"><span data-stu-id="b40c3-284">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="b40c3-285">В этом примере пользователь nawu@fimdev.net отключает активную роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="b40c3-285">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="b40c3-286">Свойство</span><span class="sxs-lookup"><span data-stu-id="b40c3-286">Property</span></span>         | <span data-ttu-id="b40c3-287">Тип</span><span class="sxs-lookup"><span data-stu-id="b40c3-287">Type</span></span>                                                     | <span data-ttu-id="b40c3-288">Обязательный</span><span class="sxs-lookup"><span data-stu-id="b40c3-288">Required</span></span> | <span data-ttu-id="b40c3-289">Значение</span><span class="sxs-lookup"><span data-stu-id="b40c3-289">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="b40c3-290">resourceId</span><span class="sxs-lookup"><span data-stu-id="b40c3-290">resourceId</span></span>       | <span data-ttu-id="b40c3-291">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-291">String</span></span>                                                   | <span data-ttu-id="b40c3-292">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-292">Yes</span></span>      | <span data-ttu-id="b40c3-293">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="b40c3-293">\<resourceId\></span></span> |
| <span data-ttu-id="b40c3-294">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="b40c3-294">roleDefinitionId</span></span> | <span data-ttu-id="b40c3-295">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-295">String</span></span>                                                   | <span data-ttu-id="b40c3-296">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-296">Yes</span></span>      | <span data-ttu-id="b40c3-297">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="b40c3-297">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="b40c3-298">Субжектид</span><span class="sxs-lookup"><span data-stu-id="b40c3-298">subjectId</span></span>        | <span data-ttu-id="b40c3-299">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-299">String</span></span>                                                   | <span data-ttu-id="b40c3-300">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-300">Yes</span></span>      | <span data-ttu-id="b40c3-301">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="b40c3-301">\<subjectId\></span></span> |
| <span data-ttu-id="b40c3-302">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="b40c3-302">assignmentState</span></span>  | <span data-ttu-id="b40c3-303">Строка</span><span class="sxs-lookup"><span data-stu-id="b40c3-303">String</span></span>                                                   | <span data-ttu-id="b40c3-304">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-304">Yes</span></span>      | <span data-ttu-id="b40c3-305">Активное</span><span class="sxs-lookup"><span data-stu-id="b40c3-305">Active</span></span> |
| <span data-ttu-id="b40c3-306">type</span><span class="sxs-lookup"><span data-stu-id="b40c3-306">type</span></span>             | <span data-ttu-id="b40c3-307">Строка</span><span class="sxs-lookup"><span data-stu-id="b40c3-307">String</span></span>                                                   | <span data-ttu-id="b40c3-308">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-308">Yes</span></span>      | <span data-ttu-id="b40c3-309">Усерремове</span><span class="sxs-lookup"><span data-stu-id="b40c3-309">UserRemove</span></span> |
| <span data-ttu-id="b40c3-310">причиной</span><span class="sxs-lookup"><span data-stu-id="b40c3-310">reason</span></span>           | <span data-ttu-id="b40c3-311">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-311">String</span></span>                                                   | <span data-ttu-id="b40c3-312">Нет</span><span class="sxs-lookup"><span data-stu-id="b40c3-312">No</span></span>       |   |
| <span data-ttu-id="b40c3-313">schedule</span><span class="sxs-lookup"><span data-stu-id="b40c3-313">schedule</span></span>         | [<span data-ttu-id="b40c3-314">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="b40c3-314">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="b40c3-315">Нет</span><span class="sxs-lookup"><span data-stu-id="b40c3-315">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="b40c3-316">Запрос</span><span class="sxs-lookup"><span data-stu-id="b40c3-316">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="b40c3-317">Отклик</span><span class="sxs-lookup"><span data-stu-id="b40c3-317">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="b40c3-318">Пример 4: Администратор удаляет пользователя из роли</span><span class="sxs-lookup"><span data-stu-id="b40c3-318">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="b40c3-319">В этом примере администратор удаляет пользователя nawu@fimdev.net из роли читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="b40c3-319">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="b40c3-320">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="b40c3-320">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="b40c3-321">Свойство</span><span class="sxs-lookup"><span data-stu-id="b40c3-321">Property</span></span>         | <span data-ttu-id="b40c3-322">Тип</span><span class="sxs-lookup"><span data-stu-id="b40c3-322">Type</span></span>                                                     | <span data-ttu-id="b40c3-323">Обязательный</span><span class="sxs-lookup"><span data-stu-id="b40c3-323">Required</span></span> | <span data-ttu-id="b40c3-324">Значение</span><span class="sxs-lookup"><span data-stu-id="b40c3-324">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="b40c3-325">resourceId</span><span class="sxs-lookup"><span data-stu-id="b40c3-325">resourceId</span></span>       | <span data-ttu-id="b40c3-326">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-326">String</span></span>                                                   | <span data-ttu-id="b40c3-327">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-327">Yes</span></span>      | <span data-ttu-id="b40c3-328">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="b40c3-328">\<resourceId\></span></span> |
| <span data-ttu-id="b40c3-329">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="b40c3-329">roleDefinitionId</span></span> | <span data-ttu-id="b40c3-330">Строка</span><span class="sxs-lookup"><span data-stu-id="b40c3-330">String</span></span>                                                   | <span data-ttu-id="b40c3-331">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-331">Yes</span></span>      | <span data-ttu-id="b40c3-332">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="b40c3-332">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="b40c3-333">Субжектид</span><span class="sxs-lookup"><span data-stu-id="b40c3-333">subjectId</span></span>        | <span data-ttu-id="b40c3-334">Строка</span><span class="sxs-lookup"><span data-stu-id="b40c3-334">String</span></span>                                                   | <span data-ttu-id="b40c3-335">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-335">Yes</span></span>      | <span data-ttu-id="b40c3-336">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="b40c3-336">\<subjectId\></span></span> |
| <span data-ttu-id="b40c3-337">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="b40c3-337">assignmentState</span></span>  | <span data-ttu-id="b40c3-338">Строка</span><span class="sxs-lookup"><span data-stu-id="b40c3-338">String</span></span>                                                   | <span data-ttu-id="b40c3-339">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-339">Yes</span></span>      | <span data-ttu-id="b40c3-340">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="b40c3-340">Eligible / Active</span></span> |
| <span data-ttu-id="b40c3-341">type</span><span class="sxs-lookup"><span data-stu-id="b40c3-341">type</span></span>             | <span data-ttu-id="b40c3-342">Строка</span><span class="sxs-lookup"><span data-stu-id="b40c3-342">String</span></span>                                                   | <span data-ttu-id="b40c3-343">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-343">Yes</span></span>      | <span data-ttu-id="b40c3-344">Админремове</span><span class="sxs-lookup"><span data-stu-id="b40c3-344">AdminRemove</span></span> |
| <span data-ttu-id="b40c3-345">причиной</span><span class="sxs-lookup"><span data-stu-id="b40c3-345">reason</span></span>           | <span data-ttu-id="b40c3-346">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-346">String</span></span>                                                   | <span data-ttu-id="b40c3-347">Нет</span><span class="sxs-lookup"><span data-stu-id="b40c3-347">No</span></span>       |   |
| <span data-ttu-id="b40c3-348">schedule</span><span class="sxs-lookup"><span data-stu-id="b40c3-348">schedule</span></span>         | [<span data-ttu-id="b40c3-349">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="b40c3-349">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="b40c3-350">Нет</span><span class="sxs-lookup"><span data-stu-id="b40c3-350">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="b40c3-351">Запрос</span><span class="sxs-lookup"><span data-stu-id="b40c3-351">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="b40c3-352">Отклик</span><span class="sxs-lookup"><span data-stu-id="b40c3-352">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="b40c3-353">Пример 5: "Администратор обновляет назначение ролей"</span><span class="sxs-lookup"><span data-stu-id="b40c3-353">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="b40c3-354">В этом примере администраторы обновляют назначение роли пользователя nawu@fimdev.net владельцу.</span><span class="sxs-lookup"><span data-stu-id="b40c3-354">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="b40c3-355">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="b40c3-355">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="b40c3-356">Свойство</span><span class="sxs-lookup"><span data-stu-id="b40c3-356">Property</span></span>         | <span data-ttu-id="b40c3-357">Тип</span><span class="sxs-lookup"><span data-stu-id="b40c3-357">Type</span></span>                                                     | <span data-ttu-id="b40c3-358">Обязательный</span><span class="sxs-lookup"><span data-stu-id="b40c3-358">Required</span></span>                | <span data-ttu-id="b40c3-359">Значение</span><span class="sxs-lookup"><span data-stu-id="b40c3-359">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="b40c3-360">resourceId</span><span class="sxs-lookup"><span data-stu-id="b40c3-360">resourceId</span></span>       | <span data-ttu-id="b40c3-361">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-361">String</span></span>                                                   | <span data-ttu-id="b40c3-362">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-362">Yes</span></span>                     | <span data-ttu-id="b40c3-363">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="b40c3-363">\<resourceId\></span></span> |
| <span data-ttu-id="b40c3-364">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="b40c3-364">roleDefinitionId</span></span> | <span data-ttu-id="b40c3-365">Строка</span><span class="sxs-lookup"><span data-stu-id="b40c3-365">String</span></span>                                                   | <span data-ttu-id="b40c3-366">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-366">Yes</span></span>                     | <span data-ttu-id="b40c3-367">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="b40c3-367">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="b40c3-368">Субжектид</span><span class="sxs-lookup"><span data-stu-id="b40c3-368">subjectId</span></span>        | <span data-ttu-id="b40c3-369">Строка</span><span class="sxs-lookup"><span data-stu-id="b40c3-369">String</span></span>                                                   | <span data-ttu-id="b40c3-370">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-370">Yes</span></span>                     | <span data-ttu-id="b40c3-371">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="b40c3-371">\<subjectId\></span></span> |
| <span data-ttu-id="b40c3-372">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="b40c3-372">assignmentState</span></span>  | <span data-ttu-id="b40c3-373">Строка</span><span class="sxs-lookup"><span data-stu-id="b40c3-373">String</span></span>                                                   | <span data-ttu-id="b40c3-374">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-374">Yes</span></span>                     | <span data-ttu-id="b40c3-375">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="b40c3-375">Eligible / Active</span></span> |
| <span data-ttu-id="b40c3-376">type</span><span class="sxs-lookup"><span data-stu-id="b40c3-376">type</span></span>             | <span data-ttu-id="b40c3-377">Строка</span><span class="sxs-lookup"><span data-stu-id="b40c3-377">String</span></span>                                                   | <span data-ttu-id="b40c3-378">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-378">Yes</span></span>                     | <span data-ttu-id="b40c3-379">Админупдате</span><span class="sxs-lookup"><span data-stu-id="b40c3-379">AdminUpdate</span></span> |
| <span data-ttu-id="b40c3-380">причиной</span><span class="sxs-lookup"><span data-stu-id="b40c3-380">reason</span></span>           | <span data-ttu-id="b40c3-381">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-381">String</span></span>                                                   | <span data-ttu-id="b40c3-382">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="b40c3-382">depends on roleSettings</span></span> |   |
| <span data-ttu-id="b40c3-383">schedule</span><span class="sxs-lookup"><span data-stu-id="b40c3-383">schedule</span></span>         | [<span data-ttu-id="b40c3-384">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="b40c3-384">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="b40c3-385">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-385">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="b40c3-386">Запрос</span><span class="sxs-lookup"><span data-stu-id="b40c3-386">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="b40c3-387">Отклик</span><span class="sxs-lookup"><span data-stu-id="b40c3-387">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="b40c3-388">Пример 6: администратор расширяет назначение ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="b40c3-388">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="b40c3-389">В этом примере показано, как расширить назначение роли истечения срока действия для пользователя АНУЖКУСЕР участнику службы управления API.</span><span class="sxs-lookup"><span data-stu-id="b40c3-389">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="b40c3-390">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="b40c3-390">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="b40c3-391">Свойство</span><span class="sxs-lookup"><span data-stu-id="b40c3-391">Property</span></span>         | <span data-ttu-id="b40c3-392">Тип</span><span class="sxs-lookup"><span data-stu-id="b40c3-392">Type</span></span>                                                     | <span data-ttu-id="b40c3-393">Обязательный</span><span class="sxs-lookup"><span data-stu-id="b40c3-393">Required</span></span>                | <span data-ttu-id="b40c3-394">Значение</span><span class="sxs-lookup"><span data-stu-id="b40c3-394">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="b40c3-395">resourceId</span><span class="sxs-lookup"><span data-stu-id="b40c3-395">resourceId</span></span>       | <span data-ttu-id="b40c3-396">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-396">String</span></span>                                                   | <span data-ttu-id="b40c3-397">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-397">Yes</span></span>                     | <span data-ttu-id="b40c3-398">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="b40c3-398">\<resourceId\></span></span> |
| <span data-ttu-id="b40c3-399">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="b40c3-399">roleDefinitionId</span></span> | <span data-ttu-id="b40c3-400">Строка</span><span class="sxs-lookup"><span data-stu-id="b40c3-400">String</span></span>                                                   | <span data-ttu-id="b40c3-401">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-401">Yes</span></span>                     | <span data-ttu-id="b40c3-402">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="b40c3-402">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="b40c3-403">Субжектид</span><span class="sxs-lookup"><span data-stu-id="b40c3-403">subjectId</span></span>        | <span data-ttu-id="b40c3-404">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-404">String</span></span>                                                   | <span data-ttu-id="b40c3-405">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-405">Yes</span></span>                     | <span data-ttu-id="b40c3-406">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="b40c3-406">\<subjectId\></span></span> |
| <span data-ttu-id="b40c3-407">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="b40c3-407">assignmentState</span></span>  | <span data-ttu-id="b40c3-408">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-408">String</span></span>                                                   | <span data-ttu-id="b40c3-409">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-409">Yes</span></span>                     | <span data-ttu-id="b40c3-410">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="b40c3-410">Eligible / Active</span></span> |
| <span data-ttu-id="b40c3-411">type</span><span class="sxs-lookup"><span data-stu-id="b40c3-411">type</span></span>             | <span data-ttu-id="b40c3-412">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-412">String</span></span>                                                   | <span data-ttu-id="b40c3-413">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-413">Yes</span></span>                     | <span data-ttu-id="b40c3-414">Админекстенд</span><span class="sxs-lookup"><span data-stu-id="b40c3-414">AdminExtend</span></span> |
| <span data-ttu-id="b40c3-415">причиной</span><span class="sxs-lookup"><span data-stu-id="b40c3-415">reason</span></span>           | <span data-ttu-id="b40c3-416">String</span><span class="sxs-lookup"><span data-stu-id="b40c3-416">String</span></span>                                                   | <span data-ttu-id="b40c3-417">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="b40c3-417">depends on roleSettings</span></span> |   |
| <span data-ttu-id="b40c3-418">schedule</span><span class="sxs-lookup"><span data-stu-id="b40c3-418">schedule</span></span>         | [<span data-ttu-id="b40c3-419">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="b40c3-419">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="b40c3-420">Да</span><span class="sxs-lookup"><span data-stu-id="b40c3-420">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="b40c3-421">Запрос</span><span class="sxs-lookup"><span data-stu-id="b40c3-421">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="b40c3-422">Отклик</span><span class="sxs-lookup"><span data-stu-id="b40c3-422">Response</span></span>

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
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
