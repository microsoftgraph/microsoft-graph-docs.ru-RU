---
title: Обновление governanceRoleSetting
description: Обновление свойств governanceRoleSetting.
localization_priority: Normal
ms.openlocfilehash: e5fc297690816227e1031af363ea7d4d38199e25
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509331"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="3fcd4-103">Обновление governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="3fcd4-103">Update governanceRoleSetting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3fcd4-104">Обновление свойств [governanceRoleSetting](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="3fcd4-104">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3fcd4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3fcd4-105">Permissions</span></span>
<span data-ttu-id="3fcd4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fcd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="3fcd4-108">**Примечание:** Этот интерфейс API также требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="3fcd4-108">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="3fcd4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3fcd4-109">Permission type</span></span>      | <span data-ttu-id="3fcd4-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3fcd4-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3fcd4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fcd4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3fcd4-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="3fcd4-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="3fcd4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fcd4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3fcd4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fcd4-114">Not supported.</span></span>    |
|<span data-ttu-id="3fcd4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3fcd4-115">Application</span></span> | <span data-ttu-id="3fcd4-116">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="3fcd4-116">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="3fcd4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fcd4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3fcd4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3fcd4-118">Request headers</span></span>
| <span data-ttu-id="3fcd4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3fcd4-119">Name</span></span>       | <span data-ttu-id="3fcd4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3fcd4-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3fcd4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fcd4-121">Authorization</span></span>  | <span data-ttu-id="3fcd4-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3fcd4-122">Bearer {code}</span></span>|
| <span data-ttu-id="3fcd4-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3fcd4-123">Content-type</span></span>  | <span data-ttu-id="3fcd4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3fcd4-124">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="3fcd4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3fcd4-125">Request body</span></span>
<span data-ttu-id="3fcd4-126">В тексте запроса задаете значения параметра [governanceRuleSettings](../resources/governancerulesetting.md) , который требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="3fcd4-126">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="3fcd4-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="3fcd4-127">Property</span></span>     | <span data-ttu-id="3fcd4-128">Тип</span><span class="sxs-lookup"><span data-stu-id="3fcd4-128">Type</span></span>   |<span data-ttu-id="3fcd4-129">Описание</span><span class="sxs-lookup"><span data-stu-id="3fcd4-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3fcd4-130">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="3fcd4-130">adminEligibleSettings</span></span>|[<span data-ttu-id="3fcd4-131">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="3fcd4-131">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="3fcd4-132">Параметры правил, которые вычисляются, когда администратор пытается добавить назначение подходящими роли.</span><span class="sxs-lookup"><span data-stu-id="3fcd4-132">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="3fcd4-133">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="3fcd4-133">adminMemberSettings</span></span>|[<span data-ttu-id="3fcd4-134">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="3fcd4-134">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="3fcd4-135">Параметры правил, которые вычисляются, когда администратор пытается добавить членами назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="3fcd4-135">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="3fcd4-136">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="3fcd4-136">userEligibleSettings</span></span>|[<span data-ttu-id="3fcd4-137">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="3fcd4-137">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="3fcd4-138">Параметры правил, которые вычисляются, когда пользователь пытается добавить назначение подходящими роли.</span><span class="sxs-lookup"><span data-stu-id="3fcd4-138">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="3fcd4-139">Это действие не поддерживается для `pimforazurerbac` сценарий в данный момент и может быть доступно в последующих сценариях.</span><span class="sxs-lookup"><span data-stu-id="3fcd4-139">This is not supported for `pimforazurerbac` scenario for now, and may be available in the future scenarios.</span></span>|
|<span data-ttu-id="3fcd4-140">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="3fcd4-140">userMemberSettings</span></span>|[<span data-ttu-id="3fcd4-141">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="3fcd4-141">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="3fcd4-142">Параметры правил, которые вычисляются при попытке активировать его назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="3fcd4-142">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="3fcd4-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fcd4-143">Response</span></span>
<span data-ttu-id="3fcd4-p103">При успешном выполнении этот метод возвращает код отклика `204 NoContent`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3fcd4-p103">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="3fcd4-146">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="3fcd4-146">Error codes</span></span>
<span data-ttu-id="3fcd4-147">Этот интерфейс API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="3fcd4-147">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="3fcd4-148">Кроме того он возвращает следующие коды ошибок.</span><span class="sxs-lookup"><span data-stu-id="3fcd4-148">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="3fcd4-149">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="3fcd4-149">Error code</span></span>     | <span data-ttu-id="3fcd4-150">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="3fcd4-150">Error message</span></span>         | <span data-ttu-id="3fcd4-151">Сведения</span><span class="sxs-lookup"><span data-stu-id="3fcd4-151">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="3fcd4-152">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="3fcd4-152">400 BadRequest</span></span>| <span data-ttu-id="3fcd4-153">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="3fcd4-153">RoleSettingNotFound</span></span>   | <span data-ttu-id="3fcd4-154">[GovernanceRoleSetting](../resources/governancerolesetting.md) не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="3fcd4-154">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="3fcd4-155">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="3fcd4-155">400 BadRequest</span></span>| <span data-ttu-id="3fcd4-156">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="3fcd4-156">InvalidRoleSetting</span></span>    | <span data-ttu-id="3fcd4-157">Недопустимые значения [governanceRuleSettings](../resources/governancerulesetting.md) , предоставляемые в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="3fcd4-157">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="3fcd4-158">Пример</span><span class="sxs-lookup"><span data-stu-id="3fcd4-158">Example</span></span> 
<span data-ttu-id="3fcd4-159">В этом примере обновляется параметр роли для настраиваемых ролей 3 в Wingtip Toys - производственного подписки.</span><span class="sxs-lookup"><span data-stu-id="3fcd4-159">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="3fcd4-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fcd4-160">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="3fcd4-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="3fcd4-161">Response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governancerolesetting-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
