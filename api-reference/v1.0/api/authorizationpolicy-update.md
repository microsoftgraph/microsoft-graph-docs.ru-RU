---
title: Обновление авторизации
description: Обновление свойств объекта authorizationPolicy.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1e57436cc396b78a8697516702004c7ea4f6d666
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231985"
---
# <a name="update-authorizationpolicy"></a><span data-ttu-id="707cc-103">Обновление авторизацииPolicy</span><span class="sxs-lookup"><span data-stu-id="707cc-103">Update authorizationPolicy</span></span>

<span data-ttu-id="707cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="707cc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="707cc-105">Обновление свойств объекта [authorizationPolicy.](../resources/authorizationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="707cc-105">Update the properties of an [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="707cc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="707cc-106">Permissions</span></span>

<span data-ttu-id="707cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="707cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="707cc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="707cc-109">Permission type</span></span>                        | <span data-ttu-id="707cc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="707cc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="707cc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="707cc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="707cc-112">Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="707cc-112">Policy.ReadWrite.Authorization</span></span>|
| <span data-ttu-id="707cc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="707cc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="707cc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="707cc-114">Not supported.</span></span> |
| <span data-ttu-id="707cc-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="707cc-115">Application</span></span>                            | <span data-ttu-id="707cc-116">Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="707cc-116">Policy.ReadWrite.Authorization</span></span>|

## <a name="http-request"></a><span data-ttu-id="707cc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="707cc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="707cc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="707cc-118">Request headers</span></span>

| <span data-ttu-id="707cc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="707cc-119">Name</span></span>       | <span data-ttu-id="707cc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="707cc-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="707cc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="707cc-121">Authorization</span></span> | <span data-ttu-id="707cc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="707cc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="707cc-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="707cc-124">Content-type</span></span> | <span data-ttu-id="707cc-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="707cc-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="707cc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="707cc-127">Request body</span></span>

<span data-ttu-id="707cc-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="707cc-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="707cc-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="707cc-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="707cc-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="707cc-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="707cc-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="707cc-131">Property</span></span>     | <span data-ttu-id="707cc-132">Тип</span><span class="sxs-lookup"><span data-stu-id="707cc-132">Type</span></span>        | <span data-ttu-id="707cc-133">Описание</span><span class="sxs-lookup"><span data-stu-id="707cc-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="707cc-134">allowedToSignUpEmailBasedSubscriptions</span><span class="sxs-lookup"><span data-stu-id="707cc-134">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="707cc-135">Логический</span><span class="sxs-lookup"><span data-stu-id="707cc-135">Boolean</span></span>| <span data-ttu-id="707cc-136">Указывает, могут ли пользователи подписываться на подписки на основе электронной почты.</span><span class="sxs-lookup"><span data-stu-id="707cc-136">Indicates whether users can sign up for email based subscriptions.</span></span> |
|<span data-ttu-id="707cc-137">allowedToUseSSPR</span><span class="sxs-lookup"><span data-stu-id="707cc-137">allowedToUseSSPR</span></span>|<span data-ttu-id="707cc-138">Логический</span><span class="sxs-lookup"><span data-stu-id="707cc-138">Boolean</span></span>| <span data-ttu-id="707cc-139">Указывает, можно ли использовать Self-Serve сброса пароля пользователями клиента.</span><span class="sxs-lookup"><span data-stu-id="707cc-139">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> |
|<span data-ttu-id="707cc-140">allowEmailVerifiedUsersToJoinOrganization</span><span class="sxs-lookup"><span data-stu-id="707cc-140">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="707cc-141">Логический</span><span class="sxs-lookup"><span data-stu-id="707cc-141">Boolean</span></span>| <span data-ttu-id="707cc-142">Указывает, может ли пользователь присоединиться к клиенту по проверке электронной почты.</span><span class="sxs-lookup"><span data-stu-id="707cc-142">Indicates whether a user can join the tenant by email validation.</span></span> |
|<span data-ttu-id="707cc-143">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="707cc-143">allowInvitesFrom</span></span>|<span data-ttu-id="707cc-144">allowInvitesFrom</span><span class="sxs-lookup"><span data-stu-id="707cc-144">allowInvitesFrom</span></span>|<span data-ttu-id="707cc-145">Указывает, кто может приглашать внешних пользователей в организацию.</span><span class="sxs-lookup"><span data-stu-id="707cc-145">Indicates who can invite external users to the organization.</span></span> <span data-ttu-id="707cc-146">Возможные значения: `none`, `adminsAndGuestInviters`, `adminsGuestInvitersAndAllMembers`, `everyone`.</span><span class="sxs-lookup"><span data-stu-id="707cc-146">Possible values are: `none`, `adminsAndGuestInviters`, `adminsGuestInvitersAndAllMembers`, `everyone`.</span></span>  <span data-ttu-id="707cc-147">`everyone` — это параметр по умолчанию для всех облачных сред, за исключением правительства США.</span><span class="sxs-lookup"><span data-stu-id="707cc-147">`everyone` is the default setting for all cloud environments except US Government.</span></span> <span data-ttu-id="707cc-148">Дополнительные значения см. в этой [таблице.](../resources/authorizationpolicy.md#allowinvitesfrom-values)</span><span class="sxs-lookup"><span data-stu-id="707cc-148">See more on the allowed values in this [table](../resources/authorizationpolicy.md#allowinvitesfrom-values).</span></span> |
|<span data-ttu-id="707cc-149">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="707cc-149">blockMsolPowerShell</span></span>|<span data-ttu-id="707cc-150">Логический</span><span class="sxs-lookup"><span data-stu-id="707cc-150">Boolean</span></span>| <span data-ttu-id="707cc-151">Чтобы отключить использование MSOL PowerShell, установите это свойство `true` .</span><span class="sxs-lookup"><span data-stu-id="707cc-151">To disable the use of MSOL PowerShell set this property to `true`.</span></span> <span data-ttu-id="707cc-152">Это также отключит доступ пользователей к конечной точке устаревшей службы, используемой MSOL PowerShell.</span><span class="sxs-lookup"><span data-stu-id="707cc-152">This will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="707cc-153">Это не влияет на azure AD Подключение Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="707cc-153">This does not affect Azure AD Connect or Microsoft Graph.</span></span> |
|<span data-ttu-id="707cc-154">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="707cc-154">defaultUserRolePermissions</span></span>|[<span data-ttu-id="707cc-155">defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="707cc-155">defaultUserRolePermissions</span></span>](../resources/defaultuserrolepermissions.md)| <span data-ttu-id="707cc-156">Указывает определенные настраиваемые разрешения для роли пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="707cc-156">Specifies certain customizable permissions for default user role.</span></span> |
|<span data-ttu-id="707cc-157">description</span><span class="sxs-lookup"><span data-stu-id="707cc-157">description</span></span>|<span data-ttu-id="707cc-158">Строка</span><span class="sxs-lookup"><span data-stu-id="707cc-158">String</span></span>| <span data-ttu-id="707cc-159">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="707cc-159">Description of this policy.</span></span>|
|<span data-ttu-id="707cc-160">displayName</span><span class="sxs-lookup"><span data-stu-id="707cc-160">displayName</span></span>|<span data-ttu-id="707cc-161">Строка</span><span class="sxs-lookup"><span data-stu-id="707cc-161">String</span></span>| <span data-ttu-id="707cc-162">Отображение имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="707cc-162">Display name for this policy.</span></span> |
|<span data-ttu-id="707cc-163">guestUserRoleId</span><span class="sxs-lookup"><span data-stu-id="707cc-163">guestUserRoleId</span></span>|<span data-ttu-id="707cc-164">Guid</span><span class="sxs-lookup"><span data-stu-id="707cc-164">Guid</span></span>| <span data-ttu-id="707cc-165">Представляет шаблон roleId для роли, которая должна быть предоставлена гостевому пользователю.</span><span class="sxs-lookup"><span data-stu-id="707cc-165">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="707cc-166">В настоящее время поддерживаются следующие роли: User `a0b1b346-4d3e-4e8b-98f8-753987be4970` (), Guest User `10dae51f-b6af-4016-8d66-8c2a99b929b3` () и Restricted Guest User `2af84b1e-32c8-42b7-82bc-daa82404023b` ().</span><span class="sxs-lookup"><span data-stu-id="707cc-166">Currently following roles are supported:  User (`a0b1b346-4d3e-4e8b-98f8-753987be4970`), Guest User (`10dae51f-b6af-4016-8d66-8c2a99b929b3`), and Restricted Guest User (`2af84b1e-32c8-42b7-82bc-daa82404023b`).</span></span> |


## <a name="response"></a><span data-ttu-id="707cc-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="707cc-167">Response</span></span>

<span data-ttu-id="707cc-p108">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="707cc-p108">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="707cc-170">Примеры</span><span class="sxs-lookup"><span data-stu-id="707cc-170">Examples</span></span>

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a><span data-ttu-id="707cc-171">Пример 1. Обновление или настройка уровня доступа к гостевому пользователю для клиента</span><span class="sxs-lookup"><span data-stu-id="707cc-171">Example 1: Update or set Guest user access level for the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="707cc-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="707cc-172">Request</span></span>

<span data-ttu-id="707cc-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="707cc-173">The following is an example of the request.</span></span> <span data-ttu-id="707cc-174">В этом примере уровень гостевого доступа изменен на ограниченный гостевой пользователь.</span><span class="sxs-lookup"><span data-stu-id="707cc-174">In this example, guest access level is modified to Restricted Guest User.</span></span>


# <a name="http"></a>[<span data-ttu-id="707cc-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="707cc-175">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="707cc-176">C#</span><span class="sxs-lookup"><span data-stu-id="707cc-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-guestuserlevel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="707cc-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="707cc-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-guestuserlevel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="707cc-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="707cc-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-guestuserlevel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="707cc-179">Java</span><span class="sxs-lookup"><span data-stu-id="707cc-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-guestuserlevel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="707cc-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="707cc-180">Response</span></span>

<span data-ttu-id="707cc-181">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="707cc-181">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-block-msol-powershell-in-tenant"></a><span data-ttu-id="707cc-182">Пример 2. Блок MSOL PowerShell в клиенте</span><span class="sxs-lookup"><span data-stu-id="707cc-182">Example 2: Block MSOL PowerShell in tenant</span></span>

#### <a name="request"></a><span data-ttu-id="707cc-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="707cc-183">Request</span></span>

<span data-ttu-id="707cc-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="707cc-184">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="707cc-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="707cc-185">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="707cc-186">C#</span><span class="sxs-lookup"><span data-stu-id="707cc-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-blockmsolpowershell-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="707cc-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="707cc-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-blockmsolpowershell-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="707cc-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="707cc-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-blockmsolpowershell-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="707cc-189">Java</span><span class="sxs-lookup"><span data-stu-id="707cc-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-blockmsolpowershell-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="707cc-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="707cc-190">Response</span></span>

<span data-ttu-id="707cc-191">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="707cc-191">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-disable-default-user-roles-permission-to-create-applications"></a><span data-ttu-id="707cc-192">Пример 3. Отключение разрешения роли пользователя по умолчанию на создание приложений</span><span class="sxs-lookup"><span data-stu-id="707cc-192">Example 3: Disable default user role's permission to create applications</span></span>

#### <a name="request"></a><span data-ttu-id="707cc-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="707cc-193">Request</span></span>

<span data-ttu-id="707cc-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="707cc-194">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="707cc-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="707cc-195">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="707cc-196">C#</span><span class="sxs-lookup"><span data-stu-id="707cc-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="707cc-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="707cc-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="707cc-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="707cc-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="707cc-199">Java</span><span class="sxs-lookup"><span data-stu-id="707cc-199">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-applications-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="707cc-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="707cc-200">Response</span></span>

<span data-ttu-id="707cc-201">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="707cc-201">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-4-enable-default-user-role-to-use-self-serve-password-reset-feature"></a><span data-ttu-id="707cc-202">Пример 4. Включить роль пользователя по умолчанию для использования функции Self-Serve сброса пароля</span><span class="sxs-lookup"><span data-stu-id="707cc-202">Example 4: Enable default user role to use Self-Serve Password Reset feature</span></span>

#### <a name="request"></a><span data-ttu-id="707cc-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="707cc-203">Request</span></span>

<span data-ttu-id="707cc-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="707cc-204">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="707cc-205">HTTP</span><span class="sxs-lookup"><span data-stu-id="707cc-205">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="707cc-206">C#</span><span class="sxs-lookup"><span data-stu-id="707cc-206">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-sspr-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="707cc-207">JavaScript</span><span class="sxs-lookup"><span data-stu-id="707cc-207">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-sspr-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="707cc-208">Objective-C</span><span class="sxs-lookup"><span data-stu-id="707cc-208">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-sspr-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="707cc-209">Java</span><span class="sxs-lookup"><span data-stu-id="707cc-209">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-sspr-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="707cc-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="707cc-210">Response</span></span>

<span data-ttu-id="707cc-211">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="707cc-211">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-5-disable-user-consent-to-apps-for-default-user-role"></a><span data-ttu-id="707cc-212">Пример 5. Отключение согласия пользователя на приложения для роли пользователя по умолчанию</span><span class="sxs-lookup"><span data-stu-id="707cc-212">Example 5: Disable user consent to apps for default user role</span></span>

#### <a name="request"></a><span data-ttu-id="707cc-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="707cc-213">Request</span></span>

<span data-ttu-id="707cc-214">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="707cc-214">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="707cc-215">HTTP</span><span class="sxs-lookup"><span data-stu-id="707cc-215">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="707cc-216">C#</span><span class="sxs-lookup"><span data-stu-id="707cc-216">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-disableuserconsent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="707cc-217">JavaScript</span><span class="sxs-lookup"><span data-stu-id="707cc-217">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-disableuserconsent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="707cc-218">Objective-C</span><span class="sxs-lookup"><span data-stu-id="707cc-218">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-disableuserconsent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="707cc-219">Java</span><span class="sxs-lookup"><span data-stu-id="707cc-219">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-disableuserconsent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="707cc-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="707cc-220">Response</span></span>

<span data-ttu-id="707cc-221">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="707cc-221">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-6-enable-user-consent-to-apps-subject-to-app-consent-policy"></a><span data-ttu-id="707cc-222">Пример 6. Включить согласие пользователя на приложения с учетом политики согласия на приложения</span><span class="sxs-lookup"><span data-stu-id="707cc-222">Example 6: Enable user consent to apps, subject to app consent policy</span></span>

#### <a name="request"></a><span data-ttu-id="707cc-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="707cc-223">Request</span></span>

<span data-ttu-id="707cc-224">Ниже приводится пример запроса, который позволяет получить согласие пользователя на [](/azure/active-directory/manage-apps/manage-app-consent-policies) приложения при условии политики согласия на встроенные приложения, которая позволяет делегировать разрешения, классифицированные "низко", для клиентских приложений от проверенных издателей или зарегистрированных в том же `microsoft-user-default-low` клиенте.</span><span class="sxs-lookup"><span data-stu-id="707cc-224">The following is an example of the request that allows user consent to apps, subject to the built-in [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies) `microsoft-user-default-low`, which allows delegated permissions classified "low", for client apps from verified publishers or registered in the same tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="707cc-225">HTTP</span><span class="sxs-lookup"><span data-stu-id="707cc-225">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="707cc-226">C#</span><span class="sxs-lookup"><span data-stu-id="707cc-226">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-enableuserconsentlow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="707cc-227">JavaScript</span><span class="sxs-lookup"><span data-stu-id="707cc-227">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-enableuserconsentlow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="707cc-228">Objective-C</span><span class="sxs-lookup"><span data-stu-id="707cc-228">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-enableuserconsentlow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="707cc-229">Java</span><span class="sxs-lookup"><span data-stu-id="707cc-229">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authzpolicy-enableuserconsentlow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="707cc-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="707cc-230">Response</span></span>

<span data-ttu-id="707cc-231">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="707cc-231">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationpolicy"
} -->

```http
HTTP/1.1 204 No Content
```
