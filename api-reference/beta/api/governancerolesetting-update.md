---
title: Обновление Говернанцеролесеттинг
description: Обновление свойств объекта Говернанцеролесеттинг.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: e8f18cae950276979330d0f4830acbd2eb4492ab
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43215811"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="d0b7d-103">Обновление Говернанцеролесеттинг</span><span class="sxs-lookup"><span data-stu-id="d0b7d-103">Update governanceRoleSetting</span></span>

<span data-ttu-id="d0b7d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0b7d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0b7d-105">Обновление свойств объекта [говернанцеролесеттинг](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="d0b7d-105">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d0b7d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0b7d-106">Permissions</span></span>
<span data-ttu-id="d0b7d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0b7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="d0b7d-109">**Примечание:** Этот API также требует, чтобы у автора запроса было по `Active` крайней мере одно`owner` назначение `user access administrator`роли администратора (или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="d0b7d-109">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="d0b7d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0b7d-110">Permission type</span></span>      | <span data-ttu-id="d0b7d-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0b7d-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0b7d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0b7d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d0b7d-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="d0b7d-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="d0b7d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0b7d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0b7d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0b7d-115">Not supported.</span></span>    |
|<span data-ttu-id="d0b7d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0b7d-116">Application</span></span> | <span data-ttu-id="d0b7d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0b7d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0b7d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0b7d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d0b7d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0b7d-119">Request headers</span></span>
| <span data-ttu-id="d0b7d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d0b7d-120">Name</span></span>       | <span data-ttu-id="d0b7d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d0b7d-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d0b7d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d0b7d-122">Authorization</span></span>  | <span data-ttu-id="d0b7d-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="d0b7d-123">Bearer {token}</span></span>|
| <span data-ttu-id="d0b7d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d0b7d-124">Content-type</span></span>  | <span data-ttu-id="d0b7d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d0b7d-125">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="d0b7d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d0b7d-126">Request body</span></span>
<span data-ttu-id="d0b7d-127">В тексте запроса укажите значения для [говернанцерулесеттингс](../resources/governancerulesetting.md) , которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="d0b7d-127">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="d0b7d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0b7d-128">Property</span></span>     | <span data-ttu-id="d0b7d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d0b7d-129">Type</span></span>   |<span data-ttu-id="d0b7d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d0b7d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0b7d-131">админелигиблесеттингс</span><span class="sxs-lookup"><span data-stu-id="d0b7d-131">adminEligibleSettings</span></span>|<span data-ttu-id="d0b7d-132">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="d0b7d-132">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="d0b7d-133">Параметры правил, которые оцениваются, когда администратор пытается добавить подходящего назначения роли.</span><span class="sxs-lookup"><span data-stu-id="d0b7d-133">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="d0b7d-134">админмемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="d0b7d-134">adminMemberSettings</span></span>|<span data-ttu-id="d0b7d-135">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="d0b7d-135">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="d0b7d-136">Параметры правил, которые оцениваются при попытке администратора добавить назначение роли прямого члена.</span><span class="sxs-lookup"><span data-stu-id="d0b7d-136">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="d0b7d-137">усерелигиблесеттингс</span><span class="sxs-lookup"><span data-stu-id="d0b7d-137">userEligibleSettings</span></span>|<span data-ttu-id="d0b7d-138">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="d0b7d-138">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="d0b7d-139">Параметры правил, которые оцениваются, когда пользователь пытается добавить подходящего назначения роли.</span><span class="sxs-lookup"><span data-stu-id="d0b7d-139">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> |
|<span data-ttu-id="d0b7d-140">усермемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="d0b7d-140">userMemberSettings</span></span>|<span data-ttu-id="d0b7d-141">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="d0b7d-141">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="d0b7d-142">Параметры правил, которые оцениваются, когда пользователь пытается активировать назначение роли.</span><span class="sxs-lookup"><span data-stu-id="d0b7d-142">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="d0b7d-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0b7d-143">Response</span></span>
<span data-ttu-id="d0b7d-p102">При успешном выполнении этот метод возвращает код отклика `204 NoContent`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d0b7d-p102">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="d0b7d-146">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="d0b7d-146">Error codes</span></span>
<span data-ttu-id="d0b7d-147">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="d0b7d-147">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="d0b7d-148">Кроме того, возвращаются следующие коды настраиваемых ошибок.</span><span class="sxs-lookup"><span data-stu-id="d0b7d-148">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="d0b7d-149">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="d0b7d-149">Error code</span></span>     | <span data-ttu-id="d0b7d-150">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="d0b7d-150">Error message</span></span>         | <span data-ttu-id="d0b7d-151">Сведения</span><span class="sxs-lookup"><span data-stu-id="d0b7d-151">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="d0b7d-152">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="d0b7d-152">400 BadRequest</span></span>| <span data-ttu-id="d0b7d-153">ролесеттингнотфаунд</span><span class="sxs-lookup"><span data-stu-id="d0b7d-153">RoleSettingNotFound</span></span>   | <span data-ttu-id="d0b7d-154">[Говернанцеролесеттинг](../resources/governancerolesetting.md) не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="d0b7d-154">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="d0b7d-155">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="d0b7d-155">400 BadRequest</span></span>| <span data-ttu-id="d0b7d-156">инвалидролесеттинг</span><span class="sxs-lookup"><span data-stu-id="d0b7d-156">InvalidRoleSetting</span></span>    | <span data-ttu-id="d0b7d-157">В тексте запроса указаны недопустимые значения [говернанцерулесеттингс](../resources/governancerulesetting.md) .</span><span class="sxs-lookup"><span data-stu-id="d0b7d-157">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="d0b7d-158">Пример</span><span class="sxs-lookup"><span data-stu-id="d0b7d-158">Example</span></span> 
<span data-ttu-id="d0b7d-159">В этом примере обновляется параметр Role для настраиваемой роли 3 в подписке Wingtip Toys — произ.</span><span class="sxs-lookup"><span data-stu-id="d0b7d-159">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="d0b7d-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0b7d-160">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d0b7d-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0b7d-161">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d0b7d-162">C#</span><span class="sxs-lookup"><span data-stu-id="d0b7d-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0b7d-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0b7d-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0b7d-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0b7d-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d0b7d-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0b7d-165">Response</span></span>
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
