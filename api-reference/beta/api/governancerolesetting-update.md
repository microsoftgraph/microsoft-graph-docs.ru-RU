---
title: Обновление управленияRoleSetting
description: Обновление свойств governanceRoleSetting.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 2c4392529d64683a183002b9f0b302495f8042e5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435787"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="8c0f7-103">Обновление управленияRoleSetting</span><span class="sxs-lookup"><span data-stu-id="8c0f7-103">Update governanceRoleSetting</span></span>

<span data-ttu-id="8c0f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c0f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c0f7-105">Обновление свойств [governanceRoleSetting.](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="8c0f7-105">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8c0f7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c0f7-106">Permissions</span></span>
<span data-ttu-id="8c0f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="8c0f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

><span data-ttu-id="8c0f7-109">**Примечание:** Этот API также требует, чтобы у запрашиваемой стороны было по крайней мере одно назначение роли администратора `Active` `owner` `user access administrator` (или) на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="8c0f7-109">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="8c0f7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c0f7-110">Permission type</span></span>      | <span data-ttu-id="8c0f7-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c0f7-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c0f7-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c0f7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8c0f7-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="8c0f7-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="8c0f7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c0f7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c0f7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c0f7-115">Not supported.</span></span>    |
|<span data-ttu-id="8c0f7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c0f7-116">Application</span></span> | <span data-ttu-id="8c0f7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c0f7-117">Not supported.</span></span> |
### <a name="azure-resources"></a><span data-ttu-id="8c0f7-118">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="8c0f7-118">Azure resources</span></span>

| <span data-ttu-id="8c0f7-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c0f7-119">Permission type</span></span> | <span data-ttu-id="8c0f7-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c0f7-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="8c0f7-121">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c0f7-121">Delegated (work or school account)</span></span> | <span data-ttu-id="8c0f7-122">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="8c0f7-122">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="8c0f7-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c0f7-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c0f7-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c0f7-124">Not supported.</span></span> |
| <span data-ttu-id="8c0f7-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c0f7-125">Application</span></span> | <span data-ttu-id="8c0f7-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c0f7-126">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="8c0f7-127">Azure AD</span><span class="sxs-lookup"><span data-stu-id="8c0f7-127">Azure AD</span></span>

| <span data-ttu-id="8c0f7-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c0f7-128">Permission type</span></span> | <span data-ttu-id="8c0f7-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c0f7-129">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="8c0f7-130">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c0f7-130">Delegated (work or school account)</span></span> | <span data-ttu-id="8c0f7-131">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="8c0f7-131">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="8c0f7-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c0f7-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c0f7-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c0f7-133">Not supported.</span></span> |
| <span data-ttu-id="8c0f7-134">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c0f7-134">Application</span></span> | <span data-ttu-id="8c0f7-135">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c0f7-135">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="8c0f7-136">Группы</span><span class="sxs-lookup"><span data-stu-id="8c0f7-136">Groups</span></span>

|<span data-ttu-id="8c0f7-137">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c0f7-137">Permission type</span></span> | <span data-ttu-id="8c0f7-138">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c0f7-138">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="8c0f7-139">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c0f7-139">Delegated (work or school account)</span></span> | <span data-ttu-id="8c0f7-140">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="8c0f7-140">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="8c0f7-141">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c0f7-141">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c0f7-142">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c0f7-142">Not supported.</span></span> |
| <span data-ttu-id="8c0f7-143">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c0f7-143">Application</span></span> | <span data-ttu-id="8c0f7-144">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c0f7-144">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c0f7-145">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c0f7-145">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8c0f7-146">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c0f7-146">Request headers</span></span>
| <span data-ttu-id="8c0f7-147">Имя</span><span class="sxs-lookup"><span data-stu-id="8c0f7-147">Name</span></span>       | <span data-ttu-id="8c0f7-148">Описание</span><span class="sxs-lookup"><span data-stu-id="8c0f7-148">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8c0f7-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c0f7-149">Authorization</span></span>  | <span data-ttu-id="8c0f7-150">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="8c0f7-150">Bearer {token}</span></span>|
| <span data-ttu-id="8c0f7-151">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c0f7-151">Content-type</span></span>  | <span data-ttu-id="8c0f7-152">application/json</span><span class="sxs-lookup"><span data-stu-id="8c0f7-152">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="8c0f7-153">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8c0f7-153">Request body</span></span>
<span data-ttu-id="8c0f7-154">В теле запроса укажи значения [для governanceRuleSettings,](../resources/governancerulesetting.md) которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="8c0f7-154">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="8c0f7-155">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c0f7-155">Property</span></span>     | <span data-ttu-id="8c0f7-156">Тип</span><span class="sxs-lookup"><span data-stu-id="8c0f7-156">Type</span></span>   |<span data-ttu-id="8c0f7-157">Описание</span><span class="sxs-lookup"><span data-stu-id="8c0f7-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c0f7-158">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="8c0f7-158">adminEligibleSettings</span></span>|<span data-ttu-id="8c0f7-159">[коллекция governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="8c0f7-159">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="8c0f7-160">Параметры правил, которые оцениваются при добавлении администратором назначения подходящих ролей.</span><span class="sxs-lookup"><span data-stu-id="8c0f7-160">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="8c0f7-161">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="8c0f7-161">adminMemberSettings</span></span>|<span data-ttu-id="8c0f7-162">[коллекция governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="8c0f7-162">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="8c0f7-163">Параметры правил, которые оцениваются, когда администратор пытается добавить назначение ролей прямого участника.</span><span class="sxs-lookup"><span data-stu-id="8c0f7-163">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="8c0f7-164">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="8c0f7-164">userEligibleSettings</span></span>|<span data-ttu-id="8c0f7-165">[коллекция governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="8c0f7-165">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="8c0f7-166">Параметры правил, оцениваемые при добавлении права на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="8c0f7-166">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> |
|<span data-ttu-id="8c0f7-167">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="8c0f7-167">userMemberSettings</span></span>|<span data-ttu-id="8c0f7-168">[коллекция governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="8c0f7-168">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="8c0f7-169">Параметры правил, которые оцениваются при попытках пользователя активировать назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="8c0f7-169">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="8c0f7-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c0f7-170">Response</span></span>
<span data-ttu-id="8c0f7-p102">При успешном выполнении этот метод возвращает код отклика `204 NoContent`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8c0f7-p102">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="8c0f7-173">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="8c0f7-173">Error codes</span></span>
<span data-ttu-id="8c0f7-174">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="8c0f7-174">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="8c0f7-175">Кроме того, он возвращает следующие пользовательские коды ошибок.</span><span class="sxs-lookup"><span data-stu-id="8c0f7-175">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="8c0f7-176">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="8c0f7-176">Error code</span></span>     | <span data-ttu-id="8c0f7-177">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="8c0f7-177">Error message</span></span>         | <span data-ttu-id="8c0f7-178">Сведения</span><span class="sxs-lookup"><span data-stu-id="8c0f7-178">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="8c0f7-179">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="8c0f7-179">400 BadRequest</span></span>| <span data-ttu-id="8c0f7-180">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="8c0f7-180">RoleSettingNotFound</span></span>   | <span data-ttu-id="8c0f7-181">В системе не существует системы [governanceRoleSetting.](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="8c0f7-181">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="8c0f7-182">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="8c0f7-182">400 BadRequest</span></span>| <span data-ttu-id="8c0f7-183">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="8c0f7-183">InvalidRoleSetting</span></span>    | <span data-ttu-id="8c0f7-184">Значения [governanceRuleSettings,](../resources/governancerulesetting.md) предоставляемые в теле запроса, не допустимы.</span><span class="sxs-lookup"><span data-stu-id="8c0f7-184">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="8c0f7-185">Пример</span><span class="sxs-lookup"><span data-stu-id="8c0f7-185">Example</span></span> 
<span data-ttu-id="8c0f7-186">В этом примере обновляется параметр роли для настраиваемой роли 3 в подписке Wingtip Toys - Prod.</span><span class="sxs-lookup"><span data-stu-id="8c0f7-186">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="8c0f7-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c0f7-187">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8c0f7-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c0f7-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_governancerolesetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5
Content-type: application/json
Content-length: 350

{
   "adminEligibleSettings":[
      {
         "ruleIdentifier":"ExpirationRule",
         "setting":"{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"
      }
   ]
}
```
# <a name="c"></a>[<span data-ttu-id="8c0f7-189">C#</span><span class="sxs-lookup"><span data-stu-id="8c0f7-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c0f7-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c0f7-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c0f7-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c0f7-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c0f7-192">Java</span><span class="sxs-lookup"><span data-stu-id="8c0f7-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-governancerolesetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8c0f7-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c0f7-193">Response</span></span>
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
  ]
}
-->


