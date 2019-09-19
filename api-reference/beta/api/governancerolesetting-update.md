---
title: Обновление Говернанцеролесеттинг
description: Обновление свойств объекта Говернанцеролесеттинг.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 20e41f118f0da2248f0744c64ab25d69da8061f2
ms.sourcegitcommit: 997fbfe36b518e0a8c230ae2e62666bb5c829e7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2019
ms.locfileid: "37041781"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="f693f-103">Обновление Говернанцеролесеттинг</span><span class="sxs-lookup"><span data-stu-id="f693f-103">Update governanceRoleSetting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f693f-104">Обновление свойств объекта [говернанцеролесеттинг](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="f693f-104">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f693f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f693f-105">Permissions</span></span>
<span data-ttu-id="f693f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f693f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="f693f-108">**Примечание:** Этот API также требует, чтобы у автора запроса было по `Active` крайней мере одно`owner` назначение `user access administrator`роли администратора (или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="f693f-108">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="f693f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f693f-109">Permission type</span></span>      | <span data-ttu-id="f693f-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f693f-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f693f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f693f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f693f-112">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="f693f-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="f693f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f693f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f693f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f693f-114">Not supported.</span></span>    |
|<span data-ttu-id="f693f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f693f-115">Application</span></span> | <span data-ttu-id="f693f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f693f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f693f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f693f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f693f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f693f-118">Request headers</span></span>
| <span data-ttu-id="f693f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f693f-119">Name</span></span>       | <span data-ttu-id="f693f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f693f-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f693f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f693f-121">Authorization</span></span>  | <span data-ttu-id="f693f-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="f693f-122">Bearer {token}</span></span>|
| <span data-ttu-id="f693f-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f693f-123">Content-type</span></span>  | <span data-ttu-id="f693f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f693f-124">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="f693f-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f693f-125">Request body</span></span>
<span data-ttu-id="f693f-126">В тексте запроса укажите значения для [говернанцерулесеттингс](../resources/governancerulesetting.md) , которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="f693f-126">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="f693f-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="f693f-127">Property</span></span>     | <span data-ttu-id="f693f-128">Тип</span><span class="sxs-lookup"><span data-stu-id="f693f-128">Type</span></span>   |<span data-ttu-id="f693f-129">Описание</span><span class="sxs-lookup"><span data-stu-id="f693f-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f693f-130">админелигиблесеттингс</span><span class="sxs-lookup"><span data-stu-id="f693f-130">adminEligibleSettings</span></span>|<span data-ttu-id="f693f-131">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="f693f-131">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="f693f-132">Параметры правил, которые оцениваются, когда администратор пытается добавить подходящего назначения роли.</span><span class="sxs-lookup"><span data-stu-id="f693f-132">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="f693f-133">админмемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="f693f-133">adminMemberSettings</span></span>|<span data-ttu-id="f693f-134">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="f693f-134">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="f693f-135">Параметры правил, которые оцениваются при попытке администратора добавить назначение роли прямого члена.</span><span class="sxs-lookup"><span data-stu-id="f693f-135">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="f693f-136">усерелигиблесеттингс</span><span class="sxs-lookup"><span data-stu-id="f693f-136">userEligibleSettings</span></span>|<span data-ttu-id="f693f-137">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="f693f-137">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="f693f-138">Параметры правил, которые оцениваются, когда пользователь пытается добавить подходящего назначения роли.</span><span class="sxs-lookup"><span data-stu-id="f693f-138">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> |
|<span data-ttu-id="f693f-139">усермемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="f693f-139">userMemberSettings</span></span>|<span data-ttu-id="f693f-140">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="f693f-140">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="f693f-141">Параметры правил, которые оцениваются, когда пользователь пытается активировать назначение роли.</span><span class="sxs-lookup"><span data-stu-id="f693f-141">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="f693f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="f693f-142">Response</span></span>
<span data-ttu-id="f693f-p102">При успешном выполнении этот метод возвращает код отклика `204 NoContent`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f693f-p102">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="f693f-145">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="f693f-145">Error codes</span></span>
<span data-ttu-id="f693f-146">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="f693f-146">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="f693f-147">Кроме того, возвращаются следующие коды настраиваемых ошибок.</span><span class="sxs-lookup"><span data-stu-id="f693f-147">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="f693f-148">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="f693f-148">Error code</span></span>     | <span data-ttu-id="f693f-149">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="f693f-149">Error message</span></span>         | <span data-ttu-id="f693f-150">Сведения</span><span class="sxs-lookup"><span data-stu-id="f693f-150">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="f693f-151">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="f693f-151">400 BadRequest</span></span>| <span data-ttu-id="f693f-152">ролесеттингнотфаунд</span><span class="sxs-lookup"><span data-stu-id="f693f-152">RoleSettingNotFound</span></span>   | <span data-ttu-id="f693f-153">[Говернанцеролесеттинг](../resources/governancerolesetting.md) не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="f693f-153">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="f693f-154">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="f693f-154">400 BadRequest</span></span>| <span data-ttu-id="f693f-155">инвалидролесеттинг</span><span class="sxs-lookup"><span data-stu-id="f693f-155">InvalidRoleSetting</span></span>    | <span data-ttu-id="f693f-156">В тексте запроса указаны недопустимые значения [говернанцерулесеттингс](../resources/governancerulesetting.md) .</span><span class="sxs-lookup"><span data-stu-id="f693f-156">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="f693f-157">Пример</span><span class="sxs-lookup"><span data-stu-id="f693f-157">Example</span></span> 
<span data-ttu-id="f693f-158">В этом примере обновляется параметр Role для настраиваемой роли 3 в подписке Wingtip Toys — произ.</span><span class="sxs-lookup"><span data-stu-id="f693f-158">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="f693f-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="f693f-159">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f693f-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="f693f-160">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f693f-161">C#</span><span class="sxs-lookup"><span data-stu-id="f693f-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f693f-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f693f-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f693f-163">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f693f-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f693f-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="f693f-164">Response</span></span>
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
