---
title: Обновление политики авторизации
description: Обновление свойств объекта authorizationPolicy.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e8ae872ad6a78f7faee94802d7d93f8775900903
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691447"
---
# <a name="update-authorizationpolicy"></a><span data-ttu-id="0345e-103">Обновление authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="0345e-103">Update authorizationPolicy</span></span>

<span data-ttu-id="0345e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0345e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0345e-105">Обновление свойств объекта [authorizationPolicy.](../resources/authorizationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0345e-105">Update the properties of an [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0345e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0345e-106">Permissions</span></span>

<span data-ttu-id="0345e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0345e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0345e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0345e-109">Permission type</span></span>                        | <span data-ttu-id="0345e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0345e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0345e-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0345e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0345e-112">Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="0345e-112">Policy.ReadWrite.Authorization</span></span>|
| <span data-ttu-id="0345e-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0345e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0345e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0345e-114">Not supported.</span></span> |
| <span data-ttu-id="0345e-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0345e-115">Application</span></span>                            | <span data-ttu-id="0345e-116">Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="0345e-116">Policy.ReadWrite.Authorization</span></span>|

## <a name="http-request"></a><span data-ttu-id="0345e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0345e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="0345e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0345e-118">Request headers</span></span>

| <span data-ttu-id="0345e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0345e-119">Name</span></span>       | <span data-ttu-id="0345e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0345e-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0345e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0345e-121">Authorization</span></span> | <span data-ttu-id="0345e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0345e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0345e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0345e-124">Content-type</span></span> | <span data-ttu-id="0345e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0345e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0345e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0345e-127">Request body</span></span>

<span data-ttu-id="0345e-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="0345e-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0345e-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="0345e-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0345e-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0345e-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0345e-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="0345e-131">Property</span></span>     | <span data-ttu-id="0345e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="0345e-132">Type</span></span>        | <span data-ttu-id="0345e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="0345e-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0345e-134">displayName</span><span class="sxs-lookup"><span data-stu-id="0345e-134">displayName</span></span>|<span data-ttu-id="0345e-135">Строка</span><span class="sxs-lookup"><span data-stu-id="0345e-135">String</span></span>| <span data-ttu-id="0345e-136">Отображаемого имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0345e-136">Display name for this policy.</span></span> |
|<span data-ttu-id="0345e-137">description</span><span class="sxs-lookup"><span data-stu-id="0345e-137">description</span></span>|<span data-ttu-id="0345e-138">Строка</span><span class="sxs-lookup"><span data-stu-id="0345e-138">String</span></span>| <span data-ttu-id="0345e-139">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="0345e-139">Description of this policy.</span></span>|
|<span data-ttu-id="0345e-140">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="0345e-140">blockMsolPowerShell</span></span>|<span data-ttu-id="0345e-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="0345e-141">Boolean</span></span>| <span data-ttu-id="0345e-142">Чтобы отключить использование MSOL PowerShell, установите для этого свойства true.</span><span class="sxs-lookup"><span data-stu-id="0345e-142">To disable the use of MSOL PowerShell set this property to true.</span></span> <span data-ttu-id="0345e-143">При установке true также будет отключен доступ пользователей к устаревшей конечной точке службы, используемой MSOL PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0345e-143">Setting to true will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="0345e-144">Это не влияет на Azure AD Connect или Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0345e-144">This does not affect Azure AD Connect or Microsoft Graph.</span></span> |
|<span data-ttu-id="0345e-145">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="0345e-145">defaultUserRolePermissions</span></span>|[<span data-ttu-id="0345e-146">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="0345e-146">defaultUserRolePermissions</span></span>](../resources/defaultuserrolepermissions.md)| <span data-ttu-id="0345e-147">Указывает определенные настраиваемые разрешения для роли пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0345e-147">Specifies certain customizable permissions for default user role.</span></span> |
|<span data-ttu-id="0345e-148">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="0345e-148">allowedToUseSSPR</span></span>|<span data-ttu-id="0345e-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="0345e-149">Boolean</span></span>| <span data-ttu-id="0345e-150">Указывает, может ли функция Self-Serve сброса пароля может использоваться пользователями в клиенте.</span><span class="sxs-lookup"><span data-stu-id="0345e-150">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> |
|<span data-ttu-id="0345e-151">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="0345e-151">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="0345e-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="0345e-152">Boolean</span></span>| <span data-ttu-id="0345e-153">Указывает, могут ли пользователи зарегистрироваться для подписок на основе электронной почты.</span><span class="sxs-lookup"><span data-stu-id="0345e-153">Indicates whether users can sign up for email based subscriptions.</span></span> |
|<span data-ttu-id="0345e-154">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="0345e-154">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="0345e-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="0345e-155">Boolean</span></span>| <span data-ttu-id="0345e-156">Указывает, может ли пользователь присоединиться к клиенту по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="0345e-156">Indicates whether a user can join the tenant by email validation.</span></span> |
|<span data-ttu-id="0345e-157">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="0345e-157">allowInvitesFrom</span></span>|<span data-ttu-id="0345e-158">Строка</span><span class="sxs-lookup"><span data-stu-id="0345e-158">String</span></span>|<span data-ttu-id="0345e-159">Указывает, кто может приглашать внешних пользователей в организацию.</span><span class="sxs-lookup"><span data-stu-id="0345e-159">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="0345e-160">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="0345e-160">Possible values are:</span></span><ul><li><span data-ttu-id="0345e-161">`none` – Запретить всем, включая администраторов, приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="0345e-161">`none` - Prevent everyone, including admins, from inviting external users.</span></span> <span data-ttu-id="0345e-162">Параметр по умолчанию для правительства США.</span><span class="sxs-lookup"><span data-stu-id="0345e-162">Default setting for US Government.</span></span></li><li><span data-ttu-id="0345e-163">`adminsAndGuestInviters` - Разрешить участникам ролей глобальных администраторов, администраторов пользователей и приглашений гостей приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="0345e-163">`adminsAndGuestInviters` - Allow members of Global Administrators, User Administrators, and Guest Inviter roles to invite external users.</span></span></li><li><span data-ttu-id="0345e-164">`adminsGuestInvitersAndAllMembers` - Разрешить вышеуказанным ролям администратора и всем другим участникам роли пользователя приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="0345e-164">`adminsGuestInvitersAndAllMembers` - Allow the above admin roles and all other User role members to invite external users.</span></span></li><li><span data-ttu-id="0345e-165">`everyone` - Разрешить всем пользователям в организации, включая гостевых пользователей, приглашать внешних пользователей.</span><span class="sxs-lookup"><span data-stu-id="0345e-165">`everyone` - Allow everyone in the organization, including guest users, to invite external users.</span></span> <span data-ttu-id="0345e-166">Настройка по умолчанию для всех облачных сред, кроме правительства США.</span><span class="sxs-lookup"><span data-stu-id="0345e-166">Default setting for all cloud environments except US Government.</span></span></li></ul> |

## <a name="response"></a><span data-ttu-id="0345e-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="0345e-167">Response</span></span>

<span data-ttu-id="0345e-p109">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0345e-p109">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0345e-170">Примеры</span><span class="sxs-lookup"><span data-stu-id="0345e-170">Examples</span></span>

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a><span data-ttu-id="0345e-171">Пример 1. Обновление или настройка уровня доступа гостевых пользователей для клиента</span><span class="sxs-lookup"><span data-stu-id="0345e-171">Example 1: Update or set Guest user access level for the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="0345e-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="0345e-172">Request</span></span>

<span data-ttu-id="0345e-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0345e-173">The following is an example of the request.</span></span> <span data-ttu-id="0345e-174">В этом примере уровень гостевого доступа изменен на "Ограниченный гостевой пользователь".</span><span class="sxs-lookup"><span data-stu-id="0345e-174">In this example, guest access level is modified to Restricted Guest User.</span></span>


# <a name="http"></a>[<span data-ttu-id="0345e-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="0345e-175">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0345e-176">C#</span><span class="sxs-lookup"><span data-stu-id="0345e-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-guestuserlevel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0345e-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0345e-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-guestuserlevel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0345e-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0345e-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-guestuserlevel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0345e-179">Java</span><span class="sxs-lookup"><span data-stu-id="0345e-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-guestuserlevel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0345e-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="0345e-180">Response</span></span>

<span data-ttu-id="0345e-181">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0345e-181">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-block-msol-powershell-in-tenant"></a><span data-ttu-id="0345e-182">Пример 2. Блокировка MSOL PowerShell в клиенте</span><span class="sxs-lookup"><span data-stu-id="0345e-182">Example 2: Block MSOL PowerShell in tenant</span></span>

#### <a name="request"></a><span data-ttu-id="0345e-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="0345e-183">Request</span></span>

<span data-ttu-id="0345e-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0345e-184">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0345e-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="0345e-185">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0345e-186">C#</span><span class="sxs-lookup"><span data-stu-id="0345e-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-blockmsolpowershell-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0345e-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0345e-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-blockmsolpowershell-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0345e-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0345e-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-blockmsolpowershell-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0345e-189">Java</span><span class="sxs-lookup"><span data-stu-id="0345e-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-blockmsolpowershell-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0345e-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="0345e-190">Response</span></span>

<span data-ttu-id="0345e-191">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0345e-191">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-disable-default-user-roles-permission-to-create-applications"></a><span data-ttu-id="0345e-192">Пример 3. Отключение разрешения роли пользователя по умолчанию на создание приложений</span><span class="sxs-lookup"><span data-stu-id="0345e-192">Example 3: Disable default user role's permission to create applications</span></span>

#### <a name="request"></a><span data-ttu-id="0345e-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="0345e-193">Request</span></span>

<span data-ttu-id="0345e-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0345e-194">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0345e-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="0345e-195">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0345e-196">C#</span><span class="sxs-lookup"><span data-stu-id="0345e-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0345e-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0345e-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0345e-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0345e-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0345e-199">Java</span><span class="sxs-lookup"><span data-stu-id="0345e-199">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-applications-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0345e-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="0345e-200">Response</span></span>

<span data-ttu-id="0345e-201">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0345e-201">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-4-enable-default-user-role-to-use-self-serve-password-reset-feature"></a><span data-ttu-id="0345e-202">Пример 4. Включить роль пользователя по умолчанию для использования функции Self-Serve сброса пароля</span><span class="sxs-lookup"><span data-stu-id="0345e-202">Example 4: Enable default user role to use Self-Serve Password Reset feature</span></span>

#### <a name="request"></a><span data-ttu-id="0345e-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="0345e-203">Request</span></span>

<span data-ttu-id="0345e-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0345e-204">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0345e-205">HTTP</span><span class="sxs-lookup"><span data-stu-id="0345e-205">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0345e-206">C#</span><span class="sxs-lookup"><span data-stu-id="0345e-206">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-sspr-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0345e-207">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0345e-207">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-sspr-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0345e-208">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0345e-208">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-sspr-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0345e-209">Java</span><span class="sxs-lookup"><span data-stu-id="0345e-209">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-sspr-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0345e-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="0345e-210">Response</span></span>

<span data-ttu-id="0345e-211">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0345e-211">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-5-disable-user-consent-to-apps-for-default-user-role"></a><span data-ttu-id="0345e-212">Пример 5. Отключение согласия пользователя на приложения для роли пользователя по умолчанию</span><span class="sxs-lookup"><span data-stu-id="0345e-212">Example 5: Disable user consent to apps for default user role</span></span>

#### <a name="request"></a><span data-ttu-id="0345e-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="0345e-213">Request</span></span>

<span data-ttu-id="0345e-214">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0345e-214">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0345e-215">HTTP</span><span class="sxs-lookup"><span data-stu-id="0345e-215">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0345e-216">C#</span><span class="sxs-lookup"><span data-stu-id="0345e-216">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-disableuserconsent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0345e-217">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0345e-217">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-disableuserconsent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0345e-218">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0345e-218">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-disableuserconsent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0345e-219">Java</span><span class="sxs-lookup"><span data-stu-id="0345e-219">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-disableuserconsent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0345e-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="0345e-220">Response</span></span>

<span data-ttu-id="0345e-221">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0345e-221">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-6-enable-user-consent-to-apps-subject-to-app-consent-policy"></a><span data-ttu-id="0345e-222">Пример 6. Разрешение согласия пользователя на приложения с помощью политики согласия приложения</span><span class="sxs-lookup"><span data-stu-id="0345e-222">Example 6: Enable user consent to apps, subject to app consent policy</span></span>

#### <a name="request"></a><span data-ttu-id="0345e-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="0345e-223">Request</span></span>

<span data-ttu-id="0345e-224">Ниже приводится пример запроса, который позволяет пользователям соглашаться с [](/azure/active-directory/manage-apps/manage-app-consent-policies) приложениями с помощью встроенной политики согласия приложения, которая позволяет делегировать разрешения, классифицированные как "низкий", для клиентских приложений от проверенных издателей или зарегистрированных в том же `microsoft-user-default-low` клиенте.</span><span class="sxs-lookup"><span data-stu-id="0345e-224">The following is an example of the request that allows user consent to apps, subject to the built-in [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies) `microsoft-user-default-low`, which allows delegated permissions classified "low", for client apps from verified publishers or registered in the same tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="0345e-225">HTTP</span><span class="sxs-lookup"><span data-stu-id="0345e-225">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0345e-226">C#</span><span class="sxs-lookup"><span data-stu-id="0345e-226">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-enableuserconsentlow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0345e-227">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0345e-227">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-enableuserconsentlow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0345e-228">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0345e-228">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-enableuserconsentlow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0345e-229">Java</span><span class="sxs-lookup"><span data-stu-id="0345e-229">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-enableuserconsentlow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0345e-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="0345e-230">Response</span></span>

<span data-ttu-id="0345e-231">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0345e-231">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationpolicy"
} -->

```http
HTTP/1.1 204 No Content
```
