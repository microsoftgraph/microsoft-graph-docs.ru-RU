---
title: Создание governanceRoleAssignmentRequest
description: Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли. В приведенной ниже таблице перечислены операции.
localization_priority: Normal
ms.openlocfilehash: 104ab1a0d4909bc2181df70bc4fc895fc4558260
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503284"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="e0885-104">Создание governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="e0885-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0885-105">Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="e0885-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="e0885-106">В приведенной ниже таблице перечислены операции.</span><span class="sxs-lookup"><span data-stu-id="e0885-106">The following table lists the operations.</span></span>

| <span data-ttu-id="e0885-107">Operation</span><span class="sxs-lookup"><span data-stu-id="e0885-107">Operation</span></span>                                   | <span data-ttu-id="e0885-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e0885-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="e0885-109">Назначение роли</span><span class="sxs-lookup"><span data-stu-id="e0885-109">Assign a role assignment</span></span>                    | <span data-ttu-id="e0885-110">Админадд</span><span class="sxs-lookup"><span data-stu-id="e0885-110">AdminAdd</span></span>    |
| <span data-ttu-id="e0885-111">Активация подходящего назначения роли</span><span class="sxs-lookup"><span data-stu-id="e0885-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="e0885-112">Усерадд</span><span class="sxs-lookup"><span data-stu-id="e0885-112">UserAdd</span></span>     |
| <span data-ttu-id="e0885-113">ДеАктивация активированного назначения роли</span><span class="sxs-lookup"><span data-stu-id="e0885-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="e0885-114">Усерремове</span><span class="sxs-lookup"><span data-stu-id="e0885-114">UserRemove</span></span>  |
| <span data-ttu-id="e0885-115">Удаление назначения роли</span><span class="sxs-lookup"><span data-stu-id="e0885-115">Remove a role assignment</span></span>                    | <span data-ttu-id="e0885-116">Админремове</span><span class="sxs-lookup"><span data-stu-id="e0885-116">AdminRemove</span></span> |
| <span data-ttu-id="e0885-117">Обновление назначения роли</span><span class="sxs-lookup"><span data-stu-id="e0885-117">Update a role assignment</span></span>                    | <span data-ttu-id="e0885-118">Админупдате</span><span class="sxs-lookup"><span data-stu-id="e0885-118">AdminUpdate</span></span> |
| <span data-ttu-id="e0885-119">Запрос на расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="e0885-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="e0885-120">Усерекстенд</span><span class="sxs-lookup"><span data-stu-id="e0885-120">UserExtend</span></span>  |
| <span data-ttu-id="e0885-121">Расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="e0885-121">Extend a role assignment</span></span>                    | <span data-ttu-id="e0885-122">Админекстенд</span><span class="sxs-lookup"><span data-stu-id="e0885-122">AdminExtend</span></span> |
| <span data-ttu-id="e0885-123">Запрос на продление назначения роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="e0885-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="e0885-124">Усерренев</span><span class="sxs-lookup"><span data-stu-id="e0885-124">UserRenew</span></span>   |
| <span data-ttu-id="e0885-125">Продление назначенной роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="e0885-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="e0885-126">Админренев</span><span class="sxs-lookup"><span data-stu-id="e0885-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="e0885-127">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e0885-127">Permissions</span></span>

<span data-ttu-id="e0885-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0885-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e0885-130">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0885-130">Permission type</span></span>                        | <span data-ttu-id="e0885-131">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e0885-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="e0885-132">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0885-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="e0885-133">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="e0885-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="e0885-134">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0885-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0885-135">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0885-135">Not supported.</span></span>                            |
| <span data-ttu-id="e0885-136">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0885-136">Application</span></span>                            | <span data-ttu-id="e0885-137">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="e0885-137">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0885-138">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0885-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="e0885-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0885-139">Request headers</span></span>

| <span data-ttu-id="e0885-140">Имя</span><span class="sxs-lookup"><span data-stu-id="e0885-140">Name</span></span>          | <span data-ttu-id="e0885-141">Описание</span><span class="sxs-lookup"><span data-stu-id="e0885-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="e0885-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0885-142">Authorization</span></span> | <span data-ttu-id="e0885-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e0885-143">Bearer {code}</span></span>    |
| <span data-ttu-id="e0885-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e0885-144">Content-type</span></span>  | <span data-ttu-id="e0885-145">application/json</span><span class="sxs-lookup"><span data-stu-id="e0885-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0885-146">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e0885-146">Request body</span></span>

<span data-ttu-id="e0885-147">В тексте запроса добавьте представление объекта [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0885-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="e0885-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0885-148">Property</span></span>         | <span data-ttu-id="e0885-149">Тип</span><span class="sxs-lookup"><span data-stu-id="e0885-149">Type</span></span>                                                     | <span data-ttu-id="e0885-150">Описание</span><span class="sxs-lookup"><span data-stu-id="e0885-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="e0885-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="e0885-151">resourceId</span></span>       | <span data-ttu-id="e0885-152">String</span><span class="sxs-lookup"><span data-stu-id="e0885-152">String</span></span>                                                   | <span data-ttu-id="e0885-153">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="e0885-153">The ID of the resource.</span></span> <span data-ttu-id="e0885-154">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="e0885-154">Required.</span></span> |
| <span data-ttu-id="e0885-155">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="e0885-155">roleDefinitionId</span></span> | <span data-ttu-id="e0885-156">String</span><span class="sxs-lookup"><span data-stu-id="e0885-156">String</span></span>                                                   | <span data-ttu-id="e0885-157">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="e0885-157">The ID of the role definition.</span></span> <span data-ttu-id="e0885-158">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="e0885-158">Required.</span></span> |
| <span data-ttu-id="e0885-159">Субжектид</span><span class="sxs-lookup"><span data-stu-id="e0885-159">subjectId</span></span>        | <span data-ttu-id="e0885-160">String</span><span class="sxs-lookup"><span data-stu-id="e0885-160">String</span></span>                                                   | <span data-ttu-id="e0885-161">ИДЕНТИФИКАТОР субъекта.</span><span class="sxs-lookup"><span data-stu-id="e0885-161">The ID of the subject.</span></span> <span data-ttu-id="e0885-162">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="e0885-162">Required.</span></span> |
| <span data-ttu-id="e0885-163">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="e0885-163">assignmentState</span></span>  | <span data-ttu-id="e0885-164">String</span><span class="sxs-lookup"><span data-stu-id="e0885-164">String</span></span>                                                   | <span data-ttu-id="e0885-165">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="e0885-165">The state of assignment.</span></span> <span data-ttu-id="e0885-166">Значение может быть `Eligible` и `Active`.</span><span class="sxs-lookup"><span data-stu-id="e0885-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="e0885-167">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="e0885-167">Required.</span></span> |
| <span data-ttu-id="e0885-168">type</span><span class="sxs-lookup"><span data-stu-id="e0885-168">type</span></span>             | <span data-ttu-id="e0885-169">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-169">String</span></span>                                                   | <span data-ttu-id="e0885-170">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="e0885-170">The request type.</span></span> <span data-ttu-id="e0885-171">Возможные значения: `AdminAdd`, `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `AdminRenew` `AdminExtend`,,,,, и. `UserExtend` `UserRenew`</span><span class="sxs-lookup"><span data-stu-id="e0885-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="e0885-172">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="e0885-172">Required.</span></span> |
| <span data-ttu-id="e0885-173">причиной</span><span class="sxs-lookup"><span data-stu-id="e0885-173">reason</span></span>           | <span data-ttu-id="e0885-174">String</span><span class="sxs-lookup"><span data-stu-id="e0885-174">String</span></span>                                                   | <span data-ttu-id="e0885-175">Необходимо указать причину для запроса на назначение роли для аудита и проверки.</span><span class="sxs-lookup"><span data-stu-id="e0885-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="e0885-176">Диспетчер</span><span class="sxs-lookup"><span data-stu-id="e0885-176">schedule</span></span>         | [<span data-ttu-id="e0885-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e0885-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="e0885-178">Расписание запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="e0885-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="e0885-179">`UserAdd`Для типа запроса `AdminAdd`,, `AdminUpdate`, и `AdminExtend`, он необходим.</span><span class="sxs-lookup"><span data-stu-id="e0885-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="e0885-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0885-180">Response</span></span>

<span data-ttu-id="e0885-181">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e0885-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="e0885-182">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="e0885-182">Error codes</span></span>

<span data-ttu-id="e0885-183">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="e0885-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="e0885-184">Кроме того, он возвращает коды ошибок, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="e0885-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="e0885-185">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="e0885-185">Error code</span></span>     | <span data-ttu-id="e0885-186">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="e0885-186">Error message</span></span>                               | <span data-ttu-id="e0885-187">Подробно</span><span class="sxs-lookup"><span data-stu-id="e0885-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="e0885-188">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="e0885-188">400 BadRequest</span></span> | <span data-ttu-id="e0885-189">Роленотфаунд</span><span class="sxs-lookup"><span data-stu-id="e0885-189">RoleNotFound</span></span>                                | <span data-ttu-id="e0885-190">Не `roleDefinitionId` удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="e0885-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="e0885-191">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="e0885-191">400 BadRequest</span></span> | <span data-ttu-id="e0885-192">Ресаурцеислоккед</span><span class="sxs-lookup"><span data-stu-id="e0885-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="e0885-193">Ресурс, указанный в теле запроса, находится в состоянии `Locked` и не может создавать запросы на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="e0885-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="e0885-194">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="e0885-194">400 BadRequest</span></span> | <span data-ttu-id="e0885-195">Субжектнотфаунд</span><span class="sxs-lookup"><span data-stu-id="e0885-195">SubjectNotFound</span></span>                             | <span data-ttu-id="e0885-196">Не `subjectId` удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="e0885-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="e0885-197">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="e0885-197">400 BadRequest</span></span> | <span data-ttu-id="e0885-198">Пендингролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="e0885-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="e0885-199">В системе уже существует ожидающий [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="e0885-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="e0885-200">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="e0885-200">400 BadRequest</span></span> | <span data-ttu-id="e0885-201">Ролеассигнментексистс</span><span class="sxs-lookup"><span data-stu-id="e0885-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="e0885-202">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , который требуется создать, уже существует в системе.</span><span class="sxs-lookup"><span data-stu-id="e0885-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="e0885-203">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="e0885-203">400 BadRequest</span></span> | <span data-ttu-id="e0885-204">Ролеассигнментдоеснотексист</span><span class="sxs-lookup"><span data-stu-id="e0885-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="e0885-205">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , запрошенный для обновления или расширения, не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="e0885-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="e0885-206">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="e0885-206">400 BadRequest</span></span> | <span data-ttu-id="e0885-207">Ролеассигнментрекуестполицивалидатионфаилед</span><span class="sxs-lookup"><span data-stu-id="e0885-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="e0885-208">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) не отвечает внутренним политикам и не может быть создан.</span><span class="sxs-lookup"><span data-stu-id="e0885-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="e0885-209">Примеры</span><span class="sxs-lookup"><span data-stu-id="e0885-209">Examples</span></span>

<span data-ttu-id="e0885-210">В следующих примерах показано, как использовать этот API.</span><span class="sxs-lookup"><span data-stu-id="e0885-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="e0885-211">Пример 1: Администратор назначает пользователю роль</span><span class="sxs-lookup"><span data-stu-id="e0885-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="e0885-212">В этом примере администратор назначает пользователю nawu@fimdev.net роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="e0885-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="e0885-213">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="e0885-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="e0885-214">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0885-214">Property</span></span>         | <span data-ttu-id="e0885-215">Тип</span><span class="sxs-lookup"><span data-stu-id="e0885-215">Type</span></span>                                                     | <span data-ttu-id="e0885-216">Обязательный</span><span class="sxs-lookup"><span data-stu-id="e0885-216">Required</span></span>                 | <span data-ttu-id="e0885-217">Значение</span><span class="sxs-lookup"><span data-stu-id="e0885-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="e0885-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="e0885-218">resourceId</span></span>       | <span data-ttu-id="e0885-219">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-219">String</span></span>                                                   | <span data-ttu-id="e0885-220">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-220">Yes</span></span>                      | <span data-ttu-id="e0885-221">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="e0885-221">\<resourceId\></span></span> |
| <span data-ttu-id="e0885-222">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="e0885-222">roleDefinitionId</span></span> | <span data-ttu-id="e0885-223">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-223">String</span></span>                                                   | <span data-ttu-id="e0885-224">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-224">Yes</span></span>                      | <span data-ttu-id="e0885-225">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="e0885-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="e0885-226">Субжектид</span><span class="sxs-lookup"><span data-stu-id="e0885-226">subjectId</span></span>        | <span data-ttu-id="e0885-227">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-227">String</span></span>                                                   | <span data-ttu-id="e0885-228">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-228">Yes</span></span>                      | <span data-ttu-id="e0885-229">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="e0885-229">\<subjectId\></span></span> |
| <span data-ttu-id="e0885-230">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="e0885-230">assignmentState</span></span>  | <span data-ttu-id="e0885-231">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-231">String</span></span>                                                   | <span data-ttu-id="e0885-232">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-232">Yes</span></span>                      | <span data-ttu-id="e0885-233">ПодХодящие/активные</span><span class="sxs-lookup"><span data-stu-id="e0885-233">Eligible / Active</span></span> |
| <span data-ttu-id="e0885-234">type</span><span class="sxs-lookup"><span data-stu-id="e0885-234">type</span></span>             | <span data-ttu-id="e0885-235">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-235">String</span></span>                                                   | <span data-ttu-id="e0885-236">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-236">Yes</span></span>                      | <span data-ttu-id="e0885-237">Админадд</span><span class="sxs-lookup"><span data-stu-id="e0885-237">AdminAdd</span></span> |
| <span data-ttu-id="e0885-238">причиной</span><span class="sxs-lookup"><span data-stu-id="e0885-238">reason</span></span>           | <span data-ttu-id="e0885-239">String</span><span class="sxs-lookup"><span data-stu-id="e0885-239">String</span></span>                                                   | <span data-ttu-id="e0885-240">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="e0885-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="e0885-241">Диспетчер</span><span class="sxs-lookup"><span data-stu-id="e0885-241">schedule</span></span>         | [<span data-ttu-id="e0885-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e0885-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="e0885-243">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="e0885-244">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0885-244">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="e0885-245">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0885-245">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="e0885-246">Пример 2: пользователь активирует подходящие роли</span><span class="sxs-lookup"><span data-stu-id="e0885-246">Example 2: User activates eligible role</span></span>

<span data-ttu-id="e0885-247">В этом примере пользователь nawu@fimdev.net активирует соответствующую роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="e0885-247">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="e0885-248">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0885-248">Property</span></span>         | <span data-ttu-id="e0885-249">Тип</span><span class="sxs-lookup"><span data-stu-id="e0885-249">Type</span></span>                                                     | <span data-ttu-id="e0885-250">Обязательный</span><span class="sxs-lookup"><span data-stu-id="e0885-250">Required</span></span>                 | <span data-ttu-id="e0885-251">Значение</span><span class="sxs-lookup"><span data-stu-id="e0885-251">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="e0885-252">resourceId</span><span class="sxs-lookup"><span data-stu-id="e0885-252">resourceId</span></span>       | <span data-ttu-id="e0885-253">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-253">String</span></span>                                                   | <span data-ttu-id="e0885-254">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-254">Yes</span></span>                      | <span data-ttu-id="e0885-255">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="e0885-255">\<resourceId\></span></span> |
| <span data-ttu-id="e0885-256">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="e0885-256">roleDefinitionId</span></span> | <span data-ttu-id="e0885-257">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-257">String</span></span>                                                   | <span data-ttu-id="e0885-258">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-258">Yes</span></span>                      | <span data-ttu-id="e0885-259">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="e0885-259">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="e0885-260">Субжектид</span><span class="sxs-lookup"><span data-stu-id="e0885-260">subjectId</span></span>        | <span data-ttu-id="e0885-261">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-261">String</span></span>                                                   | <span data-ttu-id="e0885-262">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-262">Yes</span></span>                      | <span data-ttu-id="e0885-263">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="e0885-263">\<subjectId\></span></span> |
| <span data-ttu-id="e0885-264">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="e0885-264">assignmentState</span></span>  | <span data-ttu-id="e0885-265">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-265">String</span></span>                                                   | <span data-ttu-id="e0885-266">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-266">Yes</span></span>                      | <span data-ttu-id="e0885-267">Активное</span><span class="sxs-lookup"><span data-stu-id="e0885-267">Active</span></span> |
| <span data-ttu-id="e0885-268">type</span><span class="sxs-lookup"><span data-stu-id="e0885-268">type</span></span>             | <span data-ttu-id="e0885-269">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-269">String</span></span>                                                   | <span data-ttu-id="e0885-270">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-270">Yes</span></span>                      | <span data-ttu-id="e0885-271">Усерадд</span><span class="sxs-lookup"><span data-stu-id="e0885-271">UserAdd</span></span> |
| <span data-ttu-id="e0885-272">причиной</span><span class="sxs-lookup"><span data-stu-id="e0885-272">reason</span></span>           | <span data-ttu-id="e0885-273">String</span><span class="sxs-lookup"><span data-stu-id="e0885-273">String</span></span>                                                   | <span data-ttu-id="e0885-274">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="e0885-274">depends on role Settings</span></span> |   |
| <span data-ttu-id="e0885-275">Диспетчер</span><span class="sxs-lookup"><span data-stu-id="e0885-275">schedule</span></span>         | [<span data-ttu-id="e0885-276">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e0885-276">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="e0885-277">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-277">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="e0885-278">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0885-278">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="e0885-279">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0885-279">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="e0885-280">Пример 3: пользователь отключает назначенную роль</span><span class="sxs-lookup"><span data-stu-id="e0885-280">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="e0885-281">В этом примере пользователь nawu@fimdev.net отключает активную роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="e0885-281">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="e0885-282">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0885-282">Property</span></span>         | <span data-ttu-id="e0885-283">Тип</span><span class="sxs-lookup"><span data-stu-id="e0885-283">Type</span></span>                                                     | <span data-ttu-id="e0885-284">Обязательный</span><span class="sxs-lookup"><span data-stu-id="e0885-284">Required</span></span> | <span data-ttu-id="e0885-285">Значение</span><span class="sxs-lookup"><span data-stu-id="e0885-285">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="e0885-286">resourceId</span><span class="sxs-lookup"><span data-stu-id="e0885-286">resourceId</span></span>       | <span data-ttu-id="e0885-287">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-287">String</span></span>                                                   | <span data-ttu-id="e0885-288">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-288">Yes</span></span>      | <span data-ttu-id="e0885-289">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="e0885-289">\<resourceId\></span></span> |
| <span data-ttu-id="e0885-290">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="e0885-290">roleDefinitionId</span></span> | <span data-ttu-id="e0885-291">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-291">String</span></span>                                                   | <span data-ttu-id="e0885-292">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-292">Yes</span></span>      | <span data-ttu-id="e0885-293">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="e0885-293">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="e0885-294">Субжектид</span><span class="sxs-lookup"><span data-stu-id="e0885-294">subjectId</span></span>        | <span data-ttu-id="e0885-295">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-295">String</span></span>                                                   | <span data-ttu-id="e0885-296">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-296">Yes</span></span>      | <span data-ttu-id="e0885-297">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="e0885-297">\<subjectId\></span></span> |
| <span data-ttu-id="e0885-298">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="e0885-298">assignmentState</span></span>  | <span data-ttu-id="e0885-299">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-299">String</span></span>                                                   | <span data-ttu-id="e0885-300">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-300">Yes</span></span>      | <span data-ttu-id="e0885-301">Активное</span><span class="sxs-lookup"><span data-stu-id="e0885-301">Active</span></span> |
| <span data-ttu-id="e0885-302">type</span><span class="sxs-lookup"><span data-stu-id="e0885-302">type</span></span>             | <span data-ttu-id="e0885-303">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-303">String</span></span>                                                   | <span data-ttu-id="e0885-304">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-304">Yes</span></span>      | <span data-ttu-id="e0885-305">Усерремове</span><span class="sxs-lookup"><span data-stu-id="e0885-305">UserRemove</span></span> |
| <span data-ttu-id="e0885-306">причиной</span><span class="sxs-lookup"><span data-stu-id="e0885-306">reason</span></span>           | <span data-ttu-id="e0885-307">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-307">String</span></span>                                                   | <span data-ttu-id="e0885-308">Нет</span><span class="sxs-lookup"><span data-stu-id="e0885-308">No</span></span>       |   |
| <span data-ttu-id="e0885-309">Диспетчер</span><span class="sxs-lookup"><span data-stu-id="e0885-309">schedule</span></span>         | [<span data-ttu-id="e0885-310">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e0885-310">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="e0885-311">Нет</span><span class="sxs-lookup"><span data-stu-id="e0885-311">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="e0885-312">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0885-312">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="e0885-313">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0885-313">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="e0885-314">Пример 4: Администратор удаляет пользователя из роли</span><span class="sxs-lookup"><span data-stu-id="e0885-314">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="e0885-315">В этом примере администратор удаляет пользователя nawu@fimdev.net из роли читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="e0885-315">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="e0885-316">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="e0885-316">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="e0885-317">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0885-317">Property</span></span>         | <span data-ttu-id="e0885-318">Тип</span><span class="sxs-lookup"><span data-stu-id="e0885-318">Type</span></span>                                                     | <span data-ttu-id="e0885-319">Обязательный</span><span class="sxs-lookup"><span data-stu-id="e0885-319">Required</span></span> | <span data-ttu-id="e0885-320">Значение</span><span class="sxs-lookup"><span data-stu-id="e0885-320">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="e0885-321">resourceId</span><span class="sxs-lookup"><span data-stu-id="e0885-321">resourceId</span></span>       | <span data-ttu-id="e0885-322">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-322">String</span></span>                                                   | <span data-ttu-id="e0885-323">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-323">Yes</span></span>      | <span data-ttu-id="e0885-324">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="e0885-324">\<resourceId\></span></span> |
| <span data-ttu-id="e0885-325">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="e0885-325">roleDefinitionId</span></span> | <span data-ttu-id="e0885-326">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-326">String</span></span>                                                   | <span data-ttu-id="e0885-327">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-327">Yes</span></span>      | <span data-ttu-id="e0885-328">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="e0885-328">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="e0885-329">Субжектид</span><span class="sxs-lookup"><span data-stu-id="e0885-329">subjectId</span></span>        | <span data-ttu-id="e0885-330">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-330">String</span></span>                                                   | <span data-ttu-id="e0885-331">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-331">Yes</span></span>      | <span data-ttu-id="e0885-332">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="e0885-332">\<subjectId\></span></span> |
| <span data-ttu-id="e0885-333">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="e0885-333">assignmentState</span></span>  | <span data-ttu-id="e0885-334">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-334">String</span></span>                                                   | <span data-ttu-id="e0885-335">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-335">Yes</span></span>      | <span data-ttu-id="e0885-336">ПодХодящие/активные</span><span class="sxs-lookup"><span data-stu-id="e0885-336">Eligible / Active</span></span> |
| <span data-ttu-id="e0885-337">type</span><span class="sxs-lookup"><span data-stu-id="e0885-337">type</span></span>             | <span data-ttu-id="e0885-338">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-338">String</span></span>                                                   | <span data-ttu-id="e0885-339">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-339">Yes</span></span>      | <span data-ttu-id="e0885-340">Админремове</span><span class="sxs-lookup"><span data-stu-id="e0885-340">AdminRemove</span></span> |
| <span data-ttu-id="e0885-341">причиной</span><span class="sxs-lookup"><span data-stu-id="e0885-341">reason</span></span>           | <span data-ttu-id="e0885-342">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-342">String</span></span>                                                   | <span data-ttu-id="e0885-343">Нет</span><span class="sxs-lookup"><span data-stu-id="e0885-343">No</span></span>       |   |
| <span data-ttu-id="e0885-344">Диспетчер</span><span class="sxs-lookup"><span data-stu-id="e0885-344">schedule</span></span>         | [<span data-ttu-id="e0885-345">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e0885-345">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="e0885-346">Нет</span><span class="sxs-lookup"><span data-stu-id="e0885-346">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="e0885-347">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0885-347">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="e0885-348">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0885-348">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="e0885-349">Пример 5: "Администратор обновляет назначение ролей"</span><span class="sxs-lookup"><span data-stu-id="e0885-349">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="e0885-350">В этом примере администраторы обновляют назначение роли пользователя nawu@fimdev.net владельцу.</span><span class="sxs-lookup"><span data-stu-id="e0885-350">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="e0885-351">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="e0885-351">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="e0885-352">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0885-352">Property</span></span>         | <span data-ttu-id="e0885-353">Тип</span><span class="sxs-lookup"><span data-stu-id="e0885-353">Type</span></span>                                                     | <span data-ttu-id="e0885-354">Обязательный</span><span class="sxs-lookup"><span data-stu-id="e0885-354">Required</span></span>                | <span data-ttu-id="e0885-355">Значение</span><span class="sxs-lookup"><span data-stu-id="e0885-355">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="e0885-356">resourceId</span><span class="sxs-lookup"><span data-stu-id="e0885-356">resourceId</span></span>       | <span data-ttu-id="e0885-357">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-357">String</span></span>                                                   | <span data-ttu-id="e0885-358">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-358">Yes</span></span>                     | <span data-ttu-id="e0885-359">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="e0885-359">\<resourceId\></span></span> |
| <span data-ttu-id="e0885-360">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="e0885-360">roleDefinitionId</span></span> | <span data-ttu-id="e0885-361">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-361">String</span></span>                                                   | <span data-ttu-id="e0885-362">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-362">Yes</span></span>                     | <span data-ttu-id="e0885-363">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="e0885-363">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="e0885-364">Субжектид</span><span class="sxs-lookup"><span data-stu-id="e0885-364">subjectId</span></span>        | <span data-ttu-id="e0885-365">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-365">String</span></span>                                                   | <span data-ttu-id="e0885-366">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-366">Yes</span></span>                     | <span data-ttu-id="e0885-367">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="e0885-367">\<subjectId\></span></span> |
| <span data-ttu-id="e0885-368">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="e0885-368">assignmentState</span></span>  | <span data-ttu-id="e0885-369">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-369">String</span></span>                                                   | <span data-ttu-id="e0885-370">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-370">Yes</span></span>                     | <span data-ttu-id="e0885-371">ПодХодящие/активные</span><span class="sxs-lookup"><span data-stu-id="e0885-371">Eligible / Active</span></span> |
| <span data-ttu-id="e0885-372">type</span><span class="sxs-lookup"><span data-stu-id="e0885-372">type</span></span>             | <span data-ttu-id="e0885-373">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-373">String</span></span>                                                   | <span data-ttu-id="e0885-374">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-374">Yes</span></span>                     | <span data-ttu-id="e0885-375">Админупдате</span><span class="sxs-lookup"><span data-stu-id="e0885-375">AdminUpdate</span></span> |
| <span data-ttu-id="e0885-376">причиной</span><span class="sxs-lookup"><span data-stu-id="e0885-376">reason</span></span>           | <span data-ttu-id="e0885-377">String</span><span class="sxs-lookup"><span data-stu-id="e0885-377">String</span></span>                                                   | <span data-ttu-id="e0885-378">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="e0885-378">depends on roleSettings</span></span> |   |
| <span data-ttu-id="e0885-379">Диспетчер</span><span class="sxs-lookup"><span data-stu-id="e0885-379">schedule</span></span>         | [<span data-ttu-id="e0885-380">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e0885-380">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="e0885-381">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-381">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="e0885-382">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0885-382">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="e0885-383">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0885-383">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="e0885-384">Пример 6: администратор расширяет назначение ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="e0885-384">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="e0885-385">В этом примере показано, как расширить назначение роли истечения срока действия для пользователя АНУЖКУСЕР участнику службы управления API.</span><span class="sxs-lookup"><span data-stu-id="e0885-385">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="e0885-386">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="e0885-386">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="e0885-387">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0885-387">Property</span></span>         | <span data-ttu-id="e0885-388">Тип</span><span class="sxs-lookup"><span data-stu-id="e0885-388">Type</span></span>                                                     | <span data-ttu-id="e0885-389">Обязательный</span><span class="sxs-lookup"><span data-stu-id="e0885-389">Required</span></span>                | <span data-ttu-id="e0885-390">Значение</span><span class="sxs-lookup"><span data-stu-id="e0885-390">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="e0885-391">resourceId</span><span class="sxs-lookup"><span data-stu-id="e0885-391">resourceId</span></span>       | <span data-ttu-id="e0885-392">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-392">String</span></span>                                                   | <span data-ttu-id="e0885-393">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-393">Yes</span></span>                     | <span data-ttu-id="e0885-394">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="e0885-394">\<resourceId\></span></span> |
| <span data-ttu-id="e0885-395">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="e0885-395">roleDefinitionId</span></span> | <span data-ttu-id="e0885-396">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-396">String</span></span>                                                   | <span data-ttu-id="e0885-397">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-397">Yes</span></span>                     | <span data-ttu-id="e0885-398">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="e0885-398">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="e0885-399">Субжектид</span><span class="sxs-lookup"><span data-stu-id="e0885-399">subjectId</span></span>        | <span data-ttu-id="e0885-400">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-400">String</span></span>                                                   | <span data-ttu-id="e0885-401">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-401">Yes</span></span>                     | <span data-ttu-id="e0885-402">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="e0885-402">\<subjectId\></span></span> |
| <span data-ttu-id="e0885-403">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="e0885-403">assignmentState</span></span>  | <span data-ttu-id="e0885-404">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-404">String</span></span>                                                   | <span data-ttu-id="e0885-405">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-405">Yes</span></span>                     | <span data-ttu-id="e0885-406">ПодХодящие/активные</span><span class="sxs-lookup"><span data-stu-id="e0885-406">Eligible / Active</span></span> |
| <span data-ttu-id="e0885-407">type</span><span class="sxs-lookup"><span data-stu-id="e0885-407">type</span></span>             | <span data-ttu-id="e0885-408">Строка</span><span class="sxs-lookup"><span data-stu-id="e0885-408">String</span></span>                                                   | <span data-ttu-id="e0885-409">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-409">Yes</span></span>                     | <span data-ttu-id="e0885-410">Админекстенд</span><span class="sxs-lookup"><span data-stu-id="e0885-410">AdminExtend</span></span> |
| <span data-ttu-id="e0885-411">причиной</span><span class="sxs-lookup"><span data-stu-id="e0885-411">reason</span></span>           | <span data-ttu-id="e0885-412">String</span><span class="sxs-lookup"><span data-stu-id="e0885-412">String</span></span>                                                   | <span data-ttu-id="e0885-413">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="e0885-413">depends on roleSettings</span></span> |   |
| <span data-ttu-id="e0885-414">Диспетчер</span><span class="sxs-lookup"><span data-stu-id="e0885-414">schedule</span></span>         | [<span data-ttu-id="e0885-415">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e0885-415">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="e0885-416">Да</span><span class="sxs-lookup"><span data-stu-id="e0885-416">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="e0885-417">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0885-417">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="e0885-418">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0885-418">Response</span></span>

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
