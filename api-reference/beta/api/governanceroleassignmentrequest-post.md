---
title: Создание governanceRoleAssignmentRequest
description: Создайте запрос на назначение ролей для представления операции, необходимой для назначения ролей. В следующей таблице перечислены операции.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: babca9a53ad10d5b029fdbdd4119220d143b779a
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350924"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="fde2f-104">Создание governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="fde2f-104">Create governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="fde2f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fde2f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fde2f-106">Создайте запрос на назначение ролей для представления операции, необходимой для назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="fde2f-106">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="fde2f-107">В следующей таблице перечислены операции.</span><span class="sxs-lookup"><span data-stu-id="fde2f-107">The following table lists the operations.</span></span>

| <span data-ttu-id="fde2f-108">Operation</span><span class="sxs-lookup"><span data-stu-id="fde2f-108">Operation</span></span>                                   | <span data-ttu-id="fde2f-109">Type</span><span class="sxs-lookup"><span data-stu-id="fde2f-109">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="fde2f-110">Назначение роли</span><span class="sxs-lookup"><span data-stu-id="fde2f-110">Assign a role assignment</span></span>                    | <span data-ttu-id="fde2f-111">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="fde2f-111">AdminAdd</span></span>    |
| <span data-ttu-id="fde2f-112">Активация назначения подходящих ролей</span><span class="sxs-lookup"><span data-stu-id="fde2f-112">Activate an eligible role assignment</span></span>        | <span data-ttu-id="fde2f-113">UserAdd</span><span class="sxs-lookup"><span data-stu-id="fde2f-113">UserAdd</span></span>     |
| <span data-ttu-id="fde2f-114">Отключение назначения активированной роли</span><span class="sxs-lookup"><span data-stu-id="fde2f-114">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="fde2f-115">UserRemove</span><span class="sxs-lookup"><span data-stu-id="fde2f-115">UserRemove</span></span>  |
| <span data-ttu-id="fde2f-116">Удаление назначения ролей</span><span class="sxs-lookup"><span data-stu-id="fde2f-116">Remove a role assignment</span></span>                    | <span data-ttu-id="fde2f-117">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="fde2f-117">AdminRemove</span></span> |
| <span data-ttu-id="fde2f-118">Обновление назначения ролей</span><span class="sxs-lookup"><span data-stu-id="fde2f-118">Update a role assignment</span></span>                    | <span data-ttu-id="fde2f-119">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="fde2f-119">AdminUpdate</span></span> |
| <span data-ttu-id="fde2f-120">Запрос на продление назначения ролей</span><span class="sxs-lookup"><span data-stu-id="fde2f-120">Request to extend my role assignment</span></span>        | <span data-ttu-id="fde2f-121">UserExtend</span><span class="sxs-lookup"><span data-stu-id="fde2f-121">UserExtend</span></span>  |
| <span data-ttu-id="fde2f-122">Расширение назначения ролей</span><span class="sxs-lookup"><span data-stu-id="fde2f-122">Extend a role assignment</span></span>                    | <span data-ttu-id="fde2f-123">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="fde2f-123">AdminExtend</span></span> |
| <span data-ttu-id="fde2f-124">Запрос на возобновление назначения истекшим сроком выполнения ролей</span><span class="sxs-lookup"><span data-stu-id="fde2f-124">Request to renew my expired role assignment</span></span> | <span data-ttu-id="fde2f-125">UserRenew</span><span class="sxs-lookup"><span data-stu-id="fde2f-125">UserRenew</span></span>   |
| <span data-ttu-id="fde2f-126">Возобновление назначения роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="fde2f-126">Renew an expired role assignment</span></span>            | <span data-ttu-id="fde2f-127">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="fde2f-127">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="fde2f-128">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fde2f-128">Permissions</span></span>

<span data-ttu-id="fde2f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="fde2f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="fde2f-131">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="fde2f-131">Azure resources</span></span>

| <span data-ttu-id="fde2f-132">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fde2f-132">Permission type</span></span> | <span data-ttu-id="fde2f-133">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fde2f-133">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="fde2f-134">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fde2f-134">Delegated (work or school account)</span></span> | <span data-ttu-id="fde2f-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="fde2f-135">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="fde2f-136">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fde2f-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fde2f-137">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fde2f-137">Not supported.</span></span> |
| <span data-ttu-id="fde2f-138">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fde2f-138">Application</span></span> | <span data-ttu-id="fde2f-139">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fde2f-139">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="fde2f-140">Azure AD</span><span class="sxs-lookup"><span data-stu-id="fde2f-140">Azure AD</span></span>

| <span data-ttu-id="fde2f-141">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fde2f-141">Permission type</span></span> | <span data-ttu-id="fde2f-142">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fde2f-142">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="fde2f-143">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fde2f-143">Delegated (work or school account)</span></span> | <span data-ttu-id="fde2f-144">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="fde2f-144">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="fde2f-145">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fde2f-145">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fde2f-146">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fde2f-146">Not supported.</span></span> |
| <span data-ttu-id="fde2f-147">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fde2f-147">Application</span></span> | <span data-ttu-id="fde2f-148">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fde2f-148">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="fde2f-149">Группы</span><span class="sxs-lookup"><span data-stu-id="fde2f-149">Groups</span></span>

|<span data-ttu-id="fde2f-150">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fde2f-150">Permission type</span></span> | <span data-ttu-id="fde2f-151">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fde2f-151">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="fde2f-152">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fde2f-152">Delegated (work or school account)</span></span> | <span data-ttu-id="fde2f-153">PrivilegedAccess.ReadWrite.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="fde2f-153">PrivilegedAccess.ReadWrite.AzureADGroup</span></span> |
| <span data-ttu-id="fde2f-154">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fde2f-154">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fde2f-155">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fde2f-155">Not supported.</span></span> |
| <span data-ttu-id="fde2f-156">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fde2f-156">Application</span></span> | <span data-ttu-id="fde2f-157">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fde2f-157">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fde2f-158">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fde2f-158">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="fde2f-159">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fde2f-159">Request headers</span></span>

| <span data-ttu-id="fde2f-160">Имя</span><span class="sxs-lookup"><span data-stu-id="fde2f-160">Name</span></span>          | <span data-ttu-id="fde2f-161">Описание</span><span class="sxs-lookup"><span data-stu-id="fde2f-161">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="fde2f-162">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fde2f-162">Authorization</span></span> | <span data-ttu-id="fde2f-163">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="fde2f-163">Bearer {code}</span></span>    |
| <span data-ttu-id="fde2f-164">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fde2f-164">Content-type</span></span>  | <span data-ttu-id="fde2f-165">application/json</span><span class="sxs-lookup"><span data-stu-id="fde2f-165">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="fde2f-166">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fde2f-166">Request body</span></span>

<span data-ttu-id="fde2f-167">В теле запроса поставляем представление JSON объекта [governanceRoleAssignmentRequest.](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="fde2f-167">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="fde2f-168">Свойство</span><span class="sxs-lookup"><span data-stu-id="fde2f-168">Property</span></span>         | <span data-ttu-id="fde2f-169">Тип</span><span class="sxs-lookup"><span data-stu-id="fde2f-169">Type</span></span>                                                     | <span data-ttu-id="fde2f-170">Описание</span><span class="sxs-lookup"><span data-stu-id="fde2f-170">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="fde2f-171">resourceId</span><span class="sxs-lookup"><span data-stu-id="fde2f-171">resourceId</span></span>       | <span data-ttu-id="fde2f-172">String</span><span class="sxs-lookup"><span data-stu-id="fde2f-172">String</span></span>                                                   | <span data-ttu-id="fde2f-173">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="fde2f-173">The ID of the resource.</span></span> <span data-ttu-id="fde2f-174">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fde2f-174">Required.</span></span> |
| <span data-ttu-id="fde2f-175">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="fde2f-175">roleDefinitionId</span></span> | <span data-ttu-id="fde2f-176">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-176">String</span></span>                                                   | <span data-ttu-id="fde2f-177">ID определения роли.</span><span class="sxs-lookup"><span data-stu-id="fde2f-177">The ID of the role definition.</span></span> <span data-ttu-id="fde2f-178">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fde2f-178">Required.</span></span> |
| <span data-ttu-id="fde2f-179">subjectId</span><span class="sxs-lookup"><span data-stu-id="fde2f-179">subjectId</span></span>        | <span data-ttu-id="fde2f-180">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-180">String</span></span>                                                   | <span data-ttu-id="fde2f-181">ID субъекта.</span><span class="sxs-lookup"><span data-stu-id="fde2f-181">The ID of the subject.</span></span> <span data-ttu-id="fde2f-182">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fde2f-182">Required.</span></span> |
| <span data-ttu-id="fde2f-183">assignmentState</span><span class="sxs-lookup"><span data-stu-id="fde2f-183">assignmentState</span></span>  | <span data-ttu-id="fde2f-184">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-184">String</span></span>                                                   | <span data-ttu-id="fde2f-185">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="fde2f-185">The state of assignment.</span></span> <span data-ttu-id="fde2f-186">Значение может быть `Eligible` и `Active` .</span><span class="sxs-lookup"><span data-stu-id="fde2f-186">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="fde2f-187">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="fde2f-187">Required.</span></span> |
| <span data-ttu-id="fde2f-188">type</span><span class="sxs-lookup"><span data-stu-id="fde2f-188">type</span></span>             | <span data-ttu-id="fde2f-189">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-189">String</span></span>                                                   | <span data-ttu-id="fde2f-190">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="fde2f-190">The request type.</span></span> <span data-ttu-id="fde2f-191">Значение может быть `AdminAdd` , , , , , , и `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `UserRenew` `AdminRenew` `AdminExtend` .</span><span class="sxs-lookup"><span data-stu-id="fde2f-191">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="fde2f-192">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fde2f-192">Required.</span></span> |
| <span data-ttu-id="fde2f-193">reason</span><span class="sxs-lookup"><span data-stu-id="fde2f-193">reason</span></span>           | <span data-ttu-id="fde2f-194">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-194">String</span></span>                                                   | <span data-ttu-id="fde2f-195">Причина должна быть предоставлена для запроса назначения ролей для целей аудита и проверки.</span><span class="sxs-lookup"><span data-stu-id="fde2f-195">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="fde2f-196">schedule</span><span class="sxs-lookup"><span data-stu-id="fde2f-196">schedule</span></span>         | [<span data-ttu-id="fde2f-197">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="fde2f-197">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="fde2f-198">Расписание запроса на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="fde2f-198">The schedule of the role assignment request.</span></span> <span data-ttu-id="fde2f-199">Для типа `UserAdd` запроса `AdminAdd` , и , это `AdminUpdate` `AdminExtend` необходимо.</span><span class="sxs-lookup"><span data-stu-id="fde2f-199">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="fde2f-200">Ответ</span><span class="sxs-lookup"><span data-stu-id="fde2f-200">Response</span></span>

<span data-ttu-id="fde2f-201">В случае успешного выполнения этот метод возвращает код ответа и объект `201 Created` [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fde2f-201">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="fde2f-202">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="fde2f-202">Error codes</span></span>

<span data-ttu-id="fde2f-203">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="fde2f-203">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="fde2f-204">Кроме того, он возвращает коды ошибок, перечисленные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="fde2f-204">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="fde2f-205">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="fde2f-205">Error code</span></span>     | <span data-ttu-id="fde2f-206">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="fde2f-206">Error message</span></span>                               | <span data-ttu-id="fde2f-207">Details</span><span class="sxs-lookup"><span data-stu-id="fde2f-207">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="fde2f-208">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="fde2f-208">400 BadRequest</span></span> | <span data-ttu-id="fde2f-209">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="fde2f-209">RoleNotFound</span></span>                                | <span data-ttu-id="fde2f-210">Предоставленное `roleDefinitionId` в теле запроса не удается найти.</span><span class="sxs-lookup"><span data-stu-id="fde2f-210">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="fde2f-211">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="fde2f-211">400 BadRequest</span></span> | <span data-ttu-id="fde2f-212">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="fde2f-212">ResourceIsLocked</span></span>                            | <span data-ttu-id="fde2f-213">Ресурс, предоставленный в теле запроса, находится в состоянии и `Locked` не может создавать запросы на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="fde2f-213">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="fde2f-214">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="fde2f-214">400 BadRequest</span></span> | <span data-ttu-id="fde2f-215">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="fde2f-215">SubjectNotFound</span></span>                             | <span data-ttu-id="fde2f-216">Предоставленное `subjectId` в теле запроса не удается найти.</span><span class="sxs-lookup"><span data-stu-id="fde2f-216">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="fde2f-217">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="fde2f-217">400 BadRequest</span></span> | <span data-ttu-id="fde2f-218">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="fde2f-218">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="fde2f-219">В системе уже существует ожидаемая [система governanceRoleAssignmentRequest.](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="fde2f-219">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="fde2f-220">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="fde2f-220">400 BadRequest</span></span> | <span data-ttu-id="fde2f-221">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="fde2f-221">RoleAssignmentExists</span></span>                        | <span data-ttu-id="fde2f-222">Система [governanceRoleAssignment,](../resources/governanceroleassignment.md) запрашиваемая для создания, уже существует в системе.</span><span class="sxs-lookup"><span data-stu-id="fde2f-222">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="fde2f-223">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="fde2f-223">400 BadRequest</span></span> | <span data-ttu-id="fde2f-224">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="fde2f-224">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="fde2f-225">[УправлениеRoleAssignment,](../resources/governanceroleassignment.md) запрашиваемая для обновления или расширения, не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="fde2f-225">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="fde2f-226">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="fde2f-226">400 BadRequest</span></span> | <span data-ttu-id="fde2f-227">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="fde2f-227">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="fde2f-228">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) не отвечает внутренним политикам и не может быть создан.</span><span class="sxs-lookup"><span data-stu-id="fde2f-228">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="fde2f-229">Примеры</span><span class="sxs-lookup"><span data-stu-id="fde2f-229">Examples</span></span>

<span data-ttu-id="fde2f-230">В следующих примерах покажите, как использовать этот API.</span><span class="sxs-lookup"><span data-stu-id="fde2f-230">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="fde2f-231">Пример 1. Администратор назначает пользователю роль</span><span class="sxs-lookup"><span data-stu-id="fde2f-231">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="fde2f-232">В этом примере администратор назначает nawu@contoso.com роли чтения биллинга.</span><span class="sxs-lookup"><span data-stu-id="fde2f-232">In this example, an administrator assigns user nawu@contoso.com to the Billing Reader role.</span></span>

 ><span data-ttu-id="fde2f-233">**Примечание:** В дополнение к разрешению в этом примере требуется, чтобы у запрашиваемой стороны было по крайней мере одно назначение роли администратора `Active` `owner` `user access administrator` (или) на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="fde2f-233">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="fde2f-234">Свойство</span><span class="sxs-lookup"><span data-stu-id="fde2f-234">Property</span></span>         | <span data-ttu-id="fde2f-235">Тип</span><span class="sxs-lookup"><span data-stu-id="fde2f-235">Type</span></span>                                                     | <span data-ttu-id="fde2f-236">Обязательный</span><span class="sxs-lookup"><span data-stu-id="fde2f-236">Required</span></span>                 | <span data-ttu-id="fde2f-237">Значение</span><span class="sxs-lookup"><span data-stu-id="fde2f-237">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="fde2f-238">resourceId</span><span class="sxs-lookup"><span data-stu-id="fde2f-238">resourceId</span></span>       | <span data-ttu-id="fde2f-239">String</span><span class="sxs-lookup"><span data-stu-id="fde2f-239">String</span></span>                                                   | <span data-ttu-id="fde2f-240">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-240">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="fde2f-241">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="fde2f-241">roleDefinitionId</span></span> | <span data-ttu-id="fde2f-242">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-242">String</span></span>                                                   | <span data-ttu-id="fde2f-243">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-243">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="fde2f-244">subjectId</span><span class="sxs-lookup"><span data-stu-id="fde2f-244">subjectId</span></span>        | <span data-ttu-id="fde2f-245">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-245">String</span></span>                                                   | <span data-ttu-id="fde2f-246">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-246">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="fde2f-247">assignmentState</span><span class="sxs-lookup"><span data-stu-id="fde2f-247">assignmentState</span></span>  | <span data-ttu-id="fde2f-248">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-248">String</span></span>                                                   | <span data-ttu-id="fde2f-249">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-249">Yes</span></span>                      | <span data-ttu-id="fde2f-250">Подходящая / Активная</span><span class="sxs-lookup"><span data-stu-id="fde2f-250">Eligible / Active</span></span> |
| <span data-ttu-id="fde2f-251">type</span><span class="sxs-lookup"><span data-stu-id="fde2f-251">type</span></span>             | <span data-ttu-id="fde2f-252">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-252">String</span></span>                                                   | <span data-ttu-id="fde2f-253">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-253">Yes</span></span>                      | <span data-ttu-id="fde2f-254">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="fde2f-254">AdminAdd</span></span> |
| <span data-ttu-id="fde2f-255">reason</span><span class="sxs-lookup"><span data-stu-id="fde2f-255">reason</span></span>           | <span data-ttu-id="fde2f-256">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-256">String</span></span>                                                   | <span data-ttu-id="fde2f-257">зависит от роли Параметры</span><span class="sxs-lookup"><span data-stu-id="fde2f-257">depends on role Settings</span></span> |   |
| <span data-ttu-id="fde2f-258">schedule</span><span class="sxs-lookup"><span data-stu-id="fde2f-258">schedule</span></span>         | [<span data-ttu-id="fde2f-259">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="fde2f-259">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="fde2f-260">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-260">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="fde2f-261">Запрос</span><span class="sxs-lookup"><span data-stu-id="fde2f-261">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fde2f-262">HTTP</span><span class="sxs-lookup"><span data-stu-id="fde2f-262">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post_1"
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
# <a name="c"></a>[<span data-ttu-id="fde2f-263">C#</span><span class="sxs-lookup"><span data-stu-id="fde2f-263">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fde2f-264">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fde2f-264">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fde2f-265">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fde2f-265">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fde2f-266">Java</span><span class="sxs-lookup"><span data-stu-id="fde2f-266">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="fde2f-267">Отклик</span><span class="sxs-lookup"><span data-stu-id="fde2f-267">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="fde2f-268">Пример 2. Пользователь активирует допустимую роль</span><span class="sxs-lookup"><span data-stu-id="fde2f-268">Example 2: User activates eligible role</span></span>

<span data-ttu-id="fde2f-269">В этом примере пользователь nawu@contoso.com активирует допустимую роль чтения биллинга.</span><span class="sxs-lookup"><span data-stu-id="fde2f-269">In this example, the user nawu@contoso.com activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="fde2f-270">Свойство</span><span class="sxs-lookup"><span data-stu-id="fde2f-270">Property</span></span>         | <span data-ttu-id="fde2f-271">Тип</span><span class="sxs-lookup"><span data-stu-id="fde2f-271">Type</span></span>                                                     | <span data-ttu-id="fde2f-272">Обязательный</span><span class="sxs-lookup"><span data-stu-id="fde2f-272">Required</span></span>                 | <span data-ttu-id="fde2f-273">Значение</span><span class="sxs-lookup"><span data-stu-id="fde2f-273">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="fde2f-274">resourceId</span><span class="sxs-lookup"><span data-stu-id="fde2f-274">resourceId</span></span>       | <span data-ttu-id="fde2f-275">String</span><span class="sxs-lookup"><span data-stu-id="fde2f-275">String</span></span>                                                   | <span data-ttu-id="fde2f-276">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-276">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="fde2f-277">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="fde2f-277">roleDefinitionId</span></span> | <span data-ttu-id="fde2f-278">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-278">String</span></span>                                                   | <span data-ttu-id="fde2f-279">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-279">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="fde2f-280">subjectId</span><span class="sxs-lookup"><span data-stu-id="fde2f-280">subjectId</span></span>        | <span data-ttu-id="fde2f-281">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-281">String</span></span>                                                   | <span data-ttu-id="fde2f-282">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-282">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="fde2f-283">assignmentState</span><span class="sxs-lookup"><span data-stu-id="fde2f-283">assignmentState</span></span>  | <span data-ttu-id="fde2f-284">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-284">String</span></span>                                                   | <span data-ttu-id="fde2f-285">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-285">Yes</span></span>                      | <span data-ttu-id="fde2f-286">Активное</span><span class="sxs-lookup"><span data-stu-id="fde2f-286">Active</span></span> |
| <span data-ttu-id="fde2f-287">type</span><span class="sxs-lookup"><span data-stu-id="fde2f-287">type</span></span>             | <span data-ttu-id="fde2f-288">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-288">String</span></span>                                                   | <span data-ttu-id="fde2f-289">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-289">Yes</span></span>                      | <span data-ttu-id="fde2f-290">UserAdd</span><span class="sxs-lookup"><span data-stu-id="fde2f-290">UserAdd</span></span> |
| <span data-ttu-id="fde2f-291">reason</span><span class="sxs-lookup"><span data-stu-id="fde2f-291">reason</span></span>           | <span data-ttu-id="fde2f-292">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-292">String</span></span>                                                   | <span data-ttu-id="fde2f-293">зависит от роли Параметры</span><span class="sxs-lookup"><span data-stu-id="fde2f-293">depends on role Settings</span></span> |   |
| <span data-ttu-id="fde2f-294">schedule</span><span class="sxs-lookup"><span data-stu-id="fde2f-294">schedule</span></span>         | [<span data-ttu-id="fde2f-295">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="fde2f-295">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="fde2f-296">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-296">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="fde2f-297">Запрос</span><span class="sxs-lookup"><span data-stu-id="fde2f-297">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fde2f-298">HTTP</span><span class="sxs-lookup"><span data-stu-id="fde2f-298">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post_2"
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
# <a name="c"></a>[<span data-ttu-id="fde2f-299">C#</span><span class="sxs-lookup"><span data-stu-id="fde2f-299">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fde2f-300">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fde2f-300">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fde2f-301">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fde2f-301">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fde2f-302">Java</span><span class="sxs-lookup"><span data-stu-id="fde2f-302">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fde2f-303">Отклик</span><span class="sxs-lookup"><span data-stu-id="fde2f-303">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="fde2f-304">Пример 3. Пользователь отключает назначенную роль</span><span class="sxs-lookup"><span data-stu-id="fde2f-304">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="fde2f-305">В этом примере пользователь nawu@contoso.com активную роль чтения биллинга.</span><span class="sxs-lookup"><span data-stu-id="fde2f-305">In this example, the user nawu@contoso.com deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="fde2f-306">Свойство</span><span class="sxs-lookup"><span data-stu-id="fde2f-306">Property</span></span>         | <span data-ttu-id="fde2f-307">Тип</span><span class="sxs-lookup"><span data-stu-id="fde2f-307">Type</span></span>                                                     | <span data-ttu-id="fde2f-308">Обязательный</span><span class="sxs-lookup"><span data-stu-id="fde2f-308">Required</span></span> | <span data-ttu-id="fde2f-309">Значение</span><span class="sxs-lookup"><span data-stu-id="fde2f-309">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="fde2f-310">resourceId</span><span class="sxs-lookup"><span data-stu-id="fde2f-310">resourceId</span></span>       | <span data-ttu-id="fde2f-311">String</span><span class="sxs-lookup"><span data-stu-id="fde2f-311">String</span></span>                                                   | <span data-ttu-id="fde2f-312">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-312">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="fde2f-313">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="fde2f-313">roleDefinitionId</span></span> | <span data-ttu-id="fde2f-314">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-314">String</span></span>                                                   | <span data-ttu-id="fde2f-315">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-315">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="fde2f-316">subjectId</span><span class="sxs-lookup"><span data-stu-id="fde2f-316">subjectId</span></span>        | <span data-ttu-id="fde2f-317">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-317">String</span></span>                                                   | <span data-ttu-id="fde2f-318">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-318">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="fde2f-319">assignmentState</span><span class="sxs-lookup"><span data-stu-id="fde2f-319">assignmentState</span></span>  | <span data-ttu-id="fde2f-320">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-320">String</span></span>                                                   | <span data-ttu-id="fde2f-321">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-321">Yes</span></span>      | <span data-ttu-id="fde2f-322">Активное</span><span class="sxs-lookup"><span data-stu-id="fde2f-322">Active</span></span> |
| <span data-ttu-id="fde2f-323">type</span><span class="sxs-lookup"><span data-stu-id="fde2f-323">type</span></span>             | <span data-ttu-id="fde2f-324">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-324">String</span></span>                                                   | <span data-ttu-id="fde2f-325">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-325">Yes</span></span>      | <span data-ttu-id="fde2f-326">UserRemove</span><span class="sxs-lookup"><span data-stu-id="fde2f-326">UserRemove</span></span> |
| <span data-ttu-id="fde2f-327">reason</span><span class="sxs-lookup"><span data-stu-id="fde2f-327">reason</span></span>           | <span data-ttu-id="fde2f-328">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-328">String</span></span>                                                   | <span data-ttu-id="fde2f-329">Нет</span><span class="sxs-lookup"><span data-stu-id="fde2f-329">No</span></span>       |   |
| <span data-ttu-id="fde2f-330">schedule</span><span class="sxs-lookup"><span data-stu-id="fde2f-330">schedule</span></span>         | [<span data-ttu-id="fde2f-331">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="fde2f-331">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="fde2f-332">Нет</span><span class="sxs-lookup"><span data-stu-id="fde2f-332">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="fde2f-333">Запрос</span><span class="sxs-lookup"><span data-stu-id="fde2f-333">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fde2f-334">HTTP</span><span class="sxs-lookup"><span data-stu-id="fde2f-334">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post_3"
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
# <a name="c"></a>[<span data-ttu-id="fde2f-335">C#</span><span class="sxs-lookup"><span data-stu-id="fde2f-335">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fde2f-336">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fde2f-336">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fde2f-337">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fde2f-337">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fde2f-338">Java</span><span class="sxs-lookup"><span data-stu-id="fde2f-338">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fde2f-339">Отклик</span><span class="sxs-lookup"><span data-stu-id="fde2f-339">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="fde2f-340">Пример 4. Администратор удаляет пользователя из роли</span><span class="sxs-lookup"><span data-stu-id="fde2f-340">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="fde2f-341">В этом примере администратор удаляет пользовательские nawu@contoso.com из роли Чтения биллинга.</span><span class="sxs-lookup"><span data-stu-id="fde2f-341">In this example, an administrator removes the user nawu@contoso.com from the Billing Reader role.</span></span>

 ><span data-ttu-id="fde2f-342">**Примечание:** В дополнение к разрешению в этом примере требуется, чтобы у запрашиваемой стороны было по крайней мере одно назначение роли администратора `Active` `owner` `user access administrator` (или) на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="fde2f-342">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="fde2f-343">Свойство</span><span class="sxs-lookup"><span data-stu-id="fde2f-343">Property</span></span>         | <span data-ttu-id="fde2f-344">Тип</span><span class="sxs-lookup"><span data-stu-id="fde2f-344">Type</span></span>                                                     | <span data-ttu-id="fde2f-345">Обязательный</span><span class="sxs-lookup"><span data-stu-id="fde2f-345">Required</span></span> | <span data-ttu-id="fde2f-346">Значение</span><span class="sxs-lookup"><span data-stu-id="fde2f-346">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="fde2f-347">resourceId</span><span class="sxs-lookup"><span data-stu-id="fde2f-347">resourceId</span></span>       | <span data-ttu-id="fde2f-348">String</span><span class="sxs-lookup"><span data-stu-id="fde2f-348">String</span></span>                                                   | <span data-ttu-id="fde2f-349">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-349">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="fde2f-350">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="fde2f-350">roleDefinitionId</span></span> | <span data-ttu-id="fde2f-351">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-351">String</span></span>                                                   | <span data-ttu-id="fde2f-352">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-352">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="fde2f-353">subjectId</span><span class="sxs-lookup"><span data-stu-id="fde2f-353">subjectId</span></span>        | <span data-ttu-id="fde2f-354">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-354">String</span></span>                                                   | <span data-ttu-id="fde2f-355">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-355">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="fde2f-356">assignmentState</span><span class="sxs-lookup"><span data-stu-id="fde2f-356">assignmentState</span></span>  | <span data-ttu-id="fde2f-357">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-357">String</span></span>                                                   | <span data-ttu-id="fde2f-358">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-358">Yes</span></span>      | <span data-ttu-id="fde2f-359">Подходящая / Активная</span><span class="sxs-lookup"><span data-stu-id="fde2f-359">Eligible / Active</span></span> |
| <span data-ttu-id="fde2f-360">type</span><span class="sxs-lookup"><span data-stu-id="fde2f-360">type</span></span>             | <span data-ttu-id="fde2f-361">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-361">String</span></span>                                                   | <span data-ttu-id="fde2f-362">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-362">Yes</span></span>      | <span data-ttu-id="fde2f-363">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="fde2f-363">AdminRemove</span></span> |
| <span data-ttu-id="fde2f-364">reason</span><span class="sxs-lookup"><span data-stu-id="fde2f-364">reason</span></span>           | <span data-ttu-id="fde2f-365">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-365">String</span></span>                                                   | <span data-ttu-id="fde2f-366">Нет</span><span class="sxs-lookup"><span data-stu-id="fde2f-366">No</span></span>       |   |
| <span data-ttu-id="fde2f-367">schedule</span><span class="sxs-lookup"><span data-stu-id="fde2f-367">schedule</span></span>         | [<span data-ttu-id="fde2f-368">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="fde2f-368">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="fde2f-369">Нет</span><span class="sxs-lookup"><span data-stu-id="fde2f-369">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="fde2f-370">Запрос</span><span class="sxs-lookup"><span data-stu-id="fde2f-370">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fde2f-371">HTTP</span><span class="sxs-lookup"><span data-stu-id="fde2f-371">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post_4"
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
# <a name="c"></a>[<span data-ttu-id="fde2f-372">C#</span><span class="sxs-lookup"><span data-stu-id="fde2f-372">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fde2f-373">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fde2f-373">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fde2f-374">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fde2f-374">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fde2f-375">Java</span><span class="sxs-lookup"><span data-stu-id="fde2f-375">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fde2f-376">Отклик</span><span class="sxs-lookup"><span data-stu-id="fde2f-376">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="fde2f-377">Пример 5. Назначение роли администратора</span><span class="sxs-lookup"><span data-stu-id="fde2f-377">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="fde2f-378">В этом примере администраторы обновляют назначение ролей для пользователя, nawu@contoso.com владельца.</span><span class="sxs-lookup"><span data-stu-id="fde2f-378">In this example, administrators update the role assignment for the user nawu@contoso.com to Owner.</span></span>

 ><span data-ttu-id="fde2f-379">**Примечание:** В дополнение к разрешению в этом примере требуется, чтобы у запрашиваемой стороны было по крайней мере одно назначение роли администратора `Active` `owner` `user access administrator` (или) на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="fde2f-379">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="fde2f-380">Свойство</span><span class="sxs-lookup"><span data-stu-id="fde2f-380">Property</span></span>         | <span data-ttu-id="fde2f-381">Тип</span><span class="sxs-lookup"><span data-stu-id="fde2f-381">Type</span></span>                                                     | <span data-ttu-id="fde2f-382">Обязательный</span><span class="sxs-lookup"><span data-stu-id="fde2f-382">Required</span></span>                | <span data-ttu-id="fde2f-383">Значение</span><span class="sxs-lookup"><span data-stu-id="fde2f-383">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="fde2f-384">resourceId</span><span class="sxs-lookup"><span data-stu-id="fde2f-384">resourceId</span></span>       | <span data-ttu-id="fde2f-385">String</span><span class="sxs-lookup"><span data-stu-id="fde2f-385">String</span></span>                                                   | <span data-ttu-id="fde2f-386">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-386">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="fde2f-387">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="fde2f-387">roleDefinitionId</span></span> | <span data-ttu-id="fde2f-388">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-388">String</span></span>                                                   | <span data-ttu-id="fde2f-389">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-389">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="fde2f-390">subjectId</span><span class="sxs-lookup"><span data-stu-id="fde2f-390">subjectId</span></span>        | <span data-ttu-id="fde2f-391">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-391">String</span></span>                                                   | <span data-ttu-id="fde2f-392">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-392">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="fde2f-393">assignmentState</span><span class="sxs-lookup"><span data-stu-id="fde2f-393">assignmentState</span></span>  | <span data-ttu-id="fde2f-394">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-394">String</span></span>                                                   | <span data-ttu-id="fde2f-395">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-395">Yes</span></span>                     | <span data-ttu-id="fde2f-396">Подходящая / Активная</span><span class="sxs-lookup"><span data-stu-id="fde2f-396">Eligible / Active</span></span> |
| <span data-ttu-id="fde2f-397">type</span><span class="sxs-lookup"><span data-stu-id="fde2f-397">type</span></span>             | <span data-ttu-id="fde2f-398">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-398">String</span></span>                                                   | <span data-ttu-id="fde2f-399">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-399">Yes</span></span>                     | <span data-ttu-id="fde2f-400">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="fde2f-400">AdminUpdate</span></span> |
| <span data-ttu-id="fde2f-401">reason</span><span class="sxs-lookup"><span data-stu-id="fde2f-401">reason</span></span>           | <span data-ttu-id="fde2f-402">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-402">String</span></span>                                                   | <span data-ttu-id="fde2f-403">зависит от ролиSettings</span><span class="sxs-lookup"><span data-stu-id="fde2f-403">depends on roleSettings</span></span> |   |
| <span data-ttu-id="fde2f-404">schedule</span><span class="sxs-lookup"><span data-stu-id="fde2f-404">schedule</span></span>         | [<span data-ttu-id="fde2f-405">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="fde2f-405">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="fde2f-406">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-406">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="fde2f-407">Запрос</span><span class="sxs-lookup"><span data-stu-id="fde2f-407">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fde2f-408">HTTP</span><span class="sxs-lookup"><span data-stu-id="fde2f-408">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post_5"
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
# <a name="c"></a>[<span data-ttu-id="fde2f-409">C#</span><span class="sxs-lookup"><span data-stu-id="fde2f-409">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fde2f-410">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fde2f-410">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fde2f-411">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fde2f-411">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fde2f-412">Java</span><span class="sxs-lookup"><span data-stu-id="fde2f-412">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-5-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fde2f-413">Отклик</span><span class="sxs-lookup"><span data-stu-id="fde2f-413">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="fde2f-414">Пример 6. Администратор расширяет назначение ролей по истечении срока действия</span><span class="sxs-lookup"><span data-stu-id="fde2f-414">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="fde2f-415">В этом примере расширяется назначение ролей по истечении срока действия для пользователя ANUJCUSER до участника службы управления API.</span><span class="sxs-lookup"><span data-stu-id="fde2f-415">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="fde2f-416">**Примечание:** В дополнение к разрешению в этом примере требуется, чтобы у запрашиваемой стороны было по крайней мере одно назначение роли администратора `Active` `owner` `user access administrator` (или) на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="fde2f-416">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="fde2f-417">Свойство</span><span class="sxs-lookup"><span data-stu-id="fde2f-417">Property</span></span>         | <span data-ttu-id="fde2f-418">Тип</span><span class="sxs-lookup"><span data-stu-id="fde2f-418">Type</span></span>                                                     | <span data-ttu-id="fde2f-419">Обязательный</span><span class="sxs-lookup"><span data-stu-id="fde2f-419">Required</span></span>                | <span data-ttu-id="fde2f-420">Значение</span><span class="sxs-lookup"><span data-stu-id="fde2f-420">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="fde2f-421">resourceId</span><span class="sxs-lookup"><span data-stu-id="fde2f-421">resourceId</span></span>       | <span data-ttu-id="fde2f-422">String</span><span class="sxs-lookup"><span data-stu-id="fde2f-422">String</span></span>                                                   | <span data-ttu-id="fde2f-423">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-423">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="fde2f-424">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="fde2f-424">roleDefinitionId</span></span> | <span data-ttu-id="fde2f-425">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-425">String</span></span>                                                   | <span data-ttu-id="fde2f-426">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-426">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="fde2f-427">subjectId</span><span class="sxs-lookup"><span data-stu-id="fde2f-427">subjectId</span></span>        | <span data-ttu-id="fde2f-428">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-428">String</span></span>                                                   | <span data-ttu-id="fde2f-429">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-429">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="fde2f-430">assignmentState</span><span class="sxs-lookup"><span data-stu-id="fde2f-430">assignmentState</span></span>  | <span data-ttu-id="fde2f-431">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-431">String</span></span>                                                   | <span data-ttu-id="fde2f-432">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-432">Yes</span></span>                     | <span data-ttu-id="fde2f-433">Подходящая / Активная</span><span class="sxs-lookup"><span data-stu-id="fde2f-433">Eligible / Active</span></span> |
| <span data-ttu-id="fde2f-434">type</span><span class="sxs-lookup"><span data-stu-id="fde2f-434">type</span></span>             | <span data-ttu-id="fde2f-435">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-435">String</span></span>                                                   | <span data-ttu-id="fde2f-436">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-436">Yes</span></span>                     | <span data-ttu-id="fde2f-437">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="fde2f-437">AdminExtend</span></span> |
| <span data-ttu-id="fde2f-438">reason</span><span class="sxs-lookup"><span data-stu-id="fde2f-438">reason</span></span>           | <span data-ttu-id="fde2f-439">Строка</span><span class="sxs-lookup"><span data-stu-id="fde2f-439">String</span></span>                                                   | <span data-ttu-id="fde2f-440">зависит от ролиSettings</span><span class="sxs-lookup"><span data-stu-id="fde2f-440">depends on roleSettings</span></span> |   |
| <span data-ttu-id="fde2f-441">schedule</span><span class="sxs-lookup"><span data-stu-id="fde2f-441">schedule</span></span>         | [<span data-ttu-id="fde2f-442">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="fde2f-442">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="fde2f-443">Да</span><span class="sxs-lookup"><span data-stu-id="fde2f-443">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="fde2f-444">Запрос</span><span class="sxs-lookup"><span data-stu-id="fde2f-444">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fde2f-445">HTTP</span><span class="sxs-lookup"><span data-stu-id="fde2f-445">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post_6"
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
# <a name="c"></a>[<span data-ttu-id="fde2f-446">C#</span><span class="sxs-lookup"><span data-stu-id="fde2f-446">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-6-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fde2f-447">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fde2f-447">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-6-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fde2f-448">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fde2f-448">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-6-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fde2f-449">Java</span><span class="sxs-lookup"><span data-stu-id="fde2f-449">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-6-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fde2f-450">Отклик</span><span class="sxs-lookup"><span data-stu-id="fde2f-450">Response</span></span>

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


