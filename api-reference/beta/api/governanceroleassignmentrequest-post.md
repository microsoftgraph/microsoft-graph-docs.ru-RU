---
title: Создание governanceRoleAssignmentRequest
description: Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли. В приведенной ниже таблице перечислены операции.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 8d9946425e90968d65f2592901ae6d5ac7f3c018
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42421041"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="2ef3a-104">Создание governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="2ef3a-104">Create governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="2ef3a-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2ef3a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ef3a-106">Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-106">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="2ef3a-107">В приведенной ниже таблице перечислены операции.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-107">The following table lists the operations.</span></span>

| <span data-ttu-id="2ef3a-108">Operation</span><span class="sxs-lookup"><span data-stu-id="2ef3a-108">Operation</span></span>                                   | <span data-ttu-id="2ef3a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2ef3a-109">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="2ef3a-110">Назначение роли</span><span class="sxs-lookup"><span data-stu-id="2ef3a-110">Assign a role assignment</span></span>                    | <span data-ttu-id="2ef3a-111">админадд</span><span class="sxs-lookup"><span data-stu-id="2ef3a-111">AdminAdd</span></span>    |
| <span data-ttu-id="2ef3a-112">Активация подходящего назначения роли</span><span class="sxs-lookup"><span data-stu-id="2ef3a-112">Activate an eligible role assignment</span></span>        | <span data-ttu-id="2ef3a-113">усерадд</span><span class="sxs-lookup"><span data-stu-id="2ef3a-113">UserAdd</span></span>     |
| <span data-ttu-id="2ef3a-114">Деактивация активированного назначения роли</span><span class="sxs-lookup"><span data-stu-id="2ef3a-114">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="2ef3a-115">усерремове</span><span class="sxs-lookup"><span data-stu-id="2ef3a-115">UserRemove</span></span>  |
| <span data-ttu-id="2ef3a-116">Удаление назначения роли</span><span class="sxs-lookup"><span data-stu-id="2ef3a-116">Remove a role assignment</span></span>                    | <span data-ttu-id="2ef3a-117">админремове</span><span class="sxs-lookup"><span data-stu-id="2ef3a-117">AdminRemove</span></span> |
| <span data-ttu-id="2ef3a-118">Обновление назначения роли</span><span class="sxs-lookup"><span data-stu-id="2ef3a-118">Update a role assignment</span></span>                    | <span data-ttu-id="2ef3a-119">админупдате</span><span class="sxs-lookup"><span data-stu-id="2ef3a-119">AdminUpdate</span></span> |
| <span data-ttu-id="2ef3a-120">Запрос на расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="2ef3a-120">Request to extend my role assignment</span></span>        | <span data-ttu-id="2ef3a-121">усерекстенд</span><span class="sxs-lookup"><span data-stu-id="2ef3a-121">UserExtend</span></span>  |
| <span data-ttu-id="2ef3a-122">Расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="2ef3a-122">Extend a role assignment</span></span>                    | <span data-ttu-id="2ef3a-123">админекстенд</span><span class="sxs-lookup"><span data-stu-id="2ef3a-123">AdminExtend</span></span> |
| <span data-ttu-id="2ef3a-124">Запрос на продление назначения роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="2ef3a-124">Request to renew my expired role assignment</span></span> | <span data-ttu-id="2ef3a-125">усерренев</span><span class="sxs-lookup"><span data-stu-id="2ef3a-125">UserRenew</span></span>   |
| <span data-ttu-id="2ef3a-126">Продление назначенной роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="2ef3a-126">Renew an expired role assignment</span></span>            | <span data-ttu-id="2ef3a-127">админренев</span><span class="sxs-lookup"><span data-stu-id="2ef3a-127">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="2ef3a-128">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ef3a-128">Permissions</span></span>

<span data-ttu-id="2ef3a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ef3a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2ef3a-131">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ef3a-131">Permission type</span></span>                        | <span data-ttu-id="2ef3a-132">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ef3a-132">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="2ef3a-133">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ef3a-133">Delegated (work or school account)</span></span>     | <span data-ttu-id="2ef3a-134">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="2ef3a-134">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="2ef3a-135">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ef3a-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ef3a-136">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-136">Not supported.</span></span>                            |
| <span data-ttu-id="2ef3a-137">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ef3a-137">Application</span></span>                            | <span data-ttu-id="2ef3a-138">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-138">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ef3a-139">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ef3a-139">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="2ef3a-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ef3a-140">Request headers</span></span>

| <span data-ttu-id="2ef3a-141">Имя</span><span class="sxs-lookup"><span data-stu-id="2ef3a-141">Name</span></span>          | <span data-ttu-id="2ef3a-142">Описание</span><span class="sxs-lookup"><span data-stu-id="2ef3a-142">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="2ef3a-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ef3a-143">Authorization</span></span> | <span data-ttu-id="2ef3a-144">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2ef3a-144">Bearer {code}</span></span>    |
| <span data-ttu-id="2ef3a-145">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2ef3a-145">Content-type</span></span>  | <span data-ttu-id="2ef3a-146">application/json</span><span class="sxs-lookup"><span data-stu-id="2ef3a-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ef3a-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ef3a-147">Request body</span></span>

<span data-ttu-id="2ef3a-148">В тексте запроса добавьте представление объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-148">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="2ef3a-149">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ef3a-149">Property</span></span>         | <span data-ttu-id="2ef3a-150">Тип</span><span class="sxs-lookup"><span data-stu-id="2ef3a-150">Type</span></span>                                                     | <span data-ttu-id="2ef3a-151">Описание</span><span class="sxs-lookup"><span data-stu-id="2ef3a-151">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="2ef3a-152">resourceId</span><span class="sxs-lookup"><span data-stu-id="2ef3a-152">resourceId</span></span>       | <span data-ttu-id="2ef3a-153">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-153">String</span></span>                                                   | <span data-ttu-id="2ef3a-154">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-154">The ID of the resource.</span></span> <span data-ttu-id="2ef3a-155">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-155">Required.</span></span> |
| <span data-ttu-id="2ef3a-156">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="2ef3a-156">roleDefinitionId</span></span> | <span data-ttu-id="2ef3a-157">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-157">String</span></span>                                                   | <span data-ttu-id="2ef3a-158">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-158">The ID of the role definition.</span></span> <span data-ttu-id="2ef3a-159">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-159">Required.</span></span> |
| <span data-ttu-id="2ef3a-160">субжектид</span><span class="sxs-lookup"><span data-stu-id="2ef3a-160">subjectId</span></span>        | <span data-ttu-id="2ef3a-161">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-161">String</span></span>                                                   | <span data-ttu-id="2ef3a-162">ИДЕНТИФИКАТОР субъекта.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-162">The ID of the subject.</span></span> <span data-ttu-id="2ef3a-163">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-163">Required.</span></span> |
| <span data-ttu-id="2ef3a-164">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="2ef3a-164">assignmentState</span></span>  | <span data-ttu-id="2ef3a-165">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-165">String</span></span>                                                   | <span data-ttu-id="2ef3a-166">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-166">The state of assignment.</span></span> <span data-ttu-id="2ef3a-167">Значение может быть `Eligible` и `Active`.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-167">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="2ef3a-168">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-168">Required.</span></span> |
| <span data-ttu-id="2ef3a-169">type</span><span class="sxs-lookup"><span data-stu-id="2ef3a-169">type</span></span>             | <span data-ttu-id="2ef3a-170">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-170">String</span></span>                                                   | <span data-ttu-id="2ef3a-171">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-171">The request type.</span></span> <span data-ttu-id="2ef3a-172">Возможные значения: `AdminAdd`, `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `AdminRenew` `AdminExtend`,,,,, и. `UserExtend` `UserRenew`</span><span class="sxs-lookup"><span data-stu-id="2ef3a-172">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="2ef3a-173">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-173">Required.</span></span> |
| <span data-ttu-id="2ef3a-174">reason</span><span class="sxs-lookup"><span data-stu-id="2ef3a-174">reason</span></span>           | <span data-ttu-id="2ef3a-175">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-175">String</span></span>                                                   | <span data-ttu-id="2ef3a-176">Необходимо указать причину для запроса на назначение роли для аудита и проверки.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-176">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="2ef3a-177">schedule</span><span class="sxs-lookup"><span data-stu-id="2ef3a-177">schedule</span></span>         | [<span data-ttu-id="2ef3a-178">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2ef3a-178">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="2ef3a-179">Расписание запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-179">The schedule of the role assignment request.</span></span> <span data-ttu-id="2ef3a-180">`UserAdd`Для типа запроса `AdminAdd`,, `AdminUpdate`, и `AdminExtend`, он необходим.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-180">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="2ef3a-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ef3a-181">Response</span></span>

<span data-ttu-id="2ef3a-182">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-182">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="2ef3a-183">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="2ef3a-183">Error codes</span></span>

<span data-ttu-id="2ef3a-184">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-184">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="2ef3a-185">Кроме того, он возвращает коды ошибок, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-185">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="2ef3a-186">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="2ef3a-186">Error code</span></span>     | <span data-ttu-id="2ef3a-187">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="2ef3a-187">Error message</span></span>                               | <span data-ttu-id="2ef3a-188">Сведения</span><span class="sxs-lookup"><span data-stu-id="2ef3a-188">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="2ef3a-189">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="2ef3a-189">400 BadRequest</span></span> | <span data-ttu-id="2ef3a-190">роленотфаунд</span><span class="sxs-lookup"><span data-stu-id="2ef3a-190">RoleNotFound</span></span>                                | <span data-ttu-id="2ef3a-191">Не `roleDefinitionId` удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-191">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="2ef3a-192">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="2ef3a-192">400 BadRequest</span></span> | <span data-ttu-id="2ef3a-193">ресаурцеислоккед</span><span class="sxs-lookup"><span data-stu-id="2ef3a-193">ResourceIsLocked</span></span>                            | <span data-ttu-id="2ef3a-194">Ресурс, указанный в теле запроса, находится в состоянии `Locked` и не может создавать запросы на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-194">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="2ef3a-195">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="2ef3a-195">400 BadRequest</span></span> | <span data-ttu-id="2ef3a-196">субжектнотфаунд</span><span class="sxs-lookup"><span data-stu-id="2ef3a-196">SubjectNotFound</span></span>                             | <span data-ttu-id="2ef3a-197">Не `subjectId` удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-197">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="2ef3a-198">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="2ef3a-198">400 BadRequest</span></span> | <span data-ttu-id="2ef3a-199">пендингролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="2ef3a-199">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="2ef3a-200">В системе уже существует ожидающий [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="2ef3a-200">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="2ef3a-201">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="2ef3a-201">400 BadRequest</span></span> | <span data-ttu-id="2ef3a-202">ролеассигнментексистс</span><span class="sxs-lookup"><span data-stu-id="2ef3a-202">RoleAssignmentExists</span></span>                        | <span data-ttu-id="2ef3a-203">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , который требуется создать, уже существует в системе.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-203">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="2ef3a-204">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="2ef3a-204">400 BadRequest</span></span> | <span data-ttu-id="2ef3a-205">ролеассигнментдоеснотексист</span><span class="sxs-lookup"><span data-stu-id="2ef3a-205">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="2ef3a-206">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , запрошенный для обновления или расширения, не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-206">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="2ef3a-207">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="2ef3a-207">400 BadRequest</span></span> | <span data-ttu-id="2ef3a-208">ролеассигнментрекуестполицивалидатионфаилед</span><span class="sxs-lookup"><span data-stu-id="2ef3a-208">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="2ef3a-209">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) не отвечает внутренним политикам и не может быть создан.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-209">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="2ef3a-210">Примеры</span><span class="sxs-lookup"><span data-stu-id="2ef3a-210">Examples</span></span>

<span data-ttu-id="2ef3a-211">В следующих примерах показано, как использовать этот API.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-211">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="2ef3a-212">Пример 1: Администратор назначает пользователю роль</span><span class="sxs-lookup"><span data-stu-id="2ef3a-212">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="2ef3a-213">В этом примере администратор назначает пользователю nawu@fimdev.net роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-213">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="2ef3a-214">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-214">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="2ef3a-215">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ef3a-215">Property</span></span>         | <span data-ttu-id="2ef3a-216">Тип</span><span class="sxs-lookup"><span data-stu-id="2ef3a-216">Type</span></span>                                                     | <span data-ttu-id="2ef3a-217">Обязательный</span><span class="sxs-lookup"><span data-stu-id="2ef3a-217">Required</span></span>                 | <span data-ttu-id="2ef3a-218">Значение</span><span class="sxs-lookup"><span data-stu-id="2ef3a-218">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="2ef3a-219">resourceId</span><span class="sxs-lookup"><span data-stu-id="2ef3a-219">resourceId</span></span>       | <span data-ttu-id="2ef3a-220">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-220">String</span></span>                                                   | <span data-ttu-id="2ef3a-221">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-221">Yes</span></span>                      | <span data-ttu-id="2ef3a-222">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="2ef3a-222">\<resourceId\></span></span> |
| <span data-ttu-id="2ef3a-223">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="2ef3a-223">roleDefinitionId</span></span> | <span data-ttu-id="2ef3a-224">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-224">String</span></span>                                                   | <span data-ttu-id="2ef3a-225">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-225">Yes</span></span>                      | <span data-ttu-id="2ef3a-226">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="2ef3a-226">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="2ef3a-227">субжектид</span><span class="sxs-lookup"><span data-stu-id="2ef3a-227">subjectId</span></span>        | <span data-ttu-id="2ef3a-228">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-228">String</span></span>                                                   | <span data-ttu-id="2ef3a-229">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-229">Yes</span></span>                      | <span data-ttu-id="2ef3a-230">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="2ef3a-230">\<subjectId\></span></span> |
| <span data-ttu-id="2ef3a-231">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="2ef3a-231">assignmentState</span></span>  | <span data-ttu-id="2ef3a-232">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-232">String</span></span>                                                   | <span data-ttu-id="2ef3a-233">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-233">Yes</span></span>                      | <span data-ttu-id="2ef3a-234">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="2ef3a-234">Eligible / Active</span></span> |
| <span data-ttu-id="2ef3a-235">type</span><span class="sxs-lookup"><span data-stu-id="2ef3a-235">type</span></span>             | <span data-ttu-id="2ef3a-236">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-236">String</span></span>                                                   | <span data-ttu-id="2ef3a-237">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-237">Yes</span></span>                      | <span data-ttu-id="2ef3a-238">админадд</span><span class="sxs-lookup"><span data-stu-id="2ef3a-238">AdminAdd</span></span> |
| <span data-ttu-id="2ef3a-239">reason</span><span class="sxs-lookup"><span data-stu-id="2ef3a-239">reason</span></span>           | <span data-ttu-id="2ef3a-240">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-240">String</span></span>                                                   | <span data-ttu-id="2ef3a-241">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="2ef3a-241">depends on role Settings</span></span> |   |
| <span data-ttu-id="2ef3a-242">schedule</span><span class="sxs-lookup"><span data-stu-id="2ef3a-242">schedule</span></span>         | [<span data-ttu-id="2ef3a-243">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2ef3a-243">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="2ef3a-244">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-244">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="2ef3a-245">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ef3a-245">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2ef3a-246">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ef3a-246">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2ef3a-247">C#</span><span class="sxs-lookup"><span data-stu-id="2ef3a-247">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ef3a-248">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ef3a-248">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ef3a-249">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ef3a-249">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="2ef3a-250">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ef3a-250">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="2ef3a-251">Пример 2: пользователь активирует подходящие роли</span><span class="sxs-lookup"><span data-stu-id="2ef3a-251">Example 2: User activates eligible role</span></span>

<span data-ttu-id="2ef3a-252">В этом примере пользователь nawu@fimdev.net активирует соответствующую роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-252">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="2ef3a-253">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ef3a-253">Property</span></span>         | <span data-ttu-id="2ef3a-254">Тип</span><span class="sxs-lookup"><span data-stu-id="2ef3a-254">Type</span></span>                                                     | <span data-ttu-id="2ef3a-255">Обязательный</span><span class="sxs-lookup"><span data-stu-id="2ef3a-255">Required</span></span>                 | <span data-ttu-id="2ef3a-256">Значение</span><span class="sxs-lookup"><span data-stu-id="2ef3a-256">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="2ef3a-257">resourceId</span><span class="sxs-lookup"><span data-stu-id="2ef3a-257">resourceId</span></span>       | <span data-ttu-id="2ef3a-258">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-258">String</span></span>                                                   | <span data-ttu-id="2ef3a-259">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-259">Yes</span></span>                      | <span data-ttu-id="2ef3a-260">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="2ef3a-260">\<resourceId\></span></span> |
| <span data-ttu-id="2ef3a-261">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="2ef3a-261">roleDefinitionId</span></span> | <span data-ttu-id="2ef3a-262">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-262">String</span></span>                                                   | <span data-ttu-id="2ef3a-263">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-263">Yes</span></span>                      | <span data-ttu-id="2ef3a-264">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="2ef3a-264">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="2ef3a-265">субжектид</span><span class="sxs-lookup"><span data-stu-id="2ef3a-265">subjectId</span></span>        | <span data-ttu-id="2ef3a-266">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-266">String</span></span>                                                   | <span data-ttu-id="2ef3a-267">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-267">Yes</span></span>                      | <span data-ttu-id="2ef3a-268">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="2ef3a-268">\<subjectId\></span></span> |
| <span data-ttu-id="2ef3a-269">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="2ef3a-269">assignmentState</span></span>  | <span data-ttu-id="2ef3a-270">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-270">String</span></span>                                                   | <span data-ttu-id="2ef3a-271">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-271">Yes</span></span>                      | <span data-ttu-id="2ef3a-272">Активное</span><span class="sxs-lookup"><span data-stu-id="2ef3a-272">Active</span></span> |
| <span data-ttu-id="2ef3a-273">type</span><span class="sxs-lookup"><span data-stu-id="2ef3a-273">type</span></span>             | <span data-ttu-id="2ef3a-274">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-274">String</span></span>                                                   | <span data-ttu-id="2ef3a-275">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-275">Yes</span></span>                      | <span data-ttu-id="2ef3a-276">усерадд</span><span class="sxs-lookup"><span data-stu-id="2ef3a-276">UserAdd</span></span> |
| <span data-ttu-id="2ef3a-277">reason</span><span class="sxs-lookup"><span data-stu-id="2ef3a-277">reason</span></span>           | <span data-ttu-id="2ef3a-278">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-278">String</span></span>                                                   | <span data-ttu-id="2ef3a-279">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="2ef3a-279">depends on role Settings</span></span> |   |
| <span data-ttu-id="2ef3a-280">schedule</span><span class="sxs-lookup"><span data-stu-id="2ef3a-280">schedule</span></span>         | [<span data-ttu-id="2ef3a-281">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2ef3a-281">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="2ef3a-282">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-282">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="2ef3a-283">Запросить</span><span class="sxs-lookup"><span data-stu-id="2ef3a-283">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="2ef3a-284">Ответ</span><span class="sxs-lookup"><span data-stu-id="2ef3a-284">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="2ef3a-285">Пример 3: пользователь отключает назначенную роль</span><span class="sxs-lookup"><span data-stu-id="2ef3a-285">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="2ef3a-286">В этом примере пользователь nawu@fimdev.net отключает активную роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-286">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="2ef3a-287">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ef3a-287">Property</span></span>         | <span data-ttu-id="2ef3a-288">Тип</span><span class="sxs-lookup"><span data-stu-id="2ef3a-288">Type</span></span>                                                     | <span data-ttu-id="2ef3a-289">Обязательный</span><span class="sxs-lookup"><span data-stu-id="2ef3a-289">Required</span></span> | <span data-ttu-id="2ef3a-290">Значение</span><span class="sxs-lookup"><span data-stu-id="2ef3a-290">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="2ef3a-291">resourceId</span><span class="sxs-lookup"><span data-stu-id="2ef3a-291">resourceId</span></span>       | <span data-ttu-id="2ef3a-292">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-292">String</span></span>                                                   | <span data-ttu-id="2ef3a-293">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-293">Yes</span></span>      | <span data-ttu-id="2ef3a-294">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="2ef3a-294">\<resourceId\></span></span> |
| <span data-ttu-id="2ef3a-295">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="2ef3a-295">roleDefinitionId</span></span> | <span data-ttu-id="2ef3a-296">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-296">String</span></span>                                                   | <span data-ttu-id="2ef3a-297">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-297">Yes</span></span>      | <span data-ttu-id="2ef3a-298">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="2ef3a-298">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="2ef3a-299">субжектид</span><span class="sxs-lookup"><span data-stu-id="2ef3a-299">subjectId</span></span>        | <span data-ttu-id="2ef3a-300">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-300">String</span></span>                                                   | <span data-ttu-id="2ef3a-301">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-301">Yes</span></span>      | <span data-ttu-id="2ef3a-302">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="2ef3a-302">\<subjectId\></span></span> |
| <span data-ttu-id="2ef3a-303">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="2ef3a-303">assignmentState</span></span>  | <span data-ttu-id="2ef3a-304">Строка</span><span class="sxs-lookup"><span data-stu-id="2ef3a-304">String</span></span>                                                   | <span data-ttu-id="2ef3a-305">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-305">Yes</span></span>      | <span data-ttu-id="2ef3a-306">Активное</span><span class="sxs-lookup"><span data-stu-id="2ef3a-306">Active</span></span> |
| <span data-ttu-id="2ef3a-307">type</span><span class="sxs-lookup"><span data-stu-id="2ef3a-307">type</span></span>             | <span data-ttu-id="2ef3a-308">Строка</span><span class="sxs-lookup"><span data-stu-id="2ef3a-308">String</span></span>                                                   | <span data-ttu-id="2ef3a-309">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-309">Yes</span></span>      | <span data-ttu-id="2ef3a-310">усерремове</span><span class="sxs-lookup"><span data-stu-id="2ef3a-310">UserRemove</span></span> |
| <span data-ttu-id="2ef3a-311">reason</span><span class="sxs-lookup"><span data-stu-id="2ef3a-311">reason</span></span>           | <span data-ttu-id="2ef3a-312">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-312">String</span></span>                                                   | <span data-ttu-id="2ef3a-313">Нет</span><span class="sxs-lookup"><span data-stu-id="2ef3a-313">No</span></span>       |   |
| <span data-ttu-id="2ef3a-314">schedule</span><span class="sxs-lookup"><span data-stu-id="2ef3a-314">schedule</span></span>         | [<span data-ttu-id="2ef3a-315">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2ef3a-315">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="2ef3a-316">Нет</span><span class="sxs-lookup"><span data-stu-id="2ef3a-316">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="2ef3a-317">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ef3a-317">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="2ef3a-318">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ef3a-318">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="2ef3a-319">Пример 4: Администратор удаляет пользователя из роли</span><span class="sxs-lookup"><span data-stu-id="2ef3a-319">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="2ef3a-320">В этом примере администратор удаляет пользователя nawu@fimdev.net из роли читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-320">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="2ef3a-321">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-321">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="2ef3a-322">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ef3a-322">Property</span></span>         | <span data-ttu-id="2ef3a-323">Тип</span><span class="sxs-lookup"><span data-stu-id="2ef3a-323">Type</span></span>                                                     | <span data-ttu-id="2ef3a-324">Обязательный</span><span class="sxs-lookup"><span data-stu-id="2ef3a-324">Required</span></span> | <span data-ttu-id="2ef3a-325">Значение</span><span class="sxs-lookup"><span data-stu-id="2ef3a-325">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="2ef3a-326">resourceId</span><span class="sxs-lookup"><span data-stu-id="2ef3a-326">resourceId</span></span>       | <span data-ttu-id="2ef3a-327">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-327">String</span></span>                                                   | <span data-ttu-id="2ef3a-328">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-328">Yes</span></span>      | <span data-ttu-id="2ef3a-329">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="2ef3a-329">\<resourceId\></span></span> |
| <span data-ttu-id="2ef3a-330">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="2ef3a-330">roleDefinitionId</span></span> | <span data-ttu-id="2ef3a-331">Строка</span><span class="sxs-lookup"><span data-stu-id="2ef3a-331">String</span></span>                                                   | <span data-ttu-id="2ef3a-332">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-332">Yes</span></span>      | <span data-ttu-id="2ef3a-333">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="2ef3a-333">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="2ef3a-334">субжектид</span><span class="sxs-lookup"><span data-stu-id="2ef3a-334">subjectId</span></span>        | <span data-ttu-id="2ef3a-335">Строка</span><span class="sxs-lookup"><span data-stu-id="2ef3a-335">String</span></span>                                                   | <span data-ttu-id="2ef3a-336">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-336">Yes</span></span>      | <span data-ttu-id="2ef3a-337">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="2ef3a-337">\<subjectId\></span></span> |
| <span data-ttu-id="2ef3a-338">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="2ef3a-338">assignmentState</span></span>  | <span data-ttu-id="2ef3a-339">Строка</span><span class="sxs-lookup"><span data-stu-id="2ef3a-339">String</span></span>                                                   | <span data-ttu-id="2ef3a-340">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-340">Yes</span></span>      | <span data-ttu-id="2ef3a-341">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="2ef3a-341">Eligible / Active</span></span> |
| <span data-ttu-id="2ef3a-342">type</span><span class="sxs-lookup"><span data-stu-id="2ef3a-342">type</span></span>             | <span data-ttu-id="2ef3a-343">Строка</span><span class="sxs-lookup"><span data-stu-id="2ef3a-343">String</span></span>                                                   | <span data-ttu-id="2ef3a-344">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-344">Yes</span></span>      | <span data-ttu-id="2ef3a-345">админремове</span><span class="sxs-lookup"><span data-stu-id="2ef3a-345">AdminRemove</span></span> |
| <span data-ttu-id="2ef3a-346">reason</span><span class="sxs-lookup"><span data-stu-id="2ef3a-346">reason</span></span>           | <span data-ttu-id="2ef3a-347">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-347">String</span></span>                                                   | <span data-ttu-id="2ef3a-348">Нет</span><span class="sxs-lookup"><span data-stu-id="2ef3a-348">No</span></span>       |   |
| <span data-ttu-id="2ef3a-349">schedule</span><span class="sxs-lookup"><span data-stu-id="2ef3a-349">schedule</span></span>         | [<span data-ttu-id="2ef3a-350">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2ef3a-350">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="2ef3a-351">Нет</span><span class="sxs-lookup"><span data-stu-id="2ef3a-351">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="2ef3a-352">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ef3a-352">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="2ef3a-353">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ef3a-353">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="2ef3a-354">Пример 5: "Администратор обновляет назначение ролей"</span><span class="sxs-lookup"><span data-stu-id="2ef3a-354">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="2ef3a-355">В этом примере администраторы обновляют назначение роли пользователя nawu@fimdev.net владельцу.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-355">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="2ef3a-356">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-356">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="2ef3a-357">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ef3a-357">Property</span></span>         | <span data-ttu-id="2ef3a-358">Тип</span><span class="sxs-lookup"><span data-stu-id="2ef3a-358">Type</span></span>                                                     | <span data-ttu-id="2ef3a-359">Обязательный</span><span class="sxs-lookup"><span data-stu-id="2ef3a-359">Required</span></span>                | <span data-ttu-id="2ef3a-360">Значение</span><span class="sxs-lookup"><span data-stu-id="2ef3a-360">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="2ef3a-361">resourceId</span><span class="sxs-lookup"><span data-stu-id="2ef3a-361">resourceId</span></span>       | <span data-ttu-id="2ef3a-362">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-362">String</span></span>                                                   | <span data-ttu-id="2ef3a-363">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-363">Yes</span></span>                     | <span data-ttu-id="2ef3a-364">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="2ef3a-364">\<resourceId\></span></span> |
| <span data-ttu-id="2ef3a-365">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="2ef3a-365">roleDefinitionId</span></span> | <span data-ttu-id="2ef3a-366">Строка</span><span class="sxs-lookup"><span data-stu-id="2ef3a-366">String</span></span>                                                   | <span data-ttu-id="2ef3a-367">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-367">Yes</span></span>                     | <span data-ttu-id="2ef3a-368">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="2ef3a-368">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="2ef3a-369">субжектид</span><span class="sxs-lookup"><span data-stu-id="2ef3a-369">subjectId</span></span>        | <span data-ttu-id="2ef3a-370">Строка</span><span class="sxs-lookup"><span data-stu-id="2ef3a-370">String</span></span>                                                   | <span data-ttu-id="2ef3a-371">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-371">Yes</span></span>                     | <span data-ttu-id="2ef3a-372">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="2ef3a-372">\<subjectId\></span></span> |
| <span data-ttu-id="2ef3a-373">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="2ef3a-373">assignmentState</span></span>  | <span data-ttu-id="2ef3a-374">Строка</span><span class="sxs-lookup"><span data-stu-id="2ef3a-374">String</span></span>                                                   | <span data-ttu-id="2ef3a-375">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-375">Yes</span></span>                     | <span data-ttu-id="2ef3a-376">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="2ef3a-376">Eligible / Active</span></span> |
| <span data-ttu-id="2ef3a-377">type</span><span class="sxs-lookup"><span data-stu-id="2ef3a-377">type</span></span>             | <span data-ttu-id="2ef3a-378">Строка</span><span class="sxs-lookup"><span data-stu-id="2ef3a-378">String</span></span>                                                   | <span data-ttu-id="2ef3a-379">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-379">Yes</span></span>                     | <span data-ttu-id="2ef3a-380">админупдате</span><span class="sxs-lookup"><span data-stu-id="2ef3a-380">AdminUpdate</span></span> |
| <span data-ttu-id="2ef3a-381">reason</span><span class="sxs-lookup"><span data-stu-id="2ef3a-381">reason</span></span>           | <span data-ttu-id="2ef3a-382">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-382">String</span></span>                                                   | <span data-ttu-id="2ef3a-383">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="2ef3a-383">depends on roleSettings</span></span> |   |
| <span data-ttu-id="2ef3a-384">schedule</span><span class="sxs-lookup"><span data-stu-id="2ef3a-384">schedule</span></span>         | [<span data-ttu-id="2ef3a-385">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2ef3a-385">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="2ef3a-386">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-386">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="2ef3a-387">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ef3a-387">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="2ef3a-388">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ef3a-388">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="2ef3a-389">Пример 6: администратор расширяет назначение ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="2ef3a-389">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="2ef3a-390">В этом примере показано, как расширить назначение роли истечения срока действия для пользователя АНУЖКУСЕР участнику службы управления API.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-390">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="2ef3a-391">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="2ef3a-391">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="2ef3a-392">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ef3a-392">Property</span></span>         | <span data-ttu-id="2ef3a-393">Тип</span><span class="sxs-lookup"><span data-stu-id="2ef3a-393">Type</span></span>                                                     | <span data-ttu-id="2ef3a-394">Обязательный</span><span class="sxs-lookup"><span data-stu-id="2ef3a-394">Required</span></span>                | <span data-ttu-id="2ef3a-395">Значение</span><span class="sxs-lookup"><span data-stu-id="2ef3a-395">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="2ef3a-396">resourceId</span><span class="sxs-lookup"><span data-stu-id="2ef3a-396">resourceId</span></span>       | <span data-ttu-id="2ef3a-397">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-397">String</span></span>                                                   | <span data-ttu-id="2ef3a-398">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-398">Yes</span></span>                     | <span data-ttu-id="2ef3a-399">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="2ef3a-399">\<resourceId\></span></span> |
| <span data-ttu-id="2ef3a-400">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="2ef3a-400">roleDefinitionId</span></span> | <span data-ttu-id="2ef3a-401">Строка</span><span class="sxs-lookup"><span data-stu-id="2ef3a-401">String</span></span>                                                   | <span data-ttu-id="2ef3a-402">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-402">Yes</span></span>                     | <span data-ttu-id="2ef3a-403">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="2ef3a-403">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="2ef3a-404">субжектид</span><span class="sxs-lookup"><span data-stu-id="2ef3a-404">subjectId</span></span>        | <span data-ttu-id="2ef3a-405">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-405">String</span></span>                                                   | <span data-ttu-id="2ef3a-406">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-406">Yes</span></span>                     | <span data-ttu-id="2ef3a-407">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="2ef3a-407">\<subjectId\></span></span> |
| <span data-ttu-id="2ef3a-408">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="2ef3a-408">assignmentState</span></span>  | <span data-ttu-id="2ef3a-409">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-409">String</span></span>                                                   | <span data-ttu-id="2ef3a-410">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-410">Yes</span></span>                     | <span data-ttu-id="2ef3a-411">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="2ef3a-411">Eligible / Active</span></span> |
| <span data-ttu-id="2ef3a-412">type</span><span class="sxs-lookup"><span data-stu-id="2ef3a-412">type</span></span>             | <span data-ttu-id="2ef3a-413">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-413">String</span></span>                                                   | <span data-ttu-id="2ef3a-414">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-414">Yes</span></span>                     | <span data-ttu-id="2ef3a-415">админекстенд</span><span class="sxs-lookup"><span data-stu-id="2ef3a-415">AdminExtend</span></span> |
| <span data-ttu-id="2ef3a-416">reason</span><span class="sxs-lookup"><span data-stu-id="2ef3a-416">reason</span></span>           | <span data-ttu-id="2ef3a-417">String</span><span class="sxs-lookup"><span data-stu-id="2ef3a-417">String</span></span>                                                   | <span data-ttu-id="2ef3a-418">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="2ef3a-418">depends on roleSettings</span></span> |   |
| <span data-ttu-id="2ef3a-419">schedule</span><span class="sxs-lookup"><span data-stu-id="2ef3a-419">schedule</span></span>         | [<span data-ttu-id="2ef3a-420">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2ef3a-420">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="2ef3a-421">Да</span><span class="sxs-lookup"><span data-stu-id="2ef3a-421">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="2ef3a-422">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ef3a-422">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="2ef3a-423">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ef3a-423">Response</span></span>

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
