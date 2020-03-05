---
title: Обновление Говернанцеролесеттинг
description: Обновление свойств объекта Говернанцеролесеттинг.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2cd81e24f6719ea47e7c6cf86486fbb63cd26d3b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42420817"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="8457c-103">Обновление Говернанцеролесеттинг</span><span class="sxs-lookup"><span data-stu-id="8457c-103">Update governanceRoleSetting</span></span>

<span data-ttu-id="8457c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8457c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8457c-105">Обновление свойств объекта [говернанцеролесеттинг](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="8457c-105">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8457c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8457c-106">Permissions</span></span>
<span data-ttu-id="8457c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8457c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="8457c-109">**Примечание:** Этот API также требует, чтобы у автора запроса было по `Active` крайней мере одно`owner` назначение `user access administrator`роли администратора (или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="8457c-109">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="8457c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8457c-110">Permission type</span></span>      | <span data-ttu-id="8457c-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8457c-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8457c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8457c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8457c-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="8457c-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="8457c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8457c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8457c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8457c-115">Not supported.</span></span>    |
|<span data-ttu-id="8457c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8457c-116">Application</span></span> | <span data-ttu-id="8457c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8457c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8457c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8457c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8457c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8457c-119">Request headers</span></span>
| <span data-ttu-id="8457c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8457c-120">Name</span></span>       | <span data-ttu-id="8457c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8457c-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8457c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8457c-122">Authorization</span></span>  | <span data-ttu-id="8457c-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="8457c-123">Bearer {token}</span></span>|
| <span data-ttu-id="8457c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8457c-124">Content-type</span></span>  | <span data-ttu-id="8457c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8457c-125">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="8457c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8457c-126">Request body</span></span>
<span data-ttu-id="8457c-127">В тексте запроса укажите значения для [говернанцерулесеттингс](../resources/governancerulesetting.md) , которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="8457c-127">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="8457c-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="8457c-128">Property</span></span>     | <span data-ttu-id="8457c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="8457c-129">Type</span></span>   |<span data-ttu-id="8457c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="8457c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8457c-131">админелигиблесеттингс</span><span class="sxs-lookup"><span data-stu-id="8457c-131">adminEligibleSettings</span></span>|<span data-ttu-id="8457c-132">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="8457c-132">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="8457c-133">Параметры правил, которые оцениваются, когда администратор пытается добавить подходящего назначения роли.</span><span class="sxs-lookup"><span data-stu-id="8457c-133">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="8457c-134">админмемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="8457c-134">adminMemberSettings</span></span>|<span data-ttu-id="8457c-135">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="8457c-135">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="8457c-136">Параметры правил, которые оцениваются при попытке администратора добавить назначение роли прямого члена.</span><span class="sxs-lookup"><span data-stu-id="8457c-136">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="8457c-137">усерелигиблесеттингс</span><span class="sxs-lookup"><span data-stu-id="8457c-137">userEligibleSettings</span></span>|<span data-ttu-id="8457c-138">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="8457c-138">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="8457c-139">Параметры правил, которые оцениваются, когда пользователь пытается добавить подходящего назначения роли.</span><span class="sxs-lookup"><span data-stu-id="8457c-139">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> |
|<span data-ttu-id="8457c-140">усермемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="8457c-140">userMemberSettings</span></span>|<span data-ttu-id="8457c-141">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="8457c-141">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="8457c-142">Параметры правил, которые оцениваются, когда пользователь пытается активировать назначение роли.</span><span class="sxs-lookup"><span data-stu-id="8457c-142">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="8457c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="8457c-143">Response</span></span>
<span data-ttu-id="8457c-p102">При успешном выполнении этот метод возвращает код отклика `204 NoContent`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8457c-p102">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="8457c-146">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="8457c-146">Error codes</span></span>
<span data-ttu-id="8457c-147">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="8457c-147">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="8457c-148">Кроме того, возвращаются следующие коды настраиваемых ошибок.</span><span class="sxs-lookup"><span data-stu-id="8457c-148">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="8457c-149">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="8457c-149">Error code</span></span>     | <span data-ttu-id="8457c-150">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="8457c-150">Error message</span></span>         | <span data-ttu-id="8457c-151">Сведения</span><span class="sxs-lookup"><span data-stu-id="8457c-151">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="8457c-152">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="8457c-152">400 BadRequest</span></span>| <span data-ttu-id="8457c-153">ролесеттингнотфаунд</span><span class="sxs-lookup"><span data-stu-id="8457c-153">RoleSettingNotFound</span></span>   | <span data-ttu-id="8457c-154">[Говернанцеролесеттинг](../resources/governancerolesetting.md) не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="8457c-154">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="8457c-155">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="8457c-155">400 BadRequest</span></span>| <span data-ttu-id="8457c-156">инвалидролесеттинг</span><span class="sxs-lookup"><span data-stu-id="8457c-156">InvalidRoleSetting</span></span>    | <span data-ttu-id="8457c-157">В тексте запроса указаны недопустимые значения [говернанцерулесеттингс](../resources/governancerulesetting.md) .</span><span class="sxs-lookup"><span data-stu-id="8457c-157">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="8457c-158">Пример</span><span class="sxs-lookup"><span data-stu-id="8457c-158">Example</span></span> 
<span data-ttu-id="8457c-159">В этом примере обновляется параметр Role для настраиваемой роли 3 в подписке Wingtip Toys — произ.</span><span class="sxs-lookup"><span data-stu-id="8457c-159">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="8457c-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="8457c-160">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8457c-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="8457c-161">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8457c-162">C#</span><span class="sxs-lookup"><span data-stu-id="8457c-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8457c-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8457c-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8457c-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8457c-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8457c-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="8457c-165">Response</span></span>
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
