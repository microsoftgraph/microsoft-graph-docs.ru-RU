---
title: Создание governanceRoleAssignmentRequest
description: Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли. В приведенной ниже таблице перечислены операции.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 76829c502e83b4218241df74d9fc51e43c0eeb86
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965468"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="8bef1-104">Создание governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="8bef1-104">Create governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="8bef1-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bef1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bef1-106">Создайте запрос на назначение роли, который будет представлять нужную операцию для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="8bef1-106">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="8bef1-107">В приведенной ниже таблице перечислены операции.</span><span class="sxs-lookup"><span data-stu-id="8bef1-107">The following table lists the operations.</span></span>

| <span data-ttu-id="8bef1-108">Операция</span><span class="sxs-lookup"><span data-stu-id="8bef1-108">Operation</span></span>                                   | <span data-ttu-id="8bef1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8bef1-109">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="8bef1-110">Назначение роли</span><span class="sxs-lookup"><span data-stu-id="8bef1-110">Assign a role assignment</span></span>                    | <span data-ttu-id="8bef1-111">админадд</span><span class="sxs-lookup"><span data-stu-id="8bef1-111">AdminAdd</span></span>    |
| <span data-ttu-id="8bef1-112">Активация подходящего назначения роли</span><span class="sxs-lookup"><span data-stu-id="8bef1-112">Activate an eligible role assignment</span></span>        | <span data-ttu-id="8bef1-113">усерадд</span><span class="sxs-lookup"><span data-stu-id="8bef1-113">UserAdd</span></span>     |
| <span data-ttu-id="8bef1-114">Деактивация активированного назначения роли</span><span class="sxs-lookup"><span data-stu-id="8bef1-114">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="8bef1-115">усерремове</span><span class="sxs-lookup"><span data-stu-id="8bef1-115">UserRemove</span></span>  |
| <span data-ttu-id="8bef1-116">Удаление назначения роли</span><span class="sxs-lookup"><span data-stu-id="8bef1-116">Remove a role assignment</span></span>                    | <span data-ttu-id="8bef1-117">админремове</span><span class="sxs-lookup"><span data-stu-id="8bef1-117">AdminRemove</span></span> |
| <span data-ttu-id="8bef1-118">Обновление назначения роли</span><span class="sxs-lookup"><span data-stu-id="8bef1-118">Update a role assignment</span></span>                    | <span data-ttu-id="8bef1-119">админупдате</span><span class="sxs-lookup"><span data-stu-id="8bef1-119">AdminUpdate</span></span> |
| <span data-ttu-id="8bef1-120">Запрос на расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="8bef1-120">Request to extend my role assignment</span></span>        | <span data-ttu-id="8bef1-121">усерекстенд</span><span class="sxs-lookup"><span data-stu-id="8bef1-121">UserExtend</span></span>  |
| <span data-ttu-id="8bef1-122">Расширение назначения роли</span><span class="sxs-lookup"><span data-stu-id="8bef1-122">Extend a role assignment</span></span>                    | <span data-ttu-id="8bef1-123">админекстенд</span><span class="sxs-lookup"><span data-stu-id="8bef1-123">AdminExtend</span></span> |
| <span data-ttu-id="8bef1-124">Запрос на продление назначения роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="8bef1-124">Request to renew my expired role assignment</span></span> | <span data-ttu-id="8bef1-125">усерренев</span><span class="sxs-lookup"><span data-stu-id="8bef1-125">UserRenew</span></span>   |
| <span data-ttu-id="8bef1-126">Продление назначенной роли с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="8bef1-126">Renew an expired role assignment</span></span>            | <span data-ttu-id="8bef1-127">админренев</span><span class="sxs-lookup"><span data-stu-id="8bef1-127">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="8bef1-128">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8bef1-128">Permissions</span></span>

<span data-ttu-id="8bef1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="8bef1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="8bef1-131">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="8bef1-131">Azure resources</span></span>

| <span data-ttu-id="8bef1-132">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8bef1-132">Permission type</span></span> | <span data-ttu-id="8bef1-133">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8bef1-133">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="8bef1-134">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8bef1-134">Delegated (work or school account)</span></span> | <span data-ttu-id="8bef1-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="8bef1-135">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="8bef1-136">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8bef1-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bef1-137">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bef1-137">Not supported.</span></span> |
| <span data-ttu-id="8bef1-138">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8bef1-138">Application</span></span> | <span data-ttu-id="8bef1-139">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bef1-139">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="8bef1-140">Azure AD</span><span class="sxs-lookup"><span data-stu-id="8bef1-140">Azure AD</span></span>

| <span data-ttu-id="8bef1-141">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8bef1-141">Permission type</span></span> | <span data-ttu-id="8bef1-142">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8bef1-142">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="8bef1-143">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8bef1-143">Delegated (work or school account)</span></span> | <span data-ttu-id="8bef1-144">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="8bef1-144">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="8bef1-145">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8bef1-145">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bef1-146">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bef1-146">Not supported.</span></span> |
| <span data-ttu-id="8bef1-147">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8bef1-147">Application</span></span> | <span data-ttu-id="8bef1-148">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bef1-148">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="8bef1-149">Группы</span><span class="sxs-lookup"><span data-stu-id="8bef1-149">Groups</span></span>

|<span data-ttu-id="8bef1-150">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8bef1-150">Permission type</span></span> | <span data-ttu-id="8bef1-151">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8bef1-151">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="8bef1-152">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8bef1-152">Delegated (work or school account)</span></span> | <span data-ttu-id="8bef1-153">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="8bef1-153">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="8bef1-154">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8bef1-154">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bef1-155">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bef1-155">Not supported.</span></span> |
| <span data-ttu-id="8bef1-156">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8bef1-156">Application</span></span> | <span data-ttu-id="8bef1-157">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bef1-157">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bef1-158">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8bef1-158">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="8bef1-159">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8bef1-159">Request headers</span></span>

| <span data-ttu-id="8bef1-160">Имя</span><span class="sxs-lookup"><span data-stu-id="8bef1-160">Name</span></span>          | <span data-ttu-id="8bef1-161">Описание</span><span class="sxs-lookup"><span data-stu-id="8bef1-161">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="8bef1-162">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8bef1-162">Authorization</span></span> | <span data-ttu-id="8bef1-163">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8bef1-163">Bearer {code}</span></span>    |
| <span data-ttu-id="8bef1-164">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8bef1-164">Content-type</span></span>  | <span data-ttu-id="8bef1-165">application/json</span><span class="sxs-lookup"><span data-stu-id="8bef1-165">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8bef1-166">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8bef1-166">Request body</span></span>

<span data-ttu-id="8bef1-167">В тексте запроса добавьте представление объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8bef1-167">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="8bef1-168">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bef1-168">Property</span></span>         | <span data-ttu-id="8bef1-169">Тип</span><span class="sxs-lookup"><span data-stu-id="8bef1-169">Type</span></span>                                                     | <span data-ttu-id="8bef1-170">Описание</span><span class="sxs-lookup"><span data-stu-id="8bef1-170">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="8bef1-171">resourceId</span><span class="sxs-lookup"><span data-stu-id="8bef1-171">resourceId</span></span>       | <span data-ttu-id="8bef1-172">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-172">String</span></span>                                                   | <span data-ttu-id="8bef1-173">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="8bef1-173">The ID of the resource.</span></span> <span data-ttu-id="8bef1-174">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bef1-174">Required.</span></span> |
| <span data-ttu-id="8bef1-175">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="8bef1-175">roleDefinitionId</span></span> | <span data-ttu-id="8bef1-176">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-176">String</span></span>                                                   | <span data-ttu-id="8bef1-177">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="8bef1-177">The ID of the role definition.</span></span> <span data-ttu-id="8bef1-178">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bef1-178">Required.</span></span> |
| <span data-ttu-id="8bef1-179">субжектид</span><span class="sxs-lookup"><span data-stu-id="8bef1-179">subjectId</span></span>        | <span data-ttu-id="8bef1-180">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-180">String</span></span>                                                   | <span data-ttu-id="8bef1-181">ИДЕНТИФИКАТОР субъекта.</span><span class="sxs-lookup"><span data-stu-id="8bef1-181">The ID of the subject.</span></span> <span data-ttu-id="8bef1-182">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bef1-182">Required.</span></span> |
| <span data-ttu-id="8bef1-183">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="8bef1-183">assignmentState</span></span>  | <span data-ttu-id="8bef1-184">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-184">String</span></span>                                                   | <span data-ttu-id="8bef1-185">Состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="8bef1-185">The state of assignment.</span></span> <span data-ttu-id="8bef1-186">Значение может быть `Eligible` и `Active` .</span><span class="sxs-lookup"><span data-stu-id="8bef1-186">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="8bef1-187">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="8bef1-187">Required.</span></span> |
| <span data-ttu-id="8bef1-188">type</span><span class="sxs-lookup"><span data-stu-id="8bef1-188">type</span></span>             | <span data-ttu-id="8bef1-189">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-189">String</span></span>                                                   | <span data-ttu-id="8bef1-190">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="8bef1-190">The request type.</span></span> <span data-ttu-id="8bef1-191">Возможные значения:,,,,,, `AdminAdd` `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `UserRenew` `AdminRenew` и `AdminExtend` .</span><span class="sxs-lookup"><span data-stu-id="8bef1-191">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="8bef1-192">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bef1-192">Required.</span></span> |
| <span data-ttu-id="8bef1-193">reason</span><span class="sxs-lookup"><span data-stu-id="8bef1-193">reason</span></span>           | <span data-ttu-id="8bef1-194">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-194">String</span></span>                                                   | <span data-ttu-id="8bef1-195">Необходимо указать причину для запроса на назначение роли для аудита и проверки.</span><span class="sxs-lookup"><span data-stu-id="8bef1-195">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="8bef1-196">schedule</span><span class="sxs-lookup"><span data-stu-id="8bef1-196">schedule</span></span>         | [<span data-ttu-id="8bef1-197">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8bef1-197">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="8bef1-198">Расписание запроса на назначение роли.</span><span class="sxs-lookup"><span data-stu-id="8bef1-198">The schedule of the role assignment request.</span></span> <span data-ttu-id="8bef1-199">Для типа запроса `UserAdd` ,, `AdminAdd` `AdminUpdate` , и `AdminExtend` , он необходим.</span><span class="sxs-lookup"><span data-stu-id="8bef1-199">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="8bef1-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bef1-200">Response</span></span>

<span data-ttu-id="8bef1-201">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8bef1-201">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="8bef1-202">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="8bef1-202">Error codes</span></span>

<span data-ttu-id="8bef1-203">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="8bef1-203">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="8bef1-204">Кроме того, он возвращает коды ошибок, приведенные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="8bef1-204">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="8bef1-205">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="8bef1-205">Error code</span></span>     | <span data-ttu-id="8bef1-206">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="8bef1-206">Error message</span></span>                               | <span data-ttu-id="8bef1-207">Сведения</span><span class="sxs-lookup"><span data-stu-id="8bef1-207">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="8bef1-208">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="8bef1-208">400 BadRequest</span></span> | <span data-ttu-id="8bef1-209">роленотфаунд</span><span class="sxs-lookup"><span data-stu-id="8bef1-209">RoleNotFound</span></span>                                | <span data-ttu-id="8bef1-210">`roleDefinitionId`Не удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="8bef1-210">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="8bef1-211">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="8bef1-211">400 BadRequest</span></span> | <span data-ttu-id="8bef1-212">ресаурцеислоккед</span><span class="sxs-lookup"><span data-stu-id="8bef1-212">ResourceIsLocked</span></span>                            | <span data-ttu-id="8bef1-213">Ресурс, указанный в теле запроса, находится в состоянии `Locked` и не может создавать запросы на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="8bef1-213">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="8bef1-214">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="8bef1-214">400 BadRequest</span></span> | <span data-ttu-id="8bef1-215">субжектнотфаунд</span><span class="sxs-lookup"><span data-stu-id="8bef1-215">SubjectNotFound</span></span>                             | <span data-ttu-id="8bef1-216">`subjectId`Не удается найти указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="8bef1-216">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="8bef1-217">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="8bef1-217">400 BadRequest</span></span> | <span data-ttu-id="8bef1-218">пендингролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="8bef1-218">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="8bef1-219">В системе уже существует ожидающий [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="8bef1-219">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="8bef1-220">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="8bef1-220">400 BadRequest</span></span> | <span data-ttu-id="8bef1-221">ролеассигнментексистс</span><span class="sxs-lookup"><span data-stu-id="8bef1-221">RoleAssignmentExists</span></span>                        | <span data-ttu-id="8bef1-222">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , который требуется создать, уже существует в системе.</span><span class="sxs-lookup"><span data-stu-id="8bef1-222">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="8bef1-223">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="8bef1-223">400 BadRequest</span></span> | <span data-ttu-id="8bef1-224">ролеассигнментдоеснотексист</span><span class="sxs-lookup"><span data-stu-id="8bef1-224">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="8bef1-225">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) , запрошенный для обновления или расширения, не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="8bef1-225">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="8bef1-226">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="8bef1-226">400 BadRequest</span></span> | <span data-ttu-id="8bef1-227">ролеассигнментрекуестполицивалидатионфаилед</span><span class="sxs-lookup"><span data-stu-id="8bef1-227">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="8bef1-228">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) не отвечает внутренним политикам и не может быть создан.</span><span class="sxs-lookup"><span data-stu-id="8bef1-228">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="8bef1-229">Примеры</span><span class="sxs-lookup"><span data-stu-id="8bef1-229">Examples</span></span>

<span data-ttu-id="8bef1-230">В следующих примерах показано, как использовать этот API.</span><span class="sxs-lookup"><span data-stu-id="8bef1-230">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="8bef1-231">Пример 1: Администратор назначает пользователю роль</span><span class="sxs-lookup"><span data-stu-id="8bef1-231">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="8bef1-232">В этом примере администратор назначает пользователю nawu@fimdev.net роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="8bef1-232">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="8bef1-233">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней мере одно `Active` назначение роли администратора ( `owner` или `user access administrator` ) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="8bef1-233">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="8bef1-234">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bef1-234">Property</span></span>         | <span data-ttu-id="8bef1-235">Тип</span><span class="sxs-lookup"><span data-stu-id="8bef1-235">Type</span></span>                                                     | <span data-ttu-id="8bef1-236">Обязательный</span><span class="sxs-lookup"><span data-stu-id="8bef1-236">Required</span></span>                 | <span data-ttu-id="8bef1-237">Значение</span><span class="sxs-lookup"><span data-stu-id="8bef1-237">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="8bef1-238">resourceId</span><span class="sxs-lookup"><span data-stu-id="8bef1-238">resourceId</span></span>       | <span data-ttu-id="8bef1-239">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-239">String</span></span>                                                   | <span data-ttu-id="8bef1-240">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-240">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="8bef1-241">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="8bef1-241">roleDefinitionId</span></span> | <span data-ttu-id="8bef1-242">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-242">String</span></span>                                                   | <span data-ttu-id="8bef1-243">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-243">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="8bef1-244">субжектид</span><span class="sxs-lookup"><span data-stu-id="8bef1-244">subjectId</span></span>        | <span data-ttu-id="8bef1-245">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-245">String</span></span>                                                   | <span data-ttu-id="8bef1-246">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-246">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="8bef1-247">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="8bef1-247">assignmentState</span></span>  | <span data-ttu-id="8bef1-248">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-248">String</span></span>                                                   | <span data-ttu-id="8bef1-249">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-249">Yes</span></span>                      | <span data-ttu-id="8bef1-250">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="8bef1-250">Eligible / Active</span></span> |
| <span data-ttu-id="8bef1-251">type</span><span class="sxs-lookup"><span data-stu-id="8bef1-251">type</span></span>             | <span data-ttu-id="8bef1-252">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-252">String</span></span>                                                   | <span data-ttu-id="8bef1-253">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-253">Yes</span></span>                      | <span data-ttu-id="8bef1-254">админадд</span><span class="sxs-lookup"><span data-stu-id="8bef1-254">AdminAdd</span></span> |
| <span data-ttu-id="8bef1-255">reason</span><span class="sxs-lookup"><span data-stu-id="8bef1-255">reason</span></span>           | <span data-ttu-id="8bef1-256">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-256">String</span></span>                                                   | <span data-ttu-id="8bef1-257">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="8bef1-257">depends on role Settings</span></span> |   |
| <span data-ttu-id="8bef1-258">schedule</span><span class="sxs-lookup"><span data-stu-id="8bef1-258">schedule</span></span>         | [<span data-ttu-id="8bef1-259">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8bef1-259">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="8bef1-260">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-260">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="8bef1-261">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bef1-261">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8bef1-262">HTTP</span><span class="sxs-lookup"><span data-stu-id="8bef1-262">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8bef1-263">C#</span><span class="sxs-lookup"><span data-stu-id="8bef1-263">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8bef1-264">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8bef1-264">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8bef1-265">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8bef1-265">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8bef1-266">Java</span><span class="sxs-lookup"><span data-stu-id="8bef1-266">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="8bef1-267">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bef1-267">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="8bef1-268">Пример 2: пользователь активирует подходящие роли</span><span class="sxs-lookup"><span data-stu-id="8bef1-268">Example 2: User activates eligible role</span></span>

<span data-ttu-id="8bef1-269">В этом примере пользователь nawu@fimdev.net активирует соответствующую роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="8bef1-269">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="8bef1-270">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bef1-270">Property</span></span>         | <span data-ttu-id="8bef1-271">Тип</span><span class="sxs-lookup"><span data-stu-id="8bef1-271">Type</span></span>                                                     | <span data-ttu-id="8bef1-272">Обязательный</span><span class="sxs-lookup"><span data-stu-id="8bef1-272">Required</span></span>                 | <span data-ttu-id="8bef1-273">Значение</span><span class="sxs-lookup"><span data-stu-id="8bef1-273">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="8bef1-274">resourceId</span><span class="sxs-lookup"><span data-stu-id="8bef1-274">resourceId</span></span>       | <span data-ttu-id="8bef1-275">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-275">String</span></span>                                                   | <span data-ttu-id="8bef1-276">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-276">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="8bef1-277">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="8bef1-277">roleDefinitionId</span></span> | <span data-ttu-id="8bef1-278">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-278">String</span></span>                                                   | <span data-ttu-id="8bef1-279">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-279">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="8bef1-280">субжектид</span><span class="sxs-lookup"><span data-stu-id="8bef1-280">subjectId</span></span>        | <span data-ttu-id="8bef1-281">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-281">String</span></span>                                                   | <span data-ttu-id="8bef1-282">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-282">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="8bef1-283">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="8bef1-283">assignmentState</span></span>  | <span data-ttu-id="8bef1-284">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-284">String</span></span>                                                   | <span data-ttu-id="8bef1-285">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-285">Yes</span></span>                      | <span data-ttu-id="8bef1-286">Активное</span><span class="sxs-lookup"><span data-stu-id="8bef1-286">Active</span></span> |
| <span data-ttu-id="8bef1-287">type</span><span class="sxs-lookup"><span data-stu-id="8bef1-287">type</span></span>             | <span data-ttu-id="8bef1-288">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-288">String</span></span>                                                   | <span data-ttu-id="8bef1-289">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-289">Yes</span></span>                      | <span data-ttu-id="8bef1-290">усерадд</span><span class="sxs-lookup"><span data-stu-id="8bef1-290">UserAdd</span></span> |
| <span data-ttu-id="8bef1-291">reason</span><span class="sxs-lookup"><span data-stu-id="8bef1-291">reason</span></span>           | <span data-ttu-id="8bef1-292">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-292">String</span></span>                                                   | <span data-ttu-id="8bef1-293">зависит от параметров роли</span><span class="sxs-lookup"><span data-stu-id="8bef1-293">depends on role Settings</span></span> |   |
| <span data-ttu-id="8bef1-294">schedule</span><span class="sxs-lookup"><span data-stu-id="8bef1-294">schedule</span></span>         | [<span data-ttu-id="8bef1-295">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8bef1-295">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="8bef1-296">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-296">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="8bef1-297">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bef1-297">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="8bef1-298">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bef1-298">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="8bef1-299">Пример 3: пользователь отключает назначенную роль</span><span class="sxs-lookup"><span data-stu-id="8bef1-299">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="8bef1-300">В этом примере пользователь nawu@fimdev.net отключает активную роль читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="8bef1-300">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="8bef1-301">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bef1-301">Property</span></span>         | <span data-ttu-id="8bef1-302">Тип</span><span class="sxs-lookup"><span data-stu-id="8bef1-302">Type</span></span>                                                     | <span data-ttu-id="8bef1-303">Обязательный</span><span class="sxs-lookup"><span data-stu-id="8bef1-303">Required</span></span> | <span data-ttu-id="8bef1-304">Значение</span><span class="sxs-lookup"><span data-stu-id="8bef1-304">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="8bef1-305">resourceId</span><span class="sxs-lookup"><span data-stu-id="8bef1-305">resourceId</span></span>       | <span data-ttu-id="8bef1-306">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-306">String</span></span>                                                   | <span data-ttu-id="8bef1-307">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-307">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="8bef1-308">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="8bef1-308">roleDefinitionId</span></span> | <span data-ttu-id="8bef1-309">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-309">String</span></span>                                                   | <span data-ttu-id="8bef1-310">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-310">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="8bef1-311">субжектид</span><span class="sxs-lookup"><span data-stu-id="8bef1-311">subjectId</span></span>        | <span data-ttu-id="8bef1-312">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-312">String</span></span>                                                   | <span data-ttu-id="8bef1-313">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-313">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="8bef1-314">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="8bef1-314">assignmentState</span></span>  | <span data-ttu-id="8bef1-315">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-315">String</span></span>                                                   | <span data-ttu-id="8bef1-316">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-316">Yes</span></span>      | <span data-ttu-id="8bef1-317">Активное</span><span class="sxs-lookup"><span data-stu-id="8bef1-317">Active</span></span> |
| <span data-ttu-id="8bef1-318">type</span><span class="sxs-lookup"><span data-stu-id="8bef1-318">type</span></span>             | <span data-ttu-id="8bef1-319">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-319">String</span></span>                                                   | <span data-ttu-id="8bef1-320">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-320">Yes</span></span>      | <span data-ttu-id="8bef1-321">усерремове</span><span class="sxs-lookup"><span data-stu-id="8bef1-321">UserRemove</span></span> |
| <span data-ttu-id="8bef1-322">reason</span><span class="sxs-lookup"><span data-stu-id="8bef1-322">reason</span></span>           | <span data-ttu-id="8bef1-323">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-323">String</span></span>                                                   | <span data-ttu-id="8bef1-324">Нет</span><span class="sxs-lookup"><span data-stu-id="8bef1-324">No</span></span>       |   |
| <span data-ttu-id="8bef1-325">schedule</span><span class="sxs-lookup"><span data-stu-id="8bef1-325">schedule</span></span>         | [<span data-ttu-id="8bef1-326">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8bef1-326">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="8bef1-327">Нет</span><span class="sxs-lookup"><span data-stu-id="8bef1-327">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="8bef1-328">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bef1-328">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="8bef1-329">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bef1-329">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="8bef1-330">Пример 4: Администратор удаляет пользователя из роли</span><span class="sxs-lookup"><span data-stu-id="8bef1-330">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="8bef1-331">В этом примере администратор удаляет пользователя nawu@fimdev.net из роли читателя выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="8bef1-331">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="8bef1-332">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней мере одно `Active` назначение роли администратора ( `owner` или `user access administrator` ) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="8bef1-332">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="8bef1-333">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bef1-333">Property</span></span>         | <span data-ttu-id="8bef1-334">Тип</span><span class="sxs-lookup"><span data-stu-id="8bef1-334">Type</span></span>                                                     | <span data-ttu-id="8bef1-335">Обязательный</span><span class="sxs-lookup"><span data-stu-id="8bef1-335">Required</span></span> | <span data-ttu-id="8bef1-336">Значение</span><span class="sxs-lookup"><span data-stu-id="8bef1-336">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="8bef1-337">resourceId</span><span class="sxs-lookup"><span data-stu-id="8bef1-337">resourceId</span></span>       | <span data-ttu-id="8bef1-338">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-338">String</span></span>                                                   | <span data-ttu-id="8bef1-339">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-339">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="8bef1-340">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="8bef1-340">roleDefinitionId</span></span> | <span data-ttu-id="8bef1-341">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-341">String</span></span>                                                   | <span data-ttu-id="8bef1-342">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-342">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="8bef1-343">субжектид</span><span class="sxs-lookup"><span data-stu-id="8bef1-343">subjectId</span></span>        | <span data-ttu-id="8bef1-344">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-344">String</span></span>                                                   | <span data-ttu-id="8bef1-345">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-345">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="8bef1-346">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="8bef1-346">assignmentState</span></span>  | <span data-ttu-id="8bef1-347">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-347">String</span></span>                                                   | <span data-ttu-id="8bef1-348">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-348">Yes</span></span>      | <span data-ttu-id="8bef1-349">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="8bef1-349">Eligible / Active</span></span> |
| <span data-ttu-id="8bef1-350">type</span><span class="sxs-lookup"><span data-stu-id="8bef1-350">type</span></span>             | <span data-ttu-id="8bef1-351">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-351">String</span></span>                                                   | <span data-ttu-id="8bef1-352">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-352">Yes</span></span>      | <span data-ttu-id="8bef1-353">админремове</span><span class="sxs-lookup"><span data-stu-id="8bef1-353">AdminRemove</span></span> |
| <span data-ttu-id="8bef1-354">reason</span><span class="sxs-lookup"><span data-stu-id="8bef1-354">reason</span></span>           | <span data-ttu-id="8bef1-355">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-355">String</span></span>                                                   | <span data-ttu-id="8bef1-356">Нет</span><span class="sxs-lookup"><span data-stu-id="8bef1-356">No</span></span>       |   |
| <span data-ttu-id="8bef1-357">schedule</span><span class="sxs-lookup"><span data-stu-id="8bef1-357">schedule</span></span>         | [<span data-ttu-id="8bef1-358">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8bef1-358">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="8bef1-359">Нет</span><span class="sxs-lookup"><span data-stu-id="8bef1-359">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="8bef1-360">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bef1-360">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="8bef1-361">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bef1-361">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="8bef1-362">Пример 5: "Администратор обновляет назначение ролей"</span><span class="sxs-lookup"><span data-stu-id="8bef1-362">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="8bef1-363">В этом примере администраторы обновляют назначение роли пользователя nawu@fimdev.net владельцу.</span><span class="sxs-lookup"><span data-stu-id="8bef1-363">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="8bef1-364">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней мере одно `Active` назначение роли администратора ( `owner` или `user access administrator` ) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="8bef1-364">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="8bef1-365">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bef1-365">Property</span></span>         | <span data-ttu-id="8bef1-366">Тип</span><span class="sxs-lookup"><span data-stu-id="8bef1-366">Type</span></span>                                                     | <span data-ttu-id="8bef1-367">Обязательный</span><span class="sxs-lookup"><span data-stu-id="8bef1-367">Required</span></span>                | <span data-ttu-id="8bef1-368">Значение</span><span class="sxs-lookup"><span data-stu-id="8bef1-368">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="8bef1-369">resourceId</span><span class="sxs-lookup"><span data-stu-id="8bef1-369">resourceId</span></span>       | <span data-ttu-id="8bef1-370">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-370">String</span></span>                                                   | <span data-ttu-id="8bef1-371">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-371">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="8bef1-372">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="8bef1-372">roleDefinitionId</span></span> | <span data-ttu-id="8bef1-373">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-373">String</span></span>                                                   | <span data-ttu-id="8bef1-374">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-374">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="8bef1-375">субжектид</span><span class="sxs-lookup"><span data-stu-id="8bef1-375">subjectId</span></span>        | <span data-ttu-id="8bef1-376">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-376">String</span></span>                                                   | <span data-ttu-id="8bef1-377">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-377">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="8bef1-378">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="8bef1-378">assignmentState</span></span>  | <span data-ttu-id="8bef1-379">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-379">String</span></span>                                                   | <span data-ttu-id="8bef1-380">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-380">Yes</span></span>                     | <span data-ttu-id="8bef1-381">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="8bef1-381">Eligible / Active</span></span> |
| <span data-ttu-id="8bef1-382">type</span><span class="sxs-lookup"><span data-stu-id="8bef1-382">type</span></span>             | <span data-ttu-id="8bef1-383">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-383">String</span></span>                                                   | <span data-ttu-id="8bef1-384">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-384">Yes</span></span>                     | <span data-ttu-id="8bef1-385">админупдате</span><span class="sxs-lookup"><span data-stu-id="8bef1-385">AdminUpdate</span></span> |
| <span data-ttu-id="8bef1-386">reason</span><span class="sxs-lookup"><span data-stu-id="8bef1-386">reason</span></span>           | <span data-ttu-id="8bef1-387">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-387">String</span></span>                                                   | <span data-ttu-id="8bef1-388">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="8bef1-388">depends on roleSettings</span></span> |   |
| <span data-ttu-id="8bef1-389">schedule</span><span class="sxs-lookup"><span data-stu-id="8bef1-389">schedule</span></span>         | [<span data-ttu-id="8bef1-390">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8bef1-390">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="8bef1-391">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-391">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="8bef1-392">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bef1-392">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="8bef1-393">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bef1-393">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="8bef1-394">Пример 6: администратор расширяет назначение ролей с истекшим сроком действия</span><span class="sxs-lookup"><span data-stu-id="8bef1-394">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="8bef1-395">В этом примере показано, как расширить назначение роли истечения срока действия для пользователя АНУЖКУСЕР участнику службы управления API.</span><span class="sxs-lookup"><span data-stu-id="8bef1-395">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="8bef1-396">**Примечание:** Кроме разрешения, в этом примере необходимо, чтобы у автора запроса было по крайней мере одно `Active` назначение роли администратора ( `owner` или `user access administrator` ) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="8bef1-396">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="8bef1-397">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bef1-397">Property</span></span>         | <span data-ttu-id="8bef1-398">Тип</span><span class="sxs-lookup"><span data-stu-id="8bef1-398">Type</span></span>                                                     | <span data-ttu-id="8bef1-399">Обязательный</span><span class="sxs-lookup"><span data-stu-id="8bef1-399">Required</span></span>                | <span data-ttu-id="8bef1-400">Значение</span><span class="sxs-lookup"><span data-stu-id="8bef1-400">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="8bef1-401">resourceId</span><span class="sxs-lookup"><span data-stu-id="8bef1-401">resourceId</span></span>       | <span data-ttu-id="8bef1-402">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-402">String</span></span>                                                   | <span data-ttu-id="8bef1-403">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-403">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="8bef1-404">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="8bef1-404">roleDefinitionId</span></span> | <span data-ttu-id="8bef1-405">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-405">String</span></span>                                                   | <span data-ttu-id="8bef1-406">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-406">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="8bef1-407">субжектид</span><span class="sxs-lookup"><span data-stu-id="8bef1-407">subjectId</span></span>        | <span data-ttu-id="8bef1-408">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-408">String</span></span>                                                   | <span data-ttu-id="8bef1-409">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-409">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="8bef1-410">ассигнментстате</span><span class="sxs-lookup"><span data-stu-id="8bef1-410">assignmentState</span></span>  | <span data-ttu-id="8bef1-411">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-411">String</span></span>                                                   | <span data-ttu-id="8bef1-412">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-412">Yes</span></span>                     | <span data-ttu-id="8bef1-413">Подходящие/активные</span><span class="sxs-lookup"><span data-stu-id="8bef1-413">Eligible / Active</span></span> |
| <span data-ttu-id="8bef1-414">type</span><span class="sxs-lookup"><span data-stu-id="8bef1-414">type</span></span>             | <span data-ttu-id="8bef1-415">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-415">String</span></span>                                                   | <span data-ttu-id="8bef1-416">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-416">Yes</span></span>                     | <span data-ttu-id="8bef1-417">админекстенд</span><span class="sxs-lookup"><span data-stu-id="8bef1-417">AdminExtend</span></span> |
| <span data-ttu-id="8bef1-418">reason</span><span class="sxs-lookup"><span data-stu-id="8bef1-418">reason</span></span>           | <span data-ttu-id="8bef1-419">String</span><span class="sxs-lookup"><span data-stu-id="8bef1-419">String</span></span>                                                   | <span data-ttu-id="8bef1-420">зависит от Ролесеттингс</span><span class="sxs-lookup"><span data-stu-id="8bef1-420">depends on roleSettings</span></span> |   |
| <span data-ttu-id="8bef1-421">schedule</span><span class="sxs-lookup"><span data-stu-id="8bef1-421">schedule</span></span>         | [<span data-ttu-id="8bef1-422">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8bef1-422">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="8bef1-423">Да</span><span class="sxs-lookup"><span data-stu-id="8bef1-423">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="8bef1-424">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bef1-424">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="8bef1-425">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bef1-425">Response</span></span>

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


