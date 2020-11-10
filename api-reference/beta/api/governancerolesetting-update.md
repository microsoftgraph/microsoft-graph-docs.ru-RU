---
title: Обновление Говернанцеролесеттинг
description: Обновление свойств объекта Говернанцеролесеттинг.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 24a2e96136bf416547a974bbecf004bc46d81f04
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965412"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="b13b8-103">Обновление Говернанцеролесеттинг</span><span class="sxs-lookup"><span data-stu-id="b13b8-103">Update governanceRoleSetting</span></span>

<span data-ttu-id="b13b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b13b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b13b8-105">Обновление свойств объекта [говернанцеролесеттинг](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="b13b8-105">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b13b8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b13b8-106">Permissions</span></span>
<span data-ttu-id="b13b8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="b13b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

><span data-ttu-id="b13b8-109">**Примечание:** Этот API также требует, чтобы у автора запроса было по крайней мере одно `Active` назначение роли администратора ( `owner` или `user access administrator` ) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="b13b8-109">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="b13b8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b13b8-110">Permission type</span></span>      | <span data-ttu-id="b13b8-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b13b8-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b13b8-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b13b8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b13b8-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="b13b8-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="b13b8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b13b8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b13b8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b13b8-115">Not supported.</span></span>    |
|<span data-ttu-id="b13b8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b13b8-116">Application</span></span> | <span data-ttu-id="b13b8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b13b8-117">Not supported.</span></span> |
### <a name="azure-resources"></a><span data-ttu-id="b13b8-118">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="b13b8-118">Azure resources</span></span>

| <span data-ttu-id="b13b8-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b13b8-119">Permission type</span></span> | <span data-ttu-id="b13b8-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b13b8-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="b13b8-121">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b13b8-121">Delegated (work or school account)</span></span> | <span data-ttu-id="b13b8-122">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="b13b8-122">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="b13b8-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b13b8-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b13b8-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b13b8-124">Not supported.</span></span> |
| <span data-ttu-id="b13b8-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b13b8-125">Application</span></span> | <span data-ttu-id="b13b8-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b13b8-126">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="b13b8-127">Azure AD</span><span class="sxs-lookup"><span data-stu-id="b13b8-127">Azure AD</span></span>

| <span data-ttu-id="b13b8-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b13b8-128">Permission type</span></span> | <span data-ttu-id="b13b8-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b13b8-129">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="b13b8-130">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b13b8-130">Delegated (work or school account)</span></span> | <span data-ttu-id="b13b8-131">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="b13b8-131">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="b13b8-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b13b8-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b13b8-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b13b8-133">Not supported.</span></span> |
| <span data-ttu-id="b13b8-134">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b13b8-134">Application</span></span> | <span data-ttu-id="b13b8-135">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b13b8-135">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="b13b8-136">Группы</span><span class="sxs-lookup"><span data-stu-id="b13b8-136">Groups</span></span>

|<span data-ttu-id="b13b8-137">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b13b8-137">Permission type</span></span> | <span data-ttu-id="b13b8-138">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b13b8-138">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="b13b8-139">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b13b8-139">Delegated (work or school account)</span></span> | <span data-ttu-id="b13b8-140">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="b13b8-140">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="b13b8-141">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b13b8-141">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b13b8-142">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b13b8-142">Not supported.</span></span> |
| <span data-ttu-id="b13b8-143">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b13b8-143">Application</span></span> | <span data-ttu-id="b13b8-144">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b13b8-144">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b13b8-145">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b13b8-145">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b13b8-146">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b13b8-146">Request headers</span></span>
| <span data-ttu-id="b13b8-147">Имя</span><span class="sxs-lookup"><span data-stu-id="b13b8-147">Name</span></span>       | <span data-ttu-id="b13b8-148">Описание</span><span class="sxs-lookup"><span data-stu-id="b13b8-148">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b13b8-149">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b13b8-149">Authorization</span></span>  | <span data-ttu-id="b13b8-150">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="b13b8-150">Bearer {token}</span></span>|
| <span data-ttu-id="b13b8-151">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b13b8-151">Content-type</span></span>  | <span data-ttu-id="b13b8-152">application/json</span><span class="sxs-lookup"><span data-stu-id="b13b8-152">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="b13b8-153">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b13b8-153">Request body</span></span>
<span data-ttu-id="b13b8-154">В тексте запроса укажите значения для [говернанцерулесеттингс](../resources/governancerulesetting.md) , которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="b13b8-154">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="b13b8-155">Свойство</span><span class="sxs-lookup"><span data-stu-id="b13b8-155">Property</span></span>     | <span data-ttu-id="b13b8-156">Тип</span><span class="sxs-lookup"><span data-stu-id="b13b8-156">Type</span></span>   |<span data-ttu-id="b13b8-157">Описание</span><span class="sxs-lookup"><span data-stu-id="b13b8-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b13b8-158">админелигиблесеттингс</span><span class="sxs-lookup"><span data-stu-id="b13b8-158">adminEligibleSettings</span></span>|<span data-ttu-id="b13b8-159">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="b13b8-159">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="b13b8-160">Параметры правил, которые оцениваются, когда администратор пытается добавить подходящего назначения роли.</span><span class="sxs-lookup"><span data-stu-id="b13b8-160">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="b13b8-161">админмемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="b13b8-161">adminMemberSettings</span></span>|<span data-ttu-id="b13b8-162">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="b13b8-162">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="b13b8-163">Параметры правил, которые оцениваются при попытке администратора добавить назначение роли прямого члена.</span><span class="sxs-lookup"><span data-stu-id="b13b8-163">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="b13b8-164">усерелигиблесеттингс</span><span class="sxs-lookup"><span data-stu-id="b13b8-164">userEligibleSettings</span></span>|<span data-ttu-id="b13b8-165">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="b13b8-165">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="b13b8-166">Параметры правил, которые оцениваются, когда пользователь пытается добавить подходящего назначения роли.</span><span class="sxs-lookup"><span data-stu-id="b13b8-166">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> |
|<span data-ttu-id="b13b8-167">усермемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="b13b8-167">userMemberSettings</span></span>|<span data-ttu-id="b13b8-168">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="b13b8-168">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="b13b8-169">Параметры правил, которые оцениваются, когда пользователь пытается активировать назначение роли.</span><span class="sxs-lookup"><span data-stu-id="b13b8-169">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="b13b8-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="b13b8-170">Response</span></span>
<span data-ttu-id="b13b8-p102">При успешном выполнении этот метод возвращает код отклика `204 NoContent`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b13b8-p102">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="b13b8-173">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="b13b8-173">Error codes</span></span>
<span data-ttu-id="b13b8-174">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="b13b8-174">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="b13b8-175">Кроме того, возвращаются следующие коды настраиваемых ошибок.</span><span class="sxs-lookup"><span data-stu-id="b13b8-175">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="b13b8-176">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="b13b8-176">Error code</span></span>     | <span data-ttu-id="b13b8-177">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="b13b8-177">Error message</span></span>         | <span data-ttu-id="b13b8-178">Сведения</span><span class="sxs-lookup"><span data-stu-id="b13b8-178">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="b13b8-179">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="b13b8-179">400 BadRequest</span></span>| <span data-ttu-id="b13b8-180">ролесеттингнотфаунд</span><span class="sxs-lookup"><span data-stu-id="b13b8-180">RoleSettingNotFound</span></span>   | <span data-ttu-id="b13b8-181">[Говернанцеролесеттинг](../resources/governancerolesetting.md) не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="b13b8-181">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="b13b8-182">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="b13b8-182">400 BadRequest</span></span>| <span data-ttu-id="b13b8-183">инвалидролесеттинг</span><span class="sxs-lookup"><span data-stu-id="b13b8-183">InvalidRoleSetting</span></span>    | <span data-ttu-id="b13b8-184">В тексте запроса указаны недопустимые значения [говернанцерулесеттингс](../resources/governancerulesetting.md) .</span><span class="sxs-lookup"><span data-stu-id="b13b8-184">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="b13b8-185">Пример</span><span class="sxs-lookup"><span data-stu-id="b13b8-185">Example</span></span> 
<span data-ttu-id="b13b8-186">В этом примере обновляется параметр Role для настраиваемой роли 3 в подписке Wingtip Toys — произ.</span><span class="sxs-lookup"><span data-stu-id="b13b8-186">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="b13b8-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="b13b8-187">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b13b8-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="b13b8-188">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b13b8-189">C#</span><span class="sxs-lookup"><span data-stu-id="b13b8-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b13b8-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b13b8-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b13b8-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b13b8-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b13b8-192">Java</span><span class="sxs-lookup"><span data-stu-id="b13b8-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-governancerolesetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b13b8-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="b13b8-193">Response</span></span>
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


