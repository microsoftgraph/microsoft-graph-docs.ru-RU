---
title: Обновление аусоризатионполици
description: Обновление свойств объекта Аусоризатионполици.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9ccd2e5b95059ec4e3a38eadf3f62b25377eabd3
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581242"
---
# <a name="update-authorizationpolicy"></a><span data-ttu-id="28414-103">Обновление Аусоризатионполици</span><span class="sxs-lookup"><span data-stu-id="28414-103">Update authorizationPolicy</span></span>

<span data-ttu-id="28414-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28414-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="28414-105">Обновление свойств объекта [аусоризатионполици](../resources/authorizationpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="28414-105">Update the properties of an [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="28414-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28414-106">Permissions</span></span>

<span data-ttu-id="28414-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28414-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="28414-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28414-109">Permission type</span></span>                        | <span data-ttu-id="28414-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28414-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="28414-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28414-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="28414-112">Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="28414-112">Policy.ReadWrite.Authorization</span></span>|
| <span data-ttu-id="28414-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28414-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28414-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28414-114">Not supported.</span></span> |
| <span data-ttu-id="28414-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="28414-115">Application</span></span>                            | <span data-ttu-id="28414-116">Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="28414-116">Policy.ReadWrite.Authorization</span></span>|

## <a name="http-request"></a><span data-ttu-id="28414-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28414-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="28414-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28414-118">Request headers</span></span>

| <span data-ttu-id="28414-119">Имя</span><span class="sxs-lookup"><span data-stu-id="28414-119">Name</span></span>       | <span data-ttu-id="28414-120">Описание</span><span class="sxs-lookup"><span data-stu-id="28414-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="28414-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28414-121">Authorization</span></span> | <span data-ttu-id="28414-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28414-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="28414-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="28414-124">Content-type</span></span> | <span data-ttu-id="28414-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28414-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28414-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28414-127">Request body</span></span>

<span data-ttu-id="28414-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="28414-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="28414-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="28414-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="28414-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="28414-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="28414-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="28414-131">Property</span></span>     | <span data-ttu-id="28414-132">Тип</span><span class="sxs-lookup"><span data-stu-id="28414-132">Type</span></span>        | <span data-ttu-id="28414-133">Описание</span><span class="sxs-lookup"><span data-stu-id="28414-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="28414-134">displayName</span><span class="sxs-lookup"><span data-stu-id="28414-134">displayName</span></span>|<span data-ttu-id="28414-135">String</span><span class="sxs-lookup"><span data-stu-id="28414-135">String</span></span>| <span data-ttu-id="28414-136">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="28414-136">Display name for this policy.</span></span> |
|<span data-ttu-id="28414-137">description</span><span class="sxs-lookup"><span data-stu-id="28414-137">description</span></span>|<span data-ttu-id="28414-138">String</span><span class="sxs-lookup"><span data-stu-id="28414-138">String</span></span>| <span data-ttu-id="28414-139">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="28414-139">Description of this policy.</span></span>|
|<span data-ttu-id="28414-140">блоккмсолповершелл</span><span class="sxs-lookup"><span data-stu-id="28414-140">blockMsolPowerShell</span></span>|<span data-ttu-id="28414-141">Логический</span><span class="sxs-lookup"><span data-stu-id="28414-141">Boolean</span></span>| <span data-ttu-id="28414-142">Чтобы отключить использование MSOL PowerShell, установите для этого свойства значение true.</span><span class="sxs-lookup"><span data-stu-id="28414-142">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="28414-143">Если задано значение true, также будет отключен доступ пользователей к устаревшей конечной точке службы, используемой MSOL PowerShell.</span><span class="sxs-lookup"><span data-stu-id="28414-143">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="28414-144">Это не повлияет на Azure AD Connect или Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="28414-144">This does not affect Azure AD Connect or Microsoft Graph.</span></span> |
|<span data-ttu-id="28414-145">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="28414-145">defaultUserRolePermissions</span></span>|[<span data-ttu-id="28414-146">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="28414-146">defaultUserRolePermissions</span></span>](../resources/defaultuserrolepermissions.md)| <span data-ttu-id="28414-147">Задает определенные настраиваемые разрешения для роли пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="28414-147">Specifies certain customizable permissions for default user role.</span></span> |
|<span data-ttu-id="28414-148">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="28414-148">allowedToUseSSPR</span></span>|<span data-ttu-id="28414-149">Логический</span><span class="sxs-lookup"><span data-stu-id="28414-149">Boolean</span></span>| <span data-ttu-id="28414-150">Указывает, может ли функция сброса пароля Self-Serve использоваться пользователями клиента.</span><span class="sxs-lookup"><span data-stu-id="28414-150">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> |
|<span data-ttu-id="28414-151">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="28414-151">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="28414-152">Логический</span><span class="sxs-lookup"><span data-stu-id="28414-152">Boolean</span></span>| <span data-ttu-id="28414-153">Указывает, могут ли пользователи регистрироваться на почтовые подписки.</span><span class="sxs-lookup"><span data-stu-id="28414-153">Indicates whether users can sign up for email based subscriptions.</span></span> |
|<span data-ttu-id="28414-154">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="28414-154">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="28414-155">Логический</span><span class="sxs-lookup"><span data-stu-id="28414-155">Boolean</span></span>| <span data-ttu-id="28414-156">Указывает, может ли пользователь присоединиться к клиенту по проверке электронной почты.</span><span class="sxs-lookup"><span data-stu-id="28414-156">Indicates whether a user can join the tenant by email validation.</span></span> |
|<span data-ttu-id="28414-157">алловинвитесфром</span><span class="sxs-lookup"><span data-stu-id="28414-157">allowInvitesFrom</span></span>|<span data-ttu-id="28414-158">String</span><span class="sxs-lookup"><span data-stu-id="28414-158">String</span></span>|<span data-ttu-id="28414-159">Указывает, кто может приглашать внешних пользователей в Организации.</span><span class="sxs-lookup"><span data-stu-id="28414-159">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="28414-160">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="28414-160">Possible values are:</span></span><ul><li><span data-ttu-id="28414-161">`none` — Запретить всем, в том числе администраторам, приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="28414-161">`none` - Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="28414-162">Настройка по умолчанию для государственных организаций США.</span><span class="sxs-lookup"><span data-stu-id="28414-162">Default setting for US Government.</span></span></li><li><span data-ttu-id="28414-163">`adminsAndGuestInviters` — Разрешить членам группы "Администраторы", "Администраторы пользователей" и "гость" приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="28414-163">`adminsAndGuestInviters` - Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span></li><li><span data-ttu-id="28414-164">`adminsGuestInvitersAndAllMembers` — Разрешить внешним пользователям приглашать этих ролей администратора и других участников роли пользователей.</span><span class="sxs-lookup"><span data-stu-id="28414-164">`adminsGuestInvitersAndAllMembers` - Allow the above admin roles and all other User role members to invite external users.</span></span></li><li><span data-ttu-id="28414-165">`everyone` — Разрешить всем пользователям в Организации, в том числе гостям, приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="28414-165">`everyone` - Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="28414-166">Значение по умолчанию для всех облачных сред, кроме государственных организаций США.</span><span class="sxs-lookup"><span data-stu-id="28414-166">Default setting for all cloud environments except US Government.</span></span></li></ul> |

## <a name="response"></a><span data-ttu-id="28414-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="28414-167">Response</span></span>

<span data-ttu-id="28414-p109">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="28414-p109">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="28414-170">Примеры</span><span class="sxs-lookup"><span data-stu-id="28414-170">Examples</span></span>

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a><span data-ttu-id="28414-171">Пример 1: обновление или Настройка уровня доступа гостей для клиента</span><span class="sxs-lookup"><span data-stu-id="28414-171">Example 1: Update or set Guest user access level for the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="28414-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="28414-172">Request</span></span>

<span data-ttu-id="28414-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28414-173">The following is an example of the request.</span></span> <span data-ttu-id="28414-174">В этом примере уровень гостевого доступа изменяется на "ограниченный гостевой пользователь".</span><span class="sxs-lookup"><span data-stu-id="28414-174">In this example, guest access level is modified to Restricted Guest User.</span></span>

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

#### <a name="response"></a><span data-ttu-id="28414-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="28414-175">Response</span></span>

<span data-ttu-id="28414-176">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="28414-176">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-block-msol-powershell-in-tenant"></a><span data-ttu-id="28414-177">Пример 2: Блокировка MSOL PowerShell в клиенте</span><span class="sxs-lookup"><span data-stu-id="28414-177">Example 2: Block MSOL PowerShell in tenant</span></span>

#### <a name="request"></a><span data-ttu-id="28414-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="28414-178">Request</span></span>

<span data-ttu-id="28414-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28414-179">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="28414-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="28414-180">Response</span></span>

<span data-ttu-id="28414-181">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="28414-181">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-disable-default-user-roles-permission-to-create-applications"></a><span data-ttu-id="28414-182">Пример 3: отключение разрешения роли пользователя по умолчанию для создания приложений</span><span class="sxs-lookup"><span data-stu-id="28414-182">Example 3: Disable default user role's permission to create applications</span></span>

#### <a name="request"></a><span data-ttu-id="28414-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="28414-183">Request</span></span>

<span data-ttu-id="28414-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28414-184">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="28414-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="28414-185">Response</span></span>

<span data-ttu-id="28414-186">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="28414-186">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-4-enable-default-user-role-to-use-self-serve-password-reset-feature"></a><span data-ttu-id="28414-187">Пример 4: Включение роли пользователя по умолчанию для использования функции сброса пароля Self-Serve</span><span class="sxs-lookup"><span data-stu-id="28414-187">Example 4: Enable default user role to use Self-Serve Password Reset feature</span></span>

#### <a name="request"></a><span data-ttu-id="28414-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="28414-188">Request</span></span>

<span data-ttu-id="28414-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28414-189">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="28414-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="28414-190">Response</span></span>

<span data-ttu-id="28414-191">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="28414-191">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-5-disable-user-consent-to-apps-for-default-user-role"></a><span data-ttu-id="28414-192">Пример 5: отключение согласия пользователя для приложений для роли пользователя по умолчанию</span><span class="sxs-lookup"><span data-stu-id="28414-192">Example 5: Disable user consent to apps for default user role</span></span>

#### <a name="request"></a><span data-ttu-id="28414-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="28414-193">Request</span></span>

<span data-ttu-id="28414-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28414-194">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="28414-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="28414-195">Response</span></span>

<span data-ttu-id="28414-196">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="28414-196">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-6-enable-user-consent-to-apps-subject-to-app-consent-policy"></a><span data-ttu-id="28414-197">Пример 6: включение согласия пользователя для приложений, подчиняются политике согласия приложений</span><span class="sxs-lookup"><span data-stu-id="28414-197">Example 6: Enable user consent to apps, subject to app consent policy</span></span>

#### <a name="request"></a><span data-ttu-id="28414-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="28414-198">Request</span></span>

<span data-ttu-id="28414-199">Ниже приведен пример запроса, который разрешает согласие пользователя на приложения, в соответствии со встроенной [политикой согласия приложений](/azure/active-directory/manage-apps/manage-app-consent-policies) `microsoft-user-default-low` , которая разрешает делегированные разрешения, классифицированные как низкие, для клиентских приложений из проверенных издателей или зарегистрированных в одном клиенте.</span><span class="sxs-lookup"><span data-stu-id="28414-199">The following is an example of the request that allows user consent to apps, subject to the built-in [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies) `microsoft-user-default-low`, which allows delegated permissions classified "low", for client apps from verified publishers or registered in the same tenant.</span></span>

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

#### <a name="response"></a><span data-ttu-id="28414-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="28414-200">Response</span></span>

<span data-ttu-id="28414-201">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="28414-201">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationpolicy"
} -->

```http
HTTP/1.1 204 No Content
```
