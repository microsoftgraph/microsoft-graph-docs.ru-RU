---
title: Обновление Говернанцеролесеттинг
description: Обновление свойств объекта Говернанцеролесеттинг.
localization_priority: Normal
ms.openlocfilehash: d002317a4bf626f9a60cf98f6bd73b2075bf5727
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329709"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="ba511-103">Обновление Говернанцеролесеттинг</span><span class="sxs-lookup"><span data-stu-id="ba511-103">Update governanceRoleSetting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba511-104">Обновление свойств объекта [говернанцеролесеттинг](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="ba511-104">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ba511-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba511-105">Permissions</span></span>
<span data-ttu-id="ba511-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba511-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="ba511-108">**Примечание:** Этот API также требует, чтобы у автора запроса было по `Active` крайней мере одно`owner` назначение `user access administrator`роли администратора (или) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="ba511-108">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="ba511-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba511-109">Permission type</span></span>      | <span data-ttu-id="ba511-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba511-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba511-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba511-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ba511-112">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="ba511-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="ba511-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba511-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba511-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba511-114">Not supported.</span></span>    |
|<span data-ttu-id="ba511-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba511-115">Application</span></span> | <span data-ttu-id="ba511-116">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="ba511-116">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba511-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba511-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ba511-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba511-118">Request headers</span></span>
| <span data-ttu-id="ba511-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ba511-119">Name</span></span>       | <span data-ttu-id="ba511-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ba511-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ba511-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba511-121">Authorization</span></span>  | <span data-ttu-id="ba511-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ba511-122">Bearer {code}</span></span>|
| <span data-ttu-id="ba511-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba511-123">Content-type</span></span>  | <span data-ttu-id="ba511-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ba511-124">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="ba511-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba511-125">Request body</span></span>
<span data-ttu-id="ba511-126">В тексте запроса укажите значения для [говернанцерулесеттингс](../resources/governancerulesetting.md) , которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="ba511-126">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="ba511-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba511-127">Property</span></span>     | <span data-ttu-id="ba511-128">Тип</span><span class="sxs-lookup"><span data-stu-id="ba511-128">Type</span></span>   |<span data-ttu-id="ba511-129">Описание</span><span class="sxs-lookup"><span data-stu-id="ba511-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba511-130">Админелигиблесеттингс</span><span class="sxs-lookup"><span data-stu-id="ba511-130">adminEligibleSettings</span></span>|<span data-ttu-id="ba511-131">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="ba511-131">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="ba511-132">Параметры правил, которые оцениваются, когда администратор пытается добавить подходящего назначения роли.</span><span class="sxs-lookup"><span data-stu-id="ba511-132">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="ba511-133">Админмемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="ba511-133">adminMemberSettings</span></span>|<span data-ttu-id="ba511-134">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="ba511-134">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="ba511-135">Параметры правил, которые оцениваются при попытке администратора добавить назначение роли прямого члена.</span><span class="sxs-lookup"><span data-stu-id="ba511-135">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="ba511-136">Усерелигиблесеттингс</span><span class="sxs-lookup"><span data-stu-id="ba511-136">userEligibleSettings</span></span>|<span data-ttu-id="ba511-137">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="ba511-137">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="ba511-138">Параметры правил, которые оцениваются, когда пользователь пытается добавить подходящего назначения роли.</span><span class="sxs-lookup"><span data-stu-id="ba511-138">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="ba511-139">В настоящее время этот `pimforazurerbac` сценарий не поддерживается и может быть доступен в следующих сценариях.</span><span class="sxs-lookup"><span data-stu-id="ba511-139">This is not supported for `pimforazurerbac` scenario for now, and may be available in the future scenarios.</span></span>|
|<span data-ttu-id="ba511-140">Усермемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="ba511-140">userMemberSettings</span></span>|<span data-ttu-id="ba511-141">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="ba511-141">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="ba511-142">Параметры правил, которые оцениваются, когда пользователь пытается активировать назначение роли.</span><span class="sxs-lookup"><span data-stu-id="ba511-142">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="ba511-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba511-143">Response</span></span>
<span data-ttu-id="ba511-p103">При успешном выполнении этот метод возвращает код отклика `204 NoContent`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ba511-p103">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="ba511-146">Коды ошибок</span><span class="sxs-lookup"><span data-stu-id="ba511-146">Error codes</span></span>
<span data-ttu-id="ba511-147">Этот API возвращает стандартные коды ошибок HTTP.</span><span class="sxs-lookup"><span data-stu-id="ba511-147">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="ba511-148">Кроме того, возвращаются следующие коды настраиваемых ошибок.</span><span class="sxs-lookup"><span data-stu-id="ba511-148">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="ba511-149">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="ba511-149">Error code</span></span>     | <span data-ttu-id="ba511-150">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="ba511-150">Error message</span></span>         | <span data-ttu-id="ba511-151">Сведения</span><span class="sxs-lookup"><span data-stu-id="ba511-151">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="ba511-152">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="ba511-152">400 BadRequest</span></span>| <span data-ttu-id="ba511-153">Ролесеттингнотфаунд</span><span class="sxs-lookup"><span data-stu-id="ba511-153">RoleSettingNotFound</span></span>   | <span data-ttu-id="ba511-154">[Говернанцеролесеттинг](../resources/governancerolesetting.md) не существует в системе.</span><span class="sxs-lookup"><span data-stu-id="ba511-154">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="ba511-155">400 Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="ba511-155">400 BadRequest</span></span>| <span data-ttu-id="ba511-156">Инвалидролесеттинг</span><span class="sxs-lookup"><span data-stu-id="ba511-156">InvalidRoleSetting</span></span>    | <span data-ttu-id="ba511-157">В тексте запроса указаны недопустимые значения [говернанцерулесеттингс](../resources/governancerulesetting.md) .</span><span class="sxs-lookup"><span data-stu-id="ba511-157">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="ba511-158">Пример</span><span class="sxs-lookup"><span data-stu-id="ba511-158">Example</span></span> 
<span data-ttu-id="ba511-159">В этом примере обновляется параметр Role для настраиваемой роли 3 в подписке Wingtip Toys — произ.</span><span class="sxs-lookup"><span data-stu-id="ba511-159">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="ba511-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba511-160">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="ba511-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba511-161">Response</span></span>
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
  "suppressions": []
}
-->
