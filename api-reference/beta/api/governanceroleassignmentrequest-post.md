---
title: Создание governanceRoleAssignmentRequest
description: Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли. В приведенной ниже таблице перечислены операции.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 65ba674740fc7bc756d24fa3fc57b8db13d874b6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954132"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="0d4b7-104">Создание governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="0d4b7-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d4b7-105">Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="0d4b7-106">В приведенной ниже таблице перечислены операции.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-106">The following table lists the operations.</span></span>

| <span data-ttu-id="0d4b7-107">Operation</span><span class="sxs-lookup"><span data-stu-id="0d4b7-107">Operation</span></span>                                   | <span data-ttu-id="0d4b7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0d4b7-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="0d4b7-109">Назначение роли</span><span class="sxs-lookup"><span data-stu-id="0d4b7-109">Assign a role assignment</span></span>                    | <span data-ttu-id="0d4b7-110">Админадд</span><span class="sxs-lookup"><span data-stu-id="0d4b7-110">AdminAdd</span></span>    |
| <span data-ttu-id="0d4b7-111">Активация подходящего назначения роли</span><span class="sxs-lookup"><span data-stu-id="0d4b7-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="0d4b7-112">Усерадд</span><span class="sxs-lookup"><span data-stu-id="0d4b7-112">UserAdd</span></span>     |
| <span data-ttu-id="0d4b7-113">Деактивация активированного назначения роли</span><span class="sxs-lookup"><span data-stu-id="0d4b7-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="0d4b7-114">Усерремове</span><span class="sxs-lookup"><span data-stu-id="0d4b7-114">UserRemove</span></span>  |
| <span data-ttu-id="0d4b7-115">Удаление назначения роли</span><span class="sxs-lookup"><span data-stu-id="0d4b7-115">Remove a role assignment</span></span>                    | <span data-ttu-id="0d4b7-116">Админремове</span><span class="sxs-lookup"><span data-stu-id="0d4b7-116">AdminRemove</span></span> |
| <span data-ttu-id="0d4b7-117">Обновление назначения роли</span><span class="sxs-lookup"><span data-stu-id="0d4b7-117">Update a role assignment</span></span>                    | <span data-ttu-id="0d4b7-118">Админупдате</span><span class="sxs-lookup"><span data-stu-id="0d4b7-118">AdminUpdate</span></span> |
| <span data-ttu-id="0d4b7-119">Запрос на расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="0d4b7-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="0d4b7-120">Усерекстенд</span><span class="sxs-lookup"><span data-stu-id="0d4b7-120">UserExtend</span></span>  |
| <span data-ttu-id="0d4b7-121">Расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="0d4b7-121">Extend a role assignment</span></span>                    | <span data-ttu-id="0d4b7-122">Админекстенд</span><span class="sxs-lookup"><span data-stu-id="0d4b7-122">AdminExtend</span></span> |
| <span data-ttu-id="0d4b7-123">Запрос на продление назначения роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="0d4b7-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="0d4b7-124">Усерренев</span><span class="sxs-lookup"><span data-stu-id="0d4b7-124">UserRenew</span></span>   |
| <span data-ttu-id="0d4b7-125">Продление назначенной роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="0d4b7-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="0d4b7-126">Админренев</span><span class="sxs-lookup"><span data-stu-id="0d4b7-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="0d4b7-127">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d4b7-127">Permissions</span></span>

<span data-ttu-id="0d4b7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d4b7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0d4b7-130">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d4b7-130">Permission type</span></span>                        | <span data-ttu-id="0d4b7-131">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d4b7-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="0d4b7-132">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d4b7-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="0d4b7-133">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="0d4b7-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="0d4b7-134">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d4b7-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d4b7-135">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-135">Not supported.</span></span>                            |
| <span data-ttu-id="0d4b7-136">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d4b7-136">Application</span></span>                            | <span data-ttu-id="0d4b7-137">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-137">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d4b7-138">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d4b7-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="0d4b7-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d4b7-139">Request headers</span></span>

| <span data-ttu-id="0d4b7-140">Имя</span><span class="sxs-lookup"><span data-stu-id="0d4b7-140">Name</span></span>          | <span data-ttu-id="0d4b7-141">Описание</span><span class="sxs-lookup"><span data-stu-id="0d4b7-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="0d4b7-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d4b7-142">Authorization</span></span> | <span data-ttu-id="0d4b7-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0d4b7-143">Bearer {code}</span></span>    |
| <span data-ttu-id="0d4b7-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0d4b7-144">Content-type</span></span>  | <span data-ttu-id="0d4b7-145">application/json</span><span class="sxs-lookup"><span data-stu-id="0d4b7-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d4b7-146">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0d4b7-146">Request body</span></span>

<span data-ttu-id="0d4b7-147">В тексте запроса добавьте представление объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="0d4b7-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d4b7-148">Property</span></span>         | <span data-ttu-id="0d4b7-149">Тип</span><span class="sxs-lookup"><span data-stu-id="0d4b7-149">Type</span></span>                                                     | <span data-ttu-id="0d4b7-150">Описание</span><span class="sxs-lookup"><span data-stu-id="0d4b7-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="0d4b7-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="0d4b7-151">resourceId</span></span>       | <span data-ttu-id="0d4b7-152">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-152">String</span></span>                                                   | <span data-ttu-id="0d4b7-153">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-153">The ID of the resource.</span></span> <span data-ttu-id="0d4b7-154">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-154">Required.</span></span> |
| <span data-ttu-id="0d4b7-155">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="0d4b7-155">roleDefinitionId</span></span> | <span data-ttu-id="0d4b7-156">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-156">String</span></span>                                                   | <span data-ttu-id="0d4b7-157">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-157">The ID of the role definition.</span></span> <span data-ttu-id="0d4b7-158">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-158">Required.</span></span> |
| <span data-ttu-id="0d4b7-159">Субжектид</span><span class="sxs-lookup"><span data-stu-id="0d4b7-159">subjectId</span></span>        | <span data-ttu-id="0d4b7-160">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-160">String</span></span>                                                   | <span data-ttu-id="0d4b7-161">ИДЕНТИФИКАТОР субъекта.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-161">The ID of the subject.</span></span> <span data-ttu-id="0d4b7-162">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-162">Required.</span></span> |
| <span data-ttu-id="0d4b7-163">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="0d4b7-163">assignmentState</span></span>  | <span data-ttu-id="0d4b7-164">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-164">String</span></span>                                                   | <span data-ttu-id="0d4b7-165">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-165">The state of assignment.</span></span> <span data-ttu-id="0d4b7-166">Значение может быть `Eligible` и `Active`.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="0d4b7-167">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-167">Required.</span></span> |
| <span data-ttu-id="0d4b7-168">type</span><span class="sxs-lookup"><span data-stu-id="0d4b7-168">type</span></span>             | <span data-ttu-id="0d4b7-169">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-169">String</span></span>                                                   | <span data-ttu-id="0d4b7-170">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-170">The request type.</span></span> <span data-ttu-id="0d4b7-171">Возможные значения: `AdminAdd`, `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `AdminRenew` `AdminExtend`,,,,, и. `UserExtend` `UserRenew`</span><span class="sxs-lookup"><span data-stu-id="0d4b7-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="0d4b7-172">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-172">Required.</span></span> |
| <span data-ttu-id="0d4b7-173">причиной</span><span class="sxs-lookup"><span data-stu-id="0d4b7-173">reason</span></span>           | <span data-ttu-id="0d4b7-174">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-174">String</span></span>                                                   | <span data-ttu-id="0d4b7-175">Необходимо указать причину для запроса на назначение роли для аудита и проверки.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="0d4b7-176">schedule</span><span class="sxs-lookup"><span data-stu-id="0d4b7-176">schedule</span></span>         | [<span data-ttu-id="0d4b7-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="0d4b7-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="0d4b7-178">Расписание запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="0d4b7-179">`UserAdd`Для типа запроса `AdminAdd`,, `AdminUpdate`, и `AdminExtend`, он необходим.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="0d4b7-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d4b7-180">Response</span></span>

<span data-ttu-id="0d4b7-181">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="0d4b7-182">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="0d4b7-182">Error codes</span></span>

<span data-ttu-id="0d4b7-183">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="0d4b7-184">Кроме того, он возвращает коды ошибок, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="0d4b7-185">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="0d4b7-185">Error code</span></span>     | <span data-ttu-id="0d4b7-186">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="0d4b7-186">Error message</span></span>                               | <span data-ttu-id="0d4b7-187">Сведения</span><span class="sxs-lookup"><span data-stu-id="0d4b7-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="0d4b7-188">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="0d4b7-188">400 BadRequest</span></span> | <span data-ttu-id="0d4b7-189">Роленотфаунд</span><span class="sxs-lookup"><span data-stu-id="0d4b7-189">RoleNotFound</span></span>                                | <span data-ttu-id="0d4b7-190">Не `roleDefinitionId` удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="0d4b7-191">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="0d4b7-191">400 BadRequest</span></span> | <span data-ttu-id="0d4b7-192">Ресаурцеислоккед</span><span class="sxs-lookup"><span data-stu-id="0d4b7-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="0d4b7-193">Ресурс, указанный в теле запроса, находится в состоянии `Locked` и не может создавать запросы на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="0d4b7-194">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="0d4b7-194">400 BadRequest</span></span> | <span data-ttu-id="0d4b7-195">Субжектнотфаунд</span><span class="sxs-lookup"><span data-stu-id="0d4b7-195">SubjectNotFound</span></span>                             | <span data-ttu-id="0d4b7-196">Не `subjectId` удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="0d4b7-197">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="0d4b7-197">400 BadRequest</span></span> | <span data-ttu-id="0d4b7-198">Пендингролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="0d4b7-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="0d4b7-199">В системе уже существует ожидающий [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="0d4b7-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="0d4b7-200">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="0d4b7-200">400 BadRequest</span></span> | <span data-ttu-id="0d4b7-201">Ролеассигнментексистс</span><span class="sxs-lookup"><span data-stu-id="0d4b7-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="0d4b7-202">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , который требуется создать, уже существует в системе.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="0d4b7-203">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="0d4b7-203">400 BadRequest</span></span> | <span data-ttu-id="0d4b7-204">Ролеассигнментдоеснотексист</span><span class="sxs-lookup"><span data-stu-id="0d4b7-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="0d4b7-205">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , запрошенный для обновления или расширения, не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="0d4b7-206">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="0d4b7-206">400 BadRequest</span></span> | <span data-ttu-id="0d4b7-207">Ролеассигнментрекуестполицивалидатионфаилед</span><span class="sxs-lookup"><span data-stu-id="0d4b7-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="0d4b7-208">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) не отвечает внутренним политикам и не может быть создан.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="0d4b7-209">Примеры</span><span class="sxs-lookup"><span data-stu-id="0d4b7-209">Examples</span></span>

<span data-ttu-id="0d4b7-210">В следующих примерах показано, как использовать этот API.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="0d4b7-211">Пример 1: Администратор назначает пользователю роль</span><span class="sxs-lookup"><span data-stu-id="0d4b7-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="0d4b7-212">В этом примере администратор назначает пользователю nawu@fimdev.net роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="0d4b7-213">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="0d4b7-214">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d4b7-214">Property</span></span>         | <span data-ttu-id="0d4b7-215">Тип</span><span class="sxs-lookup"><span data-stu-id="0d4b7-215">Type</span></span>                                                     | <span data-ttu-id="0d4b7-216">Обязательный</span><span class="sxs-lookup"><span data-stu-id="0d4b7-216">Required</span></span>                 | <span data-ttu-id="0d4b7-217">Значение</span><span class="sxs-lookup"><span data-stu-id="0d4b7-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="0d4b7-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="0d4b7-218">resourceId</span></span>       | <span data-ttu-id="0d4b7-219">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-219">String</span></span>                                                   | <span data-ttu-id="0d4b7-220">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-220">Yes</span></span>                      | <span data-ttu-id="0d4b7-221">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="0d4b7-221">\<resourceId\></span></span> |
| <span data-ttu-id="0d4b7-222">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="0d4b7-222">roleDefinitionId</span></span> | <span data-ttu-id="0d4b7-223">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-223">String</span></span>                                                   | <span data-ttu-id="0d4b7-224">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-224">Yes</span></span>                      | <span data-ttu-id="0d4b7-225">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="0d4b7-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="0d4b7-226">Субжектид</span><span class="sxs-lookup"><span data-stu-id="0d4b7-226">subjectId</span></span>        | <span data-ttu-id="0d4b7-227">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-227">String</span></span>                                                   | <span data-ttu-id="0d4b7-228">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-228">Yes</span></span>                      | <span data-ttu-id="0d4b7-229">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="0d4b7-229">\<subjectId\></span></span> |
| <span data-ttu-id="0d4b7-230">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="0d4b7-230">assignmentState</span></span>  | <span data-ttu-id="0d4b7-231">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-231">String</span></span>                                                   | <span data-ttu-id="0d4b7-232">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-232">Yes</span></span>                      | <span data-ttu-id="0d4b7-233">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="0d4b7-233">Eligible / Active</span></span> |
| <span data-ttu-id="0d4b7-234">type</span><span class="sxs-lookup"><span data-stu-id="0d4b7-234">type</span></span>             | <span data-ttu-id="0d4b7-235">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-235">String</span></span>                                                   | <span data-ttu-id="0d4b7-236">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-236">Yes</span></span>                      | <span data-ttu-id="0d4b7-237">Админадд</span><span class="sxs-lookup"><span data-stu-id="0d4b7-237">AdminAdd</span></span> |
| <span data-ttu-id="0d4b7-238">причиной</span><span class="sxs-lookup"><span data-stu-id="0d4b7-238">reason</span></span>           | <span data-ttu-id="0d4b7-239">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-239">String</span></span>                                                   | <span data-ttu-id="0d4b7-240">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="0d4b7-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="0d4b7-241">schedule</span><span class="sxs-lookup"><span data-stu-id="0d4b7-241">schedule</span></span>         | [<span data-ttu-id="0d4b7-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="0d4b7-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="0d4b7-243">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="0d4b7-244">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d4b7-244">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0d4b7-245">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d4b7-245">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0d4b7-246">C#</span><span class="sxs-lookup"><span data-stu-id="0d4b7-246">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0d4b7-247">Javascript</span><span class="sxs-lookup"><span data-stu-id="0d4b7-247">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0d4b7-248">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0d4b7-248">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0d4b7-249">Java</span><span class="sxs-lookup"><span data-stu-id="0d4b7-249">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="0d4b7-250">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d4b7-250">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="0d4b7-251">Пример 2: пользователь активирует подходящие роли</span><span class="sxs-lookup"><span data-stu-id="0d4b7-251">Example 2: User activates eligible role</span></span>

<span data-ttu-id="0d4b7-252">В этом примере пользователь nawu@fimdev.net активирует соответствующую роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-252">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="0d4b7-253">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d4b7-253">Property</span></span>         | <span data-ttu-id="0d4b7-254">Тип</span><span class="sxs-lookup"><span data-stu-id="0d4b7-254">Type</span></span>                                                     | <span data-ttu-id="0d4b7-255">Обязательный</span><span class="sxs-lookup"><span data-stu-id="0d4b7-255">Required</span></span>                 | <span data-ttu-id="0d4b7-256">Значение</span><span class="sxs-lookup"><span data-stu-id="0d4b7-256">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="0d4b7-257">resourceId</span><span class="sxs-lookup"><span data-stu-id="0d4b7-257">resourceId</span></span>       | <span data-ttu-id="0d4b7-258">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-258">String</span></span>                                                   | <span data-ttu-id="0d4b7-259">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-259">Yes</span></span>                      | <span data-ttu-id="0d4b7-260">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="0d4b7-260">\<resourceId\></span></span> |
| <span data-ttu-id="0d4b7-261">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="0d4b7-261">roleDefinitionId</span></span> | <span data-ttu-id="0d4b7-262">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-262">String</span></span>                                                   | <span data-ttu-id="0d4b7-263">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-263">Yes</span></span>                      | <span data-ttu-id="0d4b7-264">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="0d4b7-264">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="0d4b7-265">Субжектид</span><span class="sxs-lookup"><span data-stu-id="0d4b7-265">subjectId</span></span>        | <span data-ttu-id="0d4b7-266">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-266">String</span></span>                                                   | <span data-ttu-id="0d4b7-267">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-267">Yes</span></span>                      | <span data-ttu-id="0d4b7-268">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="0d4b7-268">\<subjectId\></span></span> |
| <span data-ttu-id="0d4b7-269">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="0d4b7-269">assignmentState</span></span>  | <span data-ttu-id="0d4b7-270">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-270">String</span></span>                                                   | <span data-ttu-id="0d4b7-271">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-271">Yes</span></span>                      | <span data-ttu-id="0d4b7-272">Активное</span><span class="sxs-lookup"><span data-stu-id="0d4b7-272">Active</span></span> |
| <span data-ttu-id="0d4b7-273">type</span><span class="sxs-lookup"><span data-stu-id="0d4b7-273">type</span></span>             | <span data-ttu-id="0d4b7-274">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-274">String</span></span>                                                   | <span data-ttu-id="0d4b7-275">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-275">Yes</span></span>                      | <span data-ttu-id="0d4b7-276">Усерадд</span><span class="sxs-lookup"><span data-stu-id="0d4b7-276">UserAdd</span></span> |
| <span data-ttu-id="0d4b7-277">причиной</span><span class="sxs-lookup"><span data-stu-id="0d4b7-277">reason</span></span>           | <span data-ttu-id="0d4b7-278">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-278">String</span></span>                                                   | <span data-ttu-id="0d4b7-279">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="0d4b7-279">depends on role Settings</span></span> |   |
| <span data-ttu-id="0d4b7-280">schedule</span><span class="sxs-lookup"><span data-stu-id="0d4b7-280">schedule</span></span>         | [<span data-ttu-id="0d4b7-281">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="0d4b7-281">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="0d4b7-282">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-282">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="0d4b7-283">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d4b7-283">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="0d4b7-284">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d4b7-284">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="0d4b7-285">Пример 3: пользователь отключает назначенную роль</span><span class="sxs-lookup"><span data-stu-id="0d4b7-285">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="0d4b7-286">В этом примере пользователь nawu@fimdev.net отключает активную роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-286">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="0d4b7-287">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d4b7-287">Property</span></span>         | <span data-ttu-id="0d4b7-288">Тип</span><span class="sxs-lookup"><span data-stu-id="0d4b7-288">Type</span></span>                                                     | <span data-ttu-id="0d4b7-289">Обязательный</span><span class="sxs-lookup"><span data-stu-id="0d4b7-289">Required</span></span> | <span data-ttu-id="0d4b7-290">Значение</span><span class="sxs-lookup"><span data-stu-id="0d4b7-290">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="0d4b7-291">resourceId</span><span class="sxs-lookup"><span data-stu-id="0d4b7-291">resourceId</span></span>       | <span data-ttu-id="0d4b7-292">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-292">String</span></span>                                                   | <span data-ttu-id="0d4b7-293">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-293">Yes</span></span>      | <span data-ttu-id="0d4b7-294">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="0d4b7-294">\<resourceId\></span></span> |
| <span data-ttu-id="0d4b7-295">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="0d4b7-295">roleDefinitionId</span></span> | <span data-ttu-id="0d4b7-296">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-296">String</span></span>                                                   | <span data-ttu-id="0d4b7-297">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-297">Yes</span></span>      | <span data-ttu-id="0d4b7-298">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="0d4b7-298">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="0d4b7-299">Субжектид</span><span class="sxs-lookup"><span data-stu-id="0d4b7-299">subjectId</span></span>        | <span data-ttu-id="0d4b7-300">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-300">String</span></span>                                                   | <span data-ttu-id="0d4b7-301">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-301">Yes</span></span>      | <span data-ttu-id="0d4b7-302">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="0d4b7-302">\<subjectId\></span></span> |
| <span data-ttu-id="0d4b7-303">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="0d4b7-303">assignmentState</span></span>  | <span data-ttu-id="0d4b7-304">Строка</span><span class="sxs-lookup"><span data-stu-id="0d4b7-304">String</span></span>                                                   | <span data-ttu-id="0d4b7-305">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-305">Yes</span></span>      | <span data-ttu-id="0d4b7-306">Активное</span><span class="sxs-lookup"><span data-stu-id="0d4b7-306">Active</span></span> |
| <span data-ttu-id="0d4b7-307">type</span><span class="sxs-lookup"><span data-stu-id="0d4b7-307">type</span></span>             | <span data-ttu-id="0d4b7-308">Строка</span><span class="sxs-lookup"><span data-stu-id="0d4b7-308">String</span></span>                                                   | <span data-ttu-id="0d4b7-309">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-309">Yes</span></span>      | <span data-ttu-id="0d4b7-310">Усерремове</span><span class="sxs-lookup"><span data-stu-id="0d4b7-310">UserRemove</span></span> |
| <span data-ttu-id="0d4b7-311">причиной</span><span class="sxs-lookup"><span data-stu-id="0d4b7-311">reason</span></span>           | <span data-ttu-id="0d4b7-312">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-312">String</span></span>                                                   | <span data-ttu-id="0d4b7-313">Нет</span><span class="sxs-lookup"><span data-stu-id="0d4b7-313">No</span></span>       |   |
| <span data-ttu-id="0d4b7-314">schedule</span><span class="sxs-lookup"><span data-stu-id="0d4b7-314">schedule</span></span>         | [<span data-ttu-id="0d4b7-315">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="0d4b7-315">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="0d4b7-316">Нет</span><span class="sxs-lookup"><span data-stu-id="0d4b7-316">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="0d4b7-317">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d4b7-317">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="0d4b7-318">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d4b7-318">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="0d4b7-319">Пример 4: Администратор удаляет пользователя из роли</span><span class="sxs-lookup"><span data-stu-id="0d4b7-319">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="0d4b7-320">В этом примере администратор удаляет пользователя nawu@fimdev.net из роли читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-320">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="0d4b7-321">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-321">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="0d4b7-322">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d4b7-322">Property</span></span>         | <span data-ttu-id="0d4b7-323">Тип</span><span class="sxs-lookup"><span data-stu-id="0d4b7-323">Type</span></span>                                                     | <span data-ttu-id="0d4b7-324">Обязательный</span><span class="sxs-lookup"><span data-stu-id="0d4b7-324">Required</span></span> | <span data-ttu-id="0d4b7-325">Значение</span><span class="sxs-lookup"><span data-stu-id="0d4b7-325">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="0d4b7-326">resourceId</span><span class="sxs-lookup"><span data-stu-id="0d4b7-326">resourceId</span></span>       | <span data-ttu-id="0d4b7-327">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-327">String</span></span>                                                   | <span data-ttu-id="0d4b7-328">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-328">Yes</span></span>      | <span data-ttu-id="0d4b7-329">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="0d4b7-329">\<resourceId\></span></span> |
| <span data-ttu-id="0d4b7-330">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="0d4b7-330">roleDefinitionId</span></span> | <span data-ttu-id="0d4b7-331">Строка</span><span class="sxs-lookup"><span data-stu-id="0d4b7-331">String</span></span>                                                   | <span data-ttu-id="0d4b7-332">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-332">Yes</span></span>      | <span data-ttu-id="0d4b7-333">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="0d4b7-333">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="0d4b7-334">Субжектид</span><span class="sxs-lookup"><span data-stu-id="0d4b7-334">subjectId</span></span>        | <span data-ttu-id="0d4b7-335">Строка</span><span class="sxs-lookup"><span data-stu-id="0d4b7-335">String</span></span>                                                   | <span data-ttu-id="0d4b7-336">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-336">Yes</span></span>      | <span data-ttu-id="0d4b7-337">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="0d4b7-337">\<subjectId\></span></span> |
| <span data-ttu-id="0d4b7-338">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="0d4b7-338">assignmentState</span></span>  | <span data-ttu-id="0d4b7-339">Строка</span><span class="sxs-lookup"><span data-stu-id="0d4b7-339">String</span></span>                                                   | <span data-ttu-id="0d4b7-340">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-340">Yes</span></span>      | <span data-ttu-id="0d4b7-341">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="0d4b7-341">Eligible / Active</span></span> |
| <span data-ttu-id="0d4b7-342">type</span><span class="sxs-lookup"><span data-stu-id="0d4b7-342">type</span></span>             | <span data-ttu-id="0d4b7-343">Строка</span><span class="sxs-lookup"><span data-stu-id="0d4b7-343">String</span></span>                                                   | <span data-ttu-id="0d4b7-344">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-344">Yes</span></span>      | <span data-ttu-id="0d4b7-345">Админремове</span><span class="sxs-lookup"><span data-stu-id="0d4b7-345">AdminRemove</span></span> |
| <span data-ttu-id="0d4b7-346">причиной</span><span class="sxs-lookup"><span data-stu-id="0d4b7-346">reason</span></span>           | <span data-ttu-id="0d4b7-347">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-347">String</span></span>                                                   | <span data-ttu-id="0d4b7-348">Нет</span><span class="sxs-lookup"><span data-stu-id="0d4b7-348">No</span></span>       |   |
| <span data-ttu-id="0d4b7-349">schedule</span><span class="sxs-lookup"><span data-stu-id="0d4b7-349">schedule</span></span>         | [<span data-ttu-id="0d4b7-350">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="0d4b7-350">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="0d4b7-351">Нет</span><span class="sxs-lookup"><span data-stu-id="0d4b7-351">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="0d4b7-352">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d4b7-352">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="0d4b7-353">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d4b7-353">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="0d4b7-354">Пример 5: "Администратор обновляет назначение ролей"</span><span class="sxs-lookup"><span data-stu-id="0d4b7-354">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="0d4b7-355">В этом примере администраторы обновляют назначение роли пользователя nawu@fimdev.net владельцу.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-355">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="0d4b7-356">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-356">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="0d4b7-357">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d4b7-357">Property</span></span>         | <span data-ttu-id="0d4b7-358">Тип</span><span class="sxs-lookup"><span data-stu-id="0d4b7-358">Type</span></span>                                                     | <span data-ttu-id="0d4b7-359">Обязательный</span><span class="sxs-lookup"><span data-stu-id="0d4b7-359">Required</span></span>                | <span data-ttu-id="0d4b7-360">Значение</span><span class="sxs-lookup"><span data-stu-id="0d4b7-360">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="0d4b7-361">resourceId</span><span class="sxs-lookup"><span data-stu-id="0d4b7-361">resourceId</span></span>       | <span data-ttu-id="0d4b7-362">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-362">String</span></span>                                                   | <span data-ttu-id="0d4b7-363">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-363">Yes</span></span>                     | <span data-ttu-id="0d4b7-364">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="0d4b7-364">\<resourceId\></span></span> |
| <span data-ttu-id="0d4b7-365">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="0d4b7-365">roleDefinitionId</span></span> | <span data-ttu-id="0d4b7-366">Строка</span><span class="sxs-lookup"><span data-stu-id="0d4b7-366">String</span></span>                                                   | <span data-ttu-id="0d4b7-367">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-367">Yes</span></span>                     | <span data-ttu-id="0d4b7-368">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="0d4b7-368">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="0d4b7-369">Субжектид</span><span class="sxs-lookup"><span data-stu-id="0d4b7-369">subjectId</span></span>        | <span data-ttu-id="0d4b7-370">Строка</span><span class="sxs-lookup"><span data-stu-id="0d4b7-370">String</span></span>                                                   | <span data-ttu-id="0d4b7-371">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-371">Yes</span></span>                     | <span data-ttu-id="0d4b7-372">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="0d4b7-372">\<subjectId\></span></span> |
| <span data-ttu-id="0d4b7-373">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="0d4b7-373">assignmentState</span></span>  | <span data-ttu-id="0d4b7-374">Строка</span><span class="sxs-lookup"><span data-stu-id="0d4b7-374">String</span></span>                                                   | <span data-ttu-id="0d4b7-375">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-375">Yes</span></span>                     | <span data-ttu-id="0d4b7-376">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="0d4b7-376">Eligible / Active</span></span> |
| <span data-ttu-id="0d4b7-377">type</span><span class="sxs-lookup"><span data-stu-id="0d4b7-377">type</span></span>             | <span data-ttu-id="0d4b7-378">Строка</span><span class="sxs-lookup"><span data-stu-id="0d4b7-378">String</span></span>                                                   | <span data-ttu-id="0d4b7-379">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-379">Yes</span></span>                     | <span data-ttu-id="0d4b7-380">Админупдате</span><span class="sxs-lookup"><span data-stu-id="0d4b7-380">AdminUpdate</span></span> |
| <span data-ttu-id="0d4b7-381">причиной</span><span class="sxs-lookup"><span data-stu-id="0d4b7-381">reason</span></span>           | <span data-ttu-id="0d4b7-382">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-382">String</span></span>                                                   | <span data-ttu-id="0d4b7-383">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="0d4b7-383">depends on roleSettings</span></span> |   |
| <span data-ttu-id="0d4b7-384">schedule</span><span class="sxs-lookup"><span data-stu-id="0d4b7-384">schedule</span></span>         | [<span data-ttu-id="0d4b7-385">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="0d4b7-385">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="0d4b7-386">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-386">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="0d4b7-387">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d4b7-387">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="0d4b7-388">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d4b7-388">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="0d4b7-389">Пример 6: администратор расширяет назначение ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="0d4b7-389">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="0d4b7-390">В этом примере показано, как расширить назначение роли истечения срока действия для пользователя АНУЖКУСЕР участнику службы управления API.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-390">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="0d4b7-391">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней `Active` мере одно назначение роли`owner` администратора `user access administrator`(или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="0d4b7-391">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="0d4b7-392">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d4b7-392">Property</span></span>         | <span data-ttu-id="0d4b7-393">Тип</span><span class="sxs-lookup"><span data-stu-id="0d4b7-393">Type</span></span>                                                     | <span data-ttu-id="0d4b7-394">Обязательный</span><span class="sxs-lookup"><span data-stu-id="0d4b7-394">Required</span></span>                | <span data-ttu-id="0d4b7-395">Значение</span><span class="sxs-lookup"><span data-stu-id="0d4b7-395">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="0d4b7-396">resourceId</span><span class="sxs-lookup"><span data-stu-id="0d4b7-396">resourceId</span></span>       | <span data-ttu-id="0d4b7-397">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-397">String</span></span>                                                   | <span data-ttu-id="0d4b7-398">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-398">Yes</span></span>                     | <span data-ttu-id="0d4b7-399">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="0d4b7-399">\<resourceId\></span></span> |
| <span data-ttu-id="0d4b7-400">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="0d4b7-400">roleDefinitionId</span></span> | <span data-ttu-id="0d4b7-401">Строка</span><span class="sxs-lookup"><span data-stu-id="0d4b7-401">String</span></span>                                                   | <span data-ttu-id="0d4b7-402">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-402">Yes</span></span>                     | <span data-ttu-id="0d4b7-403">\<Роледефинитионид\></span><span class="sxs-lookup"><span data-stu-id="0d4b7-403">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="0d4b7-404">Субжектид</span><span class="sxs-lookup"><span data-stu-id="0d4b7-404">subjectId</span></span>        | <span data-ttu-id="0d4b7-405">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-405">String</span></span>                                                   | <span data-ttu-id="0d4b7-406">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-406">Yes</span></span>                     | <span data-ttu-id="0d4b7-407">\<Субжектид\></span><span class="sxs-lookup"><span data-stu-id="0d4b7-407">\<subjectId\></span></span> |
| <span data-ttu-id="0d4b7-408">Ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="0d4b7-408">assignmentState</span></span>  | <span data-ttu-id="0d4b7-409">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-409">String</span></span>                                                   | <span data-ttu-id="0d4b7-410">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-410">Yes</span></span>                     | <span data-ttu-id="0d4b7-411">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="0d4b7-411">Eligible / Active</span></span> |
| <span data-ttu-id="0d4b7-412">type</span><span class="sxs-lookup"><span data-stu-id="0d4b7-412">type</span></span>             | <span data-ttu-id="0d4b7-413">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-413">String</span></span>                                                   | <span data-ttu-id="0d4b7-414">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-414">Yes</span></span>                     | <span data-ttu-id="0d4b7-415">Админекстенд</span><span class="sxs-lookup"><span data-stu-id="0d4b7-415">AdminExtend</span></span> |
| <span data-ttu-id="0d4b7-416">причиной</span><span class="sxs-lookup"><span data-stu-id="0d4b7-416">reason</span></span>           | <span data-ttu-id="0d4b7-417">String</span><span class="sxs-lookup"><span data-stu-id="0d4b7-417">String</span></span>                                                   | <span data-ttu-id="0d4b7-418">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="0d4b7-418">depends on roleSettings</span></span> |   |
| <span data-ttu-id="0d4b7-419">schedule</span><span class="sxs-lookup"><span data-stu-id="0d4b7-419">schedule</span></span>         | [<span data-ttu-id="0d4b7-420">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="0d4b7-420">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="0d4b7-421">Да</span><span class="sxs-lookup"><span data-stu-id="0d4b7-421">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="0d4b7-422">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d4b7-422">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="0d4b7-423">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d4b7-423">Response</span></span>

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
