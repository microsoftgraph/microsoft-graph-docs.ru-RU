---
title: Обновление governanceRoleSetting
description: Обновление свойств governanceRoleSetting.
localization_priority: Normal
ms.openlocfilehash: e76d7955576d9d514a70b52b31f4d034362aac1f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874909"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="563af-103">Обновление governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="563af-103">Update governanceRoleSetting</span></span>

> <span data-ttu-id="563af-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="563af-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="563af-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="563af-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="563af-106">Обновление свойств [governanceRoleSetting](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="563af-106">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="563af-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="563af-107">Permissions</span></span>
<span data-ttu-id="563af-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="563af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="563af-110">**Примечание:** Этот интерфейс API также требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="563af-110">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="563af-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="563af-111">Permission type</span></span>      | <span data-ttu-id="563af-112">Permissions</span><span class="sxs-lookup"><span data-stu-id="563af-112">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="563af-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="563af-113">Delegated (work or school account)</span></span> | <span data-ttu-id="563af-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="563af-114">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="563af-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="563af-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="563af-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="563af-116">Not supported.</span></span>    |
|<span data-ttu-id="563af-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="563af-117">Application</span></span> | <span data-ttu-id="563af-118">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="563af-118">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="563af-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="563af-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="563af-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="563af-120">Request headers</span></span>
| <span data-ttu-id="563af-121">Имя</span><span class="sxs-lookup"><span data-stu-id="563af-121">Name</span></span>       | <span data-ttu-id="563af-122">Описание</span><span class="sxs-lookup"><span data-stu-id="563af-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="563af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="563af-123">Authorization</span></span>  | <span data-ttu-id="563af-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="563af-124">Bearer {code}</span></span>|
| <span data-ttu-id="563af-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="563af-125">Content-type</span></span>  | <span data-ttu-id="563af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="563af-126">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="563af-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="563af-127">Request body</span></span>
<span data-ttu-id="563af-128">В тексте запроса задаете значения параметра [governanceRuleSettings](../resources/governancerulesetting.md) , который требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="563af-128">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="563af-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="563af-129">Property</span></span>     | <span data-ttu-id="563af-130">Тип</span><span class="sxs-lookup"><span data-stu-id="563af-130">Type</span></span>   |<span data-ttu-id="563af-131">Описание</span><span class="sxs-lookup"><span data-stu-id="563af-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="563af-132">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="563af-132">adminEligibleSettings</span></span>|[<span data-ttu-id="563af-133">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="563af-133">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="563af-134">Параметры правил, которые вычисляются, когда администратор пытается добавить назначение подходящими роли.</span><span class="sxs-lookup"><span data-stu-id="563af-134">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="563af-135">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="563af-135">adminMemberSettings</span></span>|[<span data-ttu-id="563af-136">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="563af-136">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="563af-137">Параметры правил, которые вычисляются, когда администратор пытается добавить членами назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="563af-137">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="563af-138">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="563af-138">userEligibleSettings</span></span>|[<span data-ttu-id="563af-139">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="563af-139">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="563af-140">Параметры правил, которые вычисляются, когда пользователь пытается добавить назначение подходящими роли.</span><span class="sxs-lookup"><span data-stu-id="563af-140">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="563af-141">Это действие не поддерживается для `pimforazurerbac` сценарий в данный момент и может быть доступно в последующих сценариях.</span><span class="sxs-lookup"><span data-stu-id="563af-141">This is not supported for `pimforazurerbac` scenario for now, and may be available in the future scenarios.</span></span>|
|<span data-ttu-id="563af-142">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="563af-142">userMemberSettings</span></span>|[<span data-ttu-id="563af-143">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="563af-143">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="563af-144">Параметры правил, которые вычисляются при попытке активировать его назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="563af-144">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="563af-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="563af-145">Response</span></span>
<span data-ttu-id="563af-p104">При успешном выполнении этот метод возвращает код отклика `204 NoContent`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="563af-p104">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="563af-148">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="563af-148">Error codes</span></span>
<span data-ttu-id="563af-149">Этот интерфейс API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="563af-149">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="563af-150">Кроме того он возвращает следующие коды ошибок.</span><span class="sxs-lookup"><span data-stu-id="563af-150">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="563af-151">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="563af-151">Error code</span></span>     | <span data-ttu-id="563af-152">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="563af-152">Error message</span></span>         | <span data-ttu-id="563af-153">Сведения</span><span class="sxs-lookup"><span data-stu-id="563af-153">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="563af-154">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="563af-154">400 BadRequest</span></span>| <span data-ttu-id="563af-155">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="563af-155">RoleSettingNotFound</span></span>   | <span data-ttu-id="563af-156">[GovernanceRoleSetting](../resources/governancerolesetting.md) не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="563af-156">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="563af-157">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="563af-157">400 BadRequest</span></span>| <span data-ttu-id="563af-158">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="563af-158">InvalidRoleSetting</span></span>    | <span data-ttu-id="563af-159">Недопустимые значения [governanceRuleSettings](../resources/governancerulesetting.md) , предоставляемые в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="563af-159">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="563af-160">Пример</span><span class="sxs-lookup"><span data-stu-id="563af-160">Example</span></span> 
<span data-ttu-id="563af-161">В этом примере обновляется параметр роли для настраиваемых ролей 3 в Wingtip Toys - производственного подписки.</span><span class="sxs-lookup"><span data-stu-id="563af-161">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="563af-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="563af-162">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="563af-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="563af-163">Response</span></span>
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
