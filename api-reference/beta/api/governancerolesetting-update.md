---
title: Обновление Говернанцеролесеттинг
description: Обновление свойств объекта Говернанцеролесеттинг.
localization_priority: Normal
ms.openlocfilehash: 6f6b9d0fb565532a4f610c6434843c1f09aa259d
ms.sourcegitcommit: f80282ff00d5aafc3e575bce447543d7dd23963d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/23/2019
ms.locfileid: "34422292"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="86a83-103">Обновление Говернанцеролесеттинг</span><span class="sxs-lookup"><span data-stu-id="86a83-103">Update governanceRoleSetting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86a83-104">Обновление свойств объекта [говернанцеролесеттинг](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="86a83-104">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="86a83-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="86a83-105">Permissions</span></span>
<span data-ttu-id="86a83-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86a83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="86a83-108">**Примечание:** Этот API также требует, чтобы у автора запроса было по `Active` крайней мере одно`owner` назначение `user access administrator`роли администратора (или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="86a83-108">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="86a83-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86a83-109">Permission type</span></span>      | <span data-ttu-id="86a83-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="86a83-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86a83-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86a83-111">Delegated (work or school account)</span></span> | <span data-ttu-id="86a83-112">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="86a83-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="86a83-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86a83-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86a83-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86a83-114">Not supported.</span></span>    |
|<span data-ttu-id="86a83-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86a83-115">Application</span></span> | <span data-ttu-id="86a83-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86a83-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="86a83-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86a83-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="86a83-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="86a83-118">Request headers</span></span>
| <span data-ttu-id="86a83-119">Имя</span><span class="sxs-lookup"><span data-stu-id="86a83-119">Name</span></span>       | <span data-ttu-id="86a83-120">Описание</span><span class="sxs-lookup"><span data-stu-id="86a83-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="86a83-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86a83-121">Authorization</span></span>  | <span data-ttu-id="86a83-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="86a83-122">Bearer {code}</span></span>|
| <span data-ttu-id="86a83-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="86a83-123">Content-type</span></span>  | <span data-ttu-id="86a83-124">application/json</span><span class="sxs-lookup"><span data-stu-id="86a83-124">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="86a83-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="86a83-125">Request body</span></span>
<span data-ttu-id="86a83-126">В тексте запроса укажите значения для [говернанцерулесеттингс](../resources/governancerulesetting.md) , которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="86a83-126">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="86a83-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="86a83-127">Property</span></span>     | <span data-ttu-id="86a83-128">Тип</span><span class="sxs-lookup"><span data-stu-id="86a83-128">Type</span></span>   |<span data-ttu-id="86a83-129">Описание</span><span class="sxs-lookup"><span data-stu-id="86a83-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86a83-130">Админелигиблесеттингс</span><span class="sxs-lookup"><span data-stu-id="86a83-130">adminEligibleSettings</span></span>|<span data-ttu-id="86a83-131">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="86a83-131">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="86a83-132">Параметры правил, которые оцениваются, когда администратор пытается добавить подходящего назначения роли.</span><span class="sxs-lookup"><span data-stu-id="86a83-132">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="86a83-133">Админмемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="86a83-133">adminMemberSettings</span></span>|<span data-ttu-id="86a83-134">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="86a83-134">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="86a83-135">Параметры правил, которые оцениваются при попытке администратора добавить назначение роли прямого члена.</span><span class="sxs-lookup"><span data-stu-id="86a83-135">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="86a83-136">Усерелигиблесеттингс</span><span class="sxs-lookup"><span data-stu-id="86a83-136">userEligibleSettings</span></span>|<span data-ttu-id="86a83-137">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="86a83-137">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="86a83-138">Параметры правил, которые оцениваются, когда пользователь пытается добавить подходящего назначения роли.</span><span class="sxs-lookup"><span data-stu-id="86a83-138">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="86a83-139">В настоящее время этот `pimforazurerbac` сценарий не поддерживается и может быть доступен в следующих сценариях.</span><span class="sxs-lookup"><span data-stu-id="86a83-139">This is not supported for `pimforazurerbac` scenario for now, and may be available in the future scenarios.</span></span>|
|<span data-ttu-id="86a83-140">Усермемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="86a83-140">userMemberSettings</span></span>|<span data-ttu-id="86a83-141">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="86a83-141">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="86a83-142">Параметры правил, которые оцениваются, когда пользователь пытается активировать назначение роли.</span><span class="sxs-lookup"><span data-stu-id="86a83-142">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="86a83-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="86a83-143">Response</span></span>
<span data-ttu-id="86a83-p103">При успешном выполнении этот метод возвращает код отклика `204 NoContent`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="86a83-p103">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="86a83-146">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="86a83-146">Error codes</span></span>
<span data-ttu-id="86a83-147">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="86a83-147">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="86a83-148">Кроме того, возвращаются следующие коды настраиваемых ошибок.</span><span class="sxs-lookup"><span data-stu-id="86a83-148">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="86a83-149">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="86a83-149">Error code</span></span>     | <span data-ttu-id="86a83-150">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="86a83-150">Error message</span></span>         | <span data-ttu-id="86a83-151">Сведения</span><span class="sxs-lookup"><span data-stu-id="86a83-151">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="86a83-152">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="86a83-152">400 BadRequest</span></span>| <span data-ttu-id="86a83-153">Ролесеттингнотфаунд</span><span class="sxs-lookup"><span data-stu-id="86a83-153">RoleSettingNotFound</span></span>   | <span data-ttu-id="86a83-154">[Говернанцеролесеттинг](../resources/governancerolesetting.md) не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="86a83-154">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="86a83-155">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="86a83-155">400 BadRequest</span></span>| <span data-ttu-id="86a83-156">Инвалидролесеттинг</span><span class="sxs-lookup"><span data-stu-id="86a83-156">InvalidRoleSetting</span></span>    | <span data-ttu-id="86a83-157">В тексте запроса указаны недопустимые значения [говернанцерулесеттингс](../resources/governancerulesetting.md) .</span><span class="sxs-lookup"><span data-stu-id="86a83-157">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="86a83-158">Пример</span><span class="sxs-lookup"><span data-stu-id="86a83-158">Example</span></span> 
<span data-ttu-id="86a83-159">В этом примере обновляется параметр Role для настраиваемой роли 3 в подписке Wingtip Toys — произ.</span><span class="sxs-lookup"><span data-stu-id="86a83-159">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="86a83-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="86a83-160">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_governancerolesetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedAccess/pimforazurerbac/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5
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
##### <a name="response"></a><span data-ttu-id="86a83-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="86a83-161">Response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="86a83-162">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="86a83-162">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="86a83-163">C#</span><span class="sxs-lookup"><span data-stu-id="86a83-163">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_governancerolesetting-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="86a83-164">Javascript</span><span class="sxs-lookup"><span data-stu-id="86a83-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_governancerolesetting-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/governancerolesetting-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governancerolesetting-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
