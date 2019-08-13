---
title: Создание governanceRoleAssignmentRequest
description: Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли. В приведенной ниже таблице перечислены операции.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 7a97d5455da11db666bbd7a53f2453ed10610735
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323593"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="f092b-104">Создание governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f092b-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f092b-105">Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="f092b-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="f092b-106">В приведенной ниже таблице перечислены операции.</span><span class="sxs-lookup"><span data-stu-id="f092b-106">The following table lists the operations.</span></span>

| <span data-ttu-id="f092b-107">Operation</span><span class="sxs-lookup"><span data-stu-id="f092b-107">Operation</span></span>                                   | <span data-ttu-id="f092b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f092b-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="f092b-109">Назначение роли</span><span class="sxs-lookup"><span data-stu-id="f092b-109">Assign a role assignment</span></span>                    | <span data-ttu-id="f092b-110">админадд</span><span class="sxs-lookup"><span data-stu-id="f092b-110">AdminAdd</span></span>    |
| <span data-ttu-id="f092b-111">Активация подходящего назначения роли</span><span class="sxs-lookup"><span data-stu-id="f092b-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="f092b-112">усерадд</span><span class="sxs-lookup"><span data-stu-id="f092b-112">UserAdd</span></span>     |
| <span data-ttu-id="f092b-113">Деактивация активированного назначения роли</span><span class="sxs-lookup"><span data-stu-id="f092b-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="f092b-114">усерремове</span><span class="sxs-lookup"><span data-stu-id="f092b-114">UserRemove</span></span>  |
| <span data-ttu-id="f092b-115">Удаление назначения роли</span><span class="sxs-lookup"><span data-stu-id="f092b-115">Remove a role assignment</span></span>                    | <span data-ttu-id="f092b-116">админремове</span><span class="sxs-lookup"><span data-stu-id="f092b-116">AdminRemove</span></span> |
| <span data-ttu-id="f092b-117">Обновление назначения роли</span><span class="sxs-lookup"><span data-stu-id="f092b-117">Update a role assignment</span></span>                    | <span data-ttu-id="f092b-118">админупдате</span><span class="sxs-lookup"><span data-stu-id="f092b-118">AdminUpdate</span></span> |
| <span data-ttu-id="f092b-119">Запрос на расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="f092b-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="f092b-120">усерекстенд</span><span class="sxs-lookup"><span data-stu-id="f092b-120">UserExtend</span></span>  |
| <span data-ttu-id="f092b-121">Расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="f092b-121">Extend a role assignment</span></span>                    | <span data-ttu-id="f092b-122">админекстенд</span><span class="sxs-lookup"><span data-stu-id="f092b-122">AdminExtend</span></span> |
| <span data-ttu-id="f092b-123">Запрос на продление назначения роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="f092b-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="f092b-124">усерренев</span><span class="sxs-lookup"><span data-stu-id="f092b-124">UserRenew</span></span>   |
| <span data-ttu-id="f092b-125">Продление назначенной роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="f092b-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="f092b-126">админренев</span><span class="sxs-lookup"><span data-stu-id="f092b-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="f092b-127">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f092b-127">Permissions</span></span>

<span data-ttu-id="f092b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f092b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f092b-130">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f092b-130">Permission type</span></span>                        | <span data-ttu-id="f092b-131">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f092b-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="f092b-132">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f092b-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="f092b-133">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="f092b-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="f092b-134">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f092b-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f092b-135">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f092b-135">Not supported.</span></span>                            |
| <span data-ttu-id="f092b-136">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f092b-136">Application</span></span>                            | <span data-ttu-id="f092b-137">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f092b-137">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f092b-138">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f092b-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="f092b-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f092b-139">Request headers</span></span>

| <span data-ttu-id="f092b-140">Имя</span><span class="sxs-lookup"><span data-stu-id="f092b-140">Name</span></span>          | <span data-ttu-id="f092b-141">Описание</span><span class="sxs-lookup"><span data-stu-id="f092b-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="f092b-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f092b-142">Authorization</span></span> | <span data-ttu-id="f092b-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f092b-143">Bearer {code}</span></span>    |
| <span data-ttu-id="f092b-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f092b-144">Content-type</span></span>  | <span data-ttu-id="f092b-145">application/json</span><span class="sxs-lookup"><span data-stu-id="f092b-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f092b-146">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f092b-146">Request body</span></span>

<span data-ttu-id="f092b-147">В тексте запроса добавьте представление объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f092b-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="f092b-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="f092b-148">Property</span></span>         | <span data-ttu-id="f092b-149">Тип</span><span class="sxs-lookup"><span data-stu-id="f092b-149">Type</span></span>                                                     | <span data-ttu-id="f092b-150">Описание</span><span class="sxs-lookup"><span data-stu-id="f092b-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="f092b-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="f092b-151">resourceId</span></span>       | <span data-ttu-id="f092b-152">String</span><span class="sxs-lookup"><span data-stu-id="f092b-152">String</span></span>                                                   | <span data-ttu-id="f092b-153">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="f092b-153">The ID of the resource.</span></span> <span data-ttu-id="f092b-154">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f092b-154">Required.</span></span> |
| <span data-ttu-id="f092b-155">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="f092b-155">roleDefinitionId</span></span> | <span data-ttu-id="f092b-156">String</span><span class="sxs-lookup"><span data-stu-id="f092b-156">String</span></span>                                                   | <span data-ttu-id="f092b-157">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="f092b-157">The ID of the role definition.</span></span> <span data-ttu-id="f092b-158">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f092b-158">Required.</span></span> |
| <span data-ttu-id="f092b-159">субжектид</span><span class="sxs-lookup"><span data-stu-id="f092b-159">subjectId</span></span>        | <span data-ttu-id="f092b-160">String</span><span class="sxs-lookup"><span data-stu-id="f092b-160">String</span></span>                                                   | <span data-ttu-id="f092b-161">ИДЕНТИФИКАТОР субъекта.</span><span class="sxs-lookup"><span data-stu-id="f092b-161">The ID of the subject.</span></span> <span data-ttu-id="f092b-162">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f092b-162">Required.</span></span> |
| <span data-ttu-id="f092b-163">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="f092b-163">assignmentState</span></span>  | <span data-ttu-id="f092b-164">String</span><span class="sxs-lookup"><span data-stu-id="f092b-164">String</span></span>                                                   | <span data-ttu-id="f092b-165">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="f092b-165">The state of assignment.</span></span> <span data-ttu-id="f092b-166">Значение может быть `Eligible` и `Active`.</span><span class="sxs-lookup"><span data-stu-id="f092b-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="f092b-167">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="f092b-167">Required.</span></span> |
| <span data-ttu-id="f092b-168">type</span><span class="sxs-lookup"><span data-stu-id="f092b-168">type</span></span>             | <span data-ttu-id="f092b-169">String</span><span class="sxs-lookup"><span data-stu-id="f092b-169">String</span></span>                                                   | <span data-ttu-id="f092b-170">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="f092b-170">The request type.</span></span> <span data-ttu-id="f092b-171">Возможные значения: `AdminAdd`, `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `AdminRenew` `AdminExtend`,,,,, и. `UserExtend` `UserRenew`</span><span class="sxs-lookup"><span data-stu-id="f092b-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="f092b-172">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f092b-172">Required.</span></span> |
| <span data-ttu-id="f092b-173">причиной</span><span class="sxs-lookup"><span data-stu-id="f092b-173">reason</span></span>           | <span data-ttu-id="f092b-174">String</span><span class="sxs-lookup"><span data-stu-id="f092b-174">String</span></span>                                                   | <span data-ttu-id="f092b-175">Необходимо указать причину для запроса на назначение роли для аудита и проверки.</span><span class="sxs-lookup"><span data-stu-id="f092b-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="f092b-176">schedule</span><span class="sxs-lookup"><span data-stu-id="f092b-176">schedule</span></span>         | [<span data-ttu-id="f092b-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f092b-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="f092b-178">Расписание запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="f092b-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="f092b-179">`UserAdd`Для типа запроса `AdminAdd`,, `AdminUpdate`, и `AdminExtend`, он необходим.</span><span class="sxs-lookup"><span data-stu-id="f092b-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="f092b-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="f092b-180">Response</span></span>

<span data-ttu-id="f092b-181">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f092b-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="f092b-182">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="f092b-182">Error codes</span></span>

<span data-ttu-id="f092b-183">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="f092b-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="f092b-184">Кроме того, он возвращает коды ошибок, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="f092b-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="f092b-185">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="f092b-185">Error code</span></span>     | <span data-ttu-id="f092b-186">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="f092b-186">Error message</span></span>                               | <span data-ttu-id="f092b-187">Сведения</span><span class="sxs-lookup"><span data-stu-id="f092b-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="f092b-188">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="f092b-188">400 BadRequest</span></span> | <span data-ttu-id="f092b-189">роленотфаунд</span><span class="sxs-lookup"><span data-stu-id="f092b-189">RoleNotFound</span></span>                                | <span data-ttu-id="f092b-190">Не `roleDefinitionId` удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="f092b-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="f092b-191">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="f092b-191">400 BadRequest</span></span> | <span data-ttu-id="f092b-192">ресаурцеислоккед</span><span class="sxs-lookup"><span data-stu-id="f092b-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="f092b-193">Ресурс, указанный в теле запроса, находится в состоянии `Locked` и не может создавать запросы на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="f092b-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="f092b-194">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="f092b-194">400 BadRequest</span></span> | <span data-ttu-id="f092b-195">субжектнотфаунд</span><span class="sxs-lookup"><span data-stu-id="f092b-195">SubjectNotFound</span></span>                             | <span data-ttu-id="f092b-196">Не `subjectId` удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="f092b-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="f092b-197">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="f092b-197">400 BadRequest</span></span> | <span data-ttu-id="f092b-198">пендингролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="f092b-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="f092b-199">В системе уже существует ожидающий [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="f092b-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="f092b-200">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="f092b-200">400 BadRequest</span></span> | <span data-ttu-id="f092b-201">ролеассигнментексистс</span><span class="sxs-lookup"><span data-stu-id="f092b-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="f092b-202">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , который требуется создать, уже существует в системе.</span><span class="sxs-lookup"><span data-stu-id="f092b-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="f092b-203">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="f092b-203">400 BadRequest</span></span> | <span data-ttu-id="f092b-204">ролеассигнментдоеснотексист</span><span class="sxs-lookup"><span data-stu-id="f092b-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="f092b-205">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , запрошенный для обновления или расширения, не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="f092b-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="f092b-206">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="f092b-206">400 BadRequest</span></span> | <span data-ttu-id="f092b-207">ролеассигнментрекуестполицивалидатионфаилед</span><span class="sxs-lookup"><span data-stu-id="f092b-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="f092b-208">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) не отвечает внутренним политикам и не может быть создан.</span><span class="sxs-lookup"><span data-stu-id="f092b-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="f092b-209">Примеры</span><span class="sxs-lookup"><span data-stu-id="f092b-209">Examples</span></span>

<span data-ttu-id="f092b-210">В следующих примерах показано, как использовать этот API.</span><span class="sxs-lookup"><span data-stu-id="f092b-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="f092b-211">Пример 1: Администратор назначает пользователю роль</span><span class="sxs-lookup"><span data-stu-id="f092b-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="f092b-212">В этом примере администратор назначает пользователю nawu@fimdev.net роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="f092b-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="f092b-213">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="f092b-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="f092b-214">Свойство</span><span class="sxs-lookup"><span data-stu-id="f092b-214">Property</span></span>         | <span data-ttu-id="f092b-215">Тип</span><span class="sxs-lookup"><span data-stu-id="f092b-215">Type</span></span>                                                     | <span data-ttu-id="f092b-216">Обязательный</span><span class="sxs-lookup"><span data-stu-id="f092b-216">Required</span></span>                 | <span data-ttu-id="f092b-217">Значение</span><span class="sxs-lookup"><span data-stu-id="f092b-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="f092b-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="f092b-218">resourceId</span></span>       | <span data-ttu-id="f092b-219">String</span><span class="sxs-lookup"><span data-stu-id="f092b-219">String</span></span>                                                   | <span data-ttu-id="f092b-220">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-220">Yes</span></span>                      | <span data-ttu-id="f092b-221">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="f092b-221">\<resourceId\></span></span> |
| <span data-ttu-id="f092b-222">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="f092b-222">roleDefinitionId</span></span> | <span data-ttu-id="f092b-223">String</span><span class="sxs-lookup"><span data-stu-id="f092b-223">String</span></span>                                                   | <span data-ttu-id="f092b-224">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-224">Yes</span></span>                      | <span data-ttu-id="f092b-225">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="f092b-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="f092b-226">субжектид</span><span class="sxs-lookup"><span data-stu-id="f092b-226">subjectId</span></span>        | <span data-ttu-id="f092b-227">String</span><span class="sxs-lookup"><span data-stu-id="f092b-227">String</span></span>                                                   | <span data-ttu-id="f092b-228">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-228">Yes</span></span>                      | <span data-ttu-id="f092b-229">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="f092b-229">\<subjectId\></span></span> |
| <span data-ttu-id="f092b-230">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="f092b-230">assignmentState</span></span>  | <span data-ttu-id="f092b-231">String</span><span class="sxs-lookup"><span data-stu-id="f092b-231">String</span></span>                                                   | <span data-ttu-id="f092b-232">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-232">Yes</span></span>                      | <span data-ttu-id="f092b-233">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="f092b-233">Eligible / Active</span></span> |
| <span data-ttu-id="f092b-234">type</span><span class="sxs-lookup"><span data-stu-id="f092b-234">type</span></span>             | <span data-ttu-id="f092b-235">String</span><span class="sxs-lookup"><span data-stu-id="f092b-235">String</span></span>                                                   | <span data-ttu-id="f092b-236">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-236">Yes</span></span>                      | <span data-ttu-id="f092b-237">админадд</span><span class="sxs-lookup"><span data-stu-id="f092b-237">AdminAdd</span></span> |
| <span data-ttu-id="f092b-238">причиной</span><span class="sxs-lookup"><span data-stu-id="f092b-238">reason</span></span>           | <span data-ttu-id="f092b-239">String</span><span class="sxs-lookup"><span data-stu-id="f092b-239">String</span></span>                                                   | <span data-ttu-id="f092b-240">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="f092b-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="f092b-241">schedule</span><span class="sxs-lookup"><span data-stu-id="f092b-241">schedule</span></span>         | [<span data-ttu-id="f092b-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f092b-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="f092b-243">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="f092b-244">Запрос</span><span class="sxs-lookup"><span data-stu-id="f092b-244">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f092b-245">HTTP</span><span class="sxs-lookup"><span data-stu-id="f092b-245">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f092b-246">C#</span><span class="sxs-lookup"><span data-stu-id="f092b-246">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f092b-247">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f092b-247">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f092b-248">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f092b-248">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f092b-249">Java</span><span class="sxs-lookup"><span data-stu-id="f092b-249">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="f092b-250">Отклик</span><span class="sxs-lookup"><span data-stu-id="f092b-250">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="f092b-251">Пример 2: пользователь активирует подходящие роли</span><span class="sxs-lookup"><span data-stu-id="f092b-251">Example 2: User activates eligible role</span></span>

<span data-ttu-id="f092b-252">В этом примере пользователь nawu@fimdev.net активирует соответствующую роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="f092b-252">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="f092b-253">Свойство</span><span class="sxs-lookup"><span data-stu-id="f092b-253">Property</span></span>         | <span data-ttu-id="f092b-254">Тип</span><span class="sxs-lookup"><span data-stu-id="f092b-254">Type</span></span>                                                     | <span data-ttu-id="f092b-255">Обязательный</span><span class="sxs-lookup"><span data-stu-id="f092b-255">Required</span></span>                 | <span data-ttu-id="f092b-256">Значение</span><span class="sxs-lookup"><span data-stu-id="f092b-256">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="f092b-257">resourceId</span><span class="sxs-lookup"><span data-stu-id="f092b-257">resourceId</span></span>       | <span data-ttu-id="f092b-258">String</span><span class="sxs-lookup"><span data-stu-id="f092b-258">String</span></span>                                                   | <span data-ttu-id="f092b-259">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-259">Yes</span></span>                      | <span data-ttu-id="f092b-260">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="f092b-260">\<resourceId\></span></span> |
| <span data-ttu-id="f092b-261">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="f092b-261">roleDefinitionId</span></span> | <span data-ttu-id="f092b-262">String</span><span class="sxs-lookup"><span data-stu-id="f092b-262">String</span></span>                                                   | <span data-ttu-id="f092b-263">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-263">Yes</span></span>                      | <span data-ttu-id="f092b-264">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="f092b-264">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="f092b-265">субжектид</span><span class="sxs-lookup"><span data-stu-id="f092b-265">subjectId</span></span>        | <span data-ttu-id="f092b-266">String</span><span class="sxs-lookup"><span data-stu-id="f092b-266">String</span></span>                                                   | <span data-ttu-id="f092b-267">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-267">Yes</span></span>                      | <span data-ttu-id="f092b-268">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="f092b-268">\<subjectId\></span></span> |
| <span data-ttu-id="f092b-269">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="f092b-269">assignmentState</span></span>  | <span data-ttu-id="f092b-270">String</span><span class="sxs-lookup"><span data-stu-id="f092b-270">String</span></span>                                                   | <span data-ttu-id="f092b-271">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-271">Yes</span></span>                      | <span data-ttu-id="f092b-272">Активное</span><span class="sxs-lookup"><span data-stu-id="f092b-272">Active</span></span> |
| <span data-ttu-id="f092b-273">type</span><span class="sxs-lookup"><span data-stu-id="f092b-273">type</span></span>             | <span data-ttu-id="f092b-274">String</span><span class="sxs-lookup"><span data-stu-id="f092b-274">String</span></span>                                                   | <span data-ttu-id="f092b-275">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-275">Yes</span></span>                      | <span data-ttu-id="f092b-276">усерадд</span><span class="sxs-lookup"><span data-stu-id="f092b-276">UserAdd</span></span> |
| <span data-ttu-id="f092b-277">причиной</span><span class="sxs-lookup"><span data-stu-id="f092b-277">reason</span></span>           | <span data-ttu-id="f092b-278">String</span><span class="sxs-lookup"><span data-stu-id="f092b-278">String</span></span>                                                   | <span data-ttu-id="f092b-279">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="f092b-279">depends on role Settings</span></span> |   |
| <span data-ttu-id="f092b-280">schedule</span><span class="sxs-lookup"><span data-stu-id="f092b-280">schedule</span></span>         | [<span data-ttu-id="f092b-281">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f092b-281">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="f092b-282">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-282">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="f092b-283">Запрос</span><span class="sxs-lookup"><span data-stu-id="f092b-283">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="f092b-284">Отклик</span><span class="sxs-lookup"><span data-stu-id="f092b-284">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="f092b-285">Пример 3: пользователь отключает назначенную роль</span><span class="sxs-lookup"><span data-stu-id="f092b-285">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="f092b-286">В этом примере пользователь nawu@fimdev.net отключает активную роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="f092b-286">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="f092b-287">Свойство</span><span class="sxs-lookup"><span data-stu-id="f092b-287">Property</span></span>         | <span data-ttu-id="f092b-288">Тип</span><span class="sxs-lookup"><span data-stu-id="f092b-288">Type</span></span>                                                     | <span data-ttu-id="f092b-289">Обязательный</span><span class="sxs-lookup"><span data-stu-id="f092b-289">Required</span></span> | <span data-ttu-id="f092b-290">Значение</span><span class="sxs-lookup"><span data-stu-id="f092b-290">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="f092b-291">resourceId</span><span class="sxs-lookup"><span data-stu-id="f092b-291">resourceId</span></span>       | <span data-ttu-id="f092b-292">String</span><span class="sxs-lookup"><span data-stu-id="f092b-292">String</span></span>                                                   | <span data-ttu-id="f092b-293">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-293">Yes</span></span>      | <span data-ttu-id="f092b-294">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="f092b-294">\<resourceId\></span></span> |
| <span data-ttu-id="f092b-295">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="f092b-295">roleDefinitionId</span></span> | <span data-ttu-id="f092b-296">String</span><span class="sxs-lookup"><span data-stu-id="f092b-296">String</span></span>                                                   | <span data-ttu-id="f092b-297">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-297">Yes</span></span>      | <span data-ttu-id="f092b-298">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="f092b-298">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="f092b-299">субжектид</span><span class="sxs-lookup"><span data-stu-id="f092b-299">subjectId</span></span>        | <span data-ttu-id="f092b-300">String</span><span class="sxs-lookup"><span data-stu-id="f092b-300">String</span></span>                                                   | <span data-ttu-id="f092b-301">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-301">Yes</span></span>      | <span data-ttu-id="f092b-302">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="f092b-302">\<subjectId\></span></span> |
| <span data-ttu-id="f092b-303">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="f092b-303">assignmentState</span></span>  | <span data-ttu-id="f092b-304">Строка</span><span class="sxs-lookup"><span data-stu-id="f092b-304">String</span></span>                                                   | <span data-ttu-id="f092b-305">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-305">Yes</span></span>      | <span data-ttu-id="f092b-306">Активное</span><span class="sxs-lookup"><span data-stu-id="f092b-306">Active</span></span> |
| <span data-ttu-id="f092b-307">type</span><span class="sxs-lookup"><span data-stu-id="f092b-307">type</span></span>             | <span data-ttu-id="f092b-308">Строка</span><span class="sxs-lookup"><span data-stu-id="f092b-308">String</span></span>                                                   | <span data-ttu-id="f092b-309">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-309">Yes</span></span>      | <span data-ttu-id="f092b-310">усерремове</span><span class="sxs-lookup"><span data-stu-id="f092b-310">UserRemove</span></span> |
| <span data-ttu-id="f092b-311">причиной</span><span class="sxs-lookup"><span data-stu-id="f092b-311">reason</span></span>           | <span data-ttu-id="f092b-312">String</span><span class="sxs-lookup"><span data-stu-id="f092b-312">String</span></span>                                                   | <span data-ttu-id="f092b-313">Нет</span><span class="sxs-lookup"><span data-stu-id="f092b-313">No</span></span>       |   |
| <span data-ttu-id="f092b-314">schedule</span><span class="sxs-lookup"><span data-stu-id="f092b-314">schedule</span></span>         | [<span data-ttu-id="f092b-315">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f092b-315">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="f092b-316">Нет</span><span class="sxs-lookup"><span data-stu-id="f092b-316">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="f092b-317">Запрос</span><span class="sxs-lookup"><span data-stu-id="f092b-317">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="f092b-318">Отклик</span><span class="sxs-lookup"><span data-stu-id="f092b-318">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="f092b-319">Пример 4: Администратор удаляет пользователя из роли</span><span class="sxs-lookup"><span data-stu-id="f092b-319">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="f092b-320">В этом примере администратор удаляет пользователя nawu@fimdev.net из роли читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="f092b-320">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="f092b-321">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="f092b-321">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="f092b-322">Свойство</span><span class="sxs-lookup"><span data-stu-id="f092b-322">Property</span></span>         | <span data-ttu-id="f092b-323">Тип</span><span class="sxs-lookup"><span data-stu-id="f092b-323">Type</span></span>                                                     | <span data-ttu-id="f092b-324">Обязательный</span><span class="sxs-lookup"><span data-stu-id="f092b-324">Required</span></span> | <span data-ttu-id="f092b-325">Значение</span><span class="sxs-lookup"><span data-stu-id="f092b-325">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="f092b-326">resourceId</span><span class="sxs-lookup"><span data-stu-id="f092b-326">resourceId</span></span>       | <span data-ttu-id="f092b-327">String</span><span class="sxs-lookup"><span data-stu-id="f092b-327">String</span></span>                                                   | <span data-ttu-id="f092b-328">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-328">Yes</span></span>      | <span data-ttu-id="f092b-329">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="f092b-329">\<resourceId\></span></span> |
| <span data-ttu-id="f092b-330">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="f092b-330">roleDefinitionId</span></span> | <span data-ttu-id="f092b-331">Строка</span><span class="sxs-lookup"><span data-stu-id="f092b-331">String</span></span>                                                   | <span data-ttu-id="f092b-332">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-332">Yes</span></span>      | <span data-ttu-id="f092b-333">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="f092b-333">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="f092b-334">субжектид</span><span class="sxs-lookup"><span data-stu-id="f092b-334">subjectId</span></span>        | <span data-ttu-id="f092b-335">Строка</span><span class="sxs-lookup"><span data-stu-id="f092b-335">String</span></span>                                                   | <span data-ttu-id="f092b-336">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-336">Yes</span></span>      | <span data-ttu-id="f092b-337">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="f092b-337">\<subjectId\></span></span> |
| <span data-ttu-id="f092b-338">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="f092b-338">assignmentState</span></span>  | <span data-ttu-id="f092b-339">Строка</span><span class="sxs-lookup"><span data-stu-id="f092b-339">String</span></span>                                                   | <span data-ttu-id="f092b-340">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-340">Yes</span></span>      | <span data-ttu-id="f092b-341">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="f092b-341">Eligible / Active</span></span> |
| <span data-ttu-id="f092b-342">type</span><span class="sxs-lookup"><span data-stu-id="f092b-342">type</span></span>             | <span data-ttu-id="f092b-343">Строка</span><span class="sxs-lookup"><span data-stu-id="f092b-343">String</span></span>                                                   | <span data-ttu-id="f092b-344">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-344">Yes</span></span>      | <span data-ttu-id="f092b-345">админремове</span><span class="sxs-lookup"><span data-stu-id="f092b-345">AdminRemove</span></span> |
| <span data-ttu-id="f092b-346">причиной</span><span class="sxs-lookup"><span data-stu-id="f092b-346">reason</span></span>           | <span data-ttu-id="f092b-347">String</span><span class="sxs-lookup"><span data-stu-id="f092b-347">String</span></span>                                                   | <span data-ttu-id="f092b-348">Нет</span><span class="sxs-lookup"><span data-stu-id="f092b-348">No</span></span>       |   |
| <span data-ttu-id="f092b-349">schedule</span><span class="sxs-lookup"><span data-stu-id="f092b-349">schedule</span></span>         | [<span data-ttu-id="f092b-350">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f092b-350">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="f092b-351">Нет</span><span class="sxs-lookup"><span data-stu-id="f092b-351">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="f092b-352">Запрос</span><span class="sxs-lookup"><span data-stu-id="f092b-352">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="f092b-353">Отклик</span><span class="sxs-lookup"><span data-stu-id="f092b-353">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="f092b-354">Пример 5: "Администратор обновляет назначение ролей"</span><span class="sxs-lookup"><span data-stu-id="f092b-354">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="f092b-355">В этом примере администраторы обновляют назначение роли пользователя nawu@fimdev.net владельцу.</span><span class="sxs-lookup"><span data-stu-id="f092b-355">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="f092b-356">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="f092b-356">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="f092b-357">Свойство</span><span class="sxs-lookup"><span data-stu-id="f092b-357">Property</span></span>         | <span data-ttu-id="f092b-358">Тип</span><span class="sxs-lookup"><span data-stu-id="f092b-358">Type</span></span>                                                     | <span data-ttu-id="f092b-359">Обязательный</span><span class="sxs-lookup"><span data-stu-id="f092b-359">Required</span></span>                | <span data-ttu-id="f092b-360">Значение</span><span class="sxs-lookup"><span data-stu-id="f092b-360">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="f092b-361">resourceId</span><span class="sxs-lookup"><span data-stu-id="f092b-361">resourceId</span></span>       | <span data-ttu-id="f092b-362">String</span><span class="sxs-lookup"><span data-stu-id="f092b-362">String</span></span>                                                   | <span data-ttu-id="f092b-363">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-363">Yes</span></span>                     | <span data-ttu-id="f092b-364">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="f092b-364">\<resourceId\></span></span> |
| <span data-ttu-id="f092b-365">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="f092b-365">roleDefinitionId</span></span> | <span data-ttu-id="f092b-366">Строка</span><span class="sxs-lookup"><span data-stu-id="f092b-366">String</span></span>                                                   | <span data-ttu-id="f092b-367">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-367">Yes</span></span>                     | <span data-ttu-id="f092b-368">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="f092b-368">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="f092b-369">субжектид</span><span class="sxs-lookup"><span data-stu-id="f092b-369">subjectId</span></span>        | <span data-ttu-id="f092b-370">Строка</span><span class="sxs-lookup"><span data-stu-id="f092b-370">String</span></span>                                                   | <span data-ttu-id="f092b-371">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-371">Yes</span></span>                     | <span data-ttu-id="f092b-372">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="f092b-372">\<subjectId\></span></span> |
| <span data-ttu-id="f092b-373">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="f092b-373">assignmentState</span></span>  | <span data-ttu-id="f092b-374">Строка</span><span class="sxs-lookup"><span data-stu-id="f092b-374">String</span></span>                                                   | <span data-ttu-id="f092b-375">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-375">Yes</span></span>                     | <span data-ttu-id="f092b-376">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="f092b-376">Eligible / Active</span></span> |
| <span data-ttu-id="f092b-377">type</span><span class="sxs-lookup"><span data-stu-id="f092b-377">type</span></span>             | <span data-ttu-id="f092b-378">Строка</span><span class="sxs-lookup"><span data-stu-id="f092b-378">String</span></span>                                                   | <span data-ttu-id="f092b-379">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-379">Yes</span></span>                     | <span data-ttu-id="f092b-380">админупдате</span><span class="sxs-lookup"><span data-stu-id="f092b-380">AdminUpdate</span></span> |
| <span data-ttu-id="f092b-381">причиной</span><span class="sxs-lookup"><span data-stu-id="f092b-381">reason</span></span>           | <span data-ttu-id="f092b-382">String</span><span class="sxs-lookup"><span data-stu-id="f092b-382">String</span></span>                                                   | <span data-ttu-id="f092b-383">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="f092b-383">depends on roleSettings</span></span> |   |
| <span data-ttu-id="f092b-384">schedule</span><span class="sxs-lookup"><span data-stu-id="f092b-384">schedule</span></span>         | [<span data-ttu-id="f092b-385">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f092b-385">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="f092b-386">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-386">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="f092b-387">Запрос</span><span class="sxs-lookup"><span data-stu-id="f092b-387">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="f092b-388">Отклик</span><span class="sxs-lookup"><span data-stu-id="f092b-388">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="f092b-389">Пример 6: администратор расширяет назначение ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="f092b-389">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="f092b-390">В этом примере показано, как расширить назначение роли истечения срока действия для пользователя АНУЖКУСЕР участнику службы управления API.</span><span class="sxs-lookup"><span data-stu-id="f092b-390">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="f092b-391">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="f092b-391">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="f092b-392">Свойство</span><span class="sxs-lookup"><span data-stu-id="f092b-392">Property</span></span>         | <span data-ttu-id="f092b-393">Тип</span><span class="sxs-lookup"><span data-stu-id="f092b-393">Type</span></span>                                                     | <span data-ttu-id="f092b-394">Обязательный</span><span class="sxs-lookup"><span data-stu-id="f092b-394">Required</span></span>                | <span data-ttu-id="f092b-395">Значение</span><span class="sxs-lookup"><span data-stu-id="f092b-395">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="f092b-396">resourceId</span><span class="sxs-lookup"><span data-stu-id="f092b-396">resourceId</span></span>       | <span data-ttu-id="f092b-397">String</span><span class="sxs-lookup"><span data-stu-id="f092b-397">String</span></span>                                                   | <span data-ttu-id="f092b-398">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-398">Yes</span></span>                     | <span data-ttu-id="f092b-399">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="f092b-399">\<resourceId\></span></span> |
| <span data-ttu-id="f092b-400">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="f092b-400">roleDefinitionId</span></span> | <span data-ttu-id="f092b-401">Строка</span><span class="sxs-lookup"><span data-stu-id="f092b-401">String</span></span>                                                   | <span data-ttu-id="f092b-402">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-402">Yes</span></span>                     | <span data-ttu-id="f092b-403">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="f092b-403">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="f092b-404">субжектид</span><span class="sxs-lookup"><span data-stu-id="f092b-404">subjectId</span></span>        | <span data-ttu-id="f092b-405">String</span><span class="sxs-lookup"><span data-stu-id="f092b-405">String</span></span>                                                   | <span data-ttu-id="f092b-406">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-406">Yes</span></span>                     | <span data-ttu-id="f092b-407">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="f092b-407">\<subjectId\></span></span> |
| <span data-ttu-id="f092b-408">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="f092b-408">assignmentState</span></span>  | <span data-ttu-id="f092b-409">String</span><span class="sxs-lookup"><span data-stu-id="f092b-409">String</span></span>                                                   | <span data-ttu-id="f092b-410">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-410">Yes</span></span>                     | <span data-ttu-id="f092b-411">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="f092b-411">Eligible / Active</span></span> |
| <span data-ttu-id="f092b-412">type</span><span class="sxs-lookup"><span data-stu-id="f092b-412">type</span></span>             | <span data-ttu-id="f092b-413">String</span><span class="sxs-lookup"><span data-stu-id="f092b-413">String</span></span>                                                   | <span data-ttu-id="f092b-414">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-414">Yes</span></span>                     | <span data-ttu-id="f092b-415">админекстенд</span><span class="sxs-lookup"><span data-stu-id="f092b-415">AdminExtend</span></span> |
| <span data-ttu-id="f092b-416">причиной</span><span class="sxs-lookup"><span data-stu-id="f092b-416">reason</span></span>           | <span data-ttu-id="f092b-417">String</span><span class="sxs-lookup"><span data-stu-id="f092b-417">String</span></span>                                                   | <span data-ttu-id="f092b-418">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="f092b-418">depends on roleSettings</span></span> |   |
| <span data-ttu-id="f092b-419">schedule</span><span class="sxs-lookup"><span data-stu-id="f092b-419">schedule</span></span>         | [<span data-ttu-id="f092b-420">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f092b-420">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="f092b-421">Да</span><span class="sxs-lookup"><span data-stu-id="f092b-421">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="f092b-422">Запрос</span><span class="sxs-lookup"><span data-stu-id="f092b-422">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="f092b-423">Отклик</span><span class="sxs-lookup"><span data-stu-id="f092b-423">Response</span></span>

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
