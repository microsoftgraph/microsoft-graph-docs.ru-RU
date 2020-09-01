---
title: Обновление аусоризатионполици
description: Обновление свойств объекта Аусоризатионполици.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 23263f65277f7635a5e03b1a955b6300845d2731
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319374"
---
# <a name="update-authorizationpolicy"></a><span data-ttu-id="6a23e-103">Обновление Аусоризатионполици</span><span class="sxs-lookup"><span data-stu-id="6a23e-103">Update authorizationPolicy</span></span>

<span data-ttu-id="6a23e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a23e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a23e-105">Обновление свойств объекта [аусоризатионполици](../resources/authorizationpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="6a23e-105">Update the properties of a [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a23e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6a23e-106">Permissions</span></span>

<span data-ttu-id="6a23e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a23e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6a23e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a23e-109">Permission type</span></span>                        | <span data-ttu-id="6a23e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a23e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6a23e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a23e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a23e-112">Policy. ReadWrite. Authorization</span><span class="sxs-lookup"><span data-stu-id="6a23e-112">Policy.ReadWrite.Authorization</span></span>|
| <span data-ttu-id="6a23e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a23e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a23e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a23e-114">Not supported.</span></span> |
| <span data-ttu-id="6a23e-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="6a23e-115">Application</span></span>                            | <span data-ttu-id="6a23e-116">Policy. ReadWrite. Authorization</span><span class="sxs-lookup"><span data-stu-id="6a23e-116">Policy.ReadWrite.Authorization</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a23e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a23e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="6a23e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6a23e-118">Request headers</span></span>

| <span data-ttu-id="6a23e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6a23e-119">Name</span></span>       | <span data-ttu-id="6a23e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6a23e-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6a23e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a23e-121">Authorization</span></span> | <span data-ttu-id="6a23e-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="6a23e-122">Bearer {token}</span></span> |
| <span data-ttu-id="6a23e-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6a23e-123">Content-type</span></span> | <span data-ttu-id="6a23e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6a23e-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a23e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6a23e-125">Request body</span></span>

<span data-ttu-id="6a23e-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="6a23e-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6a23e-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="6a23e-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6a23e-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6a23e-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6a23e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a23e-129">Property</span></span>     | <span data-ttu-id="6a23e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6a23e-130">Type</span></span>        | <span data-ttu-id="6a23e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6a23e-131">Description</span></span> |
|:-------------|:------------|:------------|  
|<span data-ttu-id="6a23e-132">displayName</span><span class="sxs-lookup"><span data-stu-id="6a23e-132">displayName</span></span>|<span data-ttu-id="6a23e-133">String</span><span class="sxs-lookup"><span data-stu-id="6a23e-133">String</span></span>| <span data-ttu-id="6a23e-134">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6a23e-134">Display name for this policy.</span></span> |  
|<span data-ttu-id="6a23e-135">description</span><span class="sxs-lookup"><span data-stu-id="6a23e-135">description</span></span>|<span data-ttu-id="6a23e-136">String</span><span class="sxs-lookup"><span data-stu-id="6a23e-136">String</span></span>| <span data-ttu-id="6a23e-137">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="6a23e-137">Description of this policy.</span></span> |  
|<span data-ttu-id="6a23e-138">гуестусерролеид</span><span class="sxs-lookup"><span data-stu-id="6a23e-138">guestUserRoleId</span></span>|<span data-ttu-id="6a23e-139">Guid</span><span class="sxs-lookup"><span data-stu-id="6a23e-139">Guid</span></span>| <span data-ttu-id="6a23e-140">Представляет templateId роли для роли, которая должна быть выделена пользователю "гость".</span><span class="sxs-lookup"><span data-stu-id="6a23e-140">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="6a23e-141">Обратитесь к [списку унифиедроледефинитионс](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) , чтобы найти список доступных шаблонов ролей.</span><span class="sxs-lookup"><span data-stu-id="6a23e-141">Refer to [List unifiedRoleDefinitions](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) to find the list of available role templates.</span></span> <span data-ttu-id="6a23e-142">Только поддерживаемые роли: User (a0b1b346-4d3e-4e8b-98f8-753987be4970), гость (10dae51f-b6af-4016-8d66-8c2a99b929b3) и пользователь с ограниченным гостями (2af84b1e-32c8-42b7-82bc-daa82404023b).</span><span class="sxs-lookup"><span data-stu-id="6a23e-142">Only supported roles today are User (a0b1b346-4d3e-4e8b-98f8-753987be4970), Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3), and Restricted Guest User (2af84b1e-32c8-42b7-82bc-daa82404023b).</span></span> | 
|<span data-ttu-id="6a23e-143">енабледпревиевфеатурес</span><span class="sxs-lookup"><span data-stu-id="6a23e-143">enabledPreviewFeatures</span></span>|<span data-ttu-id="6a23e-144">Коллекция (String)</span><span class="sxs-lookup"><span data-stu-id="6a23e-144">Collection(string)</span></span>| <span data-ttu-id="6a23e-145">Список компонентов, включенных для закрытой предварительной версии в клиенте.</span><span class="sxs-lookup"><span data-stu-id="6a23e-145">List of features enabled for private preview on the tenant.</span></span> | 
|<span data-ttu-id="6a23e-146">блоккмсолповершелл</span><span class="sxs-lookup"><span data-stu-id="6a23e-146">blockMsolPowerShell</span></span>|<span data-ttu-id="6a23e-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a23e-147">Boolean</span></span>| <span data-ttu-id="6a23e-148">Чтобы отключить использование MSOL PowerShell, задайте для этого свойства значение `true` .</span><span class="sxs-lookup"><span data-stu-id="6a23e-148">To disable the use of MSOL PowerShell, set this property to `true`.</span></span> <span data-ttu-id="6a23e-149">Параметр `true` также отключит доступ пользователей к устаревшей конечной точке службы, используемой MSOL PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6a23e-149">Setting to `true` will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="6a23e-150">Это не повлияет на Azure AD Connect или Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6a23e-150">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 
|<span data-ttu-id="6a23e-151">дефаултусерролепермиссионс</span><span class="sxs-lookup"><span data-stu-id="6a23e-151">defaultUserRolePermissions</span></span>|[<span data-ttu-id="6a23e-152">дефаултусерролепермиссионс</span><span class="sxs-lookup"><span data-stu-id="6a23e-152">defaultUserRolePermissions</span></span>](../resources/defaultUserRolePermissions.md)| <span data-ttu-id="6a23e-153">Задает определенные настраиваемые разрешения для роли пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6a23e-153">Specifies certain customizable permissions for default user role.</span></span> | 
|<span data-ttu-id="6a23e-154">алловедтаусесспр</span><span class="sxs-lookup"><span data-stu-id="6a23e-154">allowedToUseSSPR</span></span>|<span data-ttu-id="6a23e-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a23e-155">Boolean</span></span>| <span data-ttu-id="6a23e-156">Указывает, можно ли использовать функцию самостоятельного сброса пароля для пользователей клиента.</span><span class="sxs-lookup"><span data-stu-id="6a23e-156">Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant.</span></span> | 
|<span data-ttu-id="6a23e-157">алловедтосигнупемаилбаседсубскриптионс</span><span class="sxs-lookup"><span data-stu-id="6a23e-157">allowedToSignUpEmailBasedSubscriptions</span></span>|<span data-ttu-id="6a23e-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a23e-158">Boolean</span></span>| <span data-ttu-id="6a23e-159">Указывает, могут ли пользователи регистрироваться на почтовые подписки.</span><span class="sxs-lookup"><span data-stu-id="6a23e-159">Indicates whether users can sign up for email based subscriptions.</span></span> | 
|<span data-ttu-id="6a23e-160">алловемаилверифиедусерстожоинорганизатион</span><span class="sxs-lookup"><span data-stu-id="6a23e-160">allowEmailVerifiedUsersToJoinOrganization</span></span>|<span data-ttu-id="6a23e-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a23e-161">Boolean</span></span>| <span data-ttu-id="6a23e-162">Указывает, может ли пользователь присоединиться к клиенту по проверке электронной почты.</span><span class="sxs-lookup"><span data-stu-id="6a23e-162">Indicates whether a user can join the tenant by email validation.</span></span> | 

## <a name="response"></a><span data-ttu-id="6a23e-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a23e-163">Response</span></span>

<span data-ttu-id="6a23e-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6a23e-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6a23e-166">Примеры</span><span class="sxs-lookup"><span data-stu-id="6a23e-166">Examples</span></span>

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a><span data-ttu-id="6a23e-167">Пример 1: обновление или Настройка уровня доступа гостей для клиента</span><span class="sxs-lookup"><span data-stu-id="6a23e-167">Example 1: Update or set Guest user access level for the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="6a23e-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a23e-168">Request</span></span>

<span data-ttu-id="6a23e-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a23e-169">The following is an example of the request.</span></span> <span data-ttu-id="6a23e-170">В этом примере уровень гостевого доступа изменяется на "ограниченный гостевой пользователь".</span><span class="sxs-lookup"><span data-stu-id="6a23e-170">In this example, guest access level is modified to Restricted Guest User.</span></span>

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
#### <a name="response"></a><span data-ttu-id="6a23e-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a23e-171">Response</span></span>

<span data-ttu-id="6a23e-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6a23e-172">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content

```

### <a name="example-2-enable-new-feature-for-preview-on-tenant"></a><span data-ttu-id="6a23e-173">Пример 2: включение новой функции для предварительного просмотра в клиенте</span><span class="sxs-lookup"><span data-stu-id="6a23e-173">Example 2: Enable new feature for preview on tenant</span></span>

#### <a name="request"></a><span data-ttu-id="6a23e-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a23e-174">Request</span></span>

<span data-ttu-id="6a23e-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a23e-175">The following is an example of the request.</span></span>

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
#### <a name="response"></a><span data-ttu-id="6a23e-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a23e-176">Response</span></span>

<span data-ttu-id="6a23e-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6a23e-177">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```


### <a name="example-3-block-msol-powershell-in-tenant"></a><span data-ttu-id="6a23e-178">Пример 3: Блокировка MSOL PowerShell в клиенте</span><span class="sxs-lookup"><span data-stu-id="6a23e-178">Example 3: Block MSOL PowerShell in tenant</span></span>

#### <a name="request"></a><span data-ttu-id="6a23e-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a23e-179">Request</span></span>

<span data-ttu-id="6a23e-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a23e-180">The following is an example of the request.</span></span>

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
#### <a name="response"></a><span data-ttu-id="6a23e-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a23e-181">Response</span></span>

<span data-ttu-id="6a23e-182">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6a23e-182">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```
### <a name="example-4-disable-default-user-roles-permission-to-create-applications"></a><span data-ttu-id="6a23e-183">Пример 4: отключение разрешения роли пользователя по умолчанию для создания приложений</span><span class="sxs-lookup"><span data-stu-id="6a23e-183">Example 4: Disable default user role's permission to create applications</span></span>

#### <a name="request"></a><span data-ttu-id="6a23e-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a23e-184">Request</span></span>

<span data-ttu-id="6a23e-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a23e-185">The following is an example of the request.</span></span>

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
#### <a name="response"></a><span data-ttu-id="6a23e-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a23e-186">Response</span></span>

<span data-ttu-id="6a23e-187">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6a23e-187">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-5-enable-default-user-role-to-use-self-serve-password-reset-feature"></a><span data-ttu-id="6a23e-188">Пример 5: Включение роли пользователя по умолчанию для использования функции самостоятельного сброса пароля</span><span class="sxs-lookup"><span data-stu-id="6a23e-188">Example 5: Enable default user role to use Self-Serve Password Reset feature</span></span>

#### <a name="request"></a><span data-ttu-id="6a23e-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a23e-189">Request</span></span>

<span data-ttu-id="6a23e-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a23e-190">The following is an example of the request.</span></span>

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
#### <a name="response"></a><span data-ttu-id="6a23e-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a23e-191">Response</span></span>

<span data-ttu-id="6a23e-192">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6a23e-192">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```
