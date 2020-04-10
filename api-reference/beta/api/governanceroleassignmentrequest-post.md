---
title: Создание governanceRoleAssignmentRequest
description: Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли. В приведенной ниже таблице перечислены операции.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: b038ca74eb8046e4ae77a8a31715a473a3518ba1
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218873"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="3d99d-104">Создание governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="3d99d-104">Create governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="3d99d-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d99d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d99d-106">Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="3d99d-106">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="3d99d-107">В приведенной ниже таблице перечислены операции.</span><span class="sxs-lookup"><span data-stu-id="3d99d-107">The following table lists the operations.</span></span>

| <span data-ttu-id="3d99d-108">Operation</span><span class="sxs-lookup"><span data-stu-id="3d99d-108">Operation</span></span>                                   | <span data-ttu-id="3d99d-109">Type</span><span class="sxs-lookup"><span data-stu-id="3d99d-109">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="3d99d-110">Назначение роли</span><span class="sxs-lookup"><span data-stu-id="3d99d-110">Assign a role assignment</span></span>                    | <span data-ttu-id="3d99d-111">админадд</span><span class="sxs-lookup"><span data-stu-id="3d99d-111">AdminAdd</span></span>    |
| <span data-ttu-id="3d99d-112">Активация подходящего назначения роли</span><span class="sxs-lookup"><span data-stu-id="3d99d-112">Activate an eligible role assignment</span></span>        | <span data-ttu-id="3d99d-113">усерадд</span><span class="sxs-lookup"><span data-stu-id="3d99d-113">UserAdd</span></span>     |
| <span data-ttu-id="3d99d-114">Деактивация активированного назначения роли</span><span class="sxs-lookup"><span data-stu-id="3d99d-114">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="3d99d-115">усерремове</span><span class="sxs-lookup"><span data-stu-id="3d99d-115">UserRemove</span></span>  |
| <span data-ttu-id="3d99d-116">Удаление назначения роли</span><span class="sxs-lookup"><span data-stu-id="3d99d-116">Remove a role assignment</span></span>                    | <span data-ttu-id="3d99d-117">админремове</span><span class="sxs-lookup"><span data-stu-id="3d99d-117">AdminRemove</span></span> |
| <span data-ttu-id="3d99d-118">Обновление назначения роли</span><span class="sxs-lookup"><span data-stu-id="3d99d-118">Update a role assignment</span></span>                    | <span data-ttu-id="3d99d-119">админупдате</span><span class="sxs-lookup"><span data-stu-id="3d99d-119">AdminUpdate</span></span> |
| <span data-ttu-id="3d99d-120">Запрос на расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="3d99d-120">Request to extend my role assignment</span></span>        | <span data-ttu-id="3d99d-121">усерекстенд</span><span class="sxs-lookup"><span data-stu-id="3d99d-121">UserExtend</span></span>  |
| <span data-ttu-id="3d99d-122">Расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="3d99d-122">Extend a role assignment</span></span>                    | <span data-ttu-id="3d99d-123">админекстенд</span><span class="sxs-lookup"><span data-stu-id="3d99d-123">AdminExtend</span></span> |
| <span data-ttu-id="3d99d-124">Запрос на продление назначения роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="3d99d-124">Request to renew my expired role assignment</span></span> | <span data-ttu-id="3d99d-125">усерренев</span><span class="sxs-lookup"><span data-stu-id="3d99d-125">UserRenew</span></span>   |
| <span data-ttu-id="3d99d-126">Продление назначенной роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="3d99d-126">Renew an expired role assignment</span></span>            | <span data-ttu-id="3d99d-127">админренев</span><span class="sxs-lookup"><span data-stu-id="3d99d-127">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="3d99d-128">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3d99d-128">Permissions</span></span>

<span data-ttu-id="3d99d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d99d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3d99d-131">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d99d-131">Permission type</span></span>                        | <span data-ttu-id="3d99d-132">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3d99d-132">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="3d99d-133">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d99d-133">Delegated (work or school account)</span></span>     | <span data-ttu-id="3d99d-134">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="3d99d-134">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="3d99d-135">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d99d-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d99d-136">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d99d-136">Not supported.</span></span>                            |
| <span data-ttu-id="3d99d-137">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d99d-137">Application</span></span>                            | <span data-ttu-id="3d99d-138">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d99d-138">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d99d-139">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d99d-139">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="3d99d-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d99d-140">Request headers</span></span>

| <span data-ttu-id="3d99d-141">Имя</span><span class="sxs-lookup"><span data-stu-id="3d99d-141">Name</span></span>          | <span data-ttu-id="3d99d-142">Описание</span><span class="sxs-lookup"><span data-stu-id="3d99d-142">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="3d99d-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d99d-143">Authorization</span></span> | <span data-ttu-id="3d99d-144">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3d99d-144">Bearer {code}</span></span>    |
| <span data-ttu-id="3d99d-145">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3d99d-145">Content-type</span></span>  | <span data-ttu-id="3d99d-146">application/json</span><span class="sxs-lookup"><span data-stu-id="3d99d-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d99d-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d99d-147">Request body</span></span>

<span data-ttu-id="3d99d-148">В тексте запроса добавьте представление объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d99d-148">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="3d99d-149">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d99d-149">Property</span></span>         | <span data-ttu-id="3d99d-150">Тип</span><span class="sxs-lookup"><span data-stu-id="3d99d-150">Type</span></span>                                                     | <span data-ttu-id="3d99d-151">Описание</span><span class="sxs-lookup"><span data-stu-id="3d99d-151">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="3d99d-152">resourceId</span><span class="sxs-lookup"><span data-stu-id="3d99d-152">resourceId</span></span>       | <span data-ttu-id="3d99d-153">String</span><span class="sxs-lookup"><span data-stu-id="3d99d-153">String</span></span>                                                   | <span data-ttu-id="3d99d-154">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="3d99d-154">The ID of the resource.</span></span> <span data-ttu-id="3d99d-155">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="3d99d-155">Required.</span></span> |
| <span data-ttu-id="3d99d-156">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="3d99d-156">roleDefinitionId</span></span> | <span data-ttu-id="3d99d-157">Строка</span><span class="sxs-lookup"><span data-stu-id="3d99d-157">String</span></span>                                                   | <span data-ttu-id="3d99d-158">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="3d99d-158">The ID of the role definition.</span></span> <span data-ttu-id="3d99d-159">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="3d99d-159">Required.</span></span> |
| <span data-ttu-id="3d99d-160">субжектид</span><span class="sxs-lookup"><span data-stu-id="3d99d-160">subjectId</span></span>        | <span data-ttu-id="3d99d-161">Строка</span><span class="sxs-lookup"><span data-stu-id="3d99d-161">String</span></span>                                                   | <span data-ttu-id="3d99d-162">ИДЕНТИФИКАТОР субъекта.</span><span class="sxs-lookup"><span data-stu-id="3d99d-162">The ID of the subject.</span></span> <span data-ttu-id="3d99d-163">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="3d99d-163">Required.</span></span> |
| <span data-ttu-id="3d99d-164">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="3d99d-164">assignmentState</span></span>  | <span data-ttu-id="3d99d-165">Строка</span><span class="sxs-lookup"><span data-stu-id="3d99d-165">String</span></span>                                                   | <span data-ttu-id="3d99d-166">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="3d99d-166">The state of assignment.</span></span> <span data-ttu-id="3d99d-167">Значение может быть `Eligible` и `Active`.</span><span class="sxs-lookup"><span data-stu-id="3d99d-167">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="3d99d-168">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="3d99d-168">Required.</span></span> |
| <span data-ttu-id="3d99d-169">type</span><span class="sxs-lookup"><span data-stu-id="3d99d-169">type</span></span>             | <span data-ttu-id="3d99d-170">String</span><span class="sxs-lookup"><span data-stu-id="3d99d-170">String</span></span>                                                   | <span data-ttu-id="3d99d-171">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="3d99d-171">The request type.</span></span> <span data-ttu-id="3d99d-172">Возможные значения: `AdminAdd`, `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `AdminRenew` `AdminExtend`,,,,, и. `UserExtend` `UserRenew`</span><span class="sxs-lookup"><span data-stu-id="3d99d-172">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="3d99d-173">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="3d99d-173">Required.</span></span> |
| <span data-ttu-id="3d99d-174">reason</span><span class="sxs-lookup"><span data-stu-id="3d99d-174">reason</span></span>           | <span data-ttu-id="3d99d-175">Строка</span><span class="sxs-lookup"><span data-stu-id="3d99d-175">String</span></span>                                                   | <span data-ttu-id="3d99d-176">Необходимо указать причину для запроса на назначение роли для аудита и проверки.</span><span class="sxs-lookup"><span data-stu-id="3d99d-176">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="3d99d-177">schedule</span><span class="sxs-lookup"><span data-stu-id="3d99d-177">schedule</span></span>         | [<span data-ttu-id="3d99d-178">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="3d99d-178">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="3d99d-179">Расписание запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="3d99d-179">The schedule of the role assignment request.</span></span> <span data-ttu-id="3d99d-180">`UserAdd`Для типа запроса `AdminAdd`,, `AdminUpdate`, и `AdminExtend`, он необходим.</span><span class="sxs-lookup"><span data-stu-id="3d99d-180">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="3d99d-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d99d-181">Response</span></span>

<span data-ttu-id="3d99d-182">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3d99d-182">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="3d99d-183">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="3d99d-183">Error codes</span></span>

<span data-ttu-id="3d99d-184">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="3d99d-184">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="3d99d-185">Кроме того, он возвращает коды ошибок, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="3d99d-185">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="3d99d-186">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="3d99d-186">Error code</span></span>     | <span data-ttu-id="3d99d-187">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="3d99d-187">Error message</span></span>                               | <span data-ttu-id="3d99d-188">Сведения</span><span class="sxs-lookup"><span data-stu-id="3d99d-188">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="3d99d-189">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="3d99d-189">400 BadRequest</span></span> | <span data-ttu-id="3d99d-190">роленотфаунд</span><span class="sxs-lookup"><span data-stu-id="3d99d-190">RoleNotFound</span></span>                                | <span data-ttu-id="3d99d-191">Не `roleDefinitionId` удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="3d99d-191">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="3d99d-192">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="3d99d-192">400 BadRequest</span></span> | <span data-ttu-id="3d99d-193">ресаурцеислоккед</span><span class="sxs-lookup"><span data-stu-id="3d99d-193">ResourceIsLocked</span></span>                            | <span data-ttu-id="3d99d-194">Ресурс, указанный в теле запроса, находится в состоянии `Locked` и не может создавать запросы на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="3d99d-194">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="3d99d-195">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="3d99d-195">400 BadRequest</span></span> | <span data-ttu-id="3d99d-196">субжектнотфаунд</span><span class="sxs-lookup"><span data-stu-id="3d99d-196">SubjectNotFound</span></span>                             | <span data-ttu-id="3d99d-197">Не `subjectId` удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="3d99d-197">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="3d99d-198">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="3d99d-198">400 BadRequest</span></span> | <span data-ttu-id="3d99d-199">пендингролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="3d99d-199">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="3d99d-200">В системе уже существует ожидающий [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="3d99d-200">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="3d99d-201">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="3d99d-201">400 BadRequest</span></span> | <span data-ttu-id="3d99d-202">ролеассигнментексистс</span><span class="sxs-lookup"><span data-stu-id="3d99d-202">RoleAssignmentExists</span></span>                        | <span data-ttu-id="3d99d-203">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , который требуется создать, уже существует в системе.</span><span class="sxs-lookup"><span data-stu-id="3d99d-203">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="3d99d-204">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="3d99d-204">400 BadRequest</span></span> | <span data-ttu-id="3d99d-205">ролеассигнментдоеснотексист</span><span class="sxs-lookup"><span data-stu-id="3d99d-205">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="3d99d-206">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , запрошенный для обновления или расширения, не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="3d99d-206">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="3d99d-207">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="3d99d-207">400 BadRequest</span></span> | <span data-ttu-id="3d99d-208">ролеассигнментрекуестполицивалидатионфаилед</span><span class="sxs-lookup"><span data-stu-id="3d99d-208">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="3d99d-209">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) не отвечает внутренним политикам и не может быть создан.</span><span class="sxs-lookup"><span data-stu-id="3d99d-209">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="3d99d-210">Примеры</span><span class="sxs-lookup"><span data-stu-id="3d99d-210">Examples</span></span>

<span data-ttu-id="3d99d-211">В следующих примерах показано, как использовать этот API.</span><span class="sxs-lookup"><span data-stu-id="3d99d-211">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="3d99d-212">Пример 1: Администратор назначает пользователю роль</span><span class="sxs-lookup"><span data-stu-id="3d99d-212">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="3d99d-213">В этом примере администратор назначает пользователю nawu@fimdev.net роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="3d99d-213">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="3d99d-214">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="3d99d-214">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="3d99d-215">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d99d-215">Property</span></span>         | <span data-ttu-id="3d99d-216">Тип</span><span class="sxs-lookup"><span data-stu-id="3d99d-216">Type</span></span>                                                     | <span data-ttu-id="3d99d-217">Обязательное</span><span class="sxs-lookup"><span data-stu-id="3d99d-217">Required</span></span>                 | <span data-ttu-id="3d99d-218">Value</span><span class="sxs-lookup"><span data-stu-id="3d99d-218">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="3d99d-219">resourceId</span><span class="sxs-lookup"><span data-stu-id="3d99d-219">resourceId</span></span>       | <span data-ttu-id="3d99d-220">String</span><span class="sxs-lookup"><span data-stu-id="3d99d-220">String</span></span>                                                   | <span data-ttu-id="3d99d-221">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-221">Yes</span></span>                      | <span data-ttu-id="3d99d-222">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="3d99d-222">\<resourceId\></span></span> |
| <span data-ttu-id="3d99d-223">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="3d99d-223">roleDefinitionId</span></span> | <span data-ttu-id="3d99d-224">Строка</span><span class="sxs-lookup"><span data-stu-id="3d99d-224">String</span></span>                                                   | <span data-ttu-id="3d99d-225">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-225">Yes</span></span>                      | <span data-ttu-id="3d99d-226">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="3d99d-226">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="3d99d-227">субжектид</span><span class="sxs-lookup"><span data-stu-id="3d99d-227">subjectId</span></span>        | <span data-ttu-id="3d99d-228">Строка</span><span class="sxs-lookup"><span data-stu-id="3d99d-228">String</span></span>                                                   | <span data-ttu-id="3d99d-229">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-229">Yes</span></span>                      | <span data-ttu-id="3d99d-230">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="3d99d-230">\<subjectId\></span></span> |
| <span data-ttu-id="3d99d-231">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="3d99d-231">assignmentState</span></span>  | <span data-ttu-id="3d99d-232">Строка</span><span class="sxs-lookup"><span data-stu-id="3d99d-232">String</span></span>                                                   | <span data-ttu-id="3d99d-233">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-233">Yes</span></span>                      | <span data-ttu-id="3d99d-234">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="3d99d-234">Eligible / Active</span></span> |
| <span data-ttu-id="3d99d-235">type</span><span class="sxs-lookup"><span data-stu-id="3d99d-235">type</span></span>             | <span data-ttu-id="3d99d-236">Строка</span><span class="sxs-lookup"><span data-stu-id="3d99d-236">String</span></span>                                                   | <span data-ttu-id="3d99d-237">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-237">Yes</span></span>                      | <span data-ttu-id="3d99d-238">админадд</span><span class="sxs-lookup"><span data-stu-id="3d99d-238">AdminAdd</span></span> |
| <span data-ttu-id="3d99d-239">reason</span><span class="sxs-lookup"><span data-stu-id="3d99d-239">reason</span></span>           | <span data-ttu-id="3d99d-240">Строка</span><span class="sxs-lookup"><span data-stu-id="3d99d-240">String</span></span>                                                   | <span data-ttu-id="3d99d-241">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="3d99d-241">depends on role Settings</span></span> |   |
| <span data-ttu-id="3d99d-242">schedule</span><span class="sxs-lookup"><span data-stu-id="3d99d-242">schedule</span></span>         | [<span data-ttu-id="3d99d-243">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="3d99d-243">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="3d99d-244">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-244">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="3d99d-245">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d99d-245">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3d99d-246">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d99d-246">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3d99d-247">C#</span><span class="sxs-lookup"><span data-stu-id="3d99d-247">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3d99d-248">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d99d-248">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3d99d-249">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3d99d-249">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="3d99d-250">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d99d-250">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="3d99d-251">Пример 2: пользователь активирует подходящие роли</span><span class="sxs-lookup"><span data-stu-id="3d99d-251">Example 2: User activates eligible role</span></span>

<span data-ttu-id="3d99d-252">В этом примере пользователь nawu@fimdev.net активирует соответствующую роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="3d99d-252">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="3d99d-253">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d99d-253">Property</span></span>         | <span data-ttu-id="3d99d-254">Тип</span><span class="sxs-lookup"><span data-stu-id="3d99d-254">Type</span></span>                                                     | <span data-ttu-id="3d99d-255">Обязательное</span><span class="sxs-lookup"><span data-stu-id="3d99d-255">Required</span></span>                 | <span data-ttu-id="3d99d-256">Value</span><span class="sxs-lookup"><span data-stu-id="3d99d-256">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="3d99d-257">resourceId</span><span class="sxs-lookup"><span data-stu-id="3d99d-257">resourceId</span></span>       | <span data-ttu-id="3d99d-258">String</span><span class="sxs-lookup"><span data-stu-id="3d99d-258">String</span></span>                                                   | <span data-ttu-id="3d99d-259">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-259">Yes</span></span>                      | <span data-ttu-id="3d99d-260">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="3d99d-260">\<resourceId\></span></span> |
| <span data-ttu-id="3d99d-261">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="3d99d-261">roleDefinitionId</span></span> | <span data-ttu-id="3d99d-262">Строка</span><span class="sxs-lookup"><span data-stu-id="3d99d-262">String</span></span>                                                   | <span data-ttu-id="3d99d-263">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-263">Yes</span></span>                      | <span data-ttu-id="3d99d-264">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="3d99d-264">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="3d99d-265">субжектид</span><span class="sxs-lookup"><span data-stu-id="3d99d-265">subjectId</span></span>        | <span data-ttu-id="3d99d-266">Строка</span><span class="sxs-lookup"><span data-stu-id="3d99d-266">String</span></span>                                                   | <span data-ttu-id="3d99d-267">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-267">Yes</span></span>                      | <span data-ttu-id="3d99d-268">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="3d99d-268">\<subjectId\></span></span> |
| <span data-ttu-id="3d99d-269">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="3d99d-269">assignmentState</span></span>  | <span data-ttu-id="3d99d-270">Строка</span><span class="sxs-lookup"><span data-stu-id="3d99d-270">String</span></span>                                                   | <span data-ttu-id="3d99d-271">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-271">Yes</span></span>                      | <span data-ttu-id="3d99d-272">Активное</span><span class="sxs-lookup"><span data-stu-id="3d99d-272">Active</span></span> |
| <span data-ttu-id="3d99d-273">type</span><span class="sxs-lookup"><span data-stu-id="3d99d-273">type</span></span>             | <span data-ttu-id="3d99d-274">Строка</span><span class="sxs-lookup"><span data-stu-id="3d99d-274">String</span></span>                                                   | <span data-ttu-id="3d99d-275">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-275">Yes</span></span>                      | <span data-ttu-id="3d99d-276">усерадд</span><span class="sxs-lookup"><span data-stu-id="3d99d-276">UserAdd</span></span> |
| <span data-ttu-id="3d99d-277">reason</span><span class="sxs-lookup"><span data-stu-id="3d99d-277">reason</span></span>           | <span data-ttu-id="3d99d-278">Строка</span><span class="sxs-lookup"><span data-stu-id="3d99d-278">String</span></span>                                                   | <span data-ttu-id="3d99d-279">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="3d99d-279">depends on role Settings</span></span> |   |
| <span data-ttu-id="3d99d-280">schedule</span><span class="sxs-lookup"><span data-stu-id="3d99d-280">schedule</span></span>         | [<span data-ttu-id="3d99d-281">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="3d99d-281">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="3d99d-282">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-282">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="3d99d-283">Запросить</span><span class="sxs-lookup"><span data-stu-id="3d99d-283">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="3d99d-284">Ответ</span><span class="sxs-lookup"><span data-stu-id="3d99d-284">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="3d99d-285">Пример 3: пользователь отключает назначенную роль</span><span class="sxs-lookup"><span data-stu-id="3d99d-285">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="3d99d-286">В этом примере пользователь nawu@fimdev.net отключает активную роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="3d99d-286">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="3d99d-287">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d99d-287">Property</span></span>         | <span data-ttu-id="3d99d-288">Тип</span><span class="sxs-lookup"><span data-stu-id="3d99d-288">Type</span></span>                                                     | <span data-ttu-id="3d99d-289">Обязательное</span><span class="sxs-lookup"><span data-stu-id="3d99d-289">Required</span></span> | <span data-ttu-id="3d99d-290">Value</span><span class="sxs-lookup"><span data-stu-id="3d99d-290">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="3d99d-291">resourceId</span><span class="sxs-lookup"><span data-stu-id="3d99d-291">resourceId</span></span>       | <span data-ttu-id="3d99d-292">String</span><span class="sxs-lookup"><span data-stu-id="3d99d-292">String</span></span>                                                   | <span data-ttu-id="3d99d-293">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-293">Yes</span></span>      | <span data-ttu-id="3d99d-294">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="3d99d-294">\<resourceId\></span></span> |
| <span data-ttu-id="3d99d-295">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="3d99d-295">roleDefinitionId</span></span> | <span data-ttu-id="3d99d-296">Строка</span><span class="sxs-lookup"><span data-stu-id="3d99d-296">String</span></span>                                                   | <span data-ttu-id="3d99d-297">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-297">Yes</span></span>      | <span data-ttu-id="3d99d-298">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="3d99d-298">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="3d99d-299">субжектид</span><span class="sxs-lookup"><span data-stu-id="3d99d-299">subjectId</span></span>        | <span data-ttu-id="3d99d-300">Строка</span><span class="sxs-lookup"><span data-stu-id="3d99d-300">String</span></span>                                                   | <span data-ttu-id="3d99d-301">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-301">Yes</span></span>      | <span data-ttu-id="3d99d-302">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="3d99d-302">\<subjectId\></span></span> |
| <span data-ttu-id="3d99d-303">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="3d99d-303">assignmentState</span></span>  | <span data-ttu-id="3d99d-304">String</span><span class="sxs-lookup"><span data-stu-id="3d99d-304">String</span></span>                                                   | <span data-ttu-id="3d99d-305">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-305">Yes</span></span>      | <span data-ttu-id="3d99d-306">Активное</span><span class="sxs-lookup"><span data-stu-id="3d99d-306">Active</span></span> |
| <span data-ttu-id="3d99d-307">type</span><span class="sxs-lookup"><span data-stu-id="3d99d-307">type</span></span>             | <span data-ttu-id="3d99d-308">String</span><span class="sxs-lookup"><span data-stu-id="3d99d-308">String</span></span>                                                   | <span data-ttu-id="3d99d-309">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-309">Yes</span></span>      | <span data-ttu-id="3d99d-310">усерремове</span><span class="sxs-lookup"><span data-stu-id="3d99d-310">UserRemove</span></span> |
| <span data-ttu-id="3d99d-311">reason</span><span class="sxs-lookup"><span data-stu-id="3d99d-311">reason</span></span>           | <span data-ttu-id="3d99d-312">Строка</span><span class="sxs-lookup"><span data-stu-id="3d99d-312">String</span></span>                                                   | <span data-ttu-id="3d99d-313">Нет</span><span class="sxs-lookup"><span data-stu-id="3d99d-313">No</span></span>       |   |
| <span data-ttu-id="3d99d-314">schedule</span><span class="sxs-lookup"><span data-stu-id="3d99d-314">schedule</span></span>         | [<span data-ttu-id="3d99d-315">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="3d99d-315">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="3d99d-316">Нет</span><span class="sxs-lookup"><span data-stu-id="3d99d-316">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="3d99d-317">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d99d-317">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="3d99d-318">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d99d-318">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="3d99d-319">Пример 4: Администратор удаляет пользователя из роли</span><span class="sxs-lookup"><span data-stu-id="3d99d-319">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="3d99d-320">В этом примере администратор удаляет пользователя nawu@fimdev.net из роли читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="3d99d-320">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="3d99d-321">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="3d99d-321">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="3d99d-322">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d99d-322">Property</span></span>         | <span data-ttu-id="3d99d-323">Тип</span><span class="sxs-lookup"><span data-stu-id="3d99d-323">Type</span></span>                                                     | <span data-ttu-id="3d99d-324">Обязательное</span><span class="sxs-lookup"><span data-stu-id="3d99d-324">Required</span></span> | <span data-ttu-id="3d99d-325">Value</span><span class="sxs-lookup"><span data-stu-id="3d99d-325">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="3d99d-326">resourceId</span><span class="sxs-lookup"><span data-stu-id="3d99d-326">resourceId</span></span>       | <span data-ttu-id="3d99d-327">String</span><span class="sxs-lookup"><span data-stu-id="3d99d-327">String</span></span>                                                   | <span data-ttu-id="3d99d-328">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-328">Yes</span></span>      | <span data-ttu-id="3d99d-329">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="3d99d-329">\<resourceId\></span></span> |
| <span data-ttu-id="3d99d-330">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="3d99d-330">roleDefinitionId</span></span> | <span data-ttu-id="3d99d-331">String</span><span class="sxs-lookup"><span data-stu-id="3d99d-331">String</span></span>                                                   | <span data-ttu-id="3d99d-332">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-332">Yes</span></span>      | <span data-ttu-id="3d99d-333">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="3d99d-333">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="3d99d-334">субжектид</span><span class="sxs-lookup"><span data-stu-id="3d99d-334">subjectId</span></span>        | <span data-ttu-id="3d99d-335">String</span><span class="sxs-lookup"><span data-stu-id="3d99d-335">String</span></span>                                                   | <span data-ttu-id="3d99d-336">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-336">Yes</span></span>      | <span data-ttu-id="3d99d-337">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="3d99d-337">\<subjectId\></span></span> |
| <span data-ttu-id="3d99d-338">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="3d99d-338">assignmentState</span></span>  | <span data-ttu-id="3d99d-339">String</span><span class="sxs-lookup"><span data-stu-id="3d99d-339">String</span></span>                                                   | <span data-ttu-id="3d99d-340">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-340">Yes</span></span>      | <span data-ttu-id="3d99d-341">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="3d99d-341">Eligible / Active</span></span> |
| <span data-ttu-id="3d99d-342">type</span><span class="sxs-lookup"><span data-stu-id="3d99d-342">type</span></span>             | <span data-ttu-id="3d99d-343">String</span><span class="sxs-lookup"><span data-stu-id="3d99d-343">String</span></span>                                                   | <span data-ttu-id="3d99d-344">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-344">Yes</span></span>      | <span data-ttu-id="3d99d-345">админремове</span><span class="sxs-lookup"><span data-stu-id="3d99d-345">AdminRemove</span></span> |
| <span data-ttu-id="3d99d-346">reason</span><span class="sxs-lookup"><span data-stu-id="3d99d-346">reason</span></span>           | <span data-ttu-id="3d99d-347">Строка</span><span class="sxs-lookup"><span data-stu-id="3d99d-347">String</span></span>                                                   | <span data-ttu-id="3d99d-348">Нет</span><span class="sxs-lookup"><span data-stu-id="3d99d-348">No</span></span>       |   |
| <span data-ttu-id="3d99d-349">schedule</span><span class="sxs-lookup"><span data-stu-id="3d99d-349">schedule</span></span>         | [<span data-ttu-id="3d99d-350">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="3d99d-350">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="3d99d-351">Нет</span><span class="sxs-lookup"><span data-stu-id="3d99d-351">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="3d99d-352">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d99d-352">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="3d99d-353">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d99d-353">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="3d99d-354">Пример 5: "Администратор обновляет назначение ролей"</span><span class="sxs-lookup"><span data-stu-id="3d99d-354">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="3d99d-355">В этом примере администраторы обновляют назначение роли пользователя nawu@fimdev.net владельцу.</span><span class="sxs-lookup"><span data-stu-id="3d99d-355">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="3d99d-356">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="3d99d-356">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="3d99d-357">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d99d-357">Property</span></span>         | <span data-ttu-id="3d99d-358">Тип</span><span class="sxs-lookup"><span data-stu-id="3d99d-358">Type</span></span>                                                     | <span data-ttu-id="3d99d-359">Обязательное</span><span class="sxs-lookup"><span data-stu-id="3d99d-359">Required</span></span>                | <span data-ttu-id="3d99d-360">Value</span><span class="sxs-lookup"><span data-stu-id="3d99d-360">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="3d99d-361">resourceId</span><span class="sxs-lookup"><span data-stu-id="3d99d-361">resourceId</span></span>       | <span data-ttu-id="3d99d-362">String</span><span class="sxs-lookup"><span data-stu-id="3d99d-362">String</span></span>                                                   | <span data-ttu-id="3d99d-363">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-363">Yes</span></span>                     | <span data-ttu-id="3d99d-364">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="3d99d-364">\<resourceId\></span></span> |
| <span data-ttu-id="3d99d-365">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="3d99d-365">roleDefinitionId</span></span> | <span data-ttu-id="3d99d-366">String</span><span class="sxs-lookup"><span data-stu-id="3d99d-366">String</span></span>                                                   | <span data-ttu-id="3d99d-367">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-367">Yes</span></span>                     | <span data-ttu-id="3d99d-368">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="3d99d-368">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="3d99d-369">субжектид</span><span class="sxs-lookup"><span data-stu-id="3d99d-369">subjectId</span></span>        | <span data-ttu-id="3d99d-370">String</span><span class="sxs-lookup"><span data-stu-id="3d99d-370">String</span></span>                                                   | <span data-ttu-id="3d99d-371">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-371">Yes</span></span>                     | <span data-ttu-id="3d99d-372">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="3d99d-372">\<subjectId\></span></span> |
| <span data-ttu-id="3d99d-373">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="3d99d-373">assignmentState</span></span>  | <span data-ttu-id="3d99d-374">String</span><span class="sxs-lookup"><span data-stu-id="3d99d-374">String</span></span>                                                   | <span data-ttu-id="3d99d-375">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-375">Yes</span></span>                     | <span data-ttu-id="3d99d-376">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="3d99d-376">Eligible / Active</span></span> |
| <span data-ttu-id="3d99d-377">type</span><span class="sxs-lookup"><span data-stu-id="3d99d-377">type</span></span>             | <span data-ttu-id="3d99d-378">String</span><span class="sxs-lookup"><span data-stu-id="3d99d-378">String</span></span>                                                   | <span data-ttu-id="3d99d-379">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-379">Yes</span></span>                     | <span data-ttu-id="3d99d-380">админупдате</span><span class="sxs-lookup"><span data-stu-id="3d99d-380">AdminUpdate</span></span> |
| <span data-ttu-id="3d99d-381">reason</span><span class="sxs-lookup"><span data-stu-id="3d99d-381">reason</span></span>           | <span data-ttu-id="3d99d-382">Строка</span><span class="sxs-lookup"><span data-stu-id="3d99d-382">String</span></span>                                                   | <span data-ttu-id="3d99d-383">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="3d99d-383">depends on roleSettings</span></span> |   |
| <span data-ttu-id="3d99d-384">schedule</span><span class="sxs-lookup"><span data-stu-id="3d99d-384">schedule</span></span>         | [<span data-ttu-id="3d99d-385">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="3d99d-385">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="3d99d-386">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-386">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="3d99d-387">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d99d-387">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="3d99d-388">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d99d-388">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="3d99d-389">Пример 6: администратор расширяет назначение ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="3d99d-389">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="3d99d-390">В этом примере показано, как расширить назначение роли истечения срока действия для пользователя АНУЖКУСЕР участнику службы управления API.</span><span class="sxs-lookup"><span data-stu-id="3d99d-390">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="3d99d-391">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="3d99d-391">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="3d99d-392">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d99d-392">Property</span></span>         | <span data-ttu-id="3d99d-393">Тип</span><span class="sxs-lookup"><span data-stu-id="3d99d-393">Type</span></span>                                                     | <span data-ttu-id="3d99d-394">Обязательное</span><span class="sxs-lookup"><span data-stu-id="3d99d-394">Required</span></span>                | <span data-ttu-id="3d99d-395">Value</span><span class="sxs-lookup"><span data-stu-id="3d99d-395">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="3d99d-396">resourceId</span><span class="sxs-lookup"><span data-stu-id="3d99d-396">resourceId</span></span>       | <span data-ttu-id="3d99d-397">String</span><span class="sxs-lookup"><span data-stu-id="3d99d-397">String</span></span>                                                   | <span data-ttu-id="3d99d-398">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-398">Yes</span></span>                     | <span data-ttu-id="3d99d-399">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="3d99d-399">\<resourceId\></span></span> |
| <span data-ttu-id="3d99d-400">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="3d99d-400">roleDefinitionId</span></span> | <span data-ttu-id="3d99d-401">String</span><span class="sxs-lookup"><span data-stu-id="3d99d-401">String</span></span>                                                   | <span data-ttu-id="3d99d-402">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-402">Yes</span></span>                     | <span data-ttu-id="3d99d-403">\<роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="3d99d-403">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="3d99d-404">субжектид</span><span class="sxs-lookup"><span data-stu-id="3d99d-404">subjectId</span></span>        | <span data-ttu-id="3d99d-405">Строка</span><span class="sxs-lookup"><span data-stu-id="3d99d-405">String</span></span>                                                   | <span data-ttu-id="3d99d-406">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-406">Yes</span></span>                     | <span data-ttu-id="3d99d-407">\<субжектид\></span><span class="sxs-lookup"><span data-stu-id="3d99d-407">\<subjectId\></span></span> |
| <span data-ttu-id="3d99d-408">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="3d99d-408">assignmentState</span></span>  | <span data-ttu-id="3d99d-409">Строка</span><span class="sxs-lookup"><span data-stu-id="3d99d-409">String</span></span>                                                   | <span data-ttu-id="3d99d-410">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-410">Yes</span></span>                     | <span data-ttu-id="3d99d-411">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="3d99d-411">Eligible / Active</span></span> |
| <span data-ttu-id="3d99d-412">type</span><span class="sxs-lookup"><span data-stu-id="3d99d-412">type</span></span>             | <span data-ttu-id="3d99d-413">String</span><span class="sxs-lookup"><span data-stu-id="3d99d-413">String</span></span>                                                   | <span data-ttu-id="3d99d-414">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-414">Yes</span></span>                     | <span data-ttu-id="3d99d-415">админекстенд</span><span class="sxs-lookup"><span data-stu-id="3d99d-415">AdminExtend</span></span> |
| <span data-ttu-id="3d99d-416">reason</span><span class="sxs-lookup"><span data-stu-id="3d99d-416">reason</span></span>           | <span data-ttu-id="3d99d-417">Строка</span><span class="sxs-lookup"><span data-stu-id="3d99d-417">String</span></span>                                                   | <span data-ttu-id="3d99d-418">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="3d99d-418">depends on roleSettings</span></span> |   |
| <span data-ttu-id="3d99d-419">schedule</span><span class="sxs-lookup"><span data-stu-id="3d99d-419">schedule</span></span>         | [<span data-ttu-id="3d99d-420">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="3d99d-420">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="3d99d-421">Да</span><span class="sxs-lookup"><span data-stu-id="3d99d-421">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="3d99d-422">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d99d-422">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="3d99d-423">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d99d-423">Response</span></span>

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
