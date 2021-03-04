---
title: Обновление авторизации
description: Обновление свойств объекта authorizationPolicy.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 12a55657266bb7cc8d757d6be85b0ab2c92c974a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438458"
---
# <a name="update-authorizationpolicy"></a><span data-ttu-id="55d31-103">Обновление авторизацииPolicy</span><span class="sxs-lookup"><span data-stu-id="55d31-103">Update authorizationPolicy</span></span>

<span data-ttu-id="55d31-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55d31-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55d31-105">Обновление свойств объекта [authorizationPolicy.](../resources/authorizationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="55d31-105">Update the properties of a [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="55d31-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="55d31-106">Permissions</span></span>

<span data-ttu-id="55d31-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55d31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="55d31-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55d31-109">Permission type</span></span>                        | <span data-ttu-id="55d31-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55d31-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="55d31-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55d31-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="55d31-112">Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="55d31-112">Policy.ReadWrite.Authorization</span></span>|
| <span data-ttu-id="55d31-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55d31-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55d31-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55d31-114">Not supported.</span></span> |
| <span data-ttu-id="55d31-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="55d31-115">Application</span></span>                            | <span data-ttu-id="55d31-116">Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="55d31-116">Policy.ReadWrite.Authorization</span></span>|

## <a name="http-request"></a><span data-ttu-id="55d31-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55d31-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="55d31-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55d31-118">Request headers</span></span>

| <span data-ttu-id="55d31-119">Имя</span><span class="sxs-lookup"><span data-stu-id="55d31-119">Name</span></span>       | <span data-ttu-id="55d31-120">Описание</span><span class="sxs-lookup"><span data-stu-id="55d31-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="55d31-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="55d31-121">Authorization</span></span> | <span data-ttu-id="55d31-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="55d31-122">Bearer {token}</span></span> |
| <span data-ttu-id="55d31-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="55d31-123">Content-type</span></span> | <span data-ttu-id="55d31-124">application/json</span><span class="sxs-lookup"><span data-stu-id="55d31-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="55d31-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55d31-125">Request body</span></span>

<span data-ttu-id="55d31-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="55d31-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="55d31-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="55d31-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="55d31-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="55d31-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="55d31-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="55d31-129">Property</span></span>     | <span data-ttu-id="55d31-130">Тип</span><span class="sxs-lookup"><span data-stu-id="55d31-130">Type</span></span>        | <span data-ttu-id="55d31-131">Описание</span><span class="sxs-lookup"><span data-stu-id="55d31-131">Description</span></span> |
|:-------------|:------------|:------------|  
|<span data-ttu-id="55d31-132">displayName</span><span class="sxs-lookup"><span data-stu-id="55d31-132">displayName</span></span>|<span data-ttu-id="55d31-133">String</span><span class="sxs-lookup"><span data-stu-id="55d31-133">String</span></span>| <span data-ttu-id="55d31-134">Отображение имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="55d31-134">Display name for this policy.</span></span> |  
|<span data-ttu-id="55d31-135">description</span><span class="sxs-lookup"><span data-stu-id="55d31-135">description</span></span>|<span data-ttu-id="55d31-136">String</span><span class="sxs-lookup"><span data-stu-id="55d31-136">String</span></span>| <span data-ttu-id="55d31-137">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="55d31-137">Description of this policy.</span></span> |  
|<span data-ttu-id="55d31-138">guestUserRoleId</span><span class="sxs-lookup"><span data-stu-id="55d31-138">guestUserRoleId</span></span>|<span data-ttu-id="55d31-139">Guid</span><span class="sxs-lookup"><span data-stu-id="55d31-139">Guid</span></span>| <span data-ttu-id="55d31-140">Представляет шаблон roleId для роли, которая должна быть предоставлена гостевому пользователю.</span><span class="sxs-lookup"><span data-stu-id="55d31-140">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="55d31-141">Чтобы найти список доступных шаблонов ролей, обратитесь к list [unifiedRoleDefinitions.](./rbacapplication-list-roledefinitions.md)</span><span class="sxs-lookup"><span data-stu-id="55d31-141">Refer to [List unifiedRoleDefinitions](./rbacapplication-list-roledefinitions.md) to find the list of available role templates.</span></span> <span data-ttu-id="55d31-142">Только поддерживаемые роли сегодня : Пользователь (a0b1b346-4d3e-4e8b-98f8-753987be4970), Гостевой пользователь (10dae51f-b6af-401 6-8d66-8c2a99b929b3) и ограниченный гость (2af84b1e-32c8-42b7-82bc-daa82404023b).</span><span class="sxs-lookup"><span data-stu-id="55d31-142">Only supported roles today are User (a0b1b346-4d3e-4e8b-98f8-753987be4970), Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3), and Restricted Guest User (2af84b1e-32c8-42b7-82bc-daa82404023b).</span></span> | 
|<span data-ttu-id="55d31-143">enabledPreviewFeatures</span><span class="sxs-lookup"><span data-stu-id="55d31-143">enabledPreviewFeatures</span></span>|<span data-ttu-id="55d31-144">Коллекция (строка)</span><span class="sxs-lookup"><span data-stu-id="55d31-144">Collection(string)</span></span>| <span data-ttu-id="55d31-145">Список функций, включенных для личного предварительного просмотра в клиенте.</span><span class="sxs-lookup"><span data-stu-id="55d31-145">List of features enabled for private preview on the tenant.</span></span> | 
|<span data-ttu-id="55d31-146">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="55d31-146">blockMsolPowerShell</span></span>|<span data-ttu-id="55d31-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="55d31-147">Boolean</span></span>| <span data-ttu-id="55d31-148">Чтобы отключить использование MSOL PowerShell, установите это свойство `true` .</span><span class="sxs-lookup"><span data-stu-id="55d31-148">To disable the use of MSOL PowerShell, set this property to `true`.</span></span> <span data-ttu-id="55d31-149">Настройка также отключит пользовательский доступ к конечной точке устаревшей `true` службы, используемой MSOL PowerShell.</span><span class="sxs-lookup"><span data-stu-id="55d31-149">Setting to `true` will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="55d31-150">Это не влияет на Azure AD Connect или Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="55d31-150">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="55d31-151">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="55d31-151">defaultUserRolePermissions</span></span>|[<span data-ttu-id="55d31-152">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="55d31-152">defaultUserRolePermissions</span></span>](../resources/defaultUserRolePermissions.md)| <span data-ttu-id="55d31-153">Указывает определенные настраиваемые разрешения для роли пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="55d31-153">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="55d31-154">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="55d31-154">allowedToUseSSPR</span></span>|<span data-ttu-id="55d31-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="55d31-155">Boolean</span></span>| <span data-ttu-id="55d31-156">Указывает, можно ли использовать Self-Serve сброса пароля пользователями клиента.</span><span class="sxs-lookup"><span data-stu-id="55d31-156">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="55d31-157">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="55d31-157">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="55d31-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="55d31-158">Boolean</span></span>| <span data-ttu-id="55d31-159">Указывает, могут ли пользователи подписываться на подписки на основе электронной почты.</span><span class="sxs-lookup"><span data-stu-id="55d31-159">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="55d31-160">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="55d31-160">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="55d31-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="55d31-161">Boolean</span></span>| <span data-ttu-id="55d31-162">Указывает, может ли пользователь присоединиться к клиенту по проверке электронной почты.</span><span class="sxs-lookup"><span data-stu-id="55d31-162">Indicates whether a user can join the tenant by email validation.</span></span> |
| <span data-ttu-id="55d31-163">permissionGrantPolicyIdsAssignedToDefaultUserRole</span><span class="sxs-lookup"><span data-stu-id="55d31-163">permissionGrantPolicyIdsAssignedToDefaultUserRole</span></span> | <span data-ttu-id="55d31-164">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="55d31-164">String collection</span></span> | <span data-ttu-id="55d31-165">Указывает, разрешено ли согласие пользователя на приложения, [](/azure/active-directory/manage-apps/manage-app-consent-policies) и если это так, то какая политика согласия приложения регулирует разрешение для пользователей на предоставление согласия.</span><span class="sxs-lookup"><span data-stu-id="55d31-165">Indicates whether user consent to apps is allowed, and if it is, which [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies) governs the permission for users to grant consent.</span></span> <span data-ttu-id="55d31-166">Значения должны быть в формате , где находится id встроенной или настраиваемой политики согласия `managePermissionGrantsForSelf.{id}` `{id}` [приложения.](/azure/active-directory/manage-apps/manage-app-consent-policies) </span><span class="sxs-lookup"><span data-stu-id="55d31-166">Values should be in the format `managePermissionGrantsForSelf.{id}`, where `{id}` is the **id** of a built-in or custom [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies).</span></span> <span data-ttu-id="55d31-167">Пустой список указывает, что согласие пользователя на приложения отключено.</span><span class="sxs-lookup"><span data-stu-id="55d31-167">An empty list indicates user consent to apps is disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="55d31-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="55d31-168">Response</span></span>

<span data-ttu-id="55d31-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="55d31-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="55d31-171">Примеры</span><span class="sxs-lookup"><span data-stu-id="55d31-171">Examples</span></span>

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a><span data-ttu-id="55d31-172">Пример 1. Обновление или настройка уровня доступа к гостевому пользователю для клиента</span><span class="sxs-lookup"><span data-stu-id="55d31-172">Example 1: Update or set Guest user access level for the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="55d31-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="55d31-173">Request</span></span>

<span data-ttu-id="55d31-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55d31-174">The following is an example of the request.</span></span> <span data-ttu-id="55d31-175">В этом примере уровень гостевого доступа изменен на ограниченный гостевой пользователь.</span><span class="sxs-lookup"><span data-stu-id="55d31-175">In this example, guest access level is modified to Restricted Guest User.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_guestUserLevel"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "guestUserRole":"2af84b1e-32c8-42b7-82bc-daa82404023b"
}
```

#### <a name="response"></a><span data-ttu-id="55d31-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="55d31-176">Response</span></span>

<span data-ttu-id="55d31-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="55d31-177">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-enable-new-feature-for-preview-on-tenant"></a><span data-ttu-id="55d31-178">Пример 2. Включить новую функцию для предварительного просмотра в клиенте</span><span class="sxs-lookup"><span data-stu-id="55d31-178">Example 2: Enable new feature for preview on tenant</span></span>

#### <a name="request"></a><span data-ttu-id="55d31-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="55d31-179">Request</span></span>

<span data-ttu-id="55d31-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55d31-180">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="55d31-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="55d31-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_preview"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "enabledPreviewFeatures":[
      "assignGroupsToRoles"
   ]
}
```
# <a name="c"></a>[<span data-ttu-id="55d31-182">C#</span><span class="sxs-lookup"><span data-stu-id="55d31-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-preview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55d31-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55d31-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-preview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55d31-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55d31-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-preview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55d31-185">Java</span><span class="sxs-lookup"><span data-stu-id="55d31-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-preview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="55d31-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="55d31-186">Response</span></span>

<span data-ttu-id="55d31-187">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="55d31-187">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-block-msol-powershell-in-tenant"></a><span data-ttu-id="55d31-188">Пример 3. Блок MSOL PowerShell в клиенте</span><span class="sxs-lookup"><span data-stu-id="55d31-188">Example 3: Block MSOL PowerShell in tenant</span></span>

#### <a name="request"></a><span data-ttu-id="55d31-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="55d31-189">Request</span></span>

<span data-ttu-id="55d31-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55d31-190">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="55d31-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="55d31-191">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_blockMSOLPowerShell"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "blockMsolPowerShell":true
}
```
# <a name="c"></a>[<span data-ttu-id="55d31-192">C#</span><span class="sxs-lookup"><span data-stu-id="55d31-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-blockmsolpowershell-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55d31-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55d31-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-blockmsolpowershell-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55d31-194">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55d31-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-blockmsolpowershell-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55d31-195">Java</span><span class="sxs-lookup"><span data-stu-id="55d31-195">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-blockmsolpowershell-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="55d31-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="55d31-196">Response</span></span>

<span data-ttu-id="55d31-197">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="55d31-197">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-4-disable-default-user-roles-permission-to-create-applications"></a><span data-ttu-id="55d31-198">Пример 4. Отключение разрешения роли пользователя по умолчанию на создание приложений</span><span class="sxs-lookup"><span data-stu-id="55d31-198">Example 4: Disable default user role's permission to create applications</span></span>

#### <a name="request"></a><span data-ttu-id="55d31-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="55d31-199">Request</span></span>

<span data-ttu-id="55d31-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55d31-200">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="55d31-201">HTTP</span><span class="sxs-lookup"><span data-stu-id="55d31-201">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_applications"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "defaultUserRolePermissions":{
      "allowedToCreateApps":false
   }
}
```
# <a name="c"></a>[<span data-ttu-id="55d31-202">C#</span><span class="sxs-lookup"><span data-stu-id="55d31-202">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55d31-203">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55d31-203">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55d31-204">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55d31-204">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55d31-205">Java</span><span class="sxs-lookup"><span data-stu-id="55d31-205">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-applications-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="55d31-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="55d31-206">Response</span></span>

<span data-ttu-id="55d31-207">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="55d31-207">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-5-enable-default-user-role-to-use-self-serve-password-reset-feature"></a><span data-ttu-id="55d31-208">Пример 5. Включить роль пользователя по умолчанию для использования функции Self-Serve сброса пароля</span><span class="sxs-lookup"><span data-stu-id="55d31-208">Example 5: Enable default user role to use Self-Serve Password Reset feature</span></span>

#### <a name="request"></a><span data-ttu-id="55d31-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="55d31-209">Request</span></span>

<span data-ttu-id="55d31-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55d31-210">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="55d31-211">HTTP</span><span class="sxs-lookup"><span data-stu-id="55d31-211">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_SSPR"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "allowedToUseSSPR":true
}
```
# <a name="c"></a>[<span data-ttu-id="55d31-212">C#</span><span class="sxs-lookup"><span data-stu-id="55d31-212">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-sspr-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55d31-213">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55d31-213">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-sspr-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55d31-214">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55d31-214">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-sspr-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55d31-215">Java</span><span class="sxs-lookup"><span data-stu-id="55d31-215">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-sspr-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="55d31-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="55d31-216">Response</span></span>

<span data-ttu-id="55d31-217">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="55d31-217">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-6-disable-user-consent-to-apps-for-default-user-role"></a><span data-ttu-id="55d31-218">Пример 6. Отключение согласия пользователя на приложения для роли пользователя по умолчанию</span><span class="sxs-lookup"><span data-stu-id="55d31-218">Example 6: Disable user consent to apps for default user role</span></span>

#### <a name="request"></a><span data-ttu-id="55d31-219">Запрос</span><span class="sxs-lookup"><span data-stu-id="55d31-219">Request</span></span>

<span data-ttu-id="55d31-220">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55d31-220">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="55d31-221">HTTP</span><span class="sxs-lookup"><span data-stu-id="55d31-221">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_disableUserConsent"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "permissionGrantPolicyIdsAssignedToDefaultUserRole":[
   
   ]
}
```
# <a name="c"></a>[<span data-ttu-id="55d31-222">C#</span><span class="sxs-lookup"><span data-stu-id="55d31-222">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-disableuserconsent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55d31-223">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55d31-223">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-disableuserconsent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55d31-224">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55d31-224">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-disableuserconsent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55d31-225">Java</span><span class="sxs-lookup"><span data-stu-id="55d31-225">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-disableuserconsent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="55d31-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="55d31-226">Response</span></span>

<span data-ttu-id="55d31-227">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="55d31-227">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-7-enable-user-consent-to-apps-subject-to-app-consent-policy"></a><span data-ttu-id="55d31-228">Пример 7. Включить согласие пользователя на приложения с учетом политики согласия на приложения</span><span class="sxs-lookup"><span data-stu-id="55d31-228">Example 7: Enable user consent to apps, subject to app consent policy</span></span> 

#### <a name="request"></a><span data-ttu-id="55d31-229">Запрос</span><span class="sxs-lookup"><span data-stu-id="55d31-229">Request</span></span>

<span data-ttu-id="55d31-230">Ниже приводится пример запроса, который позволяет получить согласие пользователя на [](/azure/active-directory/manage-apps/manage-app-consent-policies) приложения при условии политики согласия на встроенные приложения, которая позволяет делегировать разрешения, классифицированные "низко", для клиентских приложений от проверенных издателей или зарегистрированных в том же `microsoft-user-default-low` клиенте.</span><span class="sxs-lookup"><span data-stu-id="55d31-230">The following is an example of the request that allows user consent to apps, subject to the built-in [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies) `microsoft-user-default-low`, which allows delegated permissions classified "low", for client apps from verified publishers or registered in the same tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="55d31-231">HTTP</span><span class="sxs-lookup"><span data-stu-id="55d31-231">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_enableUserConsentLow"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
   "permissionGrantPolicyIdsAssignedToDefaultUserRole":[
      "managePermissionGrantsForSelf.microsoft-user-default-low"
   ]
}
```
# <a name="c"></a>[<span data-ttu-id="55d31-232">C#</span><span class="sxs-lookup"><span data-stu-id="55d31-232">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-enableuserconsentlow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55d31-233">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55d31-233">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-enableuserconsentlow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55d31-234">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55d31-234">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-enableuserconsentlow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55d31-235">Java</span><span class="sxs-lookup"><span data-stu-id="55d31-235">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-enableuserconsentlow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="55d31-236">Отклик</span><span class="sxs-lookup"><span data-stu-id="55d31-236">Response</span></span>

<span data-ttu-id="55d31-237">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="55d31-237">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationpolicy"
} -->

```http
HTTP/1.1 204 No Content
```
