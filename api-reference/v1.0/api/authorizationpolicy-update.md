---
title: Обновление авторизации
description: Обновление свойств объекта authorizationPolicy.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e3b8cee408b25b19d0fe36b57ce445e4dcbb13ff
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434960"
---
# <a name="update-authorizationpolicy"></a><span data-ttu-id="8f5be-103">Обновление авторизацииPolicy</span><span class="sxs-lookup"><span data-stu-id="8f5be-103">Update authorizationPolicy</span></span>

<span data-ttu-id="8f5be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f5be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8f5be-105">Обновление свойств объекта [authorizationPolicy.](../resources/authorizationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8f5be-105">Update the properties of an [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f5be-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f5be-106">Permissions</span></span>

<span data-ttu-id="8f5be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f5be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f5be-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f5be-109">Permission type</span></span>                        | <span data-ttu-id="8f5be-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f5be-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8f5be-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f5be-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f5be-112">Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="8f5be-112">Policy.ReadWrite.Authorization</span></span>|
| <span data-ttu-id="8f5be-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f5be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f5be-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f5be-114">Not supported.</span></span> |
| <span data-ttu-id="8f5be-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f5be-115">Application</span></span>                            | <span data-ttu-id="8f5be-116">Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="8f5be-116">Policy.ReadWrite.Authorization</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f5be-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f5be-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="8f5be-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f5be-118">Request headers</span></span>

| <span data-ttu-id="8f5be-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8f5be-119">Name</span></span>       | <span data-ttu-id="8f5be-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8f5be-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8f5be-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f5be-121">Authorization</span></span> | <span data-ttu-id="8f5be-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f5be-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f5be-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8f5be-124">Content-type</span></span> | <span data-ttu-id="8f5be-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f5be-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f5be-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f5be-127">Request body</span></span>

<span data-ttu-id="8f5be-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="8f5be-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8f5be-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="8f5be-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8f5be-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="8f5be-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8f5be-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f5be-131">Property</span></span>     | <span data-ttu-id="8f5be-132">Тип</span><span class="sxs-lookup"><span data-stu-id="8f5be-132">Type</span></span>        | <span data-ttu-id="8f5be-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8f5be-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8f5be-134">displayName</span><span class="sxs-lookup"><span data-stu-id="8f5be-134">displayName</span></span>|<span data-ttu-id="8f5be-135">String</span><span class="sxs-lookup"><span data-stu-id="8f5be-135">String</span></span>| <span data-ttu-id="8f5be-136">Отображение имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8f5be-136">Display name for this policy.</span></span> |
|<span data-ttu-id="8f5be-137">description</span><span class="sxs-lookup"><span data-stu-id="8f5be-137">description</span></span>|<span data-ttu-id="8f5be-138">String</span><span class="sxs-lookup"><span data-stu-id="8f5be-138">String</span></span>| <span data-ttu-id="8f5be-139">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="8f5be-139">Description of this policy.</span></span>|
|<span data-ttu-id="8f5be-140">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="8f5be-140">blockMsolPowerShell</span></span>|<span data-ttu-id="8f5be-141">Логический</span><span class="sxs-lookup"><span data-stu-id="8f5be-141">Boolean</span></span>| <span data-ttu-id="8f5be-142">Чтобы отключить использование MSOL PowerShell, установите это свойство true.</span><span class="sxs-lookup"><span data-stu-id="8f5be-142">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="8f5be-143">Настройка true также отключит пользовательский доступ к устаревшей конечной точке службы, используемой MSOL PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8f5be-143">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="8f5be-144">Это не влияет на Azure AD Connect или Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8f5be-144">This does not affect Azure AD Connect or Microsoft Graph.</span></span> |
|<span data-ttu-id="8f5be-145">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="8f5be-145">defaultUserRolePermissions</span></span>|[<span data-ttu-id="8f5be-146">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="8f5be-146">defaultUserRolePermissions</span></span>](../resources/defaultuserrolepermissions.md)| <span data-ttu-id="8f5be-147">Указывает определенные настраиваемые разрешения для роли пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8f5be-147">Specifies certain customizable permissions for default user role.</span></span> |
|<span data-ttu-id="8f5be-148">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="8f5be-148">allowedToUseSSPR</span></span>|<span data-ttu-id="8f5be-149">Логический</span><span class="sxs-lookup"><span data-stu-id="8f5be-149">Boolean</span></span>| <span data-ttu-id="8f5be-150">Указывает, можно ли использовать Self-Serve сброса пароля пользователями клиента.</span><span class="sxs-lookup"><span data-stu-id="8f5be-150">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> |
|<span data-ttu-id="8f5be-151">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="8f5be-151">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="8f5be-152">Логический</span><span class="sxs-lookup"><span data-stu-id="8f5be-152">Boolean</span></span>| <span data-ttu-id="8f5be-153">Указывает, могут ли пользователи подписываться на подписки на основе электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8f5be-153">Indicates whether users can sign up for email based subscriptions.</span></span> |
|<span data-ttu-id="8f5be-154">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="8f5be-154">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="8f5be-155">Логический</span><span class="sxs-lookup"><span data-stu-id="8f5be-155">Boolean</span></span>| <span data-ttu-id="8f5be-156">Указывает, может ли пользователь присоединиться к клиенту по проверке электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8f5be-156">Indicates whether a user can join the tenant by email validation.</span></span> |
|<span data-ttu-id="8f5be-157">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="8f5be-157">allowInvitesFrom</span></span>|<span data-ttu-id="8f5be-158">String</span><span class="sxs-lookup"><span data-stu-id="8f5be-158">String</span></span>|<span data-ttu-id="8f5be-159">Указывает, кто может приглашать внешних пользователей в организацию.</span><span class="sxs-lookup"><span data-stu-id="8f5be-159">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="8f5be-160">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="8f5be-160">Possible values are:</span></span><ul><li><span data-ttu-id="8f5be-161">`none` - Запретить всем, включая администраторов, приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="8f5be-161">`none` - Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="8f5be-162">Параметр по умолчанию для правительства США.</span><span class="sxs-lookup"><span data-stu-id="8f5be-162">Default setting for US Government.</span></span></li><li><span data-ttu-id="8f5be-163">`adminsAndGuestInviters` - Разрешить участникам глобальных администраторов, администраторов пользователей и приглашенных приглашений приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="8f5be-163">`adminsAndGuestInviters` - Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span></li><li><span data-ttu-id="8f5be-164">`adminsGuestInvitersAndAllMembers` - Разрешить вышеперечисленные роли администратора и всем другим участникам роли пользователя приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="8f5be-164">`adminsGuestInvitersAndAllMembers` - Allow the above admin roles and all other User role members to invite external users.</span></span></li><li><span data-ttu-id="8f5be-165">`everyone` - Разрешить всем в организации, включая гостевых пользователей, приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="8f5be-165">`everyone` - Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="8f5be-166">Параметр по умолчанию для всех облачных сред, кроме правительства США.</span><span class="sxs-lookup"><span data-stu-id="8f5be-166">Default setting for all cloud environments except US Government.</span></span></li></ul> |

## <a name="response"></a><span data-ttu-id="8f5be-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f5be-167">Response</span></span>

<span data-ttu-id="8f5be-p109">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8f5be-p109">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8f5be-170">Примеры</span><span class="sxs-lookup"><span data-stu-id="8f5be-170">Examples</span></span>

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a><span data-ttu-id="8f5be-171">Пример 1. Обновление или настройка уровня доступа к гостевому пользователю для клиента</span><span class="sxs-lookup"><span data-stu-id="8f5be-171">Example 1: Update or set Guest user access level for the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="8f5be-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f5be-172">Request</span></span>

<span data-ttu-id="8f5be-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f5be-173">The following is an example of the request.</span></span> <span data-ttu-id="8f5be-174">В этом примере уровень гостевого доступа изменен на ограниченный гостевой пользователь.</span><span class="sxs-lookup"><span data-stu-id="8f5be-174">In this example, guest access level is modified to Restricted Guest User.</span></span>


# <a name="http"></a>[<span data-ttu-id="8f5be-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f5be-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_guestUserLevel"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
  "allowEmailVerifiedUsersToJoinOrganization":false
}
```
# <a name="c"></a>[<span data-ttu-id="8f5be-176">C#</span><span class="sxs-lookup"><span data-stu-id="8f5be-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-guestuserlevel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8f5be-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f5be-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-guestuserlevel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f5be-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f5be-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-guestuserlevel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8f5be-179">Java</span><span class="sxs-lookup"><span data-stu-id="8f5be-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-guestuserlevel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8f5be-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f5be-180">Response</span></span>

<span data-ttu-id="8f5be-181">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8f5be-181">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-block-msol-powershell-in-tenant"></a><span data-ttu-id="8f5be-182">Пример 2. Блок MSOL PowerShell в клиенте</span><span class="sxs-lookup"><span data-stu-id="8f5be-182">Example 2: Block MSOL PowerShell in tenant</span></span>

#### <a name="request"></a><span data-ttu-id="8f5be-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f5be-183">Request</span></span>

<span data-ttu-id="8f5be-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f5be-184">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8f5be-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f5be-185">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_blockMSOLPowerShell"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "blockMsolPowerShell":true
}
```
# <a name="c"></a>[<span data-ttu-id="8f5be-186">C#</span><span class="sxs-lookup"><span data-stu-id="8f5be-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-blockmsolpowershell-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8f5be-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f5be-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-blockmsolpowershell-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f5be-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f5be-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-blockmsolpowershell-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8f5be-189">Java</span><span class="sxs-lookup"><span data-stu-id="8f5be-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-blockmsolpowershell-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8f5be-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f5be-190">Response</span></span>

<span data-ttu-id="8f5be-191">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8f5be-191">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-disable-default-user-roles-permission-to-create-applications"></a><span data-ttu-id="8f5be-192">Пример 3. Отключение разрешения роли пользователя по умолчанию на создание приложений</span><span class="sxs-lookup"><span data-stu-id="8f5be-192">Example 3: Disable default user role's permission to create applications</span></span>

#### <a name="request"></a><span data-ttu-id="8f5be-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f5be-193">Request</span></span>

<span data-ttu-id="8f5be-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f5be-194">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8f5be-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f5be-195">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_applications"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "defaultUserRolePermissions":{
      "allowedToCreateApps":false
   }
}
```
# <a name="c"></a>[<span data-ttu-id="8f5be-196">C#</span><span class="sxs-lookup"><span data-stu-id="8f5be-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8f5be-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f5be-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f5be-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f5be-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8f5be-199">Java</span><span class="sxs-lookup"><span data-stu-id="8f5be-199">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-applications-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8f5be-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f5be-200">Response</span></span>

<span data-ttu-id="8f5be-201">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8f5be-201">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-4-enable-default-user-role-to-use-self-serve-password-reset-feature"></a><span data-ttu-id="8f5be-202">Пример 4. Включить роль пользователя по умолчанию для использования функции Self-Serve сброса пароля</span><span class="sxs-lookup"><span data-stu-id="8f5be-202">Example 4: Enable default user role to use Self-Serve Password Reset feature</span></span>

#### <a name="request"></a><span data-ttu-id="8f5be-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f5be-203">Request</span></span>

<span data-ttu-id="8f5be-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f5be-204">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8f5be-205">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f5be-205">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_SSPR"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "allowedToUseSSPR":true
}
```
# <a name="c"></a>[<span data-ttu-id="8f5be-206">C#</span><span class="sxs-lookup"><span data-stu-id="8f5be-206">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-sspr-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8f5be-207">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f5be-207">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-sspr-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f5be-208">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f5be-208">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-sspr-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8f5be-209">Java</span><span class="sxs-lookup"><span data-stu-id="8f5be-209">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-sspr-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8f5be-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f5be-210">Response</span></span>

<span data-ttu-id="8f5be-211">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8f5be-211">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-5-disable-user-consent-to-apps-for-default-user-role"></a><span data-ttu-id="8f5be-212">Пример 5. Отключение согласия пользователя на приложения для роли пользователя по умолчанию</span><span class="sxs-lookup"><span data-stu-id="8f5be-212">Example 5: Disable user consent to apps for default user role</span></span>

#### <a name="request"></a><span data-ttu-id="8f5be-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f5be-213">Request</span></span>

<span data-ttu-id="8f5be-214">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f5be-214">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8f5be-215">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f5be-215">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_disableUserConsent"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "defaultUserRolePermissions": {
      "permissionGrantPoliciesAssigned": []
   }
}
```
# <a name="c"></a>[<span data-ttu-id="8f5be-216">C#</span><span class="sxs-lookup"><span data-stu-id="8f5be-216">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-disableuserconsent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8f5be-217">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f5be-217">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-disableuserconsent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f5be-218">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f5be-218">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-disableuserconsent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8f5be-219">Java</span><span class="sxs-lookup"><span data-stu-id="8f5be-219">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-disableuserconsent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8f5be-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f5be-220">Response</span></span>

<span data-ttu-id="8f5be-221">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8f5be-221">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-6-enable-user-consent-to-apps-subject-to-app-consent-policy"></a><span data-ttu-id="8f5be-222">Пример 6. Включить согласие пользователя на приложения с учетом политики согласия на приложения</span><span class="sxs-lookup"><span data-stu-id="8f5be-222">Example 6: Enable user consent to apps, subject to app consent policy</span></span>

#### <a name="request"></a><span data-ttu-id="8f5be-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f5be-223">Request</span></span>

<span data-ttu-id="8f5be-224">Ниже приводится пример запроса, который позволяет получить согласие пользователя на [](/azure/active-directory/manage-apps/manage-app-consent-policies) приложения при условии политики согласия на встроенные приложения, которая позволяет делегировать разрешения, классифицированные "низко", для клиентских приложений от проверенных издателей или зарегистрированных в том же `microsoft-user-default-low` клиенте.</span><span class="sxs-lookup"><span data-stu-id="8f5be-224">The following is an example of the request that allows user consent to apps, subject to the built-in [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies) `microsoft-user-default-low`, which allows delegated permissions classified "low", for client apps from verified publishers or registered in the same tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="8f5be-225">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f5be-225">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_enableUserConsentLow"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "defaultUserRolePermissions": {
      "permissionGrantPoliciesAssigned": [
         "managePermissionGrantsForSelf.microsoft-user-default-low"
      ]
   }
}
```
# <a name="c"></a>[<span data-ttu-id="8f5be-226">C#</span><span class="sxs-lookup"><span data-stu-id="8f5be-226">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-enableuserconsentlow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8f5be-227">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f5be-227">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-enableuserconsentlow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f5be-228">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f5be-228">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-enableuserconsentlow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8f5be-229">Java</span><span class="sxs-lookup"><span data-stu-id="8f5be-229">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-enableuserconsentlow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8f5be-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f5be-230">Response</span></span>

<span data-ttu-id="8f5be-231">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8f5be-231">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationpolicy"
} -->

```http
HTTP/1.1 204 No Content
```
