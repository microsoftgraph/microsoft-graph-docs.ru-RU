---
title: Обновление аусоризатионполици
description: Обновление свойств объекта Аусоризатионполици.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d4f8bd9053db7b58e3aec81e82a5d0c2d20c2407
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48312423"
---
# <a name="update-authorizationpolicy"></a><span data-ttu-id="6f095-103">Обновление Аусоризатионполици</span><span class="sxs-lookup"><span data-stu-id="6f095-103">Update authorizationPolicy</span></span>

<span data-ttu-id="6f095-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f095-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f095-105">Обновление свойств объекта [аусоризатионполици](../resources/authorizationpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="6f095-105">Update the properties of a [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f095-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f095-106">Permissions</span></span>

<span data-ttu-id="6f095-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f095-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6f095-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f095-109">Permission type</span></span>                        | <span data-ttu-id="6f095-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f095-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6f095-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f095-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6f095-112">Policy. ReadWrite. Authorization</span><span class="sxs-lookup"><span data-stu-id="6f095-112">Policy.ReadWrite.Authorization</span></span>|
| <span data-ttu-id="6f095-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f095-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f095-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f095-114">Not supported.</span></span> |
| <span data-ttu-id="6f095-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f095-115">Application</span></span>                            | <span data-ttu-id="6f095-116">Policy. ReadWrite. Authorization</span><span class="sxs-lookup"><span data-stu-id="6f095-116">Policy.ReadWrite.Authorization</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f095-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f095-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="6f095-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f095-118">Request headers</span></span>

| <span data-ttu-id="6f095-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6f095-119">Name</span></span>       | <span data-ttu-id="6f095-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6f095-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6f095-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f095-121">Authorization</span></span> | <span data-ttu-id="6f095-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="6f095-122">Bearer {token}</span></span> |
| <span data-ttu-id="6f095-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6f095-123">Content-type</span></span> | <span data-ttu-id="6f095-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6f095-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f095-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f095-125">Request body</span></span>

<span data-ttu-id="6f095-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="6f095-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6f095-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="6f095-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6f095-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6f095-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6f095-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f095-129">Property</span></span>     | <span data-ttu-id="6f095-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6f095-130">Type</span></span>        | <span data-ttu-id="6f095-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6f095-131">Description</span></span> |
|:-------------|:------------|:------------|  
|<span data-ttu-id="6f095-132">displayName</span><span class="sxs-lookup"><span data-stu-id="6f095-132">displayName</span></span>|<span data-ttu-id="6f095-133">String</span><span class="sxs-lookup"><span data-stu-id="6f095-133">String</span></span>| <span data-ttu-id="6f095-134">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6f095-134">Display name for this policy.</span></span> |  
|<span data-ttu-id="6f095-135">description</span><span class="sxs-lookup"><span data-stu-id="6f095-135">description</span></span>|<span data-ttu-id="6f095-136">String</span><span class="sxs-lookup"><span data-stu-id="6f095-136">String</span></span>| <span data-ttu-id="6f095-137">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="6f095-137">Description of this policy.</span></span> |  
|<span data-ttu-id="6f095-138">гуестусерролеид</span><span class="sxs-lookup"><span data-stu-id="6f095-138">guestUserRoleId</span></span>|<span data-ttu-id="6f095-139">Guid</span><span class="sxs-lookup"><span data-stu-id="6f095-139">Guid</span></span>| <span data-ttu-id="6f095-140">Представляет templateId роли для роли, которая должна быть выделена пользователю "гость".</span><span class="sxs-lookup"><span data-stu-id="6f095-140">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="6f095-141">Обратитесь к [списку унифиедроледефинитионс](./rbacapplication-list-roledefinitions.md) , чтобы найти список доступных шаблонов ролей.</span><span class="sxs-lookup"><span data-stu-id="6f095-141">Refer to [List unifiedRoleDefinitions](./rbacapplication-list-roledefinitions.md) to find the list of available role templates.</span></span> <span data-ttu-id="6f095-142">Только поддерживаемые роли: User (a0b1b346-4d3e-4e8b-98f8-753987be4970), гость (10dae51f-b6af-4016-8d66-8c2a99b929b3) и пользователь с ограниченным гостями (2af84b1e-32c8-42b7-82bc-daa82404023b).</span><span class="sxs-lookup"><span data-stu-id="6f095-142">Only supported roles today are User (a0b1b346-4d3e-4e8b-98f8-753987be4970), Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3), and Restricted Guest User (2af84b1e-32c8-42b7-82bc-daa82404023b).</span></span> | 
|<span data-ttu-id="6f095-143">енабледпревиевфеатурес</span><span class="sxs-lookup"><span data-stu-id="6f095-143">enabledPreviewFeatures</span></span>|<span data-ttu-id="6f095-144">Коллекция (String)</span><span class="sxs-lookup"><span data-stu-id="6f095-144">Collection(string)</span></span>| <span data-ttu-id="6f095-145">Список компонентов, включенных для закрытой предварительной версии в клиенте.</span><span class="sxs-lookup"><span data-stu-id="6f095-145">List of features enabled for private preview on the tenant.</span></span> | 
|<span data-ttu-id="6f095-146">блоккмсолповершелл</span><span class="sxs-lookup"><span data-stu-id="6f095-146">blockMsolPowerShell</span></span>|<span data-ttu-id="6f095-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f095-147">Boolean</span></span>| <span data-ttu-id="6f095-148">Чтобы отключить использование MSOL PowerShell, задайте для этого свойства значение `true` .</span><span class="sxs-lookup"><span data-stu-id="6f095-148">To disable the use of MSOL PowerShell, set this property to `true`.</span></span> <span data-ttu-id="6f095-149">Параметр `true` также отключит доступ пользователей к устаревшей конечной точке службы, используемой MSOL PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6f095-149">Setting to `true` will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="6f095-150">Это не повлияет на Azure AD Connect или Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6f095-150">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="6f095-151">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="6f095-151">defaultUserRolePermissions</span></span>|[<span data-ttu-id="6f095-152">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="6f095-152">defaultUserRolePermissions</span></span>](../resources/defaultUserRolePermissions.md)| <span data-ttu-id="6f095-153">Задает определенные настраиваемые разрешения для роли пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6f095-153">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="6f095-154">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="6f095-154">allowedToUseSSPR</span></span>|<span data-ttu-id="6f095-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f095-155">Boolean</span></span>| <span data-ttu-id="6f095-156">Указывает, можно ли использовать функцию самостоятельного сброса пароля для пользователей клиента.</span><span class="sxs-lookup"><span data-stu-id="6f095-156">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="6f095-157">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="6f095-157">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="6f095-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f095-158">Boolean</span></span>| <span data-ttu-id="6f095-159">Указывает, могут ли пользователи регистрироваться на почтовые подписки.</span><span class="sxs-lookup"><span data-stu-id="6f095-159">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="6f095-160">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="6f095-160">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="6f095-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f095-161">Boolean</span></span>| <span data-ttu-id="6f095-162">Указывает, может ли пользователь присоединиться к клиенту по проверке электронной почты.</span><span class="sxs-lookup"><span data-stu-id="6f095-162">Indicates whether a user can join the tenant by email validation.</span></span> | 

## <a name="response"></a><span data-ttu-id="6f095-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f095-163">Response</span></span>

<span data-ttu-id="6f095-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6f095-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6f095-166">Примеры</span><span class="sxs-lookup"><span data-stu-id="6f095-166">Examples</span></span>

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a><span data-ttu-id="6f095-167">Пример 1: обновление или Настройка уровня доступа гостей для клиента</span><span class="sxs-lookup"><span data-stu-id="6f095-167">Example 1: Update or set Guest user access level for the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="6f095-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f095-168">Request</span></span>

<span data-ttu-id="6f095-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f095-169">The following is an example of the request.</span></span> <span data-ttu-id="6f095-170">В этом примере уровень гостевого доступа изменяется на "ограниченный гостевой пользователь".</span><span class="sxs-lookup"><span data-stu-id="6f095-170">In this example, guest access level is modified to Restricted Guest User.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_guestUserLevel"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
  "guestUserRole": "2af84b1e-32c8-42b7-82bc-daa82404023b"
}

```
#### <a name="response"></a><span data-ttu-id="6f095-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f095-171">Response</span></span>

<span data-ttu-id="6f095-172">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6f095-172">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content

```

### <a name="example-2-enable-new-feature-for-preview-on-tenant"></a><span data-ttu-id="6f095-173">Пример 2: включение новой функции для предварительного просмотра в клиенте</span><span class="sxs-lookup"><span data-stu-id="6f095-173">Example 2: Enable new feature for preview on tenant</span></span>

#### <a name="request"></a><span data-ttu-id="6f095-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f095-174">Request</span></span>

<span data-ttu-id="6f095-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f095-175">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f095-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f095-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_preview"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
  "enabledPreviewFeatures": ["assignGroupsToRoles"]
}

```
# <a name="c"></a>[<span data-ttu-id="6f095-177">C#</span><span class="sxs-lookup"><span data-stu-id="6f095-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-preview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f095-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f095-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-preview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f095-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f095-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-preview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6f095-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f095-180">Response</span></span>

<span data-ttu-id="6f095-181">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6f095-181">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```


### <a name="example-3-block-msol-powershell-in-tenant"></a><span data-ttu-id="6f095-182">Пример 3: Блокировка MSOL PowerShell в клиенте</span><span class="sxs-lookup"><span data-stu-id="6f095-182">Example 3: Block MSOL PowerShell in tenant</span></span>

#### <a name="request"></a><span data-ttu-id="6f095-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f095-183">Request</span></span>

<span data-ttu-id="6f095-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f095-184">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f095-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f095-185">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_blockMSOLPowerShell"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
  "blockMsolPowerShell": true
}

```
# <a name="c"></a>[<span data-ttu-id="6f095-186">C#</span><span class="sxs-lookup"><span data-stu-id="6f095-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-blockmsolpowershell-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f095-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f095-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-blockmsolpowershell-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f095-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f095-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-blockmsolpowershell-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6f095-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f095-189">Response</span></span>

<span data-ttu-id="6f095-190">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6f095-190">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```
### <a name="example-4-disable-default-user-roles-permission-to-create-applications"></a><span data-ttu-id="6f095-191">Пример 4: отключение разрешения роли пользователя по умолчанию для создания приложений</span><span class="sxs-lookup"><span data-stu-id="6f095-191">Example 4: Disable default user role's permission to create applications</span></span>

#### <a name="request"></a><span data-ttu-id="6f095-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f095-192">Request</span></span>

<span data-ttu-id="6f095-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f095-193">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f095-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f095-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_applications"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
    "defaultUserRolePermissions":
    {
      "allowedToCreateApps": false
    }
}

```
# <a name="c"></a>[<span data-ttu-id="6f095-195">C#</span><span class="sxs-lookup"><span data-stu-id="6f095-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f095-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f095-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f095-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f095-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6f095-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f095-198">Response</span></span>

<span data-ttu-id="6f095-199">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6f095-199">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-5-enable-default-user-role-to-use-self-serve-password-reset-feature"></a><span data-ttu-id="6f095-200">Пример 5: Включение роли пользователя по умолчанию для использования функции самостоятельного сброса пароля</span><span class="sxs-lookup"><span data-stu-id="6f095-200">Example 5: Enable default user role to use Self-Serve Password Reset feature</span></span>

#### <a name="request"></a><span data-ttu-id="6f095-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f095-201">Request</span></span>

<span data-ttu-id="6f095-202">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f095-202">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f095-203">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f095-203">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_SSPR"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
    "allowedToUseSSPR": true
}

```
# <a name="c"></a>[<span data-ttu-id="6f095-204">C#</span><span class="sxs-lookup"><span data-stu-id="6f095-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-sspr-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f095-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f095-205">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-sspr-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f095-206">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f095-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-sspr-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6f095-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f095-207">Response</span></span>

<span data-ttu-id="6f095-208">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6f095-208">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```
