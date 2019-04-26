---
title: Создание governanceRoleAssignmentRequest
description: Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли. В приведенной ниже таблице перечислены операции.
localization_priority: Normal
ms.openlocfilehash: b9b5f701f3f8ad283f589d07b250ce8ea63aa479
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329643"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="c8c6e-104">Создание governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="c8c6e-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8c6e-105">Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="c8c6e-106">В приведенной ниже таблице перечислены операции.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-106">The following table lists the operations.</span></span>

| <span data-ttu-id="c8c6e-107">Операция</span><span class="sxs-lookup"><span data-stu-id="c8c6e-107">Operation</span></span>                                   | <span data-ttu-id="c8c6e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c8c6e-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="c8c6e-109">Назначение роли</span><span class="sxs-lookup"><span data-stu-id="c8c6e-109">Assign a role assignment</span></span>                    | <span data-ttu-id="c8c6e-110">Админадд</span><span class="sxs-lookup"><span data-stu-id="c8c6e-110">AdminAdd</span></span>    |
| <span data-ttu-id="c8c6e-111">Активация подходящего назначения роли</span><span class="sxs-lookup"><span data-stu-id="c8c6e-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="c8c6e-112">Усерадд</span><span class="sxs-lookup"><span data-stu-id="c8c6e-112">UserAdd</span></span>     |
| <span data-ttu-id="c8c6e-113">ДеАктивация активированного назначения роли</span><span class="sxs-lookup"><span data-stu-id="c8c6e-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="c8c6e-114">Усерремове</span><span class="sxs-lookup"><span data-stu-id="c8c6e-114">UserRemove</span></span>  |
| <span data-ttu-id="c8c6e-115">Удаление назначения роли</span><span class="sxs-lookup"><span data-stu-id="c8c6e-115">Remove a role assignment</span></span>                    | <span data-ttu-id="c8c6e-116">Админремове</span><span class="sxs-lookup"><span data-stu-id="c8c6e-116">AdminRemove</span></span> |
| <span data-ttu-id="c8c6e-117">Обновление назначения роли</span><span class="sxs-lookup"><span data-stu-id="c8c6e-117">Update a role assignment</span></span>                    | <span data-ttu-id="c8c6e-118">Админупдате</span><span class="sxs-lookup"><span data-stu-id="c8c6e-118">AdminUpdate</span></span> |
| <span data-ttu-id="c8c6e-119">Запрос на расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="c8c6e-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="c8c6e-120">Усерекстенд</span><span class="sxs-lookup"><span data-stu-id="c8c6e-120">UserExtend</span></span>  |
| <span data-ttu-id="c8c6e-121">Расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="c8c6e-121">Extend a role assignment</span></span>                    | <span data-ttu-id="c8c6e-122">Админекстенд</span><span class="sxs-lookup"><span data-stu-id="c8c6e-122">AdminExtend</span></span> |
| <span data-ttu-id="c8c6e-123">Запрос на продление назначения роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="c8c6e-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="c8c6e-124">Усерренев</span><span class="sxs-lookup"><span data-stu-id="c8c6e-124">UserRenew</span></span>   |
| <span data-ttu-id="c8c6e-125">Продление назначенной роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="c8c6e-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="c8c6e-126">Админренев</span><span class="sxs-lookup"><span data-stu-id="c8c6e-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="c8c6e-127">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8c6e-127">Permissions</span></span>

<span data-ttu-id="c8c6e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8c6e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c8c6e-130">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8c6e-130">Permission type</span></span>                        | <span data-ttu-id="c8c6e-131">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8c6e-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="c8c6e-132">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8c6e-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="c8c6e-133">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="c8c6e-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="c8c6e-134">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8c6e-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8c6e-135">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-135">Not supported.</span></span>                            |
| <span data-ttu-id="c8c6e-136">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8c6e-136">Application</span></span>                            | <span data-ttu-id="c8c6e-137">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="c8c6e-137">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8c6e-138">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8c6e-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="c8c6e-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8c6e-139">Request headers</span></span>

| <span data-ttu-id="c8c6e-140">Имя</span><span class="sxs-lookup"><span data-stu-id="c8c6e-140">Name</span></span>          | <span data-ttu-id="c8c6e-141">Описание</span><span class="sxs-lookup"><span data-stu-id="c8c6e-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="c8c6e-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8c6e-142">Authorization</span></span> | <span data-ttu-id="c8c6e-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c8c6e-143">Bearer {code}</span></span>    |
| <span data-ttu-id="c8c6e-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c8c6e-144">Content-type</span></span>  | <span data-ttu-id="c8c6e-145">application/json</span><span class="sxs-lookup"><span data-stu-id="c8c6e-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8c6e-146">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8c6e-146">Request body</span></span>

<span data-ttu-id="c8c6e-147">В тексте запроса добавьте представление объекта [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="c8c6e-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8c6e-148">Property</span></span>         | <span data-ttu-id="c8c6e-149">Тип</span><span class="sxs-lookup"><span data-stu-id="c8c6e-149">Type</span></span>                                                     | <span data-ttu-id="c8c6e-150">Описание</span><span class="sxs-lookup"><span data-stu-id="c8c6e-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="c8c6e-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="c8c6e-151">resourceId</span></span>       | <span data-ttu-id="c8c6e-152">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-152">String</span></span>                                                   | <span data-ttu-id="c8c6e-153">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-153">The ID of the resource.</span></span> <span data-ttu-id="c8c6e-154">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-154">Required.</span></span> |
| <span data-ttu-id="c8c6e-155">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="c8c6e-155">roleDefinitionId</span></span> | <span data-ttu-id="c8c6e-156">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-156">String</span></span>                                                   | <span data-ttu-id="c8c6e-157">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-157">The ID of the role definition.</span></span> <span data-ttu-id="c8c6e-158">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-158">Required.</span></span> |
| <span data-ttu-id="c8c6e-159">Субжектид</span><span class="sxs-lookup"><span data-stu-id="c8c6e-159">subjectId</span></span>        | <span data-ttu-id="c8c6e-160">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-160">String</span></span>                                                   | <span data-ttu-id="c8c6e-161">ИДЕНТИФИКАТОР субъекта.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-161">The ID of the subject.</span></span> <span data-ttu-id="c8c6e-162">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-162">Required.</span></span> |
| <span data-ttu-id="c8c6e-163">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="c8c6e-163">assignmentState</span></span>  | <span data-ttu-id="c8c6e-164">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-164">String</span></span>                                                   | <span data-ttu-id="c8c6e-165">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-165">The state of assignment.</span></span> <span data-ttu-id="c8c6e-166">Значение может быть `Eligible` и `Active`.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="c8c6e-167">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-167">Required.</span></span> |
| <span data-ttu-id="c8c6e-168">type</span><span class="sxs-lookup"><span data-stu-id="c8c6e-168">type</span></span>             | <span data-ttu-id="c8c6e-169">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-169">String</span></span>                                                   | <span data-ttu-id="c8c6e-170">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-170">The request type.</span></span> <span data-ttu-id="c8c6e-171">Возможные значения: `AdminAdd`, `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `AdminRenew` `AdminExtend`,,,,, и. `UserExtend` `UserRenew`</span><span class="sxs-lookup"><span data-stu-id="c8c6e-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="c8c6e-172">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-172">Required.</span></span> |
| <span data-ttu-id="c8c6e-173">причиной</span><span class="sxs-lookup"><span data-stu-id="c8c6e-173">reason</span></span>           | <span data-ttu-id="c8c6e-174">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-174">String</span></span>                                                   | <span data-ttu-id="c8c6e-175">Необходимо указать причину для запроса на назначение роли для аудита и проверки.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="c8c6e-176">Диспетчер</span><span class="sxs-lookup"><span data-stu-id="c8c6e-176">schedule</span></span>         | [<span data-ttu-id="c8c6e-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c8c6e-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c8c6e-178">Расписание запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="c8c6e-179">`UserAdd`Для типа запроса `AdminAdd`,, `AdminUpdate`, и `AdminExtend`, он необходим.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="c8c6e-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8c6e-180">Response</span></span>

<span data-ttu-id="c8c6e-181">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="c8c6e-182">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="c8c6e-182">Error codes</span></span>

<span data-ttu-id="c8c6e-183">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="c8c6e-184">Кроме того, он возвращает коды ошибок, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="c8c6e-185">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="c8c6e-185">Error code</span></span>     | <span data-ttu-id="c8c6e-186">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="c8c6e-186">Error message</span></span>                               | <span data-ttu-id="c8c6e-187">Сведения</span><span class="sxs-lookup"><span data-stu-id="c8c6e-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="c8c6e-188">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="c8c6e-188">400 BadRequest</span></span> | <span data-ttu-id="c8c6e-189">Роленотфаунд</span><span class="sxs-lookup"><span data-stu-id="c8c6e-189">RoleNotFound</span></span>                                | <span data-ttu-id="c8c6e-190">Не `roleDefinitionId` удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="c8c6e-191">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="c8c6e-191">400 BadRequest</span></span> | <span data-ttu-id="c8c6e-192">Ресаурцеислоккед</span><span class="sxs-lookup"><span data-stu-id="c8c6e-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="c8c6e-193">Ресурс, указанный в теле запроса, находится в состоянии `Locked` и не может создавать запросы на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="c8c6e-194">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="c8c6e-194">400 BadRequest</span></span> | <span data-ttu-id="c8c6e-195">Субжектнотфаунд</span><span class="sxs-lookup"><span data-stu-id="c8c6e-195">SubjectNotFound</span></span>                             | <span data-ttu-id="c8c6e-196">Не `subjectId` удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="c8c6e-197">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="c8c6e-197">400 BadRequest</span></span> | <span data-ttu-id="c8c6e-198">Пендингролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="c8c6e-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="c8c6e-199">В системе уже существует ожидающий [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="c8c6e-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="c8c6e-200">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="c8c6e-200">400 BadRequest</span></span> | <span data-ttu-id="c8c6e-201">Ролеассигнментексистс</span><span class="sxs-lookup"><span data-stu-id="c8c6e-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="c8c6e-202">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , который требуется создать, уже существует в системе.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="c8c6e-203">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="c8c6e-203">400 BadRequest</span></span> | <span data-ttu-id="c8c6e-204">Ролеассигнментдоеснотексист</span><span class="sxs-lookup"><span data-stu-id="c8c6e-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="c8c6e-205">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , запрошенный для обновления или расширения, не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="c8c6e-206">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="c8c6e-206">400 BadRequest</span></span> | <span data-ttu-id="c8c6e-207">Ролеассигнментрекуестполицивалидатионфаилед</span><span class="sxs-lookup"><span data-stu-id="c8c6e-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="c8c6e-208">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) не отвечает внутренним политикам и не может быть создан.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="c8c6e-209">Примеры</span><span class="sxs-lookup"><span data-stu-id="c8c6e-209">Examples</span></span>

<span data-ttu-id="c8c6e-210">В следующих примерах показано, как использовать этот API.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="c8c6e-211">Пример 1: Администратор назначает пользователю роль</span><span class="sxs-lookup"><span data-stu-id="c8c6e-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="c8c6e-212">В этом примере администратор назначает пользователю nawu@fimdev.net роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="c8c6e-213">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="c8c6e-214">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8c6e-214">Property</span></span>         | <span data-ttu-id="c8c6e-215">Тип</span><span class="sxs-lookup"><span data-stu-id="c8c6e-215">Type</span></span>                                                     | <span data-ttu-id="c8c6e-216">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c8c6e-216">Required</span></span>                 | <span data-ttu-id="c8c6e-217">Значение</span><span class="sxs-lookup"><span data-stu-id="c8c6e-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="c8c6e-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="c8c6e-218">resourceId</span></span>       | <span data-ttu-id="c8c6e-219">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-219">String</span></span>                                                   | <span data-ttu-id="c8c6e-220">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-220">Yes</span></span>                      | <span data-ttu-id="c8c6e-221">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="c8c6e-221">\<resourceId\></span></span> |
| <span data-ttu-id="c8c6e-222">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="c8c6e-222">roleDefinitionId</span></span> | <span data-ttu-id="c8c6e-223">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-223">String</span></span>                                                   | <span data-ttu-id="c8c6e-224">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-224">Yes</span></span>                      | <span data-ttu-id="c8c6e-225">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="c8c6e-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="c8c6e-226">Субжектид</span><span class="sxs-lookup"><span data-stu-id="c8c6e-226">subjectId</span></span>        | <span data-ttu-id="c8c6e-227">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-227">String</span></span>                                                   | <span data-ttu-id="c8c6e-228">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-228">Yes</span></span>                      | <span data-ttu-id="c8c6e-229">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="c8c6e-229">\<subjectId\></span></span> |
| <span data-ttu-id="c8c6e-230">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="c8c6e-230">assignmentState</span></span>  | <span data-ttu-id="c8c6e-231">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-231">String</span></span>                                                   | <span data-ttu-id="c8c6e-232">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-232">Yes</span></span>                      | <span data-ttu-id="c8c6e-233">ПодХодящие/активные</span><span class="sxs-lookup"><span data-stu-id="c8c6e-233">Eligible / Active</span></span> |
| <span data-ttu-id="c8c6e-234">type</span><span class="sxs-lookup"><span data-stu-id="c8c6e-234">type</span></span>             | <span data-ttu-id="c8c6e-235">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-235">String</span></span>                                                   | <span data-ttu-id="c8c6e-236">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-236">Yes</span></span>                      | <span data-ttu-id="c8c6e-237">Админадд</span><span class="sxs-lookup"><span data-stu-id="c8c6e-237">AdminAdd</span></span> |
| <span data-ttu-id="c8c6e-238">причиной</span><span class="sxs-lookup"><span data-stu-id="c8c6e-238">reason</span></span>           | <span data-ttu-id="c8c6e-239">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-239">String</span></span>                                                   | <span data-ttu-id="c8c6e-240">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="c8c6e-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="c8c6e-241">Диспетчер</span><span class="sxs-lookup"><span data-stu-id="c8c6e-241">schedule</span></span>         | [<span data-ttu-id="c8c6e-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c8c6e-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c8c6e-243">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="c8c6e-244">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8c6e-244">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="c8c6e-245">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8c6e-245">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="c8c6e-246">Пример 2: пользователь активирует подходящие роли</span><span class="sxs-lookup"><span data-stu-id="c8c6e-246">Example 2: User activates eligible role</span></span>

<span data-ttu-id="c8c6e-247">В этом примере пользователь nawu@fimdev.net активирует соответствующую роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-247">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="c8c6e-248">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8c6e-248">Property</span></span>         | <span data-ttu-id="c8c6e-249">Тип</span><span class="sxs-lookup"><span data-stu-id="c8c6e-249">Type</span></span>                                                     | <span data-ttu-id="c8c6e-250">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c8c6e-250">Required</span></span>                 | <span data-ttu-id="c8c6e-251">Значение</span><span class="sxs-lookup"><span data-stu-id="c8c6e-251">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="c8c6e-252">resourceId</span><span class="sxs-lookup"><span data-stu-id="c8c6e-252">resourceId</span></span>       | <span data-ttu-id="c8c6e-253">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-253">String</span></span>                                                   | <span data-ttu-id="c8c6e-254">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-254">Yes</span></span>                      | <span data-ttu-id="c8c6e-255">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="c8c6e-255">\<resourceId\></span></span> |
| <span data-ttu-id="c8c6e-256">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="c8c6e-256">roleDefinitionId</span></span> | <span data-ttu-id="c8c6e-257">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-257">String</span></span>                                                   | <span data-ttu-id="c8c6e-258">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-258">Yes</span></span>                      | <span data-ttu-id="c8c6e-259">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="c8c6e-259">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="c8c6e-260">Субжектид</span><span class="sxs-lookup"><span data-stu-id="c8c6e-260">subjectId</span></span>        | <span data-ttu-id="c8c6e-261">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-261">String</span></span>                                                   | <span data-ttu-id="c8c6e-262">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-262">Yes</span></span>                      | <span data-ttu-id="c8c6e-263">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="c8c6e-263">\<subjectId\></span></span> |
| <span data-ttu-id="c8c6e-264">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="c8c6e-264">assignmentState</span></span>  | <span data-ttu-id="c8c6e-265">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-265">String</span></span>                                                   | <span data-ttu-id="c8c6e-266">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-266">Yes</span></span>                      | <span data-ttu-id="c8c6e-267">Активные</span><span class="sxs-lookup"><span data-stu-id="c8c6e-267">Active</span></span> |
| <span data-ttu-id="c8c6e-268">type</span><span class="sxs-lookup"><span data-stu-id="c8c6e-268">type</span></span>             | <span data-ttu-id="c8c6e-269">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-269">String</span></span>                                                   | <span data-ttu-id="c8c6e-270">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-270">Yes</span></span>                      | <span data-ttu-id="c8c6e-271">Усерадд</span><span class="sxs-lookup"><span data-stu-id="c8c6e-271">UserAdd</span></span> |
| <span data-ttu-id="c8c6e-272">причиной</span><span class="sxs-lookup"><span data-stu-id="c8c6e-272">reason</span></span>           | <span data-ttu-id="c8c6e-273">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-273">String</span></span>                                                   | <span data-ttu-id="c8c6e-274">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="c8c6e-274">depends on role Settings</span></span> |   |
| <span data-ttu-id="c8c6e-275">Диспетчер</span><span class="sxs-lookup"><span data-stu-id="c8c6e-275">schedule</span></span>         | [<span data-ttu-id="c8c6e-276">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c8c6e-276">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c8c6e-277">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-277">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="c8c6e-278">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8c6e-278">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="c8c6e-279">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8c6e-279">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="c8c6e-280">Пример 3: пользователь отключает назначенную роль</span><span class="sxs-lookup"><span data-stu-id="c8c6e-280">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="c8c6e-281">В этом примере пользователь nawu@fimdev.net отключает активную роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-281">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="c8c6e-282">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8c6e-282">Property</span></span>         | <span data-ttu-id="c8c6e-283">Тип</span><span class="sxs-lookup"><span data-stu-id="c8c6e-283">Type</span></span>                                                     | <span data-ttu-id="c8c6e-284">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c8c6e-284">Required</span></span> | <span data-ttu-id="c8c6e-285">Значение</span><span class="sxs-lookup"><span data-stu-id="c8c6e-285">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="c8c6e-286">resourceId</span><span class="sxs-lookup"><span data-stu-id="c8c6e-286">resourceId</span></span>       | <span data-ttu-id="c8c6e-287">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-287">String</span></span>                                                   | <span data-ttu-id="c8c6e-288">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-288">Yes</span></span>      | <span data-ttu-id="c8c6e-289">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="c8c6e-289">\<resourceId\></span></span> |
| <span data-ttu-id="c8c6e-290">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="c8c6e-290">roleDefinitionId</span></span> | <span data-ttu-id="c8c6e-291">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-291">String</span></span>                                                   | <span data-ttu-id="c8c6e-292">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-292">Yes</span></span>      | <span data-ttu-id="c8c6e-293">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="c8c6e-293">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="c8c6e-294">Субжектид</span><span class="sxs-lookup"><span data-stu-id="c8c6e-294">subjectId</span></span>        | <span data-ttu-id="c8c6e-295">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-295">String</span></span>                                                   | <span data-ttu-id="c8c6e-296">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-296">Yes</span></span>      | <span data-ttu-id="c8c6e-297">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="c8c6e-297">\<subjectId\></span></span> |
| <span data-ttu-id="c8c6e-298">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="c8c6e-298">assignmentState</span></span>  | <span data-ttu-id="c8c6e-299">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-299">String</span></span>                                                   | <span data-ttu-id="c8c6e-300">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-300">Yes</span></span>      | <span data-ttu-id="c8c6e-301">Активные</span><span class="sxs-lookup"><span data-stu-id="c8c6e-301">Active</span></span> |
| <span data-ttu-id="c8c6e-302">type</span><span class="sxs-lookup"><span data-stu-id="c8c6e-302">type</span></span>             | <span data-ttu-id="c8c6e-303">Строка</span><span class="sxs-lookup"><span data-stu-id="c8c6e-303">String</span></span>                                                   | <span data-ttu-id="c8c6e-304">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-304">Yes</span></span>      | <span data-ttu-id="c8c6e-305">Усерремове</span><span class="sxs-lookup"><span data-stu-id="c8c6e-305">UserRemove</span></span> |
| <span data-ttu-id="c8c6e-306">причиной</span><span class="sxs-lookup"><span data-stu-id="c8c6e-306">reason</span></span>           | <span data-ttu-id="c8c6e-307">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-307">String</span></span>                                                   | <span data-ttu-id="c8c6e-308">Нет</span><span class="sxs-lookup"><span data-stu-id="c8c6e-308">No</span></span>       |   |
| <span data-ttu-id="c8c6e-309">Диспетчер</span><span class="sxs-lookup"><span data-stu-id="c8c6e-309">schedule</span></span>         | [<span data-ttu-id="c8c6e-310">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c8c6e-310">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c8c6e-311">Нет</span><span class="sxs-lookup"><span data-stu-id="c8c6e-311">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="c8c6e-312">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8c6e-312">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="c8c6e-313">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8c6e-313">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="c8c6e-314">Пример 4: Администратор удаляет пользователя из роли</span><span class="sxs-lookup"><span data-stu-id="c8c6e-314">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="c8c6e-315">В этом примере администратор удаляет пользователя nawu@fimdev.net из роли читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-315">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="c8c6e-316">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-316">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="c8c6e-317">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8c6e-317">Property</span></span>         | <span data-ttu-id="c8c6e-318">Тип</span><span class="sxs-lookup"><span data-stu-id="c8c6e-318">Type</span></span>                                                     | <span data-ttu-id="c8c6e-319">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c8c6e-319">Required</span></span> | <span data-ttu-id="c8c6e-320">Значение</span><span class="sxs-lookup"><span data-stu-id="c8c6e-320">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="c8c6e-321">resourceId</span><span class="sxs-lookup"><span data-stu-id="c8c6e-321">resourceId</span></span>       | <span data-ttu-id="c8c6e-322">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-322">String</span></span>                                                   | <span data-ttu-id="c8c6e-323">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-323">Yes</span></span>      | <span data-ttu-id="c8c6e-324">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="c8c6e-324">\<resourceId\></span></span> |
| <span data-ttu-id="c8c6e-325">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="c8c6e-325">roleDefinitionId</span></span> | <span data-ttu-id="c8c6e-326">Строка</span><span class="sxs-lookup"><span data-stu-id="c8c6e-326">String</span></span>                                                   | <span data-ttu-id="c8c6e-327">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-327">Yes</span></span>      | <span data-ttu-id="c8c6e-328">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="c8c6e-328">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="c8c6e-329">Субжектид</span><span class="sxs-lookup"><span data-stu-id="c8c6e-329">subjectId</span></span>        | <span data-ttu-id="c8c6e-330">Строка</span><span class="sxs-lookup"><span data-stu-id="c8c6e-330">String</span></span>                                                   | <span data-ttu-id="c8c6e-331">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-331">Yes</span></span>      | <span data-ttu-id="c8c6e-332">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="c8c6e-332">\<subjectId\></span></span> |
| <span data-ttu-id="c8c6e-333">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="c8c6e-333">assignmentState</span></span>  | <span data-ttu-id="c8c6e-334">Строка</span><span class="sxs-lookup"><span data-stu-id="c8c6e-334">String</span></span>                                                   | <span data-ttu-id="c8c6e-335">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-335">Yes</span></span>      | <span data-ttu-id="c8c6e-336">ПодХодящие/активные</span><span class="sxs-lookup"><span data-stu-id="c8c6e-336">Eligible / Active</span></span> |
| <span data-ttu-id="c8c6e-337">type</span><span class="sxs-lookup"><span data-stu-id="c8c6e-337">type</span></span>             | <span data-ttu-id="c8c6e-338">Строка</span><span class="sxs-lookup"><span data-stu-id="c8c6e-338">String</span></span>                                                   | <span data-ttu-id="c8c6e-339">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-339">Yes</span></span>      | <span data-ttu-id="c8c6e-340">Админремове</span><span class="sxs-lookup"><span data-stu-id="c8c6e-340">AdminRemove</span></span> |
| <span data-ttu-id="c8c6e-341">причиной</span><span class="sxs-lookup"><span data-stu-id="c8c6e-341">reason</span></span>           | <span data-ttu-id="c8c6e-342">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-342">String</span></span>                                                   | <span data-ttu-id="c8c6e-343">Нет</span><span class="sxs-lookup"><span data-stu-id="c8c6e-343">No</span></span>       |   |
| <span data-ttu-id="c8c6e-344">Диспетчер</span><span class="sxs-lookup"><span data-stu-id="c8c6e-344">schedule</span></span>         | [<span data-ttu-id="c8c6e-345">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c8c6e-345">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c8c6e-346">Нет</span><span class="sxs-lookup"><span data-stu-id="c8c6e-346">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="c8c6e-347">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8c6e-347">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="c8c6e-348">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8c6e-348">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="c8c6e-349">Пример 5: "Администратор обновляет назначение ролей"</span><span class="sxs-lookup"><span data-stu-id="c8c6e-349">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="c8c6e-350">В этом примере администраторы обновляют назначение роли пользователя nawu@fimdev.net владельцу.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-350">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="c8c6e-351">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-351">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="c8c6e-352">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8c6e-352">Property</span></span>         | <span data-ttu-id="c8c6e-353">Тип</span><span class="sxs-lookup"><span data-stu-id="c8c6e-353">Type</span></span>                                                     | <span data-ttu-id="c8c6e-354">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c8c6e-354">Required</span></span>                | <span data-ttu-id="c8c6e-355">Значение</span><span class="sxs-lookup"><span data-stu-id="c8c6e-355">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="c8c6e-356">resourceId</span><span class="sxs-lookup"><span data-stu-id="c8c6e-356">resourceId</span></span>       | <span data-ttu-id="c8c6e-357">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-357">String</span></span>                                                   | <span data-ttu-id="c8c6e-358">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-358">Yes</span></span>                     | <span data-ttu-id="c8c6e-359">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="c8c6e-359">\<resourceId\></span></span> |
| <span data-ttu-id="c8c6e-360">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="c8c6e-360">roleDefinitionId</span></span> | <span data-ttu-id="c8c6e-361">Строка</span><span class="sxs-lookup"><span data-stu-id="c8c6e-361">String</span></span>                                                   | <span data-ttu-id="c8c6e-362">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-362">Yes</span></span>                     | <span data-ttu-id="c8c6e-363">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="c8c6e-363">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="c8c6e-364">Субжектид</span><span class="sxs-lookup"><span data-stu-id="c8c6e-364">subjectId</span></span>        | <span data-ttu-id="c8c6e-365">Строка</span><span class="sxs-lookup"><span data-stu-id="c8c6e-365">String</span></span>                                                   | <span data-ttu-id="c8c6e-366">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-366">Yes</span></span>                     | <span data-ttu-id="c8c6e-367">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="c8c6e-367">\<subjectId\></span></span> |
| <span data-ttu-id="c8c6e-368">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="c8c6e-368">assignmentState</span></span>  | <span data-ttu-id="c8c6e-369">Строка</span><span class="sxs-lookup"><span data-stu-id="c8c6e-369">String</span></span>                                                   | <span data-ttu-id="c8c6e-370">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-370">Yes</span></span>                     | <span data-ttu-id="c8c6e-371">ПодХодящие/активные</span><span class="sxs-lookup"><span data-stu-id="c8c6e-371">Eligible / Active</span></span> |
| <span data-ttu-id="c8c6e-372">type</span><span class="sxs-lookup"><span data-stu-id="c8c6e-372">type</span></span>             | <span data-ttu-id="c8c6e-373">Строка</span><span class="sxs-lookup"><span data-stu-id="c8c6e-373">String</span></span>                                                   | <span data-ttu-id="c8c6e-374">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-374">Yes</span></span>                     | <span data-ttu-id="c8c6e-375">Админупдате</span><span class="sxs-lookup"><span data-stu-id="c8c6e-375">AdminUpdate</span></span> |
| <span data-ttu-id="c8c6e-376">причиной</span><span class="sxs-lookup"><span data-stu-id="c8c6e-376">reason</span></span>           | <span data-ttu-id="c8c6e-377">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-377">String</span></span>                                                   | <span data-ttu-id="c8c6e-378">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="c8c6e-378">depends on roleSettings</span></span> |   |
| <span data-ttu-id="c8c6e-379">Диспетчер</span><span class="sxs-lookup"><span data-stu-id="c8c6e-379">schedule</span></span>         | [<span data-ttu-id="c8c6e-380">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c8c6e-380">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c8c6e-381">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-381">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="c8c6e-382">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8c6e-382">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="c8c6e-383">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8c6e-383">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="c8c6e-384">Пример 6: администратор расширяет назначение ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="c8c6e-384">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="c8c6e-385">В этом примере показано, как расширить назначение роли истечения срока действия для пользователя АНУЖКУСЕР участнику службы управления API.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-385">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="c8c6e-386">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-386">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="c8c6e-387">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8c6e-387">Property</span></span>         | <span data-ttu-id="c8c6e-388">Тип</span><span class="sxs-lookup"><span data-stu-id="c8c6e-388">Type</span></span>                                                     | <span data-ttu-id="c8c6e-389">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c8c6e-389">Required</span></span>                | <span data-ttu-id="c8c6e-390">Значение</span><span class="sxs-lookup"><span data-stu-id="c8c6e-390">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="c8c6e-391">resourceId</span><span class="sxs-lookup"><span data-stu-id="c8c6e-391">resourceId</span></span>       | <span data-ttu-id="c8c6e-392">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-392">String</span></span>                                                   | <span data-ttu-id="c8c6e-393">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-393">Yes</span></span>                     | <span data-ttu-id="c8c6e-394">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="c8c6e-394">\<resourceId\></span></span> |
| <span data-ttu-id="c8c6e-395">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="c8c6e-395">roleDefinitionId</span></span> | <span data-ttu-id="c8c6e-396">Строка</span><span class="sxs-lookup"><span data-stu-id="c8c6e-396">String</span></span>                                                   | <span data-ttu-id="c8c6e-397">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-397">Yes</span></span>                     | <span data-ttu-id="c8c6e-398">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="c8c6e-398">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="c8c6e-399">Субжектид</span><span class="sxs-lookup"><span data-stu-id="c8c6e-399">subjectId</span></span>        | <span data-ttu-id="c8c6e-400">Строка</span><span class="sxs-lookup"><span data-stu-id="c8c6e-400">String</span></span>                                                   | <span data-ttu-id="c8c6e-401">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-401">Yes</span></span>                     | <span data-ttu-id="c8c6e-402">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="c8c6e-402">\<subjectId\></span></span> |
| <span data-ttu-id="c8c6e-403">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="c8c6e-403">assignmentState</span></span>  | <span data-ttu-id="c8c6e-404">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-404">String</span></span>                                                   | <span data-ttu-id="c8c6e-405">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-405">Yes</span></span>                     | <span data-ttu-id="c8c6e-406">ПодХодящие/активные</span><span class="sxs-lookup"><span data-stu-id="c8c6e-406">Eligible / Active</span></span> |
| <span data-ttu-id="c8c6e-407">type</span><span class="sxs-lookup"><span data-stu-id="c8c6e-407">type</span></span>             | <span data-ttu-id="c8c6e-408">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-408">String</span></span>                                                   | <span data-ttu-id="c8c6e-409">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-409">Yes</span></span>                     | <span data-ttu-id="c8c6e-410">Админекстенд</span><span class="sxs-lookup"><span data-stu-id="c8c6e-410">AdminExtend</span></span> |
| <span data-ttu-id="c8c6e-411">причиной</span><span class="sxs-lookup"><span data-stu-id="c8c6e-411">reason</span></span>           | <span data-ttu-id="c8c6e-412">String</span><span class="sxs-lookup"><span data-stu-id="c8c6e-412">String</span></span>                                                   | <span data-ttu-id="c8c6e-413">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="c8c6e-413">depends on roleSettings</span></span> |   |
| <span data-ttu-id="c8c6e-414">Диспетчер</span><span class="sxs-lookup"><span data-stu-id="c8c6e-414">schedule</span></span>         | [<span data-ttu-id="c8c6e-415">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c8c6e-415">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c8c6e-416">Да</span><span class="sxs-lookup"><span data-stu-id="c8c6e-416">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="c8c6e-417">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8c6e-417">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="c8c6e-418">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8c6e-418">Response</span></span>

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
  "suppressions": []
}
-->
