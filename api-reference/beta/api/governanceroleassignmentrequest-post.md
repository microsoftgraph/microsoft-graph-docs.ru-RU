---
title: Создание governanceRoleAssignmentRequest
description: Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли. В приведенной ниже таблице перечислены операции.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: a49bd528ffe97e33402ab8aef51f86a07b33e5fa
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420327"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="71451-104">Создание governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="71451-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71451-105">Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="71451-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="71451-106">В приведенной ниже таблице перечислены операции.</span><span class="sxs-lookup"><span data-stu-id="71451-106">The following table lists the operations.</span></span>

| <span data-ttu-id="71451-107">Operation</span><span class="sxs-lookup"><span data-stu-id="71451-107">Operation</span></span>                                   | <span data-ttu-id="71451-108">Тип</span><span class="sxs-lookup"><span data-stu-id="71451-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="71451-109">Назначение роли</span><span class="sxs-lookup"><span data-stu-id="71451-109">Assign a role assignment</span></span>                    | <span data-ttu-id="71451-110">админадд</span><span class="sxs-lookup"><span data-stu-id="71451-110">AdminAdd</span></span>    |
| <span data-ttu-id="71451-111">Активация подходящего назначения роли</span><span class="sxs-lookup"><span data-stu-id="71451-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="71451-112">усерадд</span><span class="sxs-lookup"><span data-stu-id="71451-112">UserAdd</span></span>     |
| <span data-ttu-id="71451-113">Деактивация активированного назначения роли</span><span class="sxs-lookup"><span data-stu-id="71451-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="71451-114">усерремове</span><span class="sxs-lookup"><span data-stu-id="71451-114">UserRemove</span></span>  |
| <span data-ttu-id="71451-115">Удаление назначения роли</span><span class="sxs-lookup"><span data-stu-id="71451-115">Remove a role assignment</span></span>                    | <span data-ttu-id="71451-116">админремове</span><span class="sxs-lookup"><span data-stu-id="71451-116">AdminRemove</span></span> |
| <span data-ttu-id="71451-117">Обновление назначения роли</span><span class="sxs-lookup"><span data-stu-id="71451-117">Update a role assignment</span></span>                    | <span data-ttu-id="71451-118">админупдате</span><span class="sxs-lookup"><span data-stu-id="71451-118">AdminUpdate</span></span> |
| <span data-ttu-id="71451-119">Запрос на расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="71451-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="71451-120">усерекстенд</span><span class="sxs-lookup"><span data-stu-id="71451-120">UserExtend</span></span>  |
| <span data-ttu-id="71451-121">Расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="71451-121">Extend a role assignment</span></span>                    | <span data-ttu-id="71451-122">админекстенд</span><span class="sxs-lookup"><span data-stu-id="71451-122">AdminExtend</span></span> |
| <span data-ttu-id="71451-123">Запрос на продление назначения роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="71451-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="71451-124">усерренев</span><span class="sxs-lookup"><span data-stu-id="71451-124">UserRenew</span></span>   |
| <span data-ttu-id="71451-125">Продление назначенной роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="71451-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="71451-126">админренев</span><span class="sxs-lookup"><span data-stu-id="71451-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="71451-127">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71451-127">Permissions</span></span>

<span data-ttu-id="71451-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71451-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="71451-130">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71451-130">Permission type</span></span>                        | <span data-ttu-id="71451-131">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71451-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="71451-132">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71451-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="71451-133">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="71451-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="71451-134">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71451-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71451-135">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71451-135">Not supported.</span></span>                            |
| <span data-ttu-id="71451-136">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71451-136">Application</span></span>                            | <span data-ttu-id="71451-137">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71451-137">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="71451-138">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71451-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="71451-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71451-139">Request headers</span></span>

| <span data-ttu-id="71451-140">Имя</span><span class="sxs-lookup"><span data-stu-id="71451-140">Name</span></span>          | <span data-ttu-id="71451-141">Описание</span><span class="sxs-lookup"><span data-stu-id="71451-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="71451-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71451-142">Authorization</span></span> | <span data-ttu-id="71451-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="71451-143">Bearer {code}</span></span>    |
| <span data-ttu-id="71451-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="71451-144">Content-type</span></span>  | <span data-ttu-id="71451-145">application/json</span><span class="sxs-lookup"><span data-stu-id="71451-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="71451-146">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="71451-146">Request body</span></span>

<span data-ttu-id="71451-147">В тексте запроса добавьте представление объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71451-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="71451-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="71451-148">Property</span></span>         | <span data-ttu-id="71451-149">Тип</span><span class="sxs-lookup"><span data-stu-id="71451-149">Type</span></span>                                                     | <span data-ttu-id="71451-150">Описание</span><span class="sxs-lookup"><span data-stu-id="71451-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="71451-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="71451-151">resourceId</span></span>       | <span data-ttu-id="71451-152">String</span><span class="sxs-lookup"><span data-stu-id="71451-152">String</span></span>                                                   | <span data-ttu-id="71451-153">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="71451-153">The ID of the resource.</span></span> <span data-ttu-id="71451-154">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="71451-154">Required.</span></span> |
| <span data-ttu-id="71451-155">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="71451-155">roleDefinitionId</span></span> | <span data-ttu-id="71451-156">String</span><span class="sxs-lookup"><span data-stu-id="71451-156">String</span></span>                                                   | <span data-ttu-id="71451-157">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="71451-157">The ID of the role definition.</span></span> <span data-ttu-id="71451-158">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="71451-158">Required.</span></span> |
| <span data-ttu-id="71451-159">субжектид</span><span class="sxs-lookup"><span data-stu-id="71451-159">subjectId</span></span>        | <span data-ttu-id="71451-160">String</span><span class="sxs-lookup"><span data-stu-id="71451-160">String</span></span>                                                   | <span data-ttu-id="71451-161">ИДЕНТИФИКАТОР субъекта.</span><span class="sxs-lookup"><span data-stu-id="71451-161">The ID of the subject.</span></span> <span data-ttu-id="71451-162">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="71451-162">Required.</span></span> |
| <span data-ttu-id="71451-163">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="71451-163">assignmentState</span></span>  | <span data-ttu-id="71451-164">String</span><span class="sxs-lookup"><span data-stu-id="71451-164">String</span></span>                                                   | <span data-ttu-id="71451-165">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="71451-165">The state of assignment.</span></span> <span data-ttu-id="71451-166">Значение может быть `Eligible` и `Active`.</span><span class="sxs-lookup"><span data-stu-id="71451-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="71451-167">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="71451-167">Required.</span></span> |
| <span data-ttu-id="71451-168">type</span><span class="sxs-lookup"><span data-stu-id="71451-168">type</span></span>             | <span data-ttu-id="71451-169">String</span><span class="sxs-lookup"><span data-stu-id="71451-169">String</span></span>                                                   | <span data-ttu-id="71451-170">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="71451-170">The request type.</span></span> <span data-ttu-id="71451-171">Возможные значения: `AdminAdd`, `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `AdminRenew` `AdminExtend`,,,,, и. `UserExtend` `UserRenew`</span><span class="sxs-lookup"><span data-stu-id="71451-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="71451-172">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="71451-172">Required.</span></span> |
| <span data-ttu-id="71451-173">причиной</span><span class="sxs-lookup"><span data-stu-id="71451-173">reason</span></span>           | <span data-ttu-id="71451-174">String</span><span class="sxs-lookup"><span data-stu-id="71451-174">String</span></span>                                                   | <span data-ttu-id="71451-175">Необходимо указать причину для запроса на назначение роли для аудита и проверки.</span><span class="sxs-lookup"><span data-stu-id="71451-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="71451-176">schedule</span><span class="sxs-lookup"><span data-stu-id="71451-176">schedule</span></span>         | [<span data-ttu-id="71451-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="71451-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="71451-178">Расписание запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="71451-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="71451-179">`UserAdd`Для типа запроса `AdminAdd`,, `AdminUpdate`, и `AdminExtend`, он необходим.</span><span class="sxs-lookup"><span data-stu-id="71451-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="71451-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="71451-180">Response</span></span>

<span data-ttu-id="71451-181">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="71451-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="71451-182">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="71451-182">Error codes</span></span>

<span data-ttu-id="71451-183">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="71451-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="71451-184">Кроме того, он возвращает коды ошибок, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="71451-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="71451-185">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="71451-185">Error code</span></span>     | <span data-ttu-id="71451-186">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="71451-186">Error message</span></span>                               | <span data-ttu-id="71451-187">Сведения</span><span class="sxs-lookup"><span data-stu-id="71451-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="71451-188">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="71451-188">400 BadRequest</span></span> | <span data-ttu-id="71451-189">роленотфаунд</span><span class="sxs-lookup"><span data-stu-id="71451-189">RoleNotFound</span></span>                                | <span data-ttu-id="71451-190">Не `roleDefinitionId` удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="71451-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="71451-191">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="71451-191">400 BadRequest</span></span> | <span data-ttu-id="71451-192">ресаурцеислоккед</span><span class="sxs-lookup"><span data-stu-id="71451-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="71451-193">Ресурс, указанный в теле запроса, находится в состоянии `Locked` и не может создавать запросы на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="71451-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="71451-194">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="71451-194">400 BadRequest</span></span> | <span data-ttu-id="71451-195">субжектнотфаунд</span><span class="sxs-lookup"><span data-stu-id="71451-195">SubjectNotFound</span></span>                             | <span data-ttu-id="71451-196">Не `subjectId` удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="71451-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="71451-197">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="71451-197">400 BadRequest</span></span> | <span data-ttu-id="71451-198">пендингролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="71451-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="71451-199">В системе уже существует ожидающий [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="71451-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="71451-200">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="71451-200">400 BadRequest</span></span> | <span data-ttu-id="71451-201">ролеассигнментексистс</span><span class="sxs-lookup"><span data-stu-id="71451-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="71451-202">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , который требуется создать, уже существует в системе.</span><span class="sxs-lookup"><span data-stu-id="71451-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="71451-203">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="71451-203">400 BadRequest</span></span> | <span data-ttu-id="71451-204">ролеассигнментдоеснотексист</span><span class="sxs-lookup"><span data-stu-id="71451-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="71451-205">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , запрошенный для обновления или расширения, не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="71451-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="71451-206">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="71451-206">400 BadRequest</span></span> | <span data-ttu-id="71451-207">ролеассигнментрекуестполицивалидатионфаилед</span><span class="sxs-lookup"><span data-stu-id="71451-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="71451-208">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) не отвечает внутренним политикам и не может быть создан.</span><span class="sxs-lookup"><span data-stu-id="71451-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="71451-209">Примеры</span><span class="sxs-lookup"><span data-stu-id="71451-209">Examples</span></span>

<span data-ttu-id="71451-210">В следующих примерах показано, как использовать этот API.</span><span class="sxs-lookup"><span data-stu-id="71451-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="71451-211">Пример 1: Администратор назначает пользователю роль</span><span class="sxs-lookup"><span data-stu-id="71451-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="71451-212">В этом примере администратор назначает пользователю nawu@fimdev.net роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="71451-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="71451-213">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="71451-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="71451-214">Свойство</span><span class="sxs-lookup"><span data-stu-id="71451-214">Property</span></span>         | <span data-ttu-id="71451-215">Тип</span><span class="sxs-lookup"><span data-stu-id="71451-215">Type</span></span>                                                     | <span data-ttu-id="71451-216">Обязательный</span><span class="sxs-lookup"><span data-stu-id="71451-216">Required</span></span>                 | <span data-ttu-id="71451-217">Значение</span><span class="sxs-lookup"><span data-stu-id="71451-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="71451-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="71451-218">resourceId</span></span>       | <span data-ttu-id="71451-219">String</span><span class="sxs-lookup"><span data-stu-id="71451-219">String</span></span>                                                   | <span data-ttu-id="71451-220">Да</span><span class="sxs-lookup"><span data-stu-id="71451-220">Yes</span></span>                      | <span data-ttu-id="71451-221">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="71451-221">\<resourceId\></span></span> |
| <span data-ttu-id="71451-222">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="71451-222">roleDefinitionId</span></span> | <span data-ttu-id="71451-223">String</span><span class="sxs-lookup"><span data-stu-id="71451-223">String</span></span>                                                   | <span data-ttu-id="71451-224">Да</span><span class="sxs-lookup"><span data-stu-id="71451-224">Yes</span></span>                      | <span data-ttu-id="71451-225">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="71451-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="71451-226">субжектид</span><span class="sxs-lookup"><span data-stu-id="71451-226">subjectId</span></span>        | <span data-ttu-id="71451-227">String</span><span class="sxs-lookup"><span data-stu-id="71451-227">String</span></span>                                                   | <span data-ttu-id="71451-228">Да</span><span class="sxs-lookup"><span data-stu-id="71451-228">Yes</span></span>                      | <span data-ttu-id="71451-229">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="71451-229">\<subjectId\></span></span> |
| <span data-ttu-id="71451-230">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="71451-230">assignmentState</span></span>  | <span data-ttu-id="71451-231">String</span><span class="sxs-lookup"><span data-stu-id="71451-231">String</span></span>                                                   | <span data-ttu-id="71451-232">Да</span><span class="sxs-lookup"><span data-stu-id="71451-232">Yes</span></span>                      | <span data-ttu-id="71451-233">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="71451-233">Eligible / Active</span></span> |
| <span data-ttu-id="71451-234">type</span><span class="sxs-lookup"><span data-stu-id="71451-234">type</span></span>             | <span data-ttu-id="71451-235">String</span><span class="sxs-lookup"><span data-stu-id="71451-235">String</span></span>                                                   | <span data-ttu-id="71451-236">Да</span><span class="sxs-lookup"><span data-stu-id="71451-236">Yes</span></span>                      | <span data-ttu-id="71451-237">админадд</span><span class="sxs-lookup"><span data-stu-id="71451-237">AdminAdd</span></span> |
| <span data-ttu-id="71451-238">причиной</span><span class="sxs-lookup"><span data-stu-id="71451-238">reason</span></span>           | <span data-ttu-id="71451-239">String</span><span class="sxs-lookup"><span data-stu-id="71451-239">String</span></span>                                                   | <span data-ttu-id="71451-240">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="71451-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="71451-241">schedule</span><span class="sxs-lookup"><span data-stu-id="71451-241">schedule</span></span>         | [<span data-ttu-id="71451-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="71451-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="71451-243">Да</span><span class="sxs-lookup"><span data-stu-id="71451-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="71451-244">Запрос</span><span class="sxs-lookup"><span data-stu-id="71451-244">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="71451-245">HTTP</span><span class="sxs-lookup"><span data-stu-id="71451-245">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="71451-246">C#</span><span class="sxs-lookup"><span data-stu-id="71451-246">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="71451-247">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71451-247">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="71451-248">Цель — C</span><span class="sxs-lookup"><span data-stu-id="71451-248">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="71451-249">Отклик</span><span class="sxs-lookup"><span data-stu-id="71451-249">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="71451-250">Пример 2: пользователь активирует подходящие роли</span><span class="sxs-lookup"><span data-stu-id="71451-250">Example 2: User activates eligible role</span></span>

<span data-ttu-id="71451-251">В этом примере пользователь nawu@fimdev.net активирует соответствующую роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="71451-251">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="71451-252">Свойство</span><span class="sxs-lookup"><span data-stu-id="71451-252">Property</span></span>         | <span data-ttu-id="71451-253">Тип</span><span class="sxs-lookup"><span data-stu-id="71451-253">Type</span></span>                                                     | <span data-ttu-id="71451-254">Обязательный</span><span class="sxs-lookup"><span data-stu-id="71451-254">Required</span></span>                 | <span data-ttu-id="71451-255">Значение</span><span class="sxs-lookup"><span data-stu-id="71451-255">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="71451-256">resourceId</span><span class="sxs-lookup"><span data-stu-id="71451-256">resourceId</span></span>       | <span data-ttu-id="71451-257">String</span><span class="sxs-lookup"><span data-stu-id="71451-257">String</span></span>                                                   | <span data-ttu-id="71451-258">Да</span><span class="sxs-lookup"><span data-stu-id="71451-258">Yes</span></span>                      | <span data-ttu-id="71451-259">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="71451-259">\<resourceId\></span></span> |
| <span data-ttu-id="71451-260">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="71451-260">roleDefinitionId</span></span> | <span data-ttu-id="71451-261">String</span><span class="sxs-lookup"><span data-stu-id="71451-261">String</span></span>                                                   | <span data-ttu-id="71451-262">Да</span><span class="sxs-lookup"><span data-stu-id="71451-262">Yes</span></span>                      | <span data-ttu-id="71451-263">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="71451-263">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="71451-264">субжектид</span><span class="sxs-lookup"><span data-stu-id="71451-264">subjectId</span></span>        | <span data-ttu-id="71451-265">String</span><span class="sxs-lookup"><span data-stu-id="71451-265">String</span></span>                                                   | <span data-ttu-id="71451-266">Да</span><span class="sxs-lookup"><span data-stu-id="71451-266">Yes</span></span>                      | <span data-ttu-id="71451-267">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="71451-267">\<subjectId\></span></span> |
| <span data-ttu-id="71451-268">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="71451-268">assignmentState</span></span>  | <span data-ttu-id="71451-269">String</span><span class="sxs-lookup"><span data-stu-id="71451-269">String</span></span>                                                   | <span data-ttu-id="71451-270">Да</span><span class="sxs-lookup"><span data-stu-id="71451-270">Yes</span></span>                      | <span data-ttu-id="71451-271">Активное</span><span class="sxs-lookup"><span data-stu-id="71451-271">Active</span></span> |
| <span data-ttu-id="71451-272">type</span><span class="sxs-lookup"><span data-stu-id="71451-272">type</span></span>             | <span data-ttu-id="71451-273">String</span><span class="sxs-lookup"><span data-stu-id="71451-273">String</span></span>                                                   | <span data-ttu-id="71451-274">Да</span><span class="sxs-lookup"><span data-stu-id="71451-274">Yes</span></span>                      | <span data-ttu-id="71451-275">усерадд</span><span class="sxs-lookup"><span data-stu-id="71451-275">UserAdd</span></span> |
| <span data-ttu-id="71451-276">причиной</span><span class="sxs-lookup"><span data-stu-id="71451-276">reason</span></span>           | <span data-ttu-id="71451-277">String</span><span class="sxs-lookup"><span data-stu-id="71451-277">String</span></span>                                                   | <span data-ttu-id="71451-278">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="71451-278">depends on role Settings</span></span> |   |
| <span data-ttu-id="71451-279">schedule</span><span class="sxs-lookup"><span data-stu-id="71451-279">schedule</span></span>         | [<span data-ttu-id="71451-280">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="71451-280">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="71451-281">Да</span><span class="sxs-lookup"><span data-stu-id="71451-281">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="71451-282">Запрос</span><span class="sxs-lookup"><span data-stu-id="71451-282">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="71451-283">Отклик</span><span class="sxs-lookup"><span data-stu-id="71451-283">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="71451-284">Пример 3: пользователь отключает назначенную роль</span><span class="sxs-lookup"><span data-stu-id="71451-284">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="71451-285">В этом примере пользователь nawu@fimdev.net отключает активную роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="71451-285">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="71451-286">Свойство</span><span class="sxs-lookup"><span data-stu-id="71451-286">Property</span></span>         | <span data-ttu-id="71451-287">Тип</span><span class="sxs-lookup"><span data-stu-id="71451-287">Type</span></span>                                                     | <span data-ttu-id="71451-288">Обязательный</span><span class="sxs-lookup"><span data-stu-id="71451-288">Required</span></span> | <span data-ttu-id="71451-289">Значение</span><span class="sxs-lookup"><span data-stu-id="71451-289">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="71451-290">resourceId</span><span class="sxs-lookup"><span data-stu-id="71451-290">resourceId</span></span>       | <span data-ttu-id="71451-291">String</span><span class="sxs-lookup"><span data-stu-id="71451-291">String</span></span>                                                   | <span data-ttu-id="71451-292">Да</span><span class="sxs-lookup"><span data-stu-id="71451-292">Yes</span></span>      | <span data-ttu-id="71451-293">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="71451-293">\<resourceId\></span></span> |
| <span data-ttu-id="71451-294">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="71451-294">roleDefinitionId</span></span> | <span data-ttu-id="71451-295">String</span><span class="sxs-lookup"><span data-stu-id="71451-295">String</span></span>                                                   | <span data-ttu-id="71451-296">Да</span><span class="sxs-lookup"><span data-stu-id="71451-296">Yes</span></span>      | <span data-ttu-id="71451-297">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="71451-297">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="71451-298">субжектид</span><span class="sxs-lookup"><span data-stu-id="71451-298">subjectId</span></span>        | <span data-ttu-id="71451-299">String</span><span class="sxs-lookup"><span data-stu-id="71451-299">String</span></span>                                                   | <span data-ttu-id="71451-300">Да</span><span class="sxs-lookup"><span data-stu-id="71451-300">Yes</span></span>      | <span data-ttu-id="71451-301">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="71451-301">\<subjectId\></span></span> |
| <span data-ttu-id="71451-302">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="71451-302">assignmentState</span></span>  | <span data-ttu-id="71451-303">Строка</span><span class="sxs-lookup"><span data-stu-id="71451-303">String</span></span>                                                   | <span data-ttu-id="71451-304">Да</span><span class="sxs-lookup"><span data-stu-id="71451-304">Yes</span></span>      | <span data-ttu-id="71451-305">Активное</span><span class="sxs-lookup"><span data-stu-id="71451-305">Active</span></span> |
| <span data-ttu-id="71451-306">type</span><span class="sxs-lookup"><span data-stu-id="71451-306">type</span></span>             | <span data-ttu-id="71451-307">Строка</span><span class="sxs-lookup"><span data-stu-id="71451-307">String</span></span>                                                   | <span data-ttu-id="71451-308">Да</span><span class="sxs-lookup"><span data-stu-id="71451-308">Yes</span></span>      | <span data-ttu-id="71451-309">усерремове</span><span class="sxs-lookup"><span data-stu-id="71451-309">UserRemove</span></span> |
| <span data-ttu-id="71451-310">причиной</span><span class="sxs-lookup"><span data-stu-id="71451-310">reason</span></span>           | <span data-ttu-id="71451-311">String</span><span class="sxs-lookup"><span data-stu-id="71451-311">String</span></span>                                                   | <span data-ttu-id="71451-312">Нет</span><span class="sxs-lookup"><span data-stu-id="71451-312">No</span></span>       |   |
| <span data-ttu-id="71451-313">schedule</span><span class="sxs-lookup"><span data-stu-id="71451-313">schedule</span></span>         | [<span data-ttu-id="71451-314">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="71451-314">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="71451-315">Нет</span><span class="sxs-lookup"><span data-stu-id="71451-315">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="71451-316">Запрос</span><span class="sxs-lookup"><span data-stu-id="71451-316">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="71451-317">Отклик</span><span class="sxs-lookup"><span data-stu-id="71451-317">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="71451-318">Пример 4: Администратор удаляет пользователя из роли</span><span class="sxs-lookup"><span data-stu-id="71451-318">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="71451-319">В этом примере администратор удаляет пользователя nawu@fimdev.net из роли читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="71451-319">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="71451-320">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="71451-320">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="71451-321">Свойство</span><span class="sxs-lookup"><span data-stu-id="71451-321">Property</span></span>         | <span data-ttu-id="71451-322">Тип</span><span class="sxs-lookup"><span data-stu-id="71451-322">Type</span></span>                                                     | <span data-ttu-id="71451-323">Обязательный</span><span class="sxs-lookup"><span data-stu-id="71451-323">Required</span></span> | <span data-ttu-id="71451-324">Значение</span><span class="sxs-lookup"><span data-stu-id="71451-324">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="71451-325">resourceId</span><span class="sxs-lookup"><span data-stu-id="71451-325">resourceId</span></span>       | <span data-ttu-id="71451-326">String</span><span class="sxs-lookup"><span data-stu-id="71451-326">String</span></span>                                                   | <span data-ttu-id="71451-327">Да</span><span class="sxs-lookup"><span data-stu-id="71451-327">Yes</span></span>      | <span data-ttu-id="71451-328">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="71451-328">\<resourceId\></span></span> |
| <span data-ttu-id="71451-329">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="71451-329">roleDefinitionId</span></span> | <span data-ttu-id="71451-330">Строка</span><span class="sxs-lookup"><span data-stu-id="71451-330">String</span></span>                                                   | <span data-ttu-id="71451-331">Да</span><span class="sxs-lookup"><span data-stu-id="71451-331">Yes</span></span>      | <span data-ttu-id="71451-332">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="71451-332">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="71451-333">субжектид</span><span class="sxs-lookup"><span data-stu-id="71451-333">subjectId</span></span>        | <span data-ttu-id="71451-334">Строка</span><span class="sxs-lookup"><span data-stu-id="71451-334">String</span></span>                                                   | <span data-ttu-id="71451-335">Да</span><span class="sxs-lookup"><span data-stu-id="71451-335">Yes</span></span>      | <span data-ttu-id="71451-336">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="71451-336">\<subjectId\></span></span> |
| <span data-ttu-id="71451-337">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="71451-337">assignmentState</span></span>  | <span data-ttu-id="71451-338">Строка</span><span class="sxs-lookup"><span data-stu-id="71451-338">String</span></span>                                                   | <span data-ttu-id="71451-339">Да</span><span class="sxs-lookup"><span data-stu-id="71451-339">Yes</span></span>      | <span data-ttu-id="71451-340">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="71451-340">Eligible / Active</span></span> |
| <span data-ttu-id="71451-341">type</span><span class="sxs-lookup"><span data-stu-id="71451-341">type</span></span>             | <span data-ttu-id="71451-342">Строка</span><span class="sxs-lookup"><span data-stu-id="71451-342">String</span></span>                                                   | <span data-ttu-id="71451-343">Да</span><span class="sxs-lookup"><span data-stu-id="71451-343">Yes</span></span>      | <span data-ttu-id="71451-344">админремове</span><span class="sxs-lookup"><span data-stu-id="71451-344">AdminRemove</span></span> |
| <span data-ttu-id="71451-345">причиной</span><span class="sxs-lookup"><span data-stu-id="71451-345">reason</span></span>           | <span data-ttu-id="71451-346">String</span><span class="sxs-lookup"><span data-stu-id="71451-346">String</span></span>                                                   | <span data-ttu-id="71451-347">Нет</span><span class="sxs-lookup"><span data-stu-id="71451-347">No</span></span>       |   |
| <span data-ttu-id="71451-348">schedule</span><span class="sxs-lookup"><span data-stu-id="71451-348">schedule</span></span>         | [<span data-ttu-id="71451-349">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="71451-349">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="71451-350">Нет</span><span class="sxs-lookup"><span data-stu-id="71451-350">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="71451-351">Запрос</span><span class="sxs-lookup"><span data-stu-id="71451-351">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="71451-352">Отклик</span><span class="sxs-lookup"><span data-stu-id="71451-352">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="71451-353">Пример 5: "Администратор обновляет назначение ролей"</span><span class="sxs-lookup"><span data-stu-id="71451-353">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="71451-354">В этом примере администраторы обновляют назначение роли пользователя nawu@fimdev.net владельцу.</span><span class="sxs-lookup"><span data-stu-id="71451-354">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="71451-355">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="71451-355">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="71451-356">Свойство</span><span class="sxs-lookup"><span data-stu-id="71451-356">Property</span></span>         | <span data-ttu-id="71451-357">Тип</span><span class="sxs-lookup"><span data-stu-id="71451-357">Type</span></span>                                                     | <span data-ttu-id="71451-358">Обязательный</span><span class="sxs-lookup"><span data-stu-id="71451-358">Required</span></span>                | <span data-ttu-id="71451-359">Значение</span><span class="sxs-lookup"><span data-stu-id="71451-359">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="71451-360">resourceId</span><span class="sxs-lookup"><span data-stu-id="71451-360">resourceId</span></span>       | <span data-ttu-id="71451-361">String</span><span class="sxs-lookup"><span data-stu-id="71451-361">String</span></span>                                                   | <span data-ttu-id="71451-362">Да</span><span class="sxs-lookup"><span data-stu-id="71451-362">Yes</span></span>                     | <span data-ttu-id="71451-363">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="71451-363">\<resourceId\></span></span> |
| <span data-ttu-id="71451-364">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="71451-364">roleDefinitionId</span></span> | <span data-ttu-id="71451-365">Строка</span><span class="sxs-lookup"><span data-stu-id="71451-365">String</span></span>                                                   | <span data-ttu-id="71451-366">Да</span><span class="sxs-lookup"><span data-stu-id="71451-366">Yes</span></span>                     | <span data-ttu-id="71451-367">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="71451-367">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="71451-368">субжектид</span><span class="sxs-lookup"><span data-stu-id="71451-368">subjectId</span></span>        | <span data-ttu-id="71451-369">Строка</span><span class="sxs-lookup"><span data-stu-id="71451-369">String</span></span>                                                   | <span data-ttu-id="71451-370">Да</span><span class="sxs-lookup"><span data-stu-id="71451-370">Yes</span></span>                     | <span data-ttu-id="71451-371">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="71451-371">\<subjectId\></span></span> |
| <span data-ttu-id="71451-372">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="71451-372">assignmentState</span></span>  | <span data-ttu-id="71451-373">Строка</span><span class="sxs-lookup"><span data-stu-id="71451-373">String</span></span>                                                   | <span data-ttu-id="71451-374">Да</span><span class="sxs-lookup"><span data-stu-id="71451-374">Yes</span></span>                     | <span data-ttu-id="71451-375">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="71451-375">Eligible / Active</span></span> |
| <span data-ttu-id="71451-376">type</span><span class="sxs-lookup"><span data-stu-id="71451-376">type</span></span>             | <span data-ttu-id="71451-377">Строка</span><span class="sxs-lookup"><span data-stu-id="71451-377">String</span></span>                                                   | <span data-ttu-id="71451-378">Да</span><span class="sxs-lookup"><span data-stu-id="71451-378">Yes</span></span>                     | <span data-ttu-id="71451-379">админупдате</span><span class="sxs-lookup"><span data-stu-id="71451-379">AdminUpdate</span></span> |
| <span data-ttu-id="71451-380">причиной</span><span class="sxs-lookup"><span data-stu-id="71451-380">reason</span></span>           | <span data-ttu-id="71451-381">String</span><span class="sxs-lookup"><span data-stu-id="71451-381">String</span></span>                                                   | <span data-ttu-id="71451-382">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="71451-382">depends on roleSettings</span></span> |   |
| <span data-ttu-id="71451-383">schedule</span><span class="sxs-lookup"><span data-stu-id="71451-383">schedule</span></span>         | [<span data-ttu-id="71451-384">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="71451-384">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="71451-385">Да</span><span class="sxs-lookup"><span data-stu-id="71451-385">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="71451-386">Запрос</span><span class="sxs-lookup"><span data-stu-id="71451-386">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="71451-387">Отклик</span><span class="sxs-lookup"><span data-stu-id="71451-387">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="71451-388">Пример 6: администратор расширяет назначение ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="71451-388">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="71451-389">В этом примере показано, как расширить назначение роли истечения срока действия для пользователя АНУЖКУСЕР участнику службы управления API.</span><span class="sxs-lookup"><span data-stu-id="71451-389">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="71451-390">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="71451-390">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="71451-391">Свойство</span><span class="sxs-lookup"><span data-stu-id="71451-391">Property</span></span>         | <span data-ttu-id="71451-392">Тип</span><span class="sxs-lookup"><span data-stu-id="71451-392">Type</span></span>                                                     | <span data-ttu-id="71451-393">Обязательный</span><span class="sxs-lookup"><span data-stu-id="71451-393">Required</span></span>                | <span data-ttu-id="71451-394">Значение</span><span class="sxs-lookup"><span data-stu-id="71451-394">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="71451-395">resourceId</span><span class="sxs-lookup"><span data-stu-id="71451-395">resourceId</span></span>       | <span data-ttu-id="71451-396">String</span><span class="sxs-lookup"><span data-stu-id="71451-396">String</span></span>                                                   | <span data-ttu-id="71451-397">Да</span><span class="sxs-lookup"><span data-stu-id="71451-397">Yes</span></span>                     | <span data-ttu-id="71451-398">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="71451-398">\<resourceId\></span></span> |
| <span data-ttu-id="71451-399">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="71451-399">roleDefinitionId</span></span> | <span data-ttu-id="71451-400">Строка</span><span class="sxs-lookup"><span data-stu-id="71451-400">String</span></span>                                                   | <span data-ttu-id="71451-401">Да</span><span class="sxs-lookup"><span data-stu-id="71451-401">Yes</span></span>                     | <span data-ttu-id="71451-402">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="71451-402">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="71451-403">субжектид</span><span class="sxs-lookup"><span data-stu-id="71451-403">subjectId</span></span>        | <span data-ttu-id="71451-404">String</span><span class="sxs-lookup"><span data-stu-id="71451-404">String</span></span>                                                   | <span data-ttu-id="71451-405">Да</span><span class="sxs-lookup"><span data-stu-id="71451-405">Yes</span></span>                     | <span data-ttu-id="71451-406">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="71451-406">\<subjectId\></span></span> |
| <span data-ttu-id="71451-407">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="71451-407">assignmentState</span></span>  | <span data-ttu-id="71451-408">String</span><span class="sxs-lookup"><span data-stu-id="71451-408">String</span></span>                                                   | <span data-ttu-id="71451-409">Да</span><span class="sxs-lookup"><span data-stu-id="71451-409">Yes</span></span>                     | <span data-ttu-id="71451-410">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="71451-410">Eligible / Active</span></span> |
| <span data-ttu-id="71451-411">type</span><span class="sxs-lookup"><span data-stu-id="71451-411">type</span></span>             | <span data-ttu-id="71451-412">String</span><span class="sxs-lookup"><span data-stu-id="71451-412">String</span></span>                                                   | <span data-ttu-id="71451-413">Да</span><span class="sxs-lookup"><span data-stu-id="71451-413">Yes</span></span>                     | <span data-ttu-id="71451-414">админекстенд</span><span class="sxs-lookup"><span data-stu-id="71451-414">AdminExtend</span></span> |
| <span data-ttu-id="71451-415">причиной</span><span class="sxs-lookup"><span data-stu-id="71451-415">reason</span></span>           | <span data-ttu-id="71451-416">String</span><span class="sxs-lookup"><span data-stu-id="71451-416">String</span></span>                                                   | <span data-ttu-id="71451-417">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="71451-417">depends on roleSettings</span></span> |   |
| <span data-ttu-id="71451-418">schedule</span><span class="sxs-lookup"><span data-stu-id="71451-418">schedule</span></span>         | [<span data-ttu-id="71451-419">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="71451-419">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="71451-420">Да</span><span class="sxs-lookup"><span data-stu-id="71451-420">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="71451-421">Запрос</span><span class="sxs-lookup"><span data-stu-id="71451-421">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="71451-422">Отклик</span><span class="sxs-lookup"><span data-stu-id="71451-422">Response</span></span>

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
