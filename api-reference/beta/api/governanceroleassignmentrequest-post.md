---
title: Создание governanceRoleAssignmentRequest
description: Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли. В приведенной ниже таблице перечислены операции.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 7bff2d2ae8e6a122621e3d17de7f7acc3f4e24df
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991112"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="76697-104">Создание governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="76697-104">Create governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="76697-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76697-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76697-106">Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="76697-106">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="76697-107">В приведенной ниже таблице перечислены операции.</span><span class="sxs-lookup"><span data-stu-id="76697-107">The following table lists the operations.</span></span>

| <span data-ttu-id="76697-108">Операция</span><span class="sxs-lookup"><span data-stu-id="76697-108">Operation</span></span>                                   | <span data-ttu-id="76697-109">Тип</span><span class="sxs-lookup"><span data-stu-id="76697-109">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="76697-110">Назначение роли</span><span class="sxs-lookup"><span data-stu-id="76697-110">Assign a role assignment</span></span>                    | <span data-ttu-id="76697-111">админадд</span><span class="sxs-lookup"><span data-stu-id="76697-111">AdminAdd</span></span>    |
| <span data-ttu-id="76697-112">Активация подходящего назначения роли</span><span class="sxs-lookup"><span data-stu-id="76697-112">Activate an eligible role assignment</span></span>        | <span data-ttu-id="76697-113">усерадд</span><span class="sxs-lookup"><span data-stu-id="76697-113">UserAdd</span></span>     |
| <span data-ttu-id="76697-114">Деактивация активированного назначения роли</span><span class="sxs-lookup"><span data-stu-id="76697-114">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="76697-115">усерремове</span><span class="sxs-lookup"><span data-stu-id="76697-115">UserRemove</span></span>  |
| <span data-ttu-id="76697-116">Удаление назначения роли</span><span class="sxs-lookup"><span data-stu-id="76697-116">Remove a role assignment</span></span>                    | <span data-ttu-id="76697-117">админремове</span><span class="sxs-lookup"><span data-stu-id="76697-117">AdminRemove</span></span> |
| <span data-ttu-id="76697-118">Обновление назначения роли</span><span class="sxs-lookup"><span data-stu-id="76697-118">Update a role assignment</span></span>                    | <span data-ttu-id="76697-119">админупдате</span><span class="sxs-lookup"><span data-stu-id="76697-119">AdminUpdate</span></span> |
| <span data-ttu-id="76697-120">Запрос на расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="76697-120">Request to extend my role assignment</span></span>        | <span data-ttu-id="76697-121">усерекстенд</span><span class="sxs-lookup"><span data-stu-id="76697-121">UserExtend</span></span>  |
| <span data-ttu-id="76697-122">Расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="76697-122">Extend a role assignment</span></span>                    | <span data-ttu-id="76697-123">админекстенд</span><span class="sxs-lookup"><span data-stu-id="76697-123">AdminExtend</span></span> |
| <span data-ttu-id="76697-124">Запрос на продление назначения роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="76697-124">Request to renew my expired role assignment</span></span> | <span data-ttu-id="76697-125">усерренев</span><span class="sxs-lookup"><span data-stu-id="76697-125">UserRenew</span></span>   |
| <span data-ttu-id="76697-126">Продление назначенной роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="76697-126">Renew an expired role assignment</span></span>            | <span data-ttu-id="76697-127">админренев</span><span class="sxs-lookup"><span data-stu-id="76697-127">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="76697-128">Разрешения</span><span class="sxs-lookup"><span data-stu-id="76697-128">Permissions</span></span>

<span data-ttu-id="76697-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76697-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="76697-131">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76697-131">Permission type</span></span>                        | <span data-ttu-id="76697-132">Разрешения</span><span class="sxs-lookup"><span data-stu-id="76697-132">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="76697-133">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76697-133">Delegated (work or school account)</span></span>     | <span data-ttu-id="76697-134">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="76697-134">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="76697-135">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76697-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76697-136">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76697-136">Not supported.</span></span>                            |
| <span data-ttu-id="76697-137">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76697-137">Application</span></span>                            | <span data-ttu-id="76697-138">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76697-138">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="76697-139">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76697-139">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="76697-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="76697-140">Request headers</span></span>

| <span data-ttu-id="76697-141">Имя</span><span class="sxs-lookup"><span data-stu-id="76697-141">Name</span></span>          | <span data-ttu-id="76697-142">Описание</span><span class="sxs-lookup"><span data-stu-id="76697-142">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="76697-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76697-143">Authorization</span></span> | <span data-ttu-id="76697-144">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="76697-144">Bearer {code}</span></span>    |
| <span data-ttu-id="76697-145">Content-Type</span><span class="sxs-lookup"><span data-stu-id="76697-145">Content-type</span></span>  | <span data-ttu-id="76697-146">application/json</span><span class="sxs-lookup"><span data-stu-id="76697-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="76697-147">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="76697-147">Request body</span></span>

<span data-ttu-id="76697-148">В тексте запроса добавьте представление объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76697-148">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="76697-149">Свойство</span><span class="sxs-lookup"><span data-stu-id="76697-149">Property</span></span>         | <span data-ttu-id="76697-150">Тип</span><span class="sxs-lookup"><span data-stu-id="76697-150">Type</span></span>                                                     | <span data-ttu-id="76697-151">Описание</span><span class="sxs-lookup"><span data-stu-id="76697-151">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="76697-152">resourceId</span><span class="sxs-lookup"><span data-stu-id="76697-152">resourceId</span></span>       | <span data-ttu-id="76697-153">String</span><span class="sxs-lookup"><span data-stu-id="76697-153">String</span></span>                                                   | <span data-ttu-id="76697-154">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="76697-154">The ID of the resource.</span></span> <span data-ttu-id="76697-155">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="76697-155">Required.</span></span> |
| <span data-ttu-id="76697-156">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="76697-156">roleDefinitionId</span></span> | <span data-ttu-id="76697-157">String</span><span class="sxs-lookup"><span data-stu-id="76697-157">String</span></span>                                                   | <span data-ttu-id="76697-158">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="76697-158">The ID of the role definition.</span></span> <span data-ttu-id="76697-159">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="76697-159">Required.</span></span> |
| <span data-ttu-id="76697-160">субжектид</span><span class="sxs-lookup"><span data-stu-id="76697-160">subjectId</span></span>        | <span data-ttu-id="76697-161">String</span><span class="sxs-lookup"><span data-stu-id="76697-161">String</span></span>                                                   | <span data-ttu-id="76697-162">ИДЕНТИФИКАТОР субъекта.</span><span class="sxs-lookup"><span data-stu-id="76697-162">The ID of the subject.</span></span> <span data-ttu-id="76697-163">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="76697-163">Required.</span></span> |
| <span data-ttu-id="76697-164">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="76697-164">assignmentState</span></span>  | <span data-ttu-id="76697-165">String</span><span class="sxs-lookup"><span data-stu-id="76697-165">String</span></span>                                                   | <span data-ttu-id="76697-166">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="76697-166">The state of assignment.</span></span> <span data-ttu-id="76697-167">Значение может быть `Eligible` и `Active` .</span><span class="sxs-lookup"><span data-stu-id="76697-167">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="76697-168">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="76697-168">Required.</span></span> |
| <span data-ttu-id="76697-169">type</span><span class="sxs-lookup"><span data-stu-id="76697-169">type</span></span>             | <span data-ttu-id="76697-170">String</span><span class="sxs-lookup"><span data-stu-id="76697-170">String</span></span>                                                   | <span data-ttu-id="76697-171">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="76697-171">The request type.</span></span> <span data-ttu-id="76697-172">Возможные значения:,,,,,, `AdminAdd` `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `UserRenew` `AdminRenew` и `AdminExtend` .</span><span class="sxs-lookup"><span data-stu-id="76697-172">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="76697-173">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="76697-173">Required.</span></span> |
| <span data-ttu-id="76697-174">reason</span><span class="sxs-lookup"><span data-stu-id="76697-174">reason</span></span>           | <span data-ttu-id="76697-175">String</span><span class="sxs-lookup"><span data-stu-id="76697-175">String</span></span>                                                   | <span data-ttu-id="76697-176">Необходимо указать причину для запроса на назначение роли для аудита и проверки.</span><span class="sxs-lookup"><span data-stu-id="76697-176">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="76697-177">schedule</span><span class="sxs-lookup"><span data-stu-id="76697-177">schedule</span></span>         | [<span data-ttu-id="76697-178">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="76697-178">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="76697-179">Расписание запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="76697-179">The schedule of the role assignment request.</span></span> <span data-ttu-id="76697-180">Для типа запроса `UserAdd` ,, `AdminAdd` `AdminUpdate` , и `AdminExtend` , он необходим.</span><span class="sxs-lookup"><span data-stu-id="76697-180">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="76697-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="76697-181">Response</span></span>

<span data-ttu-id="76697-182">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="76697-182">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="76697-183">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="76697-183">Error codes</span></span>

<span data-ttu-id="76697-184">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="76697-184">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="76697-185">Кроме того, он возвращает коды ошибок, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="76697-185">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="76697-186">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="76697-186">Error code</span></span>     | <span data-ttu-id="76697-187">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="76697-187">Error message</span></span>                               | <span data-ttu-id="76697-188">Сведения</span><span class="sxs-lookup"><span data-stu-id="76697-188">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="76697-189">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="76697-189">400 BadRequest</span></span> | <span data-ttu-id="76697-190">роленотфаунд</span><span class="sxs-lookup"><span data-stu-id="76697-190">RoleNotFound</span></span>                                | <span data-ttu-id="76697-191">`roleDefinitionId`Не удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="76697-191">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="76697-192">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="76697-192">400 BadRequest</span></span> | <span data-ttu-id="76697-193">ресаурцеислоккед</span><span class="sxs-lookup"><span data-stu-id="76697-193">ResourceIsLocked</span></span>                            | <span data-ttu-id="76697-194">Ресурс, указанный в теле запроса, находится в состоянии `Locked` и не может создавать запросы на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="76697-194">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="76697-195">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="76697-195">400 BadRequest</span></span> | <span data-ttu-id="76697-196">субжектнотфаунд</span><span class="sxs-lookup"><span data-stu-id="76697-196">SubjectNotFound</span></span>                             | <span data-ttu-id="76697-197">`subjectId`Не удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="76697-197">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="76697-198">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="76697-198">400 BadRequest</span></span> | <span data-ttu-id="76697-199">пендингролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="76697-199">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="76697-200">В системе уже существует ожидающий [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="76697-200">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="76697-201">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="76697-201">400 BadRequest</span></span> | <span data-ttu-id="76697-202">ролеассигнментексистс</span><span class="sxs-lookup"><span data-stu-id="76697-202">RoleAssignmentExists</span></span>                        | <span data-ttu-id="76697-203">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , который требуется создать, уже существует в системе.</span><span class="sxs-lookup"><span data-stu-id="76697-203">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="76697-204">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="76697-204">400 BadRequest</span></span> | <span data-ttu-id="76697-205">ролеассигнментдоеснотексист</span><span class="sxs-lookup"><span data-stu-id="76697-205">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="76697-206">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , запрошенный для обновления или расширения, не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="76697-206">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="76697-207">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="76697-207">400 BadRequest</span></span> | <span data-ttu-id="76697-208">ролеассигнментрекуестполицивалидатионфаилед</span><span class="sxs-lookup"><span data-stu-id="76697-208">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="76697-209">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) не отвечает внутренним политикам и не может быть создан.</span><span class="sxs-lookup"><span data-stu-id="76697-209">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="76697-210">Примеры</span><span class="sxs-lookup"><span data-stu-id="76697-210">Examples</span></span>

<span data-ttu-id="76697-211">В следующих примерах показано, как использовать этот API.</span><span class="sxs-lookup"><span data-stu-id="76697-211">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="76697-212">Пример 1: Администратор назначает пользователю роль</span><span class="sxs-lookup"><span data-stu-id="76697-212">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="76697-213">В этом примере администратор назначает пользователю nawu@fimdev.net роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="76697-213">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="76697-214">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней мере одно `Active` назначение роли администратора ( `owner` или `user access administrator` ) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="76697-214">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="76697-215">Свойство</span><span class="sxs-lookup"><span data-stu-id="76697-215">Property</span></span>         | <span data-ttu-id="76697-216">Тип</span><span class="sxs-lookup"><span data-stu-id="76697-216">Type</span></span>                                                     | <span data-ttu-id="76697-217">Обязательный</span><span class="sxs-lookup"><span data-stu-id="76697-217">Required</span></span>                 | <span data-ttu-id="76697-218">Значение</span><span class="sxs-lookup"><span data-stu-id="76697-218">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="76697-219">resourceId</span><span class="sxs-lookup"><span data-stu-id="76697-219">resourceId</span></span>       | <span data-ttu-id="76697-220">String</span><span class="sxs-lookup"><span data-stu-id="76697-220">String</span></span>                                                   | <span data-ttu-id="76697-221">Да</span><span class="sxs-lookup"><span data-stu-id="76697-221">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="76697-222">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="76697-222">roleDefinitionId</span></span> | <span data-ttu-id="76697-223">String</span><span class="sxs-lookup"><span data-stu-id="76697-223">String</span></span>                                                   | <span data-ttu-id="76697-224">Да</span><span class="sxs-lookup"><span data-stu-id="76697-224">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="76697-225">субжектид</span><span class="sxs-lookup"><span data-stu-id="76697-225">subjectId</span></span>        | <span data-ttu-id="76697-226">String</span><span class="sxs-lookup"><span data-stu-id="76697-226">String</span></span>                                                   | <span data-ttu-id="76697-227">Да</span><span class="sxs-lookup"><span data-stu-id="76697-227">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="76697-228">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="76697-228">assignmentState</span></span>  | <span data-ttu-id="76697-229">String</span><span class="sxs-lookup"><span data-stu-id="76697-229">String</span></span>                                                   | <span data-ttu-id="76697-230">Да</span><span class="sxs-lookup"><span data-stu-id="76697-230">Yes</span></span>                      | <span data-ttu-id="76697-231">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="76697-231">Eligible / Active</span></span> |
| <span data-ttu-id="76697-232">type</span><span class="sxs-lookup"><span data-stu-id="76697-232">type</span></span>             | <span data-ttu-id="76697-233">String</span><span class="sxs-lookup"><span data-stu-id="76697-233">String</span></span>                                                   | <span data-ttu-id="76697-234">Да</span><span class="sxs-lookup"><span data-stu-id="76697-234">Yes</span></span>                      | <span data-ttu-id="76697-235">админадд</span><span class="sxs-lookup"><span data-stu-id="76697-235">AdminAdd</span></span> |
| <span data-ttu-id="76697-236">reason</span><span class="sxs-lookup"><span data-stu-id="76697-236">reason</span></span>           | <span data-ttu-id="76697-237">String</span><span class="sxs-lookup"><span data-stu-id="76697-237">String</span></span>                                                   | <span data-ttu-id="76697-238">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="76697-238">depends on role Settings</span></span> |   |
| <span data-ttu-id="76697-239">schedule</span><span class="sxs-lookup"><span data-stu-id="76697-239">schedule</span></span>         | [<span data-ttu-id="76697-240">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="76697-240">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="76697-241">Да</span><span class="sxs-lookup"><span data-stu-id="76697-241">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="76697-242">Запрос</span><span class="sxs-lookup"><span data-stu-id="76697-242">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="76697-243">HTTP</span><span class="sxs-lookup"><span data-stu-id="76697-243">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="76697-244">C#</span><span class="sxs-lookup"><span data-stu-id="76697-244">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="76697-245">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76697-245">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="76697-246">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76697-246">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="76697-247">Отклик</span><span class="sxs-lookup"><span data-stu-id="76697-247">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="76697-248">Пример 2: пользователь активирует подходящие роли</span><span class="sxs-lookup"><span data-stu-id="76697-248">Example 2: User activates eligible role</span></span>

<span data-ttu-id="76697-249">В этом примере пользователь nawu@fimdev.net активирует соответствующую роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="76697-249">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="76697-250">Свойство</span><span class="sxs-lookup"><span data-stu-id="76697-250">Property</span></span>         | <span data-ttu-id="76697-251">Тип</span><span class="sxs-lookup"><span data-stu-id="76697-251">Type</span></span>                                                     | <span data-ttu-id="76697-252">Обязательный</span><span class="sxs-lookup"><span data-stu-id="76697-252">Required</span></span>                 | <span data-ttu-id="76697-253">Значение</span><span class="sxs-lookup"><span data-stu-id="76697-253">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="76697-254">resourceId</span><span class="sxs-lookup"><span data-stu-id="76697-254">resourceId</span></span>       | <span data-ttu-id="76697-255">String</span><span class="sxs-lookup"><span data-stu-id="76697-255">String</span></span>                                                   | <span data-ttu-id="76697-256">Да</span><span class="sxs-lookup"><span data-stu-id="76697-256">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="76697-257">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="76697-257">roleDefinitionId</span></span> | <span data-ttu-id="76697-258">String</span><span class="sxs-lookup"><span data-stu-id="76697-258">String</span></span>                                                   | <span data-ttu-id="76697-259">Да</span><span class="sxs-lookup"><span data-stu-id="76697-259">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="76697-260">субжектид</span><span class="sxs-lookup"><span data-stu-id="76697-260">subjectId</span></span>        | <span data-ttu-id="76697-261">String</span><span class="sxs-lookup"><span data-stu-id="76697-261">String</span></span>                                                   | <span data-ttu-id="76697-262">Да</span><span class="sxs-lookup"><span data-stu-id="76697-262">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="76697-263">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="76697-263">assignmentState</span></span>  | <span data-ttu-id="76697-264">String</span><span class="sxs-lookup"><span data-stu-id="76697-264">String</span></span>                                                   | <span data-ttu-id="76697-265">Да</span><span class="sxs-lookup"><span data-stu-id="76697-265">Yes</span></span>                      | <span data-ttu-id="76697-266">Активное</span><span class="sxs-lookup"><span data-stu-id="76697-266">Active</span></span> |
| <span data-ttu-id="76697-267">type</span><span class="sxs-lookup"><span data-stu-id="76697-267">type</span></span>             | <span data-ttu-id="76697-268">String</span><span class="sxs-lookup"><span data-stu-id="76697-268">String</span></span>                                                   | <span data-ttu-id="76697-269">Да</span><span class="sxs-lookup"><span data-stu-id="76697-269">Yes</span></span>                      | <span data-ttu-id="76697-270">усерадд</span><span class="sxs-lookup"><span data-stu-id="76697-270">UserAdd</span></span> |
| <span data-ttu-id="76697-271">reason</span><span class="sxs-lookup"><span data-stu-id="76697-271">reason</span></span>           | <span data-ttu-id="76697-272">String</span><span class="sxs-lookup"><span data-stu-id="76697-272">String</span></span>                                                   | <span data-ttu-id="76697-273">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="76697-273">depends on role Settings</span></span> |   |
| <span data-ttu-id="76697-274">schedule</span><span class="sxs-lookup"><span data-stu-id="76697-274">schedule</span></span>         | [<span data-ttu-id="76697-275">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="76697-275">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="76697-276">Да</span><span class="sxs-lookup"><span data-stu-id="76697-276">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="76697-277">Запрос</span><span class="sxs-lookup"><span data-stu-id="76697-277">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="76697-278">Отклик</span><span class="sxs-lookup"><span data-stu-id="76697-278">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="76697-279">Пример 3: пользователь отключает назначенную роль</span><span class="sxs-lookup"><span data-stu-id="76697-279">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="76697-280">В этом примере пользователь nawu@fimdev.net отключает активную роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="76697-280">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="76697-281">Свойство</span><span class="sxs-lookup"><span data-stu-id="76697-281">Property</span></span>         | <span data-ttu-id="76697-282">Тип</span><span class="sxs-lookup"><span data-stu-id="76697-282">Type</span></span>                                                     | <span data-ttu-id="76697-283">Обязательный</span><span class="sxs-lookup"><span data-stu-id="76697-283">Required</span></span> | <span data-ttu-id="76697-284">Значение</span><span class="sxs-lookup"><span data-stu-id="76697-284">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="76697-285">resourceId</span><span class="sxs-lookup"><span data-stu-id="76697-285">resourceId</span></span>       | <span data-ttu-id="76697-286">String</span><span class="sxs-lookup"><span data-stu-id="76697-286">String</span></span>                                                   | <span data-ttu-id="76697-287">Да</span><span class="sxs-lookup"><span data-stu-id="76697-287">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="76697-288">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="76697-288">roleDefinitionId</span></span> | <span data-ttu-id="76697-289">String</span><span class="sxs-lookup"><span data-stu-id="76697-289">String</span></span>                                                   | <span data-ttu-id="76697-290">Да</span><span class="sxs-lookup"><span data-stu-id="76697-290">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="76697-291">субжектид</span><span class="sxs-lookup"><span data-stu-id="76697-291">subjectId</span></span>        | <span data-ttu-id="76697-292">String</span><span class="sxs-lookup"><span data-stu-id="76697-292">String</span></span>                                                   | <span data-ttu-id="76697-293">Да</span><span class="sxs-lookup"><span data-stu-id="76697-293">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="76697-294">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="76697-294">assignmentState</span></span>  | <span data-ttu-id="76697-295">String</span><span class="sxs-lookup"><span data-stu-id="76697-295">String</span></span>                                                   | <span data-ttu-id="76697-296">Да</span><span class="sxs-lookup"><span data-stu-id="76697-296">Yes</span></span>      | <span data-ttu-id="76697-297">Активное</span><span class="sxs-lookup"><span data-stu-id="76697-297">Active</span></span> |
| <span data-ttu-id="76697-298">type</span><span class="sxs-lookup"><span data-stu-id="76697-298">type</span></span>             | <span data-ttu-id="76697-299">String</span><span class="sxs-lookup"><span data-stu-id="76697-299">String</span></span>                                                   | <span data-ttu-id="76697-300">Да</span><span class="sxs-lookup"><span data-stu-id="76697-300">Yes</span></span>      | <span data-ttu-id="76697-301">усерремове</span><span class="sxs-lookup"><span data-stu-id="76697-301">UserRemove</span></span> |
| <span data-ttu-id="76697-302">reason</span><span class="sxs-lookup"><span data-stu-id="76697-302">reason</span></span>           | <span data-ttu-id="76697-303">String</span><span class="sxs-lookup"><span data-stu-id="76697-303">String</span></span>                                                   | <span data-ttu-id="76697-304">Нет</span><span class="sxs-lookup"><span data-stu-id="76697-304">No</span></span>       |   |
| <span data-ttu-id="76697-305">schedule</span><span class="sxs-lookup"><span data-stu-id="76697-305">schedule</span></span>         | [<span data-ttu-id="76697-306">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="76697-306">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="76697-307">Нет</span><span class="sxs-lookup"><span data-stu-id="76697-307">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="76697-308">Запрос</span><span class="sxs-lookup"><span data-stu-id="76697-308">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="76697-309">Отклик</span><span class="sxs-lookup"><span data-stu-id="76697-309">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="76697-310">Пример 4: Администратор удаляет пользователя из роли</span><span class="sxs-lookup"><span data-stu-id="76697-310">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="76697-311">В этом примере администратор удаляет пользователя nawu@fimdev.net из роли читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="76697-311">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="76697-312">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней мере одно `Active` назначение роли администратора ( `owner` или `user access administrator` ) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="76697-312">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="76697-313">Свойство</span><span class="sxs-lookup"><span data-stu-id="76697-313">Property</span></span>         | <span data-ttu-id="76697-314">Тип</span><span class="sxs-lookup"><span data-stu-id="76697-314">Type</span></span>                                                     | <span data-ttu-id="76697-315">Обязательный</span><span class="sxs-lookup"><span data-stu-id="76697-315">Required</span></span> | <span data-ttu-id="76697-316">Значение</span><span class="sxs-lookup"><span data-stu-id="76697-316">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="76697-317">resourceId</span><span class="sxs-lookup"><span data-stu-id="76697-317">resourceId</span></span>       | <span data-ttu-id="76697-318">String</span><span class="sxs-lookup"><span data-stu-id="76697-318">String</span></span>                                                   | <span data-ttu-id="76697-319">Да</span><span class="sxs-lookup"><span data-stu-id="76697-319">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="76697-320">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="76697-320">roleDefinitionId</span></span> | <span data-ttu-id="76697-321">String</span><span class="sxs-lookup"><span data-stu-id="76697-321">String</span></span>                                                   | <span data-ttu-id="76697-322">Да</span><span class="sxs-lookup"><span data-stu-id="76697-322">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="76697-323">субжектид</span><span class="sxs-lookup"><span data-stu-id="76697-323">subjectId</span></span>        | <span data-ttu-id="76697-324">String</span><span class="sxs-lookup"><span data-stu-id="76697-324">String</span></span>                                                   | <span data-ttu-id="76697-325">Да</span><span class="sxs-lookup"><span data-stu-id="76697-325">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="76697-326">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="76697-326">assignmentState</span></span>  | <span data-ttu-id="76697-327">String</span><span class="sxs-lookup"><span data-stu-id="76697-327">String</span></span>                                                   | <span data-ttu-id="76697-328">Да</span><span class="sxs-lookup"><span data-stu-id="76697-328">Yes</span></span>      | <span data-ttu-id="76697-329">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="76697-329">Eligible / Active</span></span> |
| <span data-ttu-id="76697-330">type</span><span class="sxs-lookup"><span data-stu-id="76697-330">type</span></span>             | <span data-ttu-id="76697-331">String</span><span class="sxs-lookup"><span data-stu-id="76697-331">String</span></span>                                                   | <span data-ttu-id="76697-332">Да</span><span class="sxs-lookup"><span data-stu-id="76697-332">Yes</span></span>      | <span data-ttu-id="76697-333">админремове</span><span class="sxs-lookup"><span data-stu-id="76697-333">AdminRemove</span></span> |
| <span data-ttu-id="76697-334">reason</span><span class="sxs-lookup"><span data-stu-id="76697-334">reason</span></span>           | <span data-ttu-id="76697-335">String</span><span class="sxs-lookup"><span data-stu-id="76697-335">String</span></span>                                                   | <span data-ttu-id="76697-336">Нет</span><span class="sxs-lookup"><span data-stu-id="76697-336">No</span></span>       |   |
| <span data-ttu-id="76697-337">schedule</span><span class="sxs-lookup"><span data-stu-id="76697-337">schedule</span></span>         | [<span data-ttu-id="76697-338">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="76697-338">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="76697-339">Нет</span><span class="sxs-lookup"><span data-stu-id="76697-339">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="76697-340">Запрос</span><span class="sxs-lookup"><span data-stu-id="76697-340">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="76697-341">Отклик</span><span class="sxs-lookup"><span data-stu-id="76697-341">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="76697-342">Пример 5: "Администратор обновляет назначение ролей"</span><span class="sxs-lookup"><span data-stu-id="76697-342">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="76697-343">В этом примере администраторы обновляют назначение роли пользователя nawu@fimdev.net владельцу.</span><span class="sxs-lookup"><span data-stu-id="76697-343">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="76697-344">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней мере одно `Active` назначение роли администратора ( `owner` или `user access administrator` ) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="76697-344">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="76697-345">Свойство</span><span class="sxs-lookup"><span data-stu-id="76697-345">Property</span></span>         | <span data-ttu-id="76697-346">Тип</span><span class="sxs-lookup"><span data-stu-id="76697-346">Type</span></span>                                                     | <span data-ttu-id="76697-347">Обязательный</span><span class="sxs-lookup"><span data-stu-id="76697-347">Required</span></span>                | <span data-ttu-id="76697-348">Значение</span><span class="sxs-lookup"><span data-stu-id="76697-348">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="76697-349">resourceId</span><span class="sxs-lookup"><span data-stu-id="76697-349">resourceId</span></span>       | <span data-ttu-id="76697-350">String</span><span class="sxs-lookup"><span data-stu-id="76697-350">String</span></span>                                                   | <span data-ttu-id="76697-351">Да</span><span class="sxs-lookup"><span data-stu-id="76697-351">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="76697-352">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="76697-352">roleDefinitionId</span></span> | <span data-ttu-id="76697-353">String</span><span class="sxs-lookup"><span data-stu-id="76697-353">String</span></span>                                                   | <span data-ttu-id="76697-354">Да</span><span class="sxs-lookup"><span data-stu-id="76697-354">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="76697-355">субжектид</span><span class="sxs-lookup"><span data-stu-id="76697-355">subjectId</span></span>        | <span data-ttu-id="76697-356">String</span><span class="sxs-lookup"><span data-stu-id="76697-356">String</span></span>                                                   | <span data-ttu-id="76697-357">Да</span><span class="sxs-lookup"><span data-stu-id="76697-357">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="76697-358">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="76697-358">assignmentState</span></span>  | <span data-ttu-id="76697-359">String</span><span class="sxs-lookup"><span data-stu-id="76697-359">String</span></span>                                                   | <span data-ttu-id="76697-360">Да</span><span class="sxs-lookup"><span data-stu-id="76697-360">Yes</span></span>                     | <span data-ttu-id="76697-361">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="76697-361">Eligible / Active</span></span> |
| <span data-ttu-id="76697-362">type</span><span class="sxs-lookup"><span data-stu-id="76697-362">type</span></span>             | <span data-ttu-id="76697-363">String</span><span class="sxs-lookup"><span data-stu-id="76697-363">String</span></span>                                                   | <span data-ttu-id="76697-364">Да</span><span class="sxs-lookup"><span data-stu-id="76697-364">Yes</span></span>                     | <span data-ttu-id="76697-365">админупдате</span><span class="sxs-lookup"><span data-stu-id="76697-365">AdminUpdate</span></span> |
| <span data-ttu-id="76697-366">reason</span><span class="sxs-lookup"><span data-stu-id="76697-366">reason</span></span>           | <span data-ttu-id="76697-367">String</span><span class="sxs-lookup"><span data-stu-id="76697-367">String</span></span>                                                   | <span data-ttu-id="76697-368">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="76697-368">depends on roleSettings</span></span> |   |
| <span data-ttu-id="76697-369">schedule</span><span class="sxs-lookup"><span data-stu-id="76697-369">schedule</span></span>         | [<span data-ttu-id="76697-370">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="76697-370">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="76697-371">Да</span><span class="sxs-lookup"><span data-stu-id="76697-371">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="76697-372">Запрос</span><span class="sxs-lookup"><span data-stu-id="76697-372">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="76697-373">Отклик</span><span class="sxs-lookup"><span data-stu-id="76697-373">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="76697-374">Пример 6: администратор расширяет назначение ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="76697-374">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="76697-375">В этом примере показано, как расширить назначение роли истечения срока действия для пользователя АНУЖКУСЕР участнику службы управления API.</span><span class="sxs-lookup"><span data-stu-id="76697-375">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="76697-376">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней мере одно `Active` назначение роли администратора ( `owner` или `user access administrator` ) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="76697-376">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="76697-377">Свойство</span><span class="sxs-lookup"><span data-stu-id="76697-377">Property</span></span>         | <span data-ttu-id="76697-378">Тип</span><span class="sxs-lookup"><span data-stu-id="76697-378">Type</span></span>                                                     | <span data-ttu-id="76697-379">Обязательный</span><span class="sxs-lookup"><span data-stu-id="76697-379">Required</span></span>                | <span data-ttu-id="76697-380">Значение</span><span class="sxs-lookup"><span data-stu-id="76697-380">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="76697-381">resourceId</span><span class="sxs-lookup"><span data-stu-id="76697-381">resourceId</span></span>       | <span data-ttu-id="76697-382">String</span><span class="sxs-lookup"><span data-stu-id="76697-382">String</span></span>                                                   | <span data-ttu-id="76697-383">Да</span><span class="sxs-lookup"><span data-stu-id="76697-383">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="76697-384">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="76697-384">roleDefinitionId</span></span> | <span data-ttu-id="76697-385">String</span><span class="sxs-lookup"><span data-stu-id="76697-385">String</span></span>                                                   | <span data-ttu-id="76697-386">Да</span><span class="sxs-lookup"><span data-stu-id="76697-386">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="76697-387">субжектид</span><span class="sxs-lookup"><span data-stu-id="76697-387">subjectId</span></span>        | <span data-ttu-id="76697-388">String</span><span class="sxs-lookup"><span data-stu-id="76697-388">String</span></span>                                                   | <span data-ttu-id="76697-389">Да</span><span class="sxs-lookup"><span data-stu-id="76697-389">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="76697-390">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="76697-390">assignmentState</span></span>  | <span data-ttu-id="76697-391">String</span><span class="sxs-lookup"><span data-stu-id="76697-391">String</span></span>                                                   | <span data-ttu-id="76697-392">Да</span><span class="sxs-lookup"><span data-stu-id="76697-392">Yes</span></span>                     | <span data-ttu-id="76697-393">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="76697-393">Eligible / Active</span></span> |
| <span data-ttu-id="76697-394">type</span><span class="sxs-lookup"><span data-stu-id="76697-394">type</span></span>             | <span data-ttu-id="76697-395">String</span><span class="sxs-lookup"><span data-stu-id="76697-395">String</span></span>                                                   | <span data-ttu-id="76697-396">Да</span><span class="sxs-lookup"><span data-stu-id="76697-396">Yes</span></span>                     | <span data-ttu-id="76697-397">админекстенд</span><span class="sxs-lookup"><span data-stu-id="76697-397">AdminExtend</span></span> |
| <span data-ttu-id="76697-398">reason</span><span class="sxs-lookup"><span data-stu-id="76697-398">reason</span></span>           | <span data-ttu-id="76697-399">String</span><span class="sxs-lookup"><span data-stu-id="76697-399">String</span></span>                                                   | <span data-ttu-id="76697-400">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="76697-400">depends on roleSettings</span></span> |   |
| <span data-ttu-id="76697-401">schedule</span><span class="sxs-lookup"><span data-stu-id="76697-401">schedule</span></span>         | [<span data-ttu-id="76697-402">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="76697-402">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="76697-403">Да</span><span class="sxs-lookup"><span data-stu-id="76697-403">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="76697-404">Запрос</span><span class="sxs-lookup"><span data-stu-id="76697-404">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="76697-405">Отклик</span><span class="sxs-lookup"><span data-stu-id="76697-405">Response</span></span>

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


