---
title: Обновление itemInsights
description: Обновление свойств объекта itemInsightsSettings
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 0eb17d9e0a4f3285858800f32e6954bbd344dc27
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053036"
---
# <a name="update-iteminsightssettings"></a><span data-ttu-id="45065-103">Обновление itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="45065-103">Update itemInsightsSettings</span></span>

<span data-ttu-id="45065-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45065-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45065-105">Обновление свойств указанного [ресурса itemInsightsSettings.](../resources/iteminsightssettings.md)</span><span class="sxs-lookup"><span data-stu-id="45065-105">Update properties of the specified [itemInsightsSettings](../resources/iteminsightssettings.md) resource.</span></span>

<span data-ttu-id="45065-106">Сведения о настройке конфиденциальности элементов для организации см. в статье [Настройка конфиденциальности .](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0)</span><span class="sxs-lookup"><span data-stu-id="45065-106">To learn how to customize item insights privacy for your organization, see [customize insights privacy](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0).</span></span> 

## <a name="permissions"></a><span data-ttu-id="45065-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="45065-107">Permissions</span></span>

<span data-ttu-id="45065-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45065-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45065-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45065-110">Permission type</span></span>      | <span data-ttu-id="45065-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="45065-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45065-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45065-112">Delegated (work or school account)</span></span> | <span data-ttu-id="45065-113">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45065-113">User.ReadWrite.All</span></span> |
|<span data-ttu-id="45065-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45065-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45065-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45065-115">Not supported.</span></span>    |
|<span data-ttu-id="45065-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45065-116">Application</span></span> | <span data-ttu-id="45065-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45065-117">Not supported.</span></span> |

><span data-ttu-id="45065-118">**Примечание:** Использование делегирования разрешений для этой операции требует от пользователя, вписаного, роли глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="45065-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="45065-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45065-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{organizationId}/settings/itemInsights
```

## <a name="request-headers"></a><span data-ttu-id="45065-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45065-120">Request headers</span></span>

| <span data-ttu-id="45065-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45065-121">Header</span></span>       | <span data-ttu-id="45065-122">Значение</span><span class="sxs-lookup"><span data-stu-id="45065-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="45065-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45065-123">Authorization</span></span>  | <span data-ttu-id="45065-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45065-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="45065-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="45065-126">Content-Type</span></span>  | <span data-ttu-id="45065-127">application/json</span><span class="sxs-lookup"><span data-stu-id="45065-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="45065-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45065-128">Request body</span></span>

<span data-ttu-id="45065-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="45065-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="45065-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="45065-132">Property</span></span>     | <span data-ttu-id="45065-133">Тип</span><span class="sxs-lookup"><span data-stu-id="45065-133">Type</span></span>   |<span data-ttu-id="45065-134">Описание</span><span class="sxs-lookup"><span data-stu-id="45065-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45065-135">isEnabledInOrganization</span><span class="sxs-lookup"><span data-stu-id="45065-135">isEnabledInOrganization</span></span>|<span data-ttu-id="45065-136">Логический</span><span class="sxs-lookup"><span data-stu-id="45065-136">Boolean</span></span>| <span data-ttu-id="45065-137">`true` если включена информация о элементах организации; `false` если сведения о элементах организации отключены для всех пользователей без исключений.</span><span class="sxs-lookup"><span data-stu-id="45065-137">`true` if organization item insights are enabled; `false` if organization item insights are disabled for all users without exceptions.</span></span> <span data-ttu-id="45065-138">Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="45065-138">Default is `true`.</span></span> <span data-ttu-id="45065-139">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="45065-139">Optional.</span></span>|
|<span data-ttu-id="45065-140">disabledForGroup</span><span class="sxs-lookup"><span data-stu-id="45065-140">disabledForGroup</span></span>|<span data-ttu-id="45065-141">String</span><span class="sxs-lookup"><span data-stu-id="45065-141">String</span></span>| <span data-ttu-id="45065-142">ID группы Azure AD, из которой отключены сведения о элементах участников.</span><span class="sxs-lookup"><span data-stu-id="45065-142">The ID of an Azure AD group, of which the members' item insights are disabled.</span></span> <span data-ttu-id="45065-143">Значение по умолчанию: `empty`.</span><span class="sxs-lookup"><span data-stu-id="45065-143">Default is `empty`.</span></span> <span data-ttu-id="45065-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="45065-144">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="45065-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="45065-145">Response</span></span>

<span data-ttu-id="45065-146">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект itemInsightsSettings](../resources/iteminsightssettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="45065-146">If successful, this method returns a `200 OK` response code and [itemInsightsSettings](../resources/iteminsightssettings.md) object in the response body.</span></span>

><span data-ttu-id="45065-147">**Примечание:** Эта операция проверяет достоверность значений свойств указанного ресурса **itemInsightsSettings.**</span><span class="sxs-lookup"><span data-stu-id="45065-147">**Note:** This operation verifies the validity of property values of the specified **itemInsightsSettings** resource.</span></span> <span data-ttu-id="45065-148">Если свойство **отключеноForGroup,** эта операция не проверяет наличие соответствующей группы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="45065-148">If the **disabledForGroup** property is set, this operation does not check the existence of the corresponding Azure AD Group.</span></span> <span data-ttu-id="45065-149">Это означает, что если вы установите **disabledForGroup** в группу Azure AD, которая не существовала или была удалена после этого, эта операция не сможет идентифицировать членство в группе и отключить сведения о элементах для определенных пользователей.</span><span class="sxs-lookup"><span data-stu-id="45065-149">This means, if you set **disabledForGroup** to an Azure AD group that did not exist or was deleted afterwards, this operation will not be able to identify any group membership and disable item insights for any specific users.</span></span> <span data-ttu-id="45065-150">Если **установлено isEnabledInOrganization,** операция позволит получить сведения для всех `true` пользователей организации.</span><span class="sxs-lookup"><span data-stu-id="45065-150">If **isEnabledInOrganization** is set to `true`, the operation will enable insights for all the users in the organization.</span></span> 

## <a name="example"></a><span data-ttu-id="45065-151">Пример</span><span class="sxs-lookup"><span data-stu-id="45065-151">Example</span></span> 

### <a name="request"></a><span data-ttu-id="45065-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="45065-152">Request</span></span>

<span data-ttu-id="45065-153">Вот пример запроса на то, как администратор обновляет параметр конфиденциальности **"disabledForGroup",** чтобы запретить отображать сведения о элементах пользователей определенной группы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="45065-153">Here is an example request on how admin updates "**disabledForGroup**" privacy setting in order to prohibit displaying users' item insights of a particular Azure AD group.</span></span>

# <a name="http"></a>[<span data-ttu-id="45065-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="45065-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_iteminsightssettings"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/itemInsights
Content-type: application/json

{
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```
# <a name="javascript"></a>[<span data-ttu-id="45065-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45065-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-iteminsightssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="45065-156">C#</span><span class="sxs-lookup"><span data-stu-id="45065-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-iteminsightssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45065-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45065-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-iteminsightssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45065-158">Java</span><span class="sxs-lookup"><span data-stu-id="45065-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-iteminsightssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="45065-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="45065-159">Response</span></span>

<span data-ttu-id="45065-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="45065-160">Here is an example of the response.</span></span> <span data-ttu-id="45065-161">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="45065-161">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemInsightsSettings",
  "name": "update_iteminsightssettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabledInOrganization": true,
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```


