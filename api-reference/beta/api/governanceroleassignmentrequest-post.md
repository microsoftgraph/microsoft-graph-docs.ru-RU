---
title: Создание governanceRoleAssignmentRequest
description: Создайте запрос на назначение ролей для представления операции, необходимой для назначения ролей. В следующей таблице перечислены операции.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 2cb6ee71c888e90ee082c1f70ecced2c21199939
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435863"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="c48ef-104">Создание governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="c48ef-104">Create governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="c48ef-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c48ef-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c48ef-106">Создайте запрос на назначение ролей для представления операции, необходимой для назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="c48ef-106">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="c48ef-107">В следующей таблице перечислены операции.</span><span class="sxs-lookup"><span data-stu-id="c48ef-107">The following table lists the operations.</span></span>

| <span data-ttu-id="c48ef-108">Operation</span><span class="sxs-lookup"><span data-stu-id="c48ef-108">Operation</span></span>                                   | <span data-ttu-id="c48ef-109">Type</span><span class="sxs-lookup"><span data-stu-id="c48ef-109">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="c48ef-110">Назначение роли</span><span class="sxs-lookup"><span data-stu-id="c48ef-110">Assign a role assignment</span></span>                    | <span data-ttu-id="c48ef-111">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="c48ef-111">AdminAdd</span></span>    |
| <span data-ttu-id="c48ef-112">Активация назначения подходящих ролей</span><span class="sxs-lookup"><span data-stu-id="c48ef-112">Activate an eligible role assignment</span></span>        | <span data-ttu-id="c48ef-113">UserAdd</span><span class="sxs-lookup"><span data-stu-id="c48ef-113">UserAdd</span></span>     |
| <span data-ttu-id="c48ef-114">Отключение назначения активированной роли</span><span class="sxs-lookup"><span data-stu-id="c48ef-114">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="c48ef-115">UserRemove</span><span class="sxs-lookup"><span data-stu-id="c48ef-115">UserRemove</span></span>  |
| <span data-ttu-id="c48ef-116">Удаление назначения ролей</span><span class="sxs-lookup"><span data-stu-id="c48ef-116">Remove a role assignment</span></span>                    | <span data-ttu-id="c48ef-117">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="c48ef-117">AdminRemove</span></span> |
| <span data-ttu-id="c48ef-118">Обновление назначения ролей</span><span class="sxs-lookup"><span data-stu-id="c48ef-118">Update a role assignment</span></span>                    | <span data-ttu-id="c48ef-119">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="c48ef-119">AdminUpdate</span></span> |
| <span data-ttu-id="c48ef-120">Запрос на продление назначения ролей</span><span class="sxs-lookup"><span data-stu-id="c48ef-120">Request to extend my role assignment</span></span>        | <span data-ttu-id="c48ef-121">UserExtend</span><span class="sxs-lookup"><span data-stu-id="c48ef-121">UserExtend</span></span>  |
| <span data-ttu-id="c48ef-122">Расширение назначения ролей</span><span class="sxs-lookup"><span data-stu-id="c48ef-122">Extend a role assignment</span></span>                    | <span data-ttu-id="c48ef-123">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="c48ef-123">AdminExtend</span></span> |
| <span data-ttu-id="c48ef-124">Запрос на возобновление назначения истекшим сроком выполнения ролей</span><span class="sxs-lookup"><span data-stu-id="c48ef-124">Request to renew my expired role assignment</span></span> | <span data-ttu-id="c48ef-125">UserRenew</span><span class="sxs-lookup"><span data-stu-id="c48ef-125">UserRenew</span></span>   |
| <span data-ttu-id="c48ef-126">Возобновление назначения роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="c48ef-126">Renew an expired role assignment</span></span>            | <span data-ttu-id="c48ef-127">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="c48ef-127">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="c48ef-128">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c48ef-128">Permissions</span></span>

<span data-ttu-id="c48ef-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="c48ef-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="c48ef-131">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="c48ef-131">Azure resources</span></span>

| <span data-ttu-id="c48ef-132">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c48ef-132">Permission type</span></span> | <span data-ttu-id="c48ef-133">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c48ef-133">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="c48ef-134">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c48ef-134">Delegated (work or school account)</span></span> | <span data-ttu-id="c48ef-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="c48ef-135">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="c48ef-136">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c48ef-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c48ef-137">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c48ef-137">Not supported.</span></span> |
| <span data-ttu-id="c48ef-138">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c48ef-138">Application</span></span> | <span data-ttu-id="c48ef-139">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c48ef-139">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="c48ef-140">Azure AD</span><span class="sxs-lookup"><span data-stu-id="c48ef-140">Azure AD</span></span>

| <span data-ttu-id="c48ef-141">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c48ef-141">Permission type</span></span> | <span data-ttu-id="c48ef-142">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c48ef-142">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="c48ef-143">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c48ef-143">Delegated (work or school account)</span></span> | <span data-ttu-id="c48ef-144">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="c48ef-144">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="c48ef-145">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c48ef-145">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c48ef-146">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c48ef-146">Not supported.</span></span> |
| <span data-ttu-id="c48ef-147">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c48ef-147">Application</span></span> | <span data-ttu-id="c48ef-148">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c48ef-148">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="c48ef-149">Группы</span><span class="sxs-lookup"><span data-stu-id="c48ef-149">Groups</span></span>

|<span data-ttu-id="c48ef-150">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c48ef-150">Permission type</span></span> | <span data-ttu-id="c48ef-151">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c48ef-151">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="c48ef-152">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c48ef-152">Delegated (work or school account)</span></span> | <span data-ttu-id="c48ef-153">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="c48ef-153">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="c48ef-154">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c48ef-154">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c48ef-155">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c48ef-155">Not supported.</span></span> |
| <span data-ttu-id="c48ef-156">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c48ef-156">Application</span></span> | <span data-ttu-id="c48ef-157">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c48ef-157">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c48ef-158">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c48ef-158">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="c48ef-159">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c48ef-159">Request headers</span></span>

| <span data-ttu-id="c48ef-160">Имя</span><span class="sxs-lookup"><span data-stu-id="c48ef-160">Name</span></span>          | <span data-ttu-id="c48ef-161">Описание</span><span class="sxs-lookup"><span data-stu-id="c48ef-161">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="c48ef-162">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c48ef-162">Authorization</span></span> | <span data-ttu-id="c48ef-163">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c48ef-163">Bearer {code}</span></span>    |
| <span data-ttu-id="c48ef-164">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c48ef-164">Content-type</span></span>  | <span data-ttu-id="c48ef-165">application/json</span><span class="sxs-lookup"><span data-stu-id="c48ef-165">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c48ef-166">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c48ef-166">Request body</span></span>

<span data-ttu-id="c48ef-167">В теле запроса поставляем представление JSON объекта [governanceRoleAssignmentRequest.](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="c48ef-167">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="c48ef-168">Свойство</span><span class="sxs-lookup"><span data-stu-id="c48ef-168">Property</span></span>         | <span data-ttu-id="c48ef-169">Тип</span><span class="sxs-lookup"><span data-stu-id="c48ef-169">Type</span></span>                                                     | <span data-ttu-id="c48ef-170">Описание</span><span class="sxs-lookup"><span data-stu-id="c48ef-170">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="c48ef-171">resourceId</span><span class="sxs-lookup"><span data-stu-id="c48ef-171">resourceId</span></span>       | <span data-ttu-id="c48ef-172">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-172">String</span></span>                                                   | <span data-ttu-id="c48ef-173">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="c48ef-173">The ID of the resource.</span></span> <span data-ttu-id="c48ef-174">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c48ef-174">Required.</span></span> |
| <span data-ttu-id="c48ef-175">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c48ef-175">roleDefinitionId</span></span> | <span data-ttu-id="c48ef-176">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-176">String</span></span>                                                   | <span data-ttu-id="c48ef-177">ID определения роли.</span><span class="sxs-lookup"><span data-stu-id="c48ef-177">The ID of the role definition.</span></span> <span data-ttu-id="c48ef-178">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c48ef-178">Required.</span></span> |
| <span data-ttu-id="c48ef-179">subjectId</span><span class="sxs-lookup"><span data-stu-id="c48ef-179">subjectId</span></span>        | <span data-ttu-id="c48ef-180">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-180">String</span></span>                                                   | <span data-ttu-id="c48ef-181">ID субъекта.</span><span class="sxs-lookup"><span data-stu-id="c48ef-181">The ID of the subject.</span></span> <span data-ttu-id="c48ef-182">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c48ef-182">Required.</span></span> |
| <span data-ttu-id="c48ef-183">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c48ef-183">assignmentState</span></span>  | <span data-ttu-id="c48ef-184">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-184">String</span></span>                                                   | <span data-ttu-id="c48ef-185">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="c48ef-185">The state of assignment.</span></span> <span data-ttu-id="c48ef-186">Значение может быть `Eligible` и `Active` .</span><span class="sxs-lookup"><span data-stu-id="c48ef-186">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="c48ef-187">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="c48ef-187">Required.</span></span> |
| <span data-ttu-id="c48ef-188">type</span><span class="sxs-lookup"><span data-stu-id="c48ef-188">type</span></span>             | <span data-ttu-id="c48ef-189">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-189">String</span></span>                                                   | <span data-ttu-id="c48ef-190">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="c48ef-190">The request type.</span></span> <span data-ttu-id="c48ef-191">Значение может быть `AdminAdd` , , , , , , и `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `UserRenew` `AdminRenew` `AdminExtend` .</span><span class="sxs-lookup"><span data-stu-id="c48ef-191">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="c48ef-192">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c48ef-192">Required.</span></span> |
| <span data-ttu-id="c48ef-193">reason</span><span class="sxs-lookup"><span data-stu-id="c48ef-193">reason</span></span>           | <span data-ttu-id="c48ef-194">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-194">String</span></span>                                                   | <span data-ttu-id="c48ef-195">Причина должна быть предоставлена для запроса назначения ролей для целей аудита и проверки.</span><span class="sxs-lookup"><span data-stu-id="c48ef-195">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="c48ef-196">schedule</span><span class="sxs-lookup"><span data-stu-id="c48ef-196">schedule</span></span>         | [<span data-ttu-id="c48ef-197">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c48ef-197">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c48ef-198">Расписание запроса на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="c48ef-198">The schedule of the role assignment request.</span></span> <span data-ttu-id="c48ef-199">Для типа `UserAdd` запроса `AdminAdd` , и , это `AdminUpdate` `AdminExtend` необходимо.</span><span class="sxs-lookup"><span data-stu-id="c48ef-199">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="c48ef-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="c48ef-200">Response</span></span>

<span data-ttu-id="c48ef-201">В случае успешного выполнения этот метод возвращает код ответа и объект `201 Created` [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c48ef-201">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="c48ef-202">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="c48ef-202">Error codes</span></span>

<span data-ttu-id="c48ef-203">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="c48ef-203">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="c48ef-204">Кроме того, он возвращает коды ошибок, перечисленные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="c48ef-204">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="c48ef-205">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="c48ef-205">Error code</span></span>     | <span data-ttu-id="c48ef-206">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="c48ef-206">Error message</span></span>                               | <span data-ttu-id="c48ef-207">Сведения</span><span class="sxs-lookup"><span data-stu-id="c48ef-207">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="c48ef-208">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c48ef-208">400 BadRequest</span></span> | <span data-ttu-id="c48ef-209">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="c48ef-209">RoleNotFound</span></span>                                | <span data-ttu-id="c48ef-210">Предоставленное `roleDefinitionId` в теле запроса не удается найти.</span><span class="sxs-lookup"><span data-stu-id="c48ef-210">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="c48ef-211">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c48ef-211">400 BadRequest</span></span> | <span data-ttu-id="c48ef-212">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="c48ef-212">ResourceIsLocked</span></span>                            | <span data-ttu-id="c48ef-213">Ресурс, предоставленный в теле запроса, находится в состоянии и `Locked` не может создавать запросы на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="c48ef-213">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="c48ef-214">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c48ef-214">400 BadRequest</span></span> | <span data-ttu-id="c48ef-215">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="c48ef-215">SubjectNotFound</span></span>                             | <span data-ttu-id="c48ef-216">Предоставленное `subjectId` в теле запроса не удается найти.</span><span class="sxs-lookup"><span data-stu-id="c48ef-216">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="c48ef-217">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c48ef-217">400 BadRequest</span></span> | <span data-ttu-id="c48ef-218">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="c48ef-218">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="c48ef-219">В системе уже существует ожидаемая [система governanceRoleAssignmentRequest.](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="c48ef-219">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="c48ef-220">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c48ef-220">400 BadRequest</span></span> | <span data-ttu-id="c48ef-221">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="c48ef-221">RoleAssignmentExists</span></span>                        | <span data-ttu-id="c48ef-222">Система [governanceRoleAssignment,](../resources/governanceroleassignment.md) запрашиваемая для создания, уже существует в системе.</span><span class="sxs-lookup"><span data-stu-id="c48ef-222">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="c48ef-223">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c48ef-223">400 BadRequest</span></span> | <span data-ttu-id="c48ef-224">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="c48ef-224">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="c48ef-225">[УправлениеRoleAssignment,](../resources/governanceroleassignment.md) запрашиваемая для обновления или расширения, не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="c48ef-225">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="c48ef-226">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c48ef-226">400 BadRequest</span></span> | <span data-ttu-id="c48ef-227">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="c48ef-227">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="c48ef-228">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) не отвечает внутренним политикам и не может быть создан.</span><span class="sxs-lookup"><span data-stu-id="c48ef-228">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="c48ef-229">Примеры</span><span class="sxs-lookup"><span data-stu-id="c48ef-229">Examples</span></span>

<span data-ttu-id="c48ef-230">В следующих примерах покажите, как использовать этот API.</span><span class="sxs-lookup"><span data-stu-id="c48ef-230">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="c48ef-231">Пример 1. Администратор назначает пользователю роль</span><span class="sxs-lookup"><span data-stu-id="c48ef-231">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="c48ef-232">В этом примере администратор назначает nawu@contoso.com роли чтения биллинга.</span><span class="sxs-lookup"><span data-stu-id="c48ef-232">In this example, an administrator assigns user nawu@contoso.com to the Billing Reader role.</span></span>

 ><span data-ttu-id="c48ef-233">**Примечание:** В дополнение к разрешению в этом примере требуется, чтобы у запрашиваемой стороны было по крайней мере одно назначение роли администратора `Active` `owner` `user access administrator` (или) на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="c48ef-233">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="c48ef-234">Свойство</span><span class="sxs-lookup"><span data-stu-id="c48ef-234">Property</span></span>         | <span data-ttu-id="c48ef-235">Тип</span><span class="sxs-lookup"><span data-stu-id="c48ef-235">Type</span></span>                                                     | <span data-ttu-id="c48ef-236">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c48ef-236">Required</span></span>                 | <span data-ttu-id="c48ef-237">Значение</span><span class="sxs-lookup"><span data-stu-id="c48ef-237">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="c48ef-238">resourceId</span><span class="sxs-lookup"><span data-stu-id="c48ef-238">resourceId</span></span>       | <span data-ttu-id="c48ef-239">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-239">String</span></span>                                                   | <span data-ttu-id="c48ef-240">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-240">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="c48ef-241">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c48ef-241">roleDefinitionId</span></span> | <span data-ttu-id="c48ef-242">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-242">String</span></span>                                                   | <span data-ttu-id="c48ef-243">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-243">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="c48ef-244">subjectId</span><span class="sxs-lookup"><span data-stu-id="c48ef-244">subjectId</span></span>        | <span data-ttu-id="c48ef-245">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-245">String</span></span>                                                   | <span data-ttu-id="c48ef-246">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-246">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="c48ef-247">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c48ef-247">assignmentState</span></span>  | <span data-ttu-id="c48ef-248">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-248">String</span></span>                                                   | <span data-ttu-id="c48ef-249">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-249">Yes</span></span>                      | <span data-ttu-id="c48ef-250">Подходящая / Активная</span><span class="sxs-lookup"><span data-stu-id="c48ef-250">Eligible / Active</span></span> |
| <span data-ttu-id="c48ef-251">type</span><span class="sxs-lookup"><span data-stu-id="c48ef-251">type</span></span>             | <span data-ttu-id="c48ef-252">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-252">String</span></span>                                                   | <span data-ttu-id="c48ef-253">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-253">Yes</span></span>                      | <span data-ttu-id="c48ef-254">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="c48ef-254">AdminAdd</span></span> |
| <span data-ttu-id="c48ef-255">reason</span><span class="sxs-lookup"><span data-stu-id="c48ef-255">reason</span></span>           | <span data-ttu-id="c48ef-256">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-256">String</span></span>                                                   | <span data-ttu-id="c48ef-257">зависит от параметров ролей</span><span class="sxs-lookup"><span data-stu-id="c48ef-257">depends on role Settings</span></span> |   |
| <span data-ttu-id="c48ef-258">schedule</span><span class="sxs-lookup"><span data-stu-id="c48ef-258">schedule</span></span>         | [<span data-ttu-id="c48ef-259">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c48ef-259">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c48ef-260">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-260">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="c48ef-261">Запрос</span><span class="sxs-lookup"><span data-stu-id="c48ef-261">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c48ef-262">HTTP</span><span class="sxs-lookup"><span data-stu-id="c48ef-262">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c48ef-263">C#</span><span class="sxs-lookup"><span data-stu-id="c48ef-263">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c48ef-264">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c48ef-264">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c48ef-265">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c48ef-265">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c48ef-266">Java</span><span class="sxs-lookup"><span data-stu-id="c48ef-266">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="c48ef-267">Отклик</span><span class="sxs-lookup"><span data-stu-id="c48ef-267">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="c48ef-268">Пример 2. Пользователь активирует допустимую роль</span><span class="sxs-lookup"><span data-stu-id="c48ef-268">Example 2: User activates eligible role</span></span>

<span data-ttu-id="c48ef-269">В этом примере пользователь nawu@contoso.com активирует допустимую роль чтения биллинга.</span><span class="sxs-lookup"><span data-stu-id="c48ef-269">In this example, the user nawu@contoso.com activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="c48ef-270">Свойство</span><span class="sxs-lookup"><span data-stu-id="c48ef-270">Property</span></span>         | <span data-ttu-id="c48ef-271">Тип</span><span class="sxs-lookup"><span data-stu-id="c48ef-271">Type</span></span>                                                     | <span data-ttu-id="c48ef-272">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c48ef-272">Required</span></span>                 | <span data-ttu-id="c48ef-273">Значение</span><span class="sxs-lookup"><span data-stu-id="c48ef-273">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="c48ef-274">resourceId</span><span class="sxs-lookup"><span data-stu-id="c48ef-274">resourceId</span></span>       | <span data-ttu-id="c48ef-275">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-275">String</span></span>                                                   | <span data-ttu-id="c48ef-276">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-276">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="c48ef-277">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c48ef-277">roleDefinitionId</span></span> | <span data-ttu-id="c48ef-278">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-278">String</span></span>                                                   | <span data-ttu-id="c48ef-279">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-279">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="c48ef-280">subjectId</span><span class="sxs-lookup"><span data-stu-id="c48ef-280">subjectId</span></span>        | <span data-ttu-id="c48ef-281">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-281">String</span></span>                                                   | <span data-ttu-id="c48ef-282">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-282">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="c48ef-283">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c48ef-283">assignmentState</span></span>  | <span data-ttu-id="c48ef-284">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-284">String</span></span>                                                   | <span data-ttu-id="c48ef-285">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-285">Yes</span></span>                      | <span data-ttu-id="c48ef-286">Активное</span><span class="sxs-lookup"><span data-stu-id="c48ef-286">Active</span></span> |
| <span data-ttu-id="c48ef-287">type</span><span class="sxs-lookup"><span data-stu-id="c48ef-287">type</span></span>             | <span data-ttu-id="c48ef-288">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-288">String</span></span>                                                   | <span data-ttu-id="c48ef-289">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-289">Yes</span></span>                      | <span data-ttu-id="c48ef-290">UserAdd</span><span class="sxs-lookup"><span data-stu-id="c48ef-290">UserAdd</span></span> |
| <span data-ttu-id="c48ef-291">reason</span><span class="sxs-lookup"><span data-stu-id="c48ef-291">reason</span></span>           | <span data-ttu-id="c48ef-292">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-292">String</span></span>                                                   | <span data-ttu-id="c48ef-293">зависит от параметров ролей</span><span class="sxs-lookup"><span data-stu-id="c48ef-293">depends on role Settings</span></span> |   |
| <span data-ttu-id="c48ef-294">schedule</span><span class="sxs-lookup"><span data-stu-id="c48ef-294">schedule</span></span>         | [<span data-ttu-id="c48ef-295">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c48ef-295">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c48ef-296">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-296">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="c48ef-297">Запрос</span><span class="sxs-lookup"><span data-stu-id="c48ef-297">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="c48ef-298">Отклик</span><span class="sxs-lookup"><span data-stu-id="c48ef-298">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="c48ef-299">Пример 3. Пользователь отключает назначенную роль</span><span class="sxs-lookup"><span data-stu-id="c48ef-299">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="c48ef-300">В этом примере пользователь nawu@contoso.com активную роль чтения биллинга.</span><span class="sxs-lookup"><span data-stu-id="c48ef-300">In this example, the user nawu@contoso.com deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="c48ef-301">Свойство</span><span class="sxs-lookup"><span data-stu-id="c48ef-301">Property</span></span>         | <span data-ttu-id="c48ef-302">Тип</span><span class="sxs-lookup"><span data-stu-id="c48ef-302">Type</span></span>                                                     | <span data-ttu-id="c48ef-303">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c48ef-303">Required</span></span> | <span data-ttu-id="c48ef-304">Значение</span><span class="sxs-lookup"><span data-stu-id="c48ef-304">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="c48ef-305">resourceId</span><span class="sxs-lookup"><span data-stu-id="c48ef-305">resourceId</span></span>       | <span data-ttu-id="c48ef-306">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-306">String</span></span>                                                   | <span data-ttu-id="c48ef-307">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-307">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="c48ef-308">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c48ef-308">roleDefinitionId</span></span> | <span data-ttu-id="c48ef-309">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-309">String</span></span>                                                   | <span data-ttu-id="c48ef-310">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-310">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="c48ef-311">subjectId</span><span class="sxs-lookup"><span data-stu-id="c48ef-311">subjectId</span></span>        | <span data-ttu-id="c48ef-312">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-312">String</span></span>                                                   | <span data-ttu-id="c48ef-313">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-313">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="c48ef-314">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c48ef-314">assignmentState</span></span>  | <span data-ttu-id="c48ef-315">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-315">String</span></span>                                                   | <span data-ttu-id="c48ef-316">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-316">Yes</span></span>      | <span data-ttu-id="c48ef-317">Активное</span><span class="sxs-lookup"><span data-stu-id="c48ef-317">Active</span></span> |
| <span data-ttu-id="c48ef-318">type</span><span class="sxs-lookup"><span data-stu-id="c48ef-318">type</span></span>             | <span data-ttu-id="c48ef-319">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-319">String</span></span>                                                   | <span data-ttu-id="c48ef-320">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-320">Yes</span></span>      | <span data-ttu-id="c48ef-321">UserRemove</span><span class="sxs-lookup"><span data-stu-id="c48ef-321">UserRemove</span></span> |
| <span data-ttu-id="c48ef-322">reason</span><span class="sxs-lookup"><span data-stu-id="c48ef-322">reason</span></span>           | <span data-ttu-id="c48ef-323">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-323">String</span></span>                                                   | <span data-ttu-id="c48ef-324">Нет</span><span class="sxs-lookup"><span data-stu-id="c48ef-324">No</span></span>       |   |
| <span data-ttu-id="c48ef-325">schedule</span><span class="sxs-lookup"><span data-stu-id="c48ef-325">schedule</span></span>         | [<span data-ttu-id="c48ef-326">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c48ef-326">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c48ef-327">Нет</span><span class="sxs-lookup"><span data-stu-id="c48ef-327">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="c48ef-328">Запрос</span><span class="sxs-lookup"><span data-stu-id="c48ef-328">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="c48ef-329">Отклик</span><span class="sxs-lookup"><span data-stu-id="c48ef-329">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="c48ef-330">Пример 4. Администратор удаляет пользователя из роли</span><span class="sxs-lookup"><span data-stu-id="c48ef-330">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="c48ef-331">В этом примере администратор удаляет пользовательские nawu@contoso.com из роли Чтения биллинга.</span><span class="sxs-lookup"><span data-stu-id="c48ef-331">In this example, an administrator removes the user nawu@contoso.com from the Billing Reader role.</span></span>

 ><span data-ttu-id="c48ef-332">**Примечание:** В дополнение к разрешению в этом примере требуется, чтобы у запрашиваемой стороны было по крайней мере одно назначение роли администратора `Active` `owner` `user access administrator` (или) на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="c48ef-332">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="c48ef-333">Свойство</span><span class="sxs-lookup"><span data-stu-id="c48ef-333">Property</span></span>         | <span data-ttu-id="c48ef-334">Тип</span><span class="sxs-lookup"><span data-stu-id="c48ef-334">Type</span></span>                                                     | <span data-ttu-id="c48ef-335">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c48ef-335">Required</span></span> | <span data-ttu-id="c48ef-336">Значение</span><span class="sxs-lookup"><span data-stu-id="c48ef-336">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="c48ef-337">resourceId</span><span class="sxs-lookup"><span data-stu-id="c48ef-337">resourceId</span></span>       | <span data-ttu-id="c48ef-338">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-338">String</span></span>                                                   | <span data-ttu-id="c48ef-339">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-339">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="c48ef-340">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c48ef-340">roleDefinitionId</span></span> | <span data-ttu-id="c48ef-341">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-341">String</span></span>                                                   | <span data-ttu-id="c48ef-342">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-342">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="c48ef-343">subjectId</span><span class="sxs-lookup"><span data-stu-id="c48ef-343">subjectId</span></span>        | <span data-ttu-id="c48ef-344">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-344">String</span></span>                                                   | <span data-ttu-id="c48ef-345">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-345">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="c48ef-346">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c48ef-346">assignmentState</span></span>  | <span data-ttu-id="c48ef-347">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-347">String</span></span>                                                   | <span data-ttu-id="c48ef-348">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-348">Yes</span></span>      | <span data-ttu-id="c48ef-349">Подходящая / Активная</span><span class="sxs-lookup"><span data-stu-id="c48ef-349">Eligible / Active</span></span> |
| <span data-ttu-id="c48ef-350">type</span><span class="sxs-lookup"><span data-stu-id="c48ef-350">type</span></span>             | <span data-ttu-id="c48ef-351">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-351">String</span></span>                                                   | <span data-ttu-id="c48ef-352">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-352">Yes</span></span>      | <span data-ttu-id="c48ef-353">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="c48ef-353">AdminRemove</span></span> |
| <span data-ttu-id="c48ef-354">reason</span><span class="sxs-lookup"><span data-stu-id="c48ef-354">reason</span></span>           | <span data-ttu-id="c48ef-355">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-355">String</span></span>                                                   | <span data-ttu-id="c48ef-356">Нет</span><span class="sxs-lookup"><span data-stu-id="c48ef-356">No</span></span>       |   |
| <span data-ttu-id="c48ef-357">schedule</span><span class="sxs-lookup"><span data-stu-id="c48ef-357">schedule</span></span>         | [<span data-ttu-id="c48ef-358">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c48ef-358">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c48ef-359">Нет</span><span class="sxs-lookup"><span data-stu-id="c48ef-359">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="c48ef-360">Запрос</span><span class="sxs-lookup"><span data-stu-id="c48ef-360">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="c48ef-361">Отклик</span><span class="sxs-lookup"><span data-stu-id="c48ef-361">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="c48ef-362">Пример 5. Назначение роли администратора</span><span class="sxs-lookup"><span data-stu-id="c48ef-362">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="c48ef-363">В этом примере администраторы обновляют назначение ролей для пользователя, nawu@contoso.com владельца.</span><span class="sxs-lookup"><span data-stu-id="c48ef-363">In this example, administrators update the role assignment for the user nawu@contoso.com to Owner.</span></span>

 ><span data-ttu-id="c48ef-364">**Примечание:** В дополнение к разрешению в этом примере требуется, чтобы у запрашиваемой стороны было по крайней мере одно назначение роли администратора `Active` `owner` `user access administrator` (или) на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="c48ef-364">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="c48ef-365">Свойство</span><span class="sxs-lookup"><span data-stu-id="c48ef-365">Property</span></span>         | <span data-ttu-id="c48ef-366">Тип</span><span class="sxs-lookup"><span data-stu-id="c48ef-366">Type</span></span>                                                     | <span data-ttu-id="c48ef-367">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c48ef-367">Required</span></span>                | <span data-ttu-id="c48ef-368">Значение</span><span class="sxs-lookup"><span data-stu-id="c48ef-368">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="c48ef-369">resourceId</span><span class="sxs-lookup"><span data-stu-id="c48ef-369">resourceId</span></span>       | <span data-ttu-id="c48ef-370">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-370">String</span></span>                                                   | <span data-ttu-id="c48ef-371">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-371">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="c48ef-372">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c48ef-372">roleDefinitionId</span></span> | <span data-ttu-id="c48ef-373">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-373">String</span></span>                                                   | <span data-ttu-id="c48ef-374">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-374">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="c48ef-375">subjectId</span><span class="sxs-lookup"><span data-stu-id="c48ef-375">subjectId</span></span>        | <span data-ttu-id="c48ef-376">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-376">String</span></span>                                                   | <span data-ttu-id="c48ef-377">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-377">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="c48ef-378">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c48ef-378">assignmentState</span></span>  | <span data-ttu-id="c48ef-379">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-379">String</span></span>                                                   | <span data-ttu-id="c48ef-380">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-380">Yes</span></span>                     | <span data-ttu-id="c48ef-381">Подходящая / Активная</span><span class="sxs-lookup"><span data-stu-id="c48ef-381">Eligible / Active</span></span> |
| <span data-ttu-id="c48ef-382">type</span><span class="sxs-lookup"><span data-stu-id="c48ef-382">type</span></span>             | <span data-ttu-id="c48ef-383">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-383">String</span></span>                                                   | <span data-ttu-id="c48ef-384">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-384">Yes</span></span>                     | <span data-ttu-id="c48ef-385">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="c48ef-385">AdminUpdate</span></span> |
| <span data-ttu-id="c48ef-386">reason</span><span class="sxs-lookup"><span data-stu-id="c48ef-386">reason</span></span>           | <span data-ttu-id="c48ef-387">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-387">String</span></span>                                                   | <span data-ttu-id="c48ef-388">зависит от ролиSettings</span><span class="sxs-lookup"><span data-stu-id="c48ef-388">depends on roleSettings</span></span> |   |
| <span data-ttu-id="c48ef-389">schedule</span><span class="sxs-lookup"><span data-stu-id="c48ef-389">schedule</span></span>         | [<span data-ttu-id="c48ef-390">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c48ef-390">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c48ef-391">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-391">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="c48ef-392">Запрос</span><span class="sxs-lookup"><span data-stu-id="c48ef-392">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="c48ef-393">Отклик</span><span class="sxs-lookup"><span data-stu-id="c48ef-393">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="c48ef-394">Пример 6. Администратор расширяет назначение ролей по истечении срока действия</span><span class="sxs-lookup"><span data-stu-id="c48ef-394">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="c48ef-395">В этом примере расширяется назначение ролей по истечении срока действия для пользователя ANUJCUSER до участника службы управления API.</span><span class="sxs-lookup"><span data-stu-id="c48ef-395">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="c48ef-396">**Примечание:** В дополнение к разрешению в этом примере требуется, чтобы у запрашиваемой стороны было по крайней мере одно назначение роли администратора `Active` `owner` `user access administrator` (или) на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="c48ef-396">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="c48ef-397">Свойство</span><span class="sxs-lookup"><span data-stu-id="c48ef-397">Property</span></span>         | <span data-ttu-id="c48ef-398">Тип</span><span class="sxs-lookup"><span data-stu-id="c48ef-398">Type</span></span>                                                     | <span data-ttu-id="c48ef-399">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c48ef-399">Required</span></span>                | <span data-ttu-id="c48ef-400">Значение</span><span class="sxs-lookup"><span data-stu-id="c48ef-400">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="c48ef-401">resourceId</span><span class="sxs-lookup"><span data-stu-id="c48ef-401">resourceId</span></span>       | <span data-ttu-id="c48ef-402">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-402">String</span></span>                                                   | <span data-ttu-id="c48ef-403">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-403">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="c48ef-404">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c48ef-404">roleDefinitionId</span></span> | <span data-ttu-id="c48ef-405">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-405">String</span></span>                                                   | <span data-ttu-id="c48ef-406">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-406">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="c48ef-407">subjectId</span><span class="sxs-lookup"><span data-stu-id="c48ef-407">subjectId</span></span>        | <span data-ttu-id="c48ef-408">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-408">String</span></span>                                                   | <span data-ttu-id="c48ef-409">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-409">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="c48ef-410">assignmentState</span><span class="sxs-lookup"><span data-stu-id="c48ef-410">assignmentState</span></span>  | <span data-ttu-id="c48ef-411">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-411">String</span></span>                                                   | <span data-ttu-id="c48ef-412">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-412">Yes</span></span>                     | <span data-ttu-id="c48ef-413">Подходящая / Активная</span><span class="sxs-lookup"><span data-stu-id="c48ef-413">Eligible / Active</span></span> |
| <span data-ttu-id="c48ef-414">type</span><span class="sxs-lookup"><span data-stu-id="c48ef-414">type</span></span>             | <span data-ttu-id="c48ef-415">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-415">String</span></span>                                                   | <span data-ttu-id="c48ef-416">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-416">Yes</span></span>                     | <span data-ttu-id="c48ef-417">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="c48ef-417">AdminExtend</span></span> |
| <span data-ttu-id="c48ef-418">reason</span><span class="sxs-lookup"><span data-stu-id="c48ef-418">reason</span></span>           | <span data-ttu-id="c48ef-419">String</span><span class="sxs-lookup"><span data-stu-id="c48ef-419">String</span></span>                                                   | <span data-ttu-id="c48ef-420">зависит от ролиSettings</span><span class="sxs-lookup"><span data-stu-id="c48ef-420">depends on roleSettings</span></span> |   |
| <span data-ttu-id="c48ef-421">schedule</span><span class="sxs-lookup"><span data-stu-id="c48ef-421">schedule</span></span>         | [<span data-ttu-id="c48ef-422">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c48ef-422">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c48ef-423">Да</span><span class="sxs-lookup"><span data-stu-id="c48ef-423">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="c48ef-424">Запрос</span><span class="sxs-lookup"><span data-stu-id="c48ef-424">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="c48ef-425">Отклик</span><span class="sxs-lookup"><span data-stu-id="c48ef-425">Response</span></span>

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


