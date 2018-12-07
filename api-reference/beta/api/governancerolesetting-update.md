---
title: Обновление governanceRoleSetting
description: Обновление свойств governanceRoleSetting.
ms.openlocfilehash: 2d9417c99e63b1b4c7302c2afdda4c272b2fce82
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191118"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="549d1-103">Обновление governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="549d1-103">Update governanceRoleSetting</span></span>

> <span data-ttu-id="549d1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="549d1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="549d1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="549d1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="549d1-106">Обновление свойств [governanceRoleSetting](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="549d1-106">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="549d1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="549d1-107">Permissions</span></span>
<span data-ttu-id="549d1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="549d1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="549d1-110">**Примечание:** Этот интерфейс API также требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="549d1-110">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="549d1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="549d1-111">Permission type</span></span>      | <span data-ttu-id="549d1-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="549d1-112">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="549d1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="549d1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="549d1-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="549d1-114">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="549d1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="549d1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="549d1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="549d1-116">Not supported.</span></span>    |
|<span data-ttu-id="549d1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="549d1-117">Application</span></span> | <span data-ttu-id="549d1-118">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="549d1-118">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="549d1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="549d1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="549d1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="549d1-120">Request headers</span></span>
| <span data-ttu-id="549d1-121">Имя</span><span class="sxs-lookup"><span data-stu-id="549d1-121">Name</span></span>       | <span data-ttu-id="549d1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="549d1-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="549d1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="549d1-123">Authorization</span></span>  | <span data-ttu-id="549d1-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="549d1-124">Bearer {code}</span></span>|
| <span data-ttu-id="549d1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="549d1-125">Content-type</span></span>  | <span data-ttu-id="549d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="549d1-126">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="549d1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="549d1-127">Request body</span></span>
<span data-ttu-id="549d1-128">В тексте запроса задаете значения параметра [governanceRuleSettings](../resources/governancerulesetting.md) , который требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="549d1-128">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="549d1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="549d1-129">Property</span></span>     | <span data-ttu-id="549d1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="549d1-130">Type</span></span>   |<span data-ttu-id="549d1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="549d1-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="549d1-132">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="549d1-132">adminEligibleSettings</span></span>|[<span data-ttu-id="549d1-133">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="549d1-133">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="549d1-134">Параметры правил, которые вычисляются, когда администратор пытается добавить назначение подходящими роли.</span><span class="sxs-lookup"><span data-stu-id="549d1-134">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="549d1-135">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="549d1-135">adminMemberSettings</span></span>|[<span data-ttu-id="549d1-136">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="549d1-136">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="549d1-137">Параметры правил, которые вычисляются, когда администратор пытается добавить членами назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="549d1-137">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="549d1-138">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="549d1-138">userEligibleSettings</span></span>|[<span data-ttu-id="549d1-139">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="549d1-139">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="549d1-140">Параметры правил, которые вычисляются, когда пользователь пытается добавить назначение подходящими роли.</span><span class="sxs-lookup"><span data-stu-id="549d1-140">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="549d1-141">Это действие не поддерживается для `pimforazurerbac` сценарий в данный момент и может быть доступно в последующих сценариях.</span><span class="sxs-lookup"><span data-stu-id="549d1-141">This is not supported for `pimforazurerbac` scenario for now, and may be available in the future scenarios.</span></span>|
|<span data-ttu-id="549d1-142">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="549d1-142">userMemberSettings</span></span>|[<span data-ttu-id="549d1-143">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="549d1-143">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="549d1-144">Параметры правил, которые вычисляются при попытке активировать его назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="549d1-144">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="549d1-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="549d1-145">Response</span></span>
<span data-ttu-id="549d1-p104">При успешном выполнении этот метод возвращает код отклика `204 NoContent`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="549d1-p104">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="549d1-148">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="549d1-148">Error codes</span></span>
<span data-ttu-id="549d1-149">Этот интерфейс API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="549d1-149">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="549d1-150">Кроме того он возвращает следующие коды ошибок.</span><span class="sxs-lookup"><span data-stu-id="549d1-150">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="549d1-151">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="549d1-151">Error code</span></span>     | <span data-ttu-id="549d1-152">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="549d1-152">Error message</span></span>         | <span data-ttu-id="549d1-153">Сведения</span><span class="sxs-lookup"><span data-stu-id="549d1-153">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="549d1-154">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="549d1-154">400 BadRequest</span></span>| <span data-ttu-id="549d1-155">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="549d1-155">RoleSettingNotFound</span></span>   | <span data-ttu-id="549d1-156">[GovernanceRoleSetting](../resources/governancerolesetting.md) не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="549d1-156">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="549d1-157">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="549d1-157">400 BadRequest</span></span>| <span data-ttu-id="549d1-158">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="549d1-158">InvalidRoleSetting</span></span>    | <span data-ttu-id="549d1-159">Недопустимые значения [governanceRuleSettings](../resources/governancerulesetting.md) , предоставляемые в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="549d1-159">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="549d1-160">Пример</span><span class="sxs-lookup"><span data-stu-id="549d1-160">Example</span></span> 
<span data-ttu-id="549d1-161">В этом примере обновляется параметр роли для настраиваемых ролей 3 в Wingtip Toys - производственного подписки.</span><span class="sxs-lookup"><span data-stu-id="549d1-161">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="549d1-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="549d1-162">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_governancerolesetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedAccess/pimforazurerbac/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5
Content-type: application/json
Content-length: 350

{
  "adminEligibleSettings":[{"ruleIdentifier":"ExpirationRule","setting":"{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"}]
}
```
##### <a name="response"></a><span data-ttu-id="549d1-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="549d1-163">Response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
