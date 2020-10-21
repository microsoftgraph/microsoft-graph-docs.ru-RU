---
title: Обновление Говернанцеролесеттинг
description: Обновление свойств объекта Говернанцеролесеттинг.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 3ae917f9b92ee743173842b3ed9ccf2a2bea3edd
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634870"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="3563c-103">Обновление Говернанцеролесеттинг</span><span class="sxs-lookup"><span data-stu-id="3563c-103">Update governanceRoleSetting</span></span>

<span data-ttu-id="3563c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3563c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3563c-105">Обновление свойств объекта [говернанцеролесеттинг](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="3563c-105">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3563c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3563c-106">Permissions</span></span>
<span data-ttu-id="3563c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="3563c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

><span data-ttu-id="3563c-109">**Примечание:** Этот API также требует, чтобы у автора запроса было по крайней мере одно `Active` назначение роли администратора ( `owner` или `user access administrator` ) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="3563c-109">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="3563c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3563c-110">Permission type</span></span>      | <span data-ttu-id="3563c-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3563c-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3563c-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3563c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3563c-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="3563c-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="3563c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3563c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3563c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3563c-115">Not supported.</span></span>    |
|<span data-ttu-id="3563c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3563c-116">Application</span></span> | <span data-ttu-id="3563c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3563c-117">Not supported.</span></span> |
### <a name="azure-resources"></a><span data-ttu-id="3563c-118">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="3563c-118">Azure resources</span></span>

| <span data-ttu-id="3563c-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3563c-119">Permission type</span></span> | <span data-ttu-id="3563c-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3563c-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="3563c-121">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3563c-121">Delegated (work or school account)</span></span> | <span data-ttu-id="3563c-122">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="3563c-122">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="3563c-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3563c-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3563c-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3563c-124">Not supported.</span></span> |
| <span data-ttu-id="3563c-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3563c-125">Application</span></span> | <span data-ttu-id="3563c-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3563c-126">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="3563c-127">Azure AD</span><span class="sxs-lookup"><span data-stu-id="3563c-127">Azure AD</span></span>

| <span data-ttu-id="3563c-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3563c-128">Permission type</span></span> | <span data-ttu-id="3563c-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3563c-129">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="3563c-130">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3563c-130">Delegated (work or school account)</span></span> | <span data-ttu-id="3563c-131">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="3563c-131">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="3563c-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3563c-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3563c-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3563c-133">Not supported.</span></span> |
| <span data-ttu-id="3563c-134">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3563c-134">Application</span></span> | <span data-ttu-id="3563c-135">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3563c-135">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="3563c-136">Группы</span><span class="sxs-lookup"><span data-stu-id="3563c-136">Groups</span></span>

|<span data-ttu-id="3563c-137">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3563c-137">Permission type</span></span> | <span data-ttu-id="3563c-138">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3563c-138">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="3563c-139">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3563c-139">Delegated (work or school account)</span></span> | <span data-ttu-id="3563c-140">Привилежедакцесс. ReadWrite. Азуреадграупс</span><span class="sxs-lookup"><span data-stu-id="3563c-140">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="3563c-141">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3563c-141">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3563c-142">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3563c-142">Not supported.</span></span> |
| <span data-ttu-id="3563c-143">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3563c-143">Application</span></span> | <span data-ttu-id="3563c-144">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3563c-144">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3563c-145">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3563c-145">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3563c-146">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3563c-146">Request headers</span></span>
| <span data-ttu-id="3563c-147">Имя</span><span class="sxs-lookup"><span data-stu-id="3563c-147">Name</span></span>       | <span data-ttu-id="3563c-148">Описание</span><span class="sxs-lookup"><span data-stu-id="3563c-148">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3563c-149">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3563c-149">Authorization</span></span>  | <span data-ttu-id="3563c-150">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="3563c-150">Bearer {token}</span></span>|
| <span data-ttu-id="3563c-151">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3563c-151">Content-type</span></span>  | <span data-ttu-id="3563c-152">application/json</span><span class="sxs-lookup"><span data-stu-id="3563c-152">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="3563c-153">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3563c-153">Request body</span></span>
<span data-ttu-id="3563c-154">В тексте запроса укажите значения для [говернанцерулесеттингс](../resources/governancerulesetting.md) , которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="3563c-154">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="3563c-155">Свойство</span><span class="sxs-lookup"><span data-stu-id="3563c-155">Property</span></span>     | <span data-ttu-id="3563c-156">Тип</span><span class="sxs-lookup"><span data-stu-id="3563c-156">Type</span></span>   |<span data-ttu-id="3563c-157">Описание</span><span class="sxs-lookup"><span data-stu-id="3563c-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3563c-158">админелигиблесеттингс</span><span class="sxs-lookup"><span data-stu-id="3563c-158">adminEligibleSettings</span></span>|<span data-ttu-id="3563c-159">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="3563c-159">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="3563c-160">Параметры правил, которые оцениваются, когда администратор пытается добавить подходящего назначения роли.</span><span class="sxs-lookup"><span data-stu-id="3563c-160">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="3563c-161">админмемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="3563c-161">adminMemberSettings</span></span>|<span data-ttu-id="3563c-162">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="3563c-162">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="3563c-163">Параметры правил, которые оцениваются при попытке администратора добавить назначение роли прямого члена.</span><span class="sxs-lookup"><span data-stu-id="3563c-163">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="3563c-164">усерелигиблесеттингс</span><span class="sxs-lookup"><span data-stu-id="3563c-164">userEligibleSettings</span></span>|<span data-ttu-id="3563c-165">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="3563c-165">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="3563c-166">Параметры правил, которые оцениваются, когда пользователь пытается добавить подходящего назначения роли.</span><span class="sxs-lookup"><span data-stu-id="3563c-166">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> |
|<span data-ttu-id="3563c-167">усермемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="3563c-167">userMemberSettings</span></span>|<span data-ttu-id="3563c-168">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="3563c-168">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="3563c-169">Параметры правил, которые оцениваются, когда пользователь пытается активировать назначение роли.</span><span class="sxs-lookup"><span data-stu-id="3563c-169">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="3563c-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="3563c-170">Response</span></span>
<span data-ttu-id="3563c-p102">При успешном выполнении этот метод возвращает код отклика `204 NoContent`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3563c-p102">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="3563c-173">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="3563c-173">Error codes</span></span>
<span data-ttu-id="3563c-174">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="3563c-174">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="3563c-175">Кроме того, возвращаются следующие коды настраиваемых ошибок.</span><span class="sxs-lookup"><span data-stu-id="3563c-175">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="3563c-176">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="3563c-176">Error code</span></span>     | <span data-ttu-id="3563c-177">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="3563c-177">Error message</span></span>         | <span data-ttu-id="3563c-178">Сведения</span><span class="sxs-lookup"><span data-stu-id="3563c-178">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="3563c-179">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="3563c-179">400 BadRequest</span></span>| <span data-ttu-id="3563c-180">ролесеттингнотфаунд</span><span class="sxs-lookup"><span data-stu-id="3563c-180">RoleSettingNotFound</span></span>   | <span data-ttu-id="3563c-181">[Говернанцеролесеттинг](../resources/governancerolesetting.md) не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="3563c-181">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="3563c-182">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="3563c-182">400 BadRequest</span></span>| <span data-ttu-id="3563c-183">инвалидролесеттинг</span><span class="sxs-lookup"><span data-stu-id="3563c-183">InvalidRoleSetting</span></span>    | <span data-ttu-id="3563c-184">В тексте запроса указаны недопустимые значения [говернанцерулесеттингс](../resources/governancerulesetting.md) .</span><span class="sxs-lookup"><span data-stu-id="3563c-184">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="3563c-185">Пример</span><span class="sxs-lookup"><span data-stu-id="3563c-185">Example</span></span> 
<span data-ttu-id="3563c-186">В этом примере обновляется параметр Role для настраиваемой роли 3 в подписке Wingtip Toys — произ.</span><span class="sxs-lookup"><span data-stu-id="3563c-186">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="3563c-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="3563c-187">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3563c-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="3563c-188">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3563c-189">C#</span><span class="sxs-lookup"><span data-stu-id="3563c-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3563c-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3563c-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3563c-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3563c-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3563c-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="3563c-192">Response</span></span>
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


