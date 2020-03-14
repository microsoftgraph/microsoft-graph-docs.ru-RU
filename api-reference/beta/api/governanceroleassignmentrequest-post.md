---
title: Создание governanceRoleAssignmentRequest
description: Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли. В приведенной ниже таблице перечислены операции.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identitiy-platform
ms.openlocfilehash: 2a55cddba5be097e36b85a81e7f451ae92a2a2a6
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639823"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="4c608-104">Создание governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="4c608-104">Create governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="4c608-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c608-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c608-106">Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="4c608-106">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="4c608-107">В приведенной ниже таблице перечислены операции.</span><span class="sxs-lookup"><span data-stu-id="4c608-107">The following table lists the operations.</span></span>

| <span data-ttu-id="4c608-108">Operation</span><span class="sxs-lookup"><span data-stu-id="4c608-108">Operation</span></span>                                   | <span data-ttu-id="4c608-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4c608-109">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="4c608-110">Назначение роли</span><span class="sxs-lookup"><span data-stu-id="4c608-110">Assign a role assignment</span></span>                    | <span data-ttu-id="4c608-111">админадд</span><span class="sxs-lookup"><span data-stu-id="4c608-111">AdminAdd</span></span>    |
| <span data-ttu-id="4c608-112">Активация подходящего назначения роли</span><span class="sxs-lookup"><span data-stu-id="4c608-112">Activate an eligible role assignment</span></span>        | <span data-ttu-id="4c608-113">усерадд</span><span class="sxs-lookup"><span data-stu-id="4c608-113">UserAdd</span></span>     |
| <span data-ttu-id="4c608-114">Деактивация активированного назначения роли</span><span class="sxs-lookup"><span data-stu-id="4c608-114">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="4c608-115">усерремове</span><span class="sxs-lookup"><span data-stu-id="4c608-115">UserRemove</span></span>  |
| <span data-ttu-id="4c608-116">Удаление назначения роли</span><span class="sxs-lookup"><span data-stu-id="4c608-116">Remove a role assignment</span></span>                    | <span data-ttu-id="4c608-117">админремове</span><span class="sxs-lookup"><span data-stu-id="4c608-117">AdminRemove</span></span> |
| <span data-ttu-id="4c608-118">Обновление назначения роли</span><span class="sxs-lookup"><span data-stu-id="4c608-118">Update a role assignment</span></span>                    | <span data-ttu-id="4c608-119">админупдате</span><span class="sxs-lookup"><span data-stu-id="4c608-119">AdminUpdate</span></span> |
| <span data-ttu-id="4c608-120">Запрос на расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="4c608-120">Request to extend my role assignment</span></span>        | <span data-ttu-id="4c608-121">усерекстенд</span><span class="sxs-lookup"><span data-stu-id="4c608-121">UserExtend</span></span>  |
| <span data-ttu-id="4c608-122">Расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="4c608-122">Extend a role assignment</span></span>                    | <span data-ttu-id="4c608-123">админекстенд</span><span class="sxs-lookup"><span data-stu-id="4c608-123">AdminExtend</span></span> |
| <span data-ttu-id="4c608-124">Запрос на продление назначения роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="4c608-124">Request to renew my expired role assignment</span></span> | <span data-ttu-id="4c608-125">усерренев</span><span class="sxs-lookup"><span data-stu-id="4c608-125">UserRenew</span></span>   |
| <span data-ttu-id="4c608-126">Продление назначенной роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="4c608-126">Renew an expired role assignment</span></span>            | <span data-ttu-id="4c608-127">админренев</span><span class="sxs-lookup"><span data-stu-id="4c608-127">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="4c608-128">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c608-128">Permissions</span></span>

<span data-ttu-id="4c608-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c608-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c608-131">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c608-131">Permission type</span></span>                        | <span data-ttu-id="4c608-132">Permissions</span><span class="sxs-lookup"><span data-stu-id="4c608-132">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="4c608-133">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c608-133">Delegated (work or school account)</span></span>     | <span data-ttu-id="4c608-134">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="4c608-134">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="4c608-135">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c608-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c608-136">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c608-136">Not supported.</span></span>                            |
| <span data-ttu-id="4c608-137">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c608-137">Application</span></span>                            | <span data-ttu-id="4c608-138">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c608-138">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c608-139">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c608-139">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="4c608-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c608-140">Request headers</span></span>

| <span data-ttu-id="4c608-141">Имя</span><span class="sxs-lookup"><span data-stu-id="4c608-141">Name</span></span>          | <span data-ttu-id="4c608-142">Описание</span><span class="sxs-lookup"><span data-stu-id="4c608-142">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="4c608-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c608-143">Authorization</span></span> | <span data-ttu-id="4c608-144">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4c608-144">Bearer {code}</span></span>    |
| <span data-ttu-id="4c608-145">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4c608-145">Content-type</span></span>  | <span data-ttu-id="4c608-146">application/json</span><span class="sxs-lookup"><span data-stu-id="4c608-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c608-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c608-147">Request body</span></span>

<span data-ttu-id="4c608-148">В тексте запроса добавьте представление объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c608-148">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="4c608-149">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c608-149">Property</span></span>         | <span data-ttu-id="4c608-150">Тип</span><span class="sxs-lookup"><span data-stu-id="4c608-150">Type</span></span>                                                     | <span data-ttu-id="4c608-151">Описание</span><span class="sxs-lookup"><span data-stu-id="4c608-151">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="4c608-152">resourceId</span><span class="sxs-lookup"><span data-stu-id="4c608-152">resourceId</span></span>       | <span data-ttu-id="4c608-153">String</span><span class="sxs-lookup"><span data-stu-id="4c608-153">String</span></span>                                                   | <span data-ttu-id="4c608-154">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="4c608-154">The ID of the resource.</span></span> <span data-ttu-id="4c608-155">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="4c608-155">Required.</span></span> |
| <span data-ttu-id="4c608-156">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="4c608-156">roleDefinitionId</span></span> | <span data-ttu-id="4c608-157">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-157">String</span></span>                                                   | <span data-ttu-id="4c608-158">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="4c608-158">The ID of the role definition.</span></span> <span data-ttu-id="4c608-159">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="4c608-159">Required.</span></span> |
| <span data-ttu-id="4c608-160">субжектид</span><span class="sxs-lookup"><span data-stu-id="4c608-160">subjectId</span></span>        | <span data-ttu-id="4c608-161">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-161">String</span></span>                                                   | <span data-ttu-id="4c608-162">ИДЕНТИФИКАТОР субъекта.</span><span class="sxs-lookup"><span data-stu-id="4c608-162">The ID of the subject.</span></span> <span data-ttu-id="4c608-163">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="4c608-163">Required.</span></span> |
| <span data-ttu-id="4c608-164">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="4c608-164">assignmentState</span></span>  | <span data-ttu-id="4c608-165">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-165">String</span></span>                                                   | <span data-ttu-id="4c608-166">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="4c608-166">The state of assignment.</span></span> <span data-ttu-id="4c608-167">Значение может быть `Eligible` и `Active`.</span><span class="sxs-lookup"><span data-stu-id="4c608-167">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="4c608-168">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="4c608-168">Required.</span></span> |
| <span data-ttu-id="4c608-169">type</span><span class="sxs-lookup"><span data-stu-id="4c608-169">type</span></span>             | <span data-ttu-id="4c608-170">String</span><span class="sxs-lookup"><span data-stu-id="4c608-170">String</span></span>                                                   | <span data-ttu-id="4c608-171">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="4c608-171">The request type.</span></span> <span data-ttu-id="4c608-172">Возможные значения: `AdminAdd`, `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `AdminRenew` `AdminExtend`,,,,, и. `UserExtend` `UserRenew`</span><span class="sxs-lookup"><span data-stu-id="4c608-172">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="4c608-173">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="4c608-173">Required.</span></span> |
| <span data-ttu-id="4c608-174">reason</span><span class="sxs-lookup"><span data-stu-id="4c608-174">reason</span></span>           | <span data-ttu-id="4c608-175">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-175">String</span></span>                                                   | <span data-ttu-id="4c608-176">Необходимо указать причину для запроса на назначение роли для аудита и проверки.</span><span class="sxs-lookup"><span data-stu-id="4c608-176">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="4c608-177">schedule</span><span class="sxs-lookup"><span data-stu-id="4c608-177">schedule</span></span>         | [<span data-ttu-id="4c608-178">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="4c608-178">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="4c608-179">Расписание запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="4c608-179">The schedule of the role assignment request.</span></span> <span data-ttu-id="4c608-180">`UserAdd`Для типа запроса `AdminAdd`,, `AdminUpdate`, и `AdminExtend`, он необходим.</span><span class="sxs-lookup"><span data-stu-id="4c608-180">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="4c608-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c608-181">Response</span></span>

<span data-ttu-id="4c608-182">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c608-182">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="4c608-183">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="4c608-183">Error codes</span></span>

<span data-ttu-id="4c608-184">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="4c608-184">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="4c608-185">Кроме того, он возвращает коды ошибок, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="4c608-185">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="4c608-186">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="4c608-186">Error code</span></span>     | <span data-ttu-id="4c608-187">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="4c608-187">Error message</span></span>                               | <span data-ttu-id="4c608-188">Сведения</span><span class="sxs-lookup"><span data-stu-id="4c608-188">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="4c608-189">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="4c608-189">400 BadRequest</span></span> | <span data-ttu-id="4c608-190">роленотфаунд</span><span class="sxs-lookup"><span data-stu-id="4c608-190">RoleNotFound</span></span>                                | <span data-ttu-id="4c608-191">Не `roleDefinitionId` удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="4c608-191">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="4c608-192">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="4c608-192">400 BadRequest</span></span> | <span data-ttu-id="4c608-193">ресаурцеислоккед</span><span class="sxs-lookup"><span data-stu-id="4c608-193">ResourceIsLocked</span></span>                            | <span data-ttu-id="4c608-194">Ресурс, указанный в теле запроса, находится в состоянии `Locked` и не может создавать запросы на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="4c608-194">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="4c608-195">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="4c608-195">400 BadRequest</span></span> | <span data-ttu-id="4c608-196">субжектнотфаунд</span><span class="sxs-lookup"><span data-stu-id="4c608-196">SubjectNotFound</span></span>                             | <span data-ttu-id="4c608-197">Не `subjectId` удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="4c608-197">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="4c608-198">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="4c608-198">400 BadRequest</span></span> | <span data-ttu-id="4c608-199">пендингролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="4c608-199">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="4c608-200">В системе уже существует ожидающий [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="4c608-200">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="4c608-201">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="4c608-201">400 BadRequest</span></span> | <span data-ttu-id="4c608-202">ролеассигнментексистс</span><span class="sxs-lookup"><span data-stu-id="4c608-202">RoleAssignmentExists</span></span>                        | <span data-ttu-id="4c608-203">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , который требуется создать, уже существует в системе.</span><span class="sxs-lookup"><span data-stu-id="4c608-203">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="4c608-204">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="4c608-204">400 BadRequest</span></span> | <span data-ttu-id="4c608-205">ролеассигнментдоеснотексист</span><span class="sxs-lookup"><span data-stu-id="4c608-205">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="4c608-206">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , запрошенный для обновления или расширения, не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="4c608-206">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="4c608-207">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="4c608-207">400 BadRequest</span></span> | <span data-ttu-id="4c608-208">ролеассигнментрекуестполицивалидатионфаилед</span><span class="sxs-lookup"><span data-stu-id="4c608-208">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="4c608-209">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) не отвечает внутренним политикам и не может быть создан.</span><span class="sxs-lookup"><span data-stu-id="4c608-209">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="4c608-210">Примеры</span><span class="sxs-lookup"><span data-stu-id="4c608-210">Examples</span></span>

<span data-ttu-id="4c608-211">В следующих примерах показано, как использовать этот API.</span><span class="sxs-lookup"><span data-stu-id="4c608-211">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="4c608-212">Пример 1: Администратор назначает пользователю роль</span><span class="sxs-lookup"><span data-stu-id="4c608-212">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="4c608-213">В этом примере администратор назначает пользователю nawu@fimdev.net роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="4c608-213">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="4c608-214">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="4c608-214">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="4c608-215">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c608-215">Property</span></span>         | <span data-ttu-id="4c608-216">Тип</span><span class="sxs-lookup"><span data-stu-id="4c608-216">Type</span></span>                                                     | <span data-ttu-id="4c608-217">Обязательное</span><span class="sxs-lookup"><span data-stu-id="4c608-217">Required</span></span>                 | <span data-ttu-id="4c608-218">Значение</span><span class="sxs-lookup"><span data-stu-id="4c608-218">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="4c608-219">resourceId</span><span class="sxs-lookup"><span data-stu-id="4c608-219">resourceId</span></span>       | <span data-ttu-id="4c608-220">String</span><span class="sxs-lookup"><span data-stu-id="4c608-220">String</span></span>                                                   | <span data-ttu-id="4c608-221">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-221">Yes</span></span>                      | <span data-ttu-id="4c608-222">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="4c608-222">\<resourceId\></span></span> |
| <span data-ttu-id="4c608-223">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="4c608-223">roleDefinitionId</span></span> | <span data-ttu-id="4c608-224">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-224">String</span></span>                                                   | <span data-ttu-id="4c608-225">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-225">Yes</span></span>                      | <span data-ttu-id="4c608-226">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="4c608-226">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="4c608-227">субжектид</span><span class="sxs-lookup"><span data-stu-id="4c608-227">subjectId</span></span>        | <span data-ttu-id="4c608-228">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-228">String</span></span>                                                   | <span data-ttu-id="4c608-229">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-229">Yes</span></span>                      | <span data-ttu-id="4c608-230">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="4c608-230">\<subjectId\></span></span> |
| <span data-ttu-id="4c608-231">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="4c608-231">assignmentState</span></span>  | <span data-ttu-id="4c608-232">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-232">String</span></span>                                                   | <span data-ttu-id="4c608-233">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-233">Yes</span></span>                      | <span data-ttu-id="4c608-234">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="4c608-234">Eligible / Active</span></span> |
| <span data-ttu-id="4c608-235">type</span><span class="sxs-lookup"><span data-stu-id="4c608-235">type</span></span>             | <span data-ttu-id="4c608-236">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-236">String</span></span>                                                   | <span data-ttu-id="4c608-237">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-237">Yes</span></span>                      | <span data-ttu-id="4c608-238">админадд</span><span class="sxs-lookup"><span data-stu-id="4c608-238">AdminAdd</span></span> |
| <span data-ttu-id="4c608-239">reason</span><span class="sxs-lookup"><span data-stu-id="4c608-239">reason</span></span>           | <span data-ttu-id="4c608-240">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-240">String</span></span>                                                   | <span data-ttu-id="4c608-241">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="4c608-241">depends on role Settings</span></span> |   |
| <span data-ttu-id="4c608-242">schedule</span><span class="sxs-lookup"><span data-stu-id="4c608-242">schedule</span></span>         | [<span data-ttu-id="4c608-243">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="4c608-243">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="4c608-244">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-244">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="4c608-245">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c608-245">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4c608-246">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c608-246">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4c608-247">C#</span><span class="sxs-lookup"><span data-stu-id="4c608-247">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c608-248">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c608-248">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c608-249">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c608-249">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="4c608-250">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c608-250">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="4c608-251">Пример 2: пользователь активирует подходящие роли</span><span class="sxs-lookup"><span data-stu-id="4c608-251">Example 2: User activates eligible role</span></span>

<span data-ttu-id="4c608-252">В этом примере пользователь nawu@fimdev.net активирует соответствующую роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="4c608-252">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="4c608-253">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c608-253">Property</span></span>         | <span data-ttu-id="4c608-254">Тип</span><span class="sxs-lookup"><span data-stu-id="4c608-254">Type</span></span>                                                     | <span data-ttu-id="4c608-255">Обязательное</span><span class="sxs-lookup"><span data-stu-id="4c608-255">Required</span></span>                 | <span data-ttu-id="4c608-256">Значение</span><span class="sxs-lookup"><span data-stu-id="4c608-256">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="4c608-257">resourceId</span><span class="sxs-lookup"><span data-stu-id="4c608-257">resourceId</span></span>       | <span data-ttu-id="4c608-258">String</span><span class="sxs-lookup"><span data-stu-id="4c608-258">String</span></span>                                                   | <span data-ttu-id="4c608-259">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-259">Yes</span></span>                      | <span data-ttu-id="4c608-260">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="4c608-260">\<resourceId\></span></span> |
| <span data-ttu-id="4c608-261">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="4c608-261">roleDefinitionId</span></span> | <span data-ttu-id="4c608-262">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-262">String</span></span>                                                   | <span data-ttu-id="4c608-263">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-263">Yes</span></span>                      | <span data-ttu-id="4c608-264">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="4c608-264">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="4c608-265">субжектид</span><span class="sxs-lookup"><span data-stu-id="4c608-265">subjectId</span></span>        | <span data-ttu-id="4c608-266">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-266">String</span></span>                                                   | <span data-ttu-id="4c608-267">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-267">Yes</span></span>                      | <span data-ttu-id="4c608-268">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="4c608-268">\<subjectId\></span></span> |
| <span data-ttu-id="4c608-269">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="4c608-269">assignmentState</span></span>  | <span data-ttu-id="4c608-270">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-270">String</span></span>                                                   | <span data-ttu-id="4c608-271">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-271">Yes</span></span>                      | <span data-ttu-id="4c608-272">Активное</span><span class="sxs-lookup"><span data-stu-id="4c608-272">Active</span></span> |
| <span data-ttu-id="4c608-273">type</span><span class="sxs-lookup"><span data-stu-id="4c608-273">type</span></span>             | <span data-ttu-id="4c608-274">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-274">String</span></span>                                                   | <span data-ttu-id="4c608-275">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-275">Yes</span></span>                      | <span data-ttu-id="4c608-276">усерадд</span><span class="sxs-lookup"><span data-stu-id="4c608-276">UserAdd</span></span> |
| <span data-ttu-id="4c608-277">reason</span><span class="sxs-lookup"><span data-stu-id="4c608-277">reason</span></span>           | <span data-ttu-id="4c608-278">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-278">String</span></span>                                                   | <span data-ttu-id="4c608-279">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="4c608-279">depends on role Settings</span></span> |   |
| <span data-ttu-id="4c608-280">schedule</span><span class="sxs-lookup"><span data-stu-id="4c608-280">schedule</span></span>         | [<span data-ttu-id="4c608-281">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="4c608-281">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="4c608-282">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-282">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="4c608-283">Запросить</span><span class="sxs-lookup"><span data-stu-id="4c608-283">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="4c608-284">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c608-284">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="4c608-285">Пример 3: пользователь отключает назначенную роль</span><span class="sxs-lookup"><span data-stu-id="4c608-285">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="4c608-286">В этом примере пользователь nawu@fimdev.net отключает активную роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="4c608-286">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="4c608-287">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c608-287">Property</span></span>         | <span data-ttu-id="4c608-288">Тип</span><span class="sxs-lookup"><span data-stu-id="4c608-288">Type</span></span>                                                     | <span data-ttu-id="4c608-289">Обязательное</span><span class="sxs-lookup"><span data-stu-id="4c608-289">Required</span></span> | <span data-ttu-id="4c608-290">Значение</span><span class="sxs-lookup"><span data-stu-id="4c608-290">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="4c608-291">resourceId</span><span class="sxs-lookup"><span data-stu-id="4c608-291">resourceId</span></span>       | <span data-ttu-id="4c608-292">String</span><span class="sxs-lookup"><span data-stu-id="4c608-292">String</span></span>                                                   | <span data-ttu-id="4c608-293">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-293">Yes</span></span>      | <span data-ttu-id="4c608-294">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="4c608-294">\<resourceId\></span></span> |
| <span data-ttu-id="4c608-295">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="4c608-295">roleDefinitionId</span></span> | <span data-ttu-id="4c608-296">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-296">String</span></span>                                                   | <span data-ttu-id="4c608-297">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-297">Yes</span></span>      | <span data-ttu-id="4c608-298">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="4c608-298">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="4c608-299">субжектид</span><span class="sxs-lookup"><span data-stu-id="4c608-299">subjectId</span></span>        | <span data-ttu-id="4c608-300">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-300">String</span></span>                                                   | <span data-ttu-id="4c608-301">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-301">Yes</span></span>      | <span data-ttu-id="4c608-302">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="4c608-302">\<subjectId\></span></span> |
| <span data-ttu-id="4c608-303">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="4c608-303">assignmentState</span></span>  | <span data-ttu-id="4c608-304">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-304">String</span></span>                                                   | <span data-ttu-id="4c608-305">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-305">Yes</span></span>      | <span data-ttu-id="4c608-306">Активное</span><span class="sxs-lookup"><span data-stu-id="4c608-306">Active</span></span> |
| <span data-ttu-id="4c608-307">type</span><span class="sxs-lookup"><span data-stu-id="4c608-307">type</span></span>             | <span data-ttu-id="4c608-308">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-308">String</span></span>                                                   | <span data-ttu-id="4c608-309">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-309">Yes</span></span>      | <span data-ttu-id="4c608-310">усерремове</span><span class="sxs-lookup"><span data-stu-id="4c608-310">UserRemove</span></span> |
| <span data-ttu-id="4c608-311">reason</span><span class="sxs-lookup"><span data-stu-id="4c608-311">reason</span></span>           | <span data-ttu-id="4c608-312">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-312">String</span></span>                                                   | <span data-ttu-id="4c608-313">Нет</span><span class="sxs-lookup"><span data-stu-id="4c608-313">No</span></span>       |   |
| <span data-ttu-id="4c608-314">schedule</span><span class="sxs-lookup"><span data-stu-id="4c608-314">schedule</span></span>         | [<span data-ttu-id="4c608-315">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="4c608-315">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="4c608-316">Нет</span><span class="sxs-lookup"><span data-stu-id="4c608-316">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="4c608-317">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c608-317">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="4c608-318">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c608-318">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="4c608-319">Пример 4: Администратор удаляет пользователя из роли</span><span class="sxs-lookup"><span data-stu-id="4c608-319">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="4c608-320">В этом примере администратор удаляет пользователя nawu@fimdev.net из роли читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="4c608-320">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="4c608-321">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="4c608-321">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="4c608-322">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c608-322">Property</span></span>         | <span data-ttu-id="4c608-323">Тип</span><span class="sxs-lookup"><span data-stu-id="4c608-323">Type</span></span>                                                     | <span data-ttu-id="4c608-324">Обязательное</span><span class="sxs-lookup"><span data-stu-id="4c608-324">Required</span></span> | <span data-ttu-id="4c608-325">Значение</span><span class="sxs-lookup"><span data-stu-id="4c608-325">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="4c608-326">resourceId</span><span class="sxs-lookup"><span data-stu-id="4c608-326">resourceId</span></span>       | <span data-ttu-id="4c608-327">String</span><span class="sxs-lookup"><span data-stu-id="4c608-327">String</span></span>                                                   | <span data-ttu-id="4c608-328">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-328">Yes</span></span>      | <span data-ttu-id="4c608-329">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="4c608-329">\<resourceId\></span></span> |
| <span data-ttu-id="4c608-330">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="4c608-330">roleDefinitionId</span></span> | <span data-ttu-id="4c608-331">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-331">String</span></span>                                                   | <span data-ttu-id="4c608-332">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-332">Yes</span></span>      | <span data-ttu-id="4c608-333">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="4c608-333">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="4c608-334">субжектид</span><span class="sxs-lookup"><span data-stu-id="4c608-334">subjectId</span></span>        | <span data-ttu-id="4c608-335">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-335">String</span></span>                                                   | <span data-ttu-id="4c608-336">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-336">Yes</span></span>      | <span data-ttu-id="4c608-337">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="4c608-337">\<subjectId\></span></span> |
| <span data-ttu-id="4c608-338">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="4c608-338">assignmentState</span></span>  | <span data-ttu-id="4c608-339">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-339">String</span></span>                                                   | <span data-ttu-id="4c608-340">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-340">Yes</span></span>      | <span data-ttu-id="4c608-341">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="4c608-341">Eligible / Active</span></span> |
| <span data-ttu-id="4c608-342">type</span><span class="sxs-lookup"><span data-stu-id="4c608-342">type</span></span>             | <span data-ttu-id="4c608-343">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-343">String</span></span>                                                   | <span data-ttu-id="4c608-344">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-344">Yes</span></span>      | <span data-ttu-id="4c608-345">админремове</span><span class="sxs-lookup"><span data-stu-id="4c608-345">AdminRemove</span></span> |
| <span data-ttu-id="4c608-346">reason</span><span class="sxs-lookup"><span data-stu-id="4c608-346">reason</span></span>           | <span data-ttu-id="4c608-347">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-347">String</span></span>                                                   | <span data-ttu-id="4c608-348">Нет</span><span class="sxs-lookup"><span data-stu-id="4c608-348">No</span></span>       |   |
| <span data-ttu-id="4c608-349">schedule</span><span class="sxs-lookup"><span data-stu-id="4c608-349">schedule</span></span>         | [<span data-ttu-id="4c608-350">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="4c608-350">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="4c608-351">Нет</span><span class="sxs-lookup"><span data-stu-id="4c608-351">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="4c608-352">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c608-352">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="4c608-353">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c608-353">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="4c608-354">Пример 5: "Администратор обновляет назначение ролей"</span><span class="sxs-lookup"><span data-stu-id="4c608-354">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="4c608-355">В этом примере администраторы обновляют назначение роли пользователя nawu@fimdev.net владельцу.</span><span class="sxs-lookup"><span data-stu-id="4c608-355">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="4c608-356">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="4c608-356">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="4c608-357">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c608-357">Property</span></span>         | <span data-ttu-id="4c608-358">Тип</span><span class="sxs-lookup"><span data-stu-id="4c608-358">Type</span></span>                                                     | <span data-ttu-id="4c608-359">Обязательное</span><span class="sxs-lookup"><span data-stu-id="4c608-359">Required</span></span>                | <span data-ttu-id="4c608-360">Значение</span><span class="sxs-lookup"><span data-stu-id="4c608-360">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="4c608-361">resourceId</span><span class="sxs-lookup"><span data-stu-id="4c608-361">resourceId</span></span>       | <span data-ttu-id="4c608-362">String</span><span class="sxs-lookup"><span data-stu-id="4c608-362">String</span></span>                                                   | <span data-ttu-id="4c608-363">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-363">Yes</span></span>                     | <span data-ttu-id="4c608-364">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="4c608-364">\<resourceId\></span></span> |
| <span data-ttu-id="4c608-365">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="4c608-365">roleDefinitionId</span></span> | <span data-ttu-id="4c608-366">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-366">String</span></span>                                                   | <span data-ttu-id="4c608-367">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-367">Yes</span></span>                     | <span data-ttu-id="4c608-368">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="4c608-368">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="4c608-369">субжектид</span><span class="sxs-lookup"><span data-stu-id="4c608-369">subjectId</span></span>        | <span data-ttu-id="4c608-370">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-370">String</span></span>                                                   | <span data-ttu-id="4c608-371">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-371">Yes</span></span>                     | <span data-ttu-id="4c608-372">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="4c608-372">\<subjectId\></span></span> |
| <span data-ttu-id="4c608-373">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="4c608-373">assignmentState</span></span>  | <span data-ttu-id="4c608-374">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-374">String</span></span>                                                   | <span data-ttu-id="4c608-375">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-375">Yes</span></span>                     | <span data-ttu-id="4c608-376">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="4c608-376">Eligible / Active</span></span> |
| <span data-ttu-id="4c608-377">type</span><span class="sxs-lookup"><span data-stu-id="4c608-377">type</span></span>             | <span data-ttu-id="4c608-378">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-378">String</span></span>                                                   | <span data-ttu-id="4c608-379">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-379">Yes</span></span>                     | <span data-ttu-id="4c608-380">админупдате</span><span class="sxs-lookup"><span data-stu-id="4c608-380">AdminUpdate</span></span> |
| <span data-ttu-id="4c608-381">reason</span><span class="sxs-lookup"><span data-stu-id="4c608-381">reason</span></span>           | <span data-ttu-id="4c608-382">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-382">String</span></span>                                                   | <span data-ttu-id="4c608-383">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="4c608-383">depends on roleSettings</span></span> |   |
| <span data-ttu-id="4c608-384">schedule</span><span class="sxs-lookup"><span data-stu-id="4c608-384">schedule</span></span>         | [<span data-ttu-id="4c608-385">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="4c608-385">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="4c608-386">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-386">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="4c608-387">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c608-387">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="4c608-388">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c608-388">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="4c608-389">Пример 6: администратор расширяет назначение ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="4c608-389">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="4c608-390">В этом примере показано, как расширить назначение роли истечения срока действия для пользователя АНУЖКУСЕР участнику службы управления API.</span><span class="sxs-lookup"><span data-stu-id="4c608-390">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="4c608-391">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="4c608-391">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="4c608-392">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c608-392">Property</span></span>         | <span data-ttu-id="4c608-393">Тип</span><span class="sxs-lookup"><span data-stu-id="4c608-393">Type</span></span>                                                     | <span data-ttu-id="4c608-394">Обязательное</span><span class="sxs-lookup"><span data-stu-id="4c608-394">Required</span></span>                | <span data-ttu-id="4c608-395">Значение</span><span class="sxs-lookup"><span data-stu-id="4c608-395">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="4c608-396">resourceId</span><span class="sxs-lookup"><span data-stu-id="4c608-396">resourceId</span></span>       | <span data-ttu-id="4c608-397">String</span><span class="sxs-lookup"><span data-stu-id="4c608-397">String</span></span>                                                   | <span data-ttu-id="4c608-398">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-398">Yes</span></span>                     | <span data-ttu-id="4c608-399">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="4c608-399">\<resourceId\></span></span> |
| <span data-ttu-id="4c608-400">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="4c608-400">roleDefinitionId</span></span> | <span data-ttu-id="4c608-401">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-401">String</span></span>                                                   | <span data-ttu-id="4c608-402">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-402">Yes</span></span>                     | <span data-ttu-id="4c608-403">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="4c608-403">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="4c608-404">субжектид</span><span class="sxs-lookup"><span data-stu-id="4c608-404">subjectId</span></span>        | <span data-ttu-id="4c608-405">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-405">String</span></span>                                                   | <span data-ttu-id="4c608-406">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-406">Yes</span></span>                     | <span data-ttu-id="4c608-407">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="4c608-407">\<subjectId\></span></span> |
| <span data-ttu-id="4c608-408">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="4c608-408">assignmentState</span></span>  | <span data-ttu-id="4c608-409">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-409">String</span></span>                                                   | <span data-ttu-id="4c608-410">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-410">Yes</span></span>                     | <span data-ttu-id="4c608-411">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="4c608-411">Eligible / Active</span></span> |
| <span data-ttu-id="4c608-412">type</span><span class="sxs-lookup"><span data-stu-id="4c608-412">type</span></span>             | <span data-ttu-id="4c608-413">String</span><span class="sxs-lookup"><span data-stu-id="4c608-413">String</span></span>                                                   | <span data-ttu-id="4c608-414">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-414">Yes</span></span>                     | <span data-ttu-id="4c608-415">админекстенд</span><span class="sxs-lookup"><span data-stu-id="4c608-415">AdminExtend</span></span> |
| <span data-ttu-id="4c608-416">reason</span><span class="sxs-lookup"><span data-stu-id="4c608-416">reason</span></span>           | <span data-ttu-id="4c608-417">Строка</span><span class="sxs-lookup"><span data-stu-id="4c608-417">String</span></span>                                                   | <span data-ttu-id="4c608-418">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="4c608-418">depends on roleSettings</span></span> |   |
| <span data-ttu-id="4c608-419">schedule</span><span class="sxs-lookup"><span data-stu-id="4c608-419">schedule</span></span>         | [<span data-ttu-id="4c608-420">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="4c608-420">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="4c608-421">Да</span><span class="sxs-lookup"><span data-stu-id="4c608-421">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="4c608-422">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c608-422">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="4c608-423">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c608-423">Response</span></span>

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
