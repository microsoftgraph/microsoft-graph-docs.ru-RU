---
title: Создание governanceRoleAssignmentRequest
description: Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли. В приведенной ниже таблице перечислены операции.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: a76727ffd927f7d91b953c313b11a59e4512a65e
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635000"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="31bcd-104">Создание governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="31bcd-104">Create governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="31bcd-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31bcd-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31bcd-106">Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="31bcd-106">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="31bcd-107">В приведенной ниже таблице перечислены операции.</span><span class="sxs-lookup"><span data-stu-id="31bcd-107">The following table lists the operations.</span></span>

| <span data-ttu-id="31bcd-108">Operation</span><span class="sxs-lookup"><span data-stu-id="31bcd-108">Operation</span></span>                                   | <span data-ttu-id="31bcd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="31bcd-109">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="31bcd-110">Назначение роли</span><span class="sxs-lookup"><span data-stu-id="31bcd-110">Assign a role assignment</span></span>                    | <span data-ttu-id="31bcd-111">админадд</span><span class="sxs-lookup"><span data-stu-id="31bcd-111">AdminAdd</span></span>    |
| <span data-ttu-id="31bcd-112">Активация подходящего назначения роли</span><span class="sxs-lookup"><span data-stu-id="31bcd-112">Activate an eligible role assignment</span></span>        | <span data-ttu-id="31bcd-113">усерадд</span><span class="sxs-lookup"><span data-stu-id="31bcd-113">UserAdd</span></span>     |
| <span data-ttu-id="31bcd-114">Деактивация активированного назначения роли</span><span class="sxs-lookup"><span data-stu-id="31bcd-114">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="31bcd-115">усерремове</span><span class="sxs-lookup"><span data-stu-id="31bcd-115">UserRemove</span></span>  |
| <span data-ttu-id="31bcd-116">Удаление назначения роли</span><span class="sxs-lookup"><span data-stu-id="31bcd-116">Remove a role assignment</span></span>                    | <span data-ttu-id="31bcd-117">админремове</span><span class="sxs-lookup"><span data-stu-id="31bcd-117">AdminRemove</span></span> |
| <span data-ttu-id="31bcd-118">Обновление назначения роли</span><span class="sxs-lookup"><span data-stu-id="31bcd-118">Update a role assignment</span></span>                    | <span data-ttu-id="31bcd-119">админупдате</span><span class="sxs-lookup"><span data-stu-id="31bcd-119">AdminUpdate</span></span> |
| <span data-ttu-id="31bcd-120">Запрос на расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="31bcd-120">Request to extend my role assignment</span></span>        | <span data-ttu-id="31bcd-121">усерекстенд</span><span class="sxs-lookup"><span data-stu-id="31bcd-121">UserExtend</span></span>  |
| <span data-ttu-id="31bcd-122">Расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="31bcd-122">Extend a role assignment</span></span>                    | <span data-ttu-id="31bcd-123">админекстенд</span><span class="sxs-lookup"><span data-stu-id="31bcd-123">AdminExtend</span></span> |
| <span data-ttu-id="31bcd-124">Запрос на продление назначения роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="31bcd-124">Request to renew my expired role assignment</span></span> | <span data-ttu-id="31bcd-125">усерренев</span><span class="sxs-lookup"><span data-stu-id="31bcd-125">UserRenew</span></span>   |
| <span data-ttu-id="31bcd-126">Продление назначенной роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="31bcd-126">Renew an expired role assignment</span></span>            | <span data-ttu-id="31bcd-127">админренев</span><span class="sxs-lookup"><span data-stu-id="31bcd-127">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="31bcd-128">Разрешения</span><span class="sxs-lookup"><span data-stu-id="31bcd-128">Permissions</span></span>

<span data-ttu-id="31bcd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="31bcd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="31bcd-131">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="31bcd-131">Azure resources</span></span>

| <span data-ttu-id="31bcd-132">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31bcd-132">Permission type</span></span> | <span data-ttu-id="31bcd-133">Разрешения</span><span class="sxs-lookup"><span data-stu-id="31bcd-133">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="31bcd-134">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31bcd-134">Delegated (work or school account)</span></span> | <span data-ttu-id="31bcd-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="31bcd-135">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="31bcd-136">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31bcd-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31bcd-137">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31bcd-137">Not supported.</span></span> |
| <span data-ttu-id="31bcd-138">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31bcd-138">Application</span></span> | <span data-ttu-id="31bcd-139">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31bcd-139">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="31bcd-140">Azure AD</span><span class="sxs-lookup"><span data-stu-id="31bcd-140">Azure AD</span></span>

| <span data-ttu-id="31bcd-141">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31bcd-141">Permission type</span></span> | <span data-ttu-id="31bcd-142">Разрешения</span><span class="sxs-lookup"><span data-stu-id="31bcd-142">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="31bcd-143">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31bcd-143">Delegated (work or school account)</span></span> | <span data-ttu-id="31bcd-144">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="31bcd-144">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="31bcd-145">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31bcd-145">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31bcd-146">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31bcd-146">Not supported.</span></span> |
| <span data-ttu-id="31bcd-147">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31bcd-147">Application</span></span> | <span data-ttu-id="31bcd-148">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31bcd-148">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="31bcd-149">Группы</span><span class="sxs-lookup"><span data-stu-id="31bcd-149">Groups</span></span>

|<span data-ttu-id="31bcd-150">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31bcd-150">Permission type</span></span> | <span data-ttu-id="31bcd-151">Разрешения</span><span class="sxs-lookup"><span data-stu-id="31bcd-151">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="31bcd-152">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31bcd-152">Delegated (work or school account)</span></span> | <span data-ttu-id="31bcd-153">Привилежедакцесс. ReadWrite. Азуреадграупс</span><span class="sxs-lookup"><span data-stu-id="31bcd-153">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="31bcd-154">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31bcd-154">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31bcd-155">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31bcd-155">Not supported.</span></span> |
| <span data-ttu-id="31bcd-156">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31bcd-156">Application</span></span> | <span data-ttu-id="31bcd-157">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31bcd-157">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="31bcd-158">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31bcd-158">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="31bcd-159">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31bcd-159">Request headers</span></span>

| <span data-ttu-id="31bcd-160">Имя</span><span class="sxs-lookup"><span data-stu-id="31bcd-160">Name</span></span>          | <span data-ttu-id="31bcd-161">Описание</span><span class="sxs-lookup"><span data-stu-id="31bcd-161">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="31bcd-162">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31bcd-162">Authorization</span></span> | <span data-ttu-id="31bcd-163">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="31bcd-163">Bearer {code}</span></span>    |
| <span data-ttu-id="31bcd-164">Content-Type</span><span class="sxs-lookup"><span data-stu-id="31bcd-164">Content-type</span></span>  | <span data-ttu-id="31bcd-165">application/json</span><span class="sxs-lookup"><span data-stu-id="31bcd-165">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="31bcd-166">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="31bcd-166">Request body</span></span>

<span data-ttu-id="31bcd-167">В тексте запроса добавьте представление объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31bcd-167">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="31bcd-168">Свойство</span><span class="sxs-lookup"><span data-stu-id="31bcd-168">Property</span></span>         | <span data-ttu-id="31bcd-169">Тип</span><span class="sxs-lookup"><span data-stu-id="31bcd-169">Type</span></span>                                                     | <span data-ttu-id="31bcd-170">Описание</span><span class="sxs-lookup"><span data-stu-id="31bcd-170">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="31bcd-171">resourceId</span><span class="sxs-lookup"><span data-stu-id="31bcd-171">resourceId</span></span>       | <span data-ttu-id="31bcd-172">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-172">String</span></span>                                                   | <span data-ttu-id="31bcd-173">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="31bcd-173">The ID of the resource.</span></span> <span data-ttu-id="31bcd-174">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31bcd-174">Required.</span></span> |
| <span data-ttu-id="31bcd-175">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="31bcd-175">roleDefinitionId</span></span> | <span data-ttu-id="31bcd-176">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-176">String</span></span>                                                   | <span data-ttu-id="31bcd-177">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="31bcd-177">The ID of the role definition.</span></span> <span data-ttu-id="31bcd-178">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31bcd-178">Required.</span></span> |
| <span data-ttu-id="31bcd-179">субжектид</span><span class="sxs-lookup"><span data-stu-id="31bcd-179">subjectId</span></span>        | <span data-ttu-id="31bcd-180">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-180">String</span></span>                                                   | <span data-ttu-id="31bcd-181">ИДЕНТИФИКАТОР субъекта.</span><span class="sxs-lookup"><span data-stu-id="31bcd-181">The ID of the subject.</span></span> <span data-ttu-id="31bcd-182">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31bcd-182">Required.</span></span> |
| <span data-ttu-id="31bcd-183">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="31bcd-183">assignmentState</span></span>  | <span data-ttu-id="31bcd-184">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-184">String</span></span>                                                   | <span data-ttu-id="31bcd-185">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="31bcd-185">The state of assignment.</span></span> <span data-ttu-id="31bcd-186">Значение может быть `Eligible` и `Active` .</span><span class="sxs-lookup"><span data-stu-id="31bcd-186">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="31bcd-187">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="31bcd-187">Required.</span></span> |
| <span data-ttu-id="31bcd-188">type</span><span class="sxs-lookup"><span data-stu-id="31bcd-188">type</span></span>             | <span data-ttu-id="31bcd-189">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-189">String</span></span>                                                   | <span data-ttu-id="31bcd-190">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="31bcd-190">The request type.</span></span> <span data-ttu-id="31bcd-191">Возможные значения:,,,,,, `AdminAdd` `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `UserRenew` `AdminRenew` и `AdminExtend` .</span><span class="sxs-lookup"><span data-stu-id="31bcd-191">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="31bcd-192">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31bcd-192">Required.</span></span> |
| <span data-ttu-id="31bcd-193">reason</span><span class="sxs-lookup"><span data-stu-id="31bcd-193">reason</span></span>           | <span data-ttu-id="31bcd-194">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-194">String</span></span>                                                   | <span data-ttu-id="31bcd-195">Необходимо указать причину для запроса на назначение роли для аудита и проверки.</span><span class="sxs-lookup"><span data-stu-id="31bcd-195">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="31bcd-196">schedule</span><span class="sxs-lookup"><span data-stu-id="31bcd-196">schedule</span></span>         | [<span data-ttu-id="31bcd-197">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="31bcd-197">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="31bcd-198">Расписание запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="31bcd-198">The schedule of the role assignment request.</span></span> <span data-ttu-id="31bcd-199">Для типа запроса `UserAdd` ,, `AdminAdd` `AdminUpdate` , и `AdminExtend` , он необходим.</span><span class="sxs-lookup"><span data-stu-id="31bcd-199">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="31bcd-200">Ответ</span><span class="sxs-lookup"><span data-stu-id="31bcd-200">Response</span></span>

<span data-ttu-id="31bcd-201">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="31bcd-201">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="31bcd-202">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="31bcd-202">Error codes</span></span>

<span data-ttu-id="31bcd-203">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="31bcd-203">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="31bcd-204">Кроме того, он возвращает коды ошибок, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="31bcd-204">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="31bcd-205">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="31bcd-205">Error code</span></span>     | <span data-ttu-id="31bcd-206">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="31bcd-206">Error message</span></span>                               | <span data-ttu-id="31bcd-207">Сведения</span><span class="sxs-lookup"><span data-stu-id="31bcd-207">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="31bcd-208">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="31bcd-208">400 BadRequest</span></span> | <span data-ttu-id="31bcd-209">роленотфаунд</span><span class="sxs-lookup"><span data-stu-id="31bcd-209">RoleNotFound</span></span>                                | <span data-ttu-id="31bcd-210">`roleDefinitionId`Не удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="31bcd-210">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="31bcd-211">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="31bcd-211">400 BadRequest</span></span> | <span data-ttu-id="31bcd-212">ресаурцеислоккед</span><span class="sxs-lookup"><span data-stu-id="31bcd-212">ResourceIsLocked</span></span>                            | <span data-ttu-id="31bcd-213">Ресурс, указанный в теле запроса, находится в состоянии `Locked` и не может создавать запросы на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="31bcd-213">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="31bcd-214">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="31bcd-214">400 BadRequest</span></span> | <span data-ttu-id="31bcd-215">субжектнотфаунд</span><span class="sxs-lookup"><span data-stu-id="31bcd-215">SubjectNotFound</span></span>                             | <span data-ttu-id="31bcd-216">`subjectId`Не удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="31bcd-216">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="31bcd-217">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="31bcd-217">400 BadRequest</span></span> | <span data-ttu-id="31bcd-218">пендингролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="31bcd-218">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="31bcd-219">В системе уже существует ожидающий [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="31bcd-219">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="31bcd-220">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="31bcd-220">400 BadRequest</span></span> | <span data-ttu-id="31bcd-221">ролеассигнментексистс</span><span class="sxs-lookup"><span data-stu-id="31bcd-221">RoleAssignmentExists</span></span>                        | <span data-ttu-id="31bcd-222">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , который требуется создать, уже существует в системе.</span><span class="sxs-lookup"><span data-stu-id="31bcd-222">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="31bcd-223">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="31bcd-223">400 BadRequest</span></span> | <span data-ttu-id="31bcd-224">ролеассигнментдоеснотексист</span><span class="sxs-lookup"><span data-stu-id="31bcd-224">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="31bcd-225">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , запрошенный для обновления или расширения, не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="31bcd-225">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="31bcd-226">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="31bcd-226">400 BadRequest</span></span> | <span data-ttu-id="31bcd-227">ролеассигнментрекуестполицивалидатионфаилед</span><span class="sxs-lookup"><span data-stu-id="31bcd-227">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="31bcd-228">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) не отвечает внутренним политикам и не может быть создан.</span><span class="sxs-lookup"><span data-stu-id="31bcd-228">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="31bcd-229">Примеры</span><span class="sxs-lookup"><span data-stu-id="31bcd-229">Examples</span></span>

<span data-ttu-id="31bcd-230">В следующих примерах показано, как использовать этот API.</span><span class="sxs-lookup"><span data-stu-id="31bcd-230">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="31bcd-231">Пример 1: Администратор назначает пользователю роль</span><span class="sxs-lookup"><span data-stu-id="31bcd-231">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="31bcd-232">В этом примере администратор назначает пользователю nawu@fimdev.net роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="31bcd-232">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="31bcd-233">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней мере одно `Active` назначение роли администратора ( `owner` или `user access administrator` ) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="31bcd-233">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="31bcd-234">Свойство</span><span class="sxs-lookup"><span data-stu-id="31bcd-234">Property</span></span>         | <span data-ttu-id="31bcd-235">Тип</span><span class="sxs-lookup"><span data-stu-id="31bcd-235">Type</span></span>                                                     | <span data-ttu-id="31bcd-236">Обязательный</span><span class="sxs-lookup"><span data-stu-id="31bcd-236">Required</span></span>                 | <span data-ttu-id="31bcd-237">Значение</span><span class="sxs-lookup"><span data-stu-id="31bcd-237">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="31bcd-238">resourceId</span><span class="sxs-lookup"><span data-stu-id="31bcd-238">resourceId</span></span>       | <span data-ttu-id="31bcd-239">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-239">String</span></span>                                                   | <span data-ttu-id="31bcd-240">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-240">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="31bcd-241">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="31bcd-241">roleDefinitionId</span></span> | <span data-ttu-id="31bcd-242">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-242">String</span></span>                                                   | <span data-ttu-id="31bcd-243">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-243">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="31bcd-244">субжектид</span><span class="sxs-lookup"><span data-stu-id="31bcd-244">subjectId</span></span>        | <span data-ttu-id="31bcd-245">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-245">String</span></span>                                                   | <span data-ttu-id="31bcd-246">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-246">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="31bcd-247">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="31bcd-247">assignmentState</span></span>  | <span data-ttu-id="31bcd-248">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-248">String</span></span>                                                   | <span data-ttu-id="31bcd-249">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-249">Yes</span></span>                      | <span data-ttu-id="31bcd-250">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="31bcd-250">Eligible / Active</span></span> |
| <span data-ttu-id="31bcd-251">type</span><span class="sxs-lookup"><span data-stu-id="31bcd-251">type</span></span>             | <span data-ttu-id="31bcd-252">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-252">String</span></span>                                                   | <span data-ttu-id="31bcd-253">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-253">Yes</span></span>                      | <span data-ttu-id="31bcd-254">админадд</span><span class="sxs-lookup"><span data-stu-id="31bcd-254">AdminAdd</span></span> |
| <span data-ttu-id="31bcd-255">reason</span><span class="sxs-lookup"><span data-stu-id="31bcd-255">reason</span></span>           | <span data-ttu-id="31bcd-256">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-256">String</span></span>                                                   | <span data-ttu-id="31bcd-257">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="31bcd-257">depends on role Settings</span></span> |   |
| <span data-ttu-id="31bcd-258">schedule</span><span class="sxs-lookup"><span data-stu-id="31bcd-258">schedule</span></span>         | [<span data-ttu-id="31bcd-259">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="31bcd-259">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="31bcd-260">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-260">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="31bcd-261">Запрос</span><span class="sxs-lookup"><span data-stu-id="31bcd-261">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="31bcd-262">HTTP</span><span class="sxs-lookup"><span data-stu-id="31bcd-262">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="31bcd-263">C#</span><span class="sxs-lookup"><span data-stu-id="31bcd-263">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31bcd-264">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31bcd-264">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31bcd-265">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31bcd-265">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="31bcd-266">Отклик</span><span class="sxs-lookup"><span data-stu-id="31bcd-266">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="31bcd-267">Пример 2: пользователь активирует подходящие роли</span><span class="sxs-lookup"><span data-stu-id="31bcd-267">Example 2: User activates eligible role</span></span>

<span data-ttu-id="31bcd-268">В этом примере пользователь nawu@fimdev.net активирует соответствующую роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="31bcd-268">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="31bcd-269">Свойство</span><span class="sxs-lookup"><span data-stu-id="31bcd-269">Property</span></span>         | <span data-ttu-id="31bcd-270">Тип</span><span class="sxs-lookup"><span data-stu-id="31bcd-270">Type</span></span>                                                     | <span data-ttu-id="31bcd-271">Обязательный</span><span class="sxs-lookup"><span data-stu-id="31bcd-271">Required</span></span>                 | <span data-ttu-id="31bcd-272">Значение</span><span class="sxs-lookup"><span data-stu-id="31bcd-272">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="31bcd-273">resourceId</span><span class="sxs-lookup"><span data-stu-id="31bcd-273">resourceId</span></span>       | <span data-ttu-id="31bcd-274">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-274">String</span></span>                                                   | <span data-ttu-id="31bcd-275">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-275">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="31bcd-276">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="31bcd-276">roleDefinitionId</span></span> | <span data-ttu-id="31bcd-277">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-277">String</span></span>                                                   | <span data-ttu-id="31bcd-278">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-278">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="31bcd-279">субжектид</span><span class="sxs-lookup"><span data-stu-id="31bcd-279">subjectId</span></span>        | <span data-ttu-id="31bcd-280">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-280">String</span></span>                                                   | <span data-ttu-id="31bcd-281">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-281">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="31bcd-282">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="31bcd-282">assignmentState</span></span>  | <span data-ttu-id="31bcd-283">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-283">String</span></span>                                                   | <span data-ttu-id="31bcd-284">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-284">Yes</span></span>                      | <span data-ttu-id="31bcd-285">Активное</span><span class="sxs-lookup"><span data-stu-id="31bcd-285">Active</span></span> |
| <span data-ttu-id="31bcd-286">type</span><span class="sxs-lookup"><span data-stu-id="31bcd-286">type</span></span>             | <span data-ttu-id="31bcd-287">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-287">String</span></span>                                                   | <span data-ttu-id="31bcd-288">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-288">Yes</span></span>                      | <span data-ttu-id="31bcd-289">усерадд</span><span class="sxs-lookup"><span data-stu-id="31bcd-289">UserAdd</span></span> |
| <span data-ttu-id="31bcd-290">reason</span><span class="sxs-lookup"><span data-stu-id="31bcd-290">reason</span></span>           | <span data-ttu-id="31bcd-291">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-291">String</span></span>                                                   | <span data-ttu-id="31bcd-292">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="31bcd-292">depends on role Settings</span></span> |   |
| <span data-ttu-id="31bcd-293">schedule</span><span class="sxs-lookup"><span data-stu-id="31bcd-293">schedule</span></span>         | [<span data-ttu-id="31bcd-294">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="31bcd-294">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="31bcd-295">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-295">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="31bcd-296">Запрос</span><span class="sxs-lookup"><span data-stu-id="31bcd-296">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="31bcd-297">Ответ</span><span class="sxs-lookup"><span data-stu-id="31bcd-297">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="31bcd-298">Пример 3: пользователь отключает назначенную роль</span><span class="sxs-lookup"><span data-stu-id="31bcd-298">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="31bcd-299">В этом примере пользователь nawu@fimdev.net отключает активную роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="31bcd-299">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="31bcd-300">Свойство</span><span class="sxs-lookup"><span data-stu-id="31bcd-300">Property</span></span>         | <span data-ttu-id="31bcd-301">Тип</span><span class="sxs-lookup"><span data-stu-id="31bcd-301">Type</span></span>                                                     | <span data-ttu-id="31bcd-302">Обязательный</span><span class="sxs-lookup"><span data-stu-id="31bcd-302">Required</span></span> | <span data-ttu-id="31bcd-303">Значение</span><span class="sxs-lookup"><span data-stu-id="31bcd-303">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="31bcd-304">resourceId</span><span class="sxs-lookup"><span data-stu-id="31bcd-304">resourceId</span></span>       | <span data-ttu-id="31bcd-305">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-305">String</span></span>                                                   | <span data-ttu-id="31bcd-306">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-306">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="31bcd-307">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="31bcd-307">roleDefinitionId</span></span> | <span data-ttu-id="31bcd-308">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-308">String</span></span>                                                   | <span data-ttu-id="31bcd-309">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-309">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="31bcd-310">субжектид</span><span class="sxs-lookup"><span data-stu-id="31bcd-310">subjectId</span></span>        | <span data-ttu-id="31bcd-311">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-311">String</span></span>                                                   | <span data-ttu-id="31bcd-312">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-312">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="31bcd-313">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="31bcd-313">assignmentState</span></span>  | <span data-ttu-id="31bcd-314">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-314">String</span></span>                                                   | <span data-ttu-id="31bcd-315">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-315">Yes</span></span>      | <span data-ttu-id="31bcd-316">Активное</span><span class="sxs-lookup"><span data-stu-id="31bcd-316">Active</span></span> |
| <span data-ttu-id="31bcd-317">type</span><span class="sxs-lookup"><span data-stu-id="31bcd-317">type</span></span>             | <span data-ttu-id="31bcd-318">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-318">String</span></span>                                                   | <span data-ttu-id="31bcd-319">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-319">Yes</span></span>      | <span data-ttu-id="31bcd-320">усерремове</span><span class="sxs-lookup"><span data-stu-id="31bcd-320">UserRemove</span></span> |
| <span data-ttu-id="31bcd-321">reason</span><span class="sxs-lookup"><span data-stu-id="31bcd-321">reason</span></span>           | <span data-ttu-id="31bcd-322">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-322">String</span></span>                                                   | <span data-ttu-id="31bcd-323">Нет</span><span class="sxs-lookup"><span data-stu-id="31bcd-323">No</span></span>       |   |
| <span data-ttu-id="31bcd-324">schedule</span><span class="sxs-lookup"><span data-stu-id="31bcd-324">schedule</span></span>         | [<span data-ttu-id="31bcd-325">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="31bcd-325">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="31bcd-326">Нет</span><span class="sxs-lookup"><span data-stu-id="31bcd-326">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="31bcd-327">Запрос</span><span class="sxs-lookup"><span data-stu-id="31bcd-327">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="31bcd-328">Ответ</span><span class="sxs-lookup"><span data-stu-id="31bcd-328">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="31bcd-329">Пример 4: Администратор удаляет пользователя из роли</span><span class="sxs-lookup"><span data-stu-id="31bcd-329">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="31bcd-330">В этом примере администратор удаляет пользователя nawu@fimdev.net из роли читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="31bcd-330">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="31bcd-331">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней мере одно `Active` назначение роли администратора ( `owner` или `user access administrator` ) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="31bcd-331">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="31bcd-332">Свойство</span><span class="sxs-lookup"><span data-stu-id="31bcd-332">Property</span></span>         | <span data-ttu-id="31bcd-333">Тип</span><span class="sxs-lookup"><span data-stu-id="31bcd-333">Type</span></span>                                                     | <span data-ttu-id="31bcd-334">Обязательный</span><span class="sxs-lookup"><span data-stu-id="31bcd-334">Required</span></span> | <span data-ttu-id="31bcd-335">Значение</span><span class="sxs-lookup"><span data-stu-id="31bcd-335">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="31bcd-336">resourceId</span><span class="sxs-lookup"><span data-stu-id="31bcd-336">resourceId</span></span>       | <span data-ttu-id="31bcd-337">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-337">String</span></span>                                                   | <span data-ttu-id="31bcd-338">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-338">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="31bcd-339">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="31bcd-339">roleDefinitionId</span></span> | <span data-ttu-id="31bcd-340">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-340">String</span></span>                                                   | <span data-ttu-id="31bcd-341">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-341">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="31bcd-342">субжектид</span><span class="sxs-lookup"><span data-stu-id="31bcd-342">subjectId</span></span>        | <span data-ttu-id="31bcd-343">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-343">String</span></span>                                                   | <span data-ttu-id="31bcd-344">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-344">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="31bcd-345">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="31bcd-345">assignmentState</span></span>  | <span data-ttu-id="31bcd-346">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-346">String</span></span>                                                   | <span data-ttu-id="31bcd-347">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-347">Yes</span></span>      | <span data-ttu-id="31bcd-348">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="31bcd-348">Eligible / Active</span></span> |
| <span data-ttu-id="31bcd-349">type</span><span class="sxs-lookup"><span data-stu-id="31bcd-349">type</span></span>             | <span data-ttu-id="31bcd-350">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-350">String</span></span>                                                   | <span data-ttu-id="31bcd-351">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-351">Yes</span></span>      | <span data-ttu-id="31bcd-352">админремове</span><span class="sxs-lookup"><span data-stu-id="31bcd-352">AdminRemove</span></span> |
| <span data-ttu-id="31bcd-353">reason</span><span class="sxs-lookup"><span data-stu-id="31bcd-353">reason</span></span>           | <span data-ttu-id="31bcd-354">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-354">String</span></span>                                                   | <span data-ttu-id="31bcd-355">Нет</span><span class="sxs-lookup"><span data-stu-id="31bcd-355">No</span></span>       |   |
| <span data-ttu-id="31bcd-356">schedule</span><span class="sxs-lookup"><span data-stu-id="31bcd-356">schedule</span></span>         | [<span data-ttu-id="31bcd-357">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="31bcd-357">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="31bcd-358">Нет</span><span class="sxs-lookup"><span data-stu-id="31bcd-358">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="31bcd-359">Запрос</span><span class="sxs-lookup"><span data-stu-id="31bcd-359">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="31bcd-360">Ответ</span><span class="sxs-lookup"><span data-stu-id="31bcd-360">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="31bcd-361">Пример 5: "Администратор обновляет назначение ролей"</span><span class="sxs-lookup"><span data-stu-id="31bcd-361">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="31bcd-362">В этом примере администраторы обновляют назначение роли пользователя nawu@fimdev.net владельцу.</span><span class="sxs-lookup"><span data-stu-id="31bcd-362">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="31bcd-363">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней мере одно `Active` назначение роли администратора ( `owner` или `user access administrator` ) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="31bcd-363">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="31bcd-364">Свойство</span><span class="sxs-lookup"><span data-stu-id="31bcd-364">Property</span></span>         | <span data-ttu-id="31bcd-365">Тип</span><span class="sxs-lookup"><span data-stu-id="31bcd-365">Type</span></span>                                                     | <span data-ttu-id="31bcd-366">Обязательный</span><span class="sxs-lookup"><span data-stu-id="31bcd-366">Required</span></span>                | <span data-ttu-id="31bcd-367">Значение</span><span class="sxs-lookup"><span data-stu-id="31bcd-367">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="31bcd-368">resourceId</span><span class="sxs-lookup"><span data-stu-id="31bcd-368">resourceId</span></span>       | <span data-ttu-id="31bcd-369">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-369">String</span></span>                                                   | <span data-ttu-id="31bcd-370">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-370">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="31bcd-371">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="31bcd-371">roleDefinitionId</span></span> | <span data-ttu-id="31bcd-372">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-372">String</span></span>                                                   | <span data-ttu-id="31bcd-373">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-373">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="31bcd-374">субжектид</span><span class="sxs-lookup"><span data-stu-id="31bcd-374">subjectId</span></span>        | <span data-ttu-id="31bcd-375">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-375">String</span></span>                                                   | <span data-ttu-id="31bcd-376">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-376">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="31bcd-377">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="31bcd-377">assignmentState</span></span>  | <span data-ttu-id="31bcd-378">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-378">String</span></span>                                                   | <span data-ttu-id="31bcd-379">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-379">Yes</span></span>                     | <span data-ttu-id="31bcd-380">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="31bcd-380">Eligible / Active</span></span> |
| <span data-ttu-id="31bcd-381">type</span><span class="sxs-lookup"><span data-stu-id="31bcd-381">type</span></span>             | <span data-ttu-id="31bcd-382">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-382">String</span></span>                                                   | <span data-ttu-id="31bcd-383">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-383">Yes</span></span>                     | <span data-ttu-id="31bcd-384">админупдате</span><span class="sxs-lookup"><span data-stu-id="31bcd-384">AdminUpdate</span></span> |
| <span data-ttu-id="31bcd-385">reason</span><span class="sxs-lookup"><span data-stu-id="31bcd-385">reason</span></span>           | <span data-ttu-id="31bcd-386">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-386">String</span></span>                                                   | <span data-ttu-id="31bcd-387">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="31bcd-387">depends on roleSettings</span></span> |   |
| <span data-ttu-id="31bcd-388">schedule</span><span class="sxs-lookup"><span data-stu-id="31bcd-388">schedule</span></span>         | [<span data-ttu-id="31bcd-389">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="31bcd-389">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="31bcd-390">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-390">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="31bcd-391">Запрос</span><span class="sxs-lookup"><span data-stu-id="31bcd-391">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="31bcd-392">Ответ</span><span class="sxs-lookup"><span data-stu-id="31bcd-392">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="31bcd-393">Пример 6: администратор расширяет назначение ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="31bcd-393">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="31bcd-394">В этом примере показано, как расширить назначение роли истечения срока действия для пользователя АНУЖКУСЕР участнику службы управления API.</span><span class="sxs-lookup"><span data-stu-id="31bcd-394">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="31bcd-395">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней мере одно `Active` назначение роли администратора ( `owner` или `user access administrator` ) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="31bcd-395">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="31bcd-396">Свойство</span><span class="sxs-lookup"><span data-stu-id="31bcd-396">Property</span></span>         | <span data-ttu-id="31bcd-397">Тип</span><span class="sxs-lookup"><span data-stu-id="31bcd-397">Type</span></span>                                                     | <span data-ttu-id="31bcd-398">Обязательный</span><span class="sxs-lookup"><span data-stu-id="31bcd-398">Required</span></span>                | <span data-ttu-id="31bcd-399">Значение</span><span class="sxs-lookup"><span data-stu-id="31bcd-399">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="31bcd-400">resourceId</span><span class="sxs-lookup"><span data-stu-id="31bcd-400">resourceId</span></span>       | <span data-ttu-id="31bcd-401">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-401">String</span></span>                                                   | <span data-ttu-id="31bcd-402">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-402">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="31bcd-403">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="31bcd-403">roleDefinitionId</span></span> | <span data-ttu-id="31bcd-404">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-404">String</span></span>                                                   | <span data-ttu-id="31bcd-405">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-405">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="31bcd-406">субжектид</span><span class="sxs-lookup"><span data-stu-id="31bcd-406">subjectId</span></span>        | <span data-ttu-id="31bcd-407">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-407">String</span></span>                                                   | <span data-ttu-id="31bcd-408">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-408">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="31bcd-409">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="31bcd-409">assignmentState</span></span>  | <span data-ttu-id="31bcd-410">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-410">String</span></span>                                                   | <span data-ttu-id="31bcd-411">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-411">Yes</span></span>                     | <span data-ttu-id="31bcd-412">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="31bcd-412">Eligible / Active</span></span> |
| <span data-ttu-id="31bcd-413">type</span><span class="sxs-lookup"><span data-stu-id="31bcd-413">type</span></span>             | <span data-ttu-id="31bcd-414">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-414">String</span></span>                                                   | <span data-ttu-id="31bcd-415">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-415">Yes</span></span>                     | <span data-ttu-id="31bcd-416">админекстенд</span><span class="sxs-lookup"><span data-stu-id="31bcd-416">AdminExtend</span></span> |
| <span data-ttu-id="31bcd-417">reason</span><span class="sxs-lookup"><span data-stu-id="31bcd-417">reason</span></span>           | <span data-ttu-id="31bcd-418">String</span><span class="sxs-lookup"><span data-stu-id="31bcd-418">String</span></span>                                                   | <span data-ttu-id="31bcd-419">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="31bcd-419">depends on roleSettings</span></span> |   |
| <span data-ttu-id="31bcd-420">schedule</span><span class="sxs-lookup"><span data-stu-id="31bcd-420">schedule</span></span>         | [<span data-ttu-id="31bcd-421">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="31bcd-421">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="31bcd-422">Да</span><span class="sxs-lookup"><span data-stu-id="31bcd-422">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="31bcd-423">Запрос</span><span class="sxs-lookup"><span data-stu-id="31bcd-423">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="31bcd-424">Отклик</span><span class="sxs-lookup"><span data-stu-id="31bcd-424">Response</span></span>

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


