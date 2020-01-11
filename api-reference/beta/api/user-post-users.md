---
title: Создание пользователя
description: Создание пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0719415786a00b07485761c72985abcc47106dd0
ms.sourcegitcommit: 2a601cffdb8df375b2ee32a1f35b8f71e0ffd04f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2020
ms.locfileid: "41023105"
---
# <a name="create-user"></a><span data-ttu-id="cb4b0-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="cb4b0-103">Create user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb4b0-p101">Создание [пользователя](../resources/user.md). В теле запроса указан пользователь, которого нужно создать. Вам нужно указать как минимум обязательные свойства для пользователя. При необходимости вы можете указать другие записываемые свойства.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-p101">Create a new [user](../resources/user.md). The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>

<span data-ttu-id="cb4b0-108">Эта операция по умолчанию возвращает только подмножество свойств для каждого пользователя.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-108">This operation returns by default only a subset of the properties for each user.</span></span> <span data-ttu-id="cb4b0-109">Эти свойства по умолчанию указаны в разделе [Свойства](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="cb4b0-109">These default properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="cb4b0-110">Чтобы получить свойства, которые не возвращаются по умолчанию, выполните [операцию GET](user-get.md) и укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-110">To get properties that are not returned by default, do a [GET operation](user-get.md) and specify the properties in a `$select` OData query option.</span></span>

>[!NOTE]
><span data-ttu-id="cb4b0-111">Чтобы создать внешних пользователей, используйте [API приглашений](invitation-post.md).</span><span class="sxs-lookup"><span data-stu-id="cb4b0-111">To create external users, use the [invitation API](invitation-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cb4b0-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb4b0-112">Permissions</span></span>

<span data-ttu-id="cb4b0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb4b0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb4b0-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb4b0-115">Permission type</span></span>      | <span data-ttu-id="cb4b0-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb4b0-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb4b0-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb4b0-117">Delegated (work or school account)</span></span> | <span data-ttu-id="cb4b0-118">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cb4b0-118">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cb4b0-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb4b0-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb4b0-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-120">Not supported.</span></span>    |
|<span data-ttu-id="cb4b0-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb4b0-121">Application</span></span> | <span data-ttu-id="cb4b0-122">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb4b0-122">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb4b0-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb4b0-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="cb4b0-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb4b0-124">Request headers</span></span>
| <span data-ttu-id="cb4b0-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb4b0-125">Header</span></span>       | <span data-ttu-id="cb4b0-126">Значение</span><span class="sxs-lookup"><span data-stu-id="cb4b0-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cb4b0-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb4b0-127">Authorization</span></span>  | <span data-ttu-id="cb4b0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cb4b0-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cb4b0-130">Content-Type</span></span>  | <span data-ttu-id="cb4b0-131">application/json</span><span class="sxs-lookup"><span data-stu-id="cb4b0-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cb4b0-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cb4b0-132">Request body</span></span>

<span data-ttu-id="cb4b0-133">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-133">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="cb4b0-134">В следующей таблице перечислены свойства, необходимые при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-134">The following table lists the properties that are required when you create a user.</span></span> <span data-ttu-id="cb4b0-135">Если вы включаете свойство **удостоверения** для создаваемого пользователя, не все перечисленные свойства являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-135">If you're including an **identities** property for the user you're creating, not all the properties listed are required.</span></span> <span data-ttu-id="cb4b0-136">Для [удостоверения локальной учетной записи B2C](../resources/objectidentity.md)требуется **только passwordprofile необходима** , а для \*\*\*\* `DisablePasswordExpiration`пассвордполици необходимо задать значение.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-136">For a [B2C local account identity](../resources/objectidentity.md), only  **passwordProfile** is required, and **passwordPolicy** must be set to `DisablePasswordExpiration`.</span></span> <span data-ttu-id="cb4b0-137">Для социальных удостоверений никакие свойства не требуются.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-137">For a social identity, none of the properties are required.</span></span>

| <span data-ttu-id="cb4b0-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="cb4b0-138">Parameter</span></span> | <span data-ttu-id="cb4b0-139">Тип</span><span class="sxs-lookup"><span data-stu-id="cb4b0-139">Type</span></span> | <span data-ttu-id="cb4b0-140">Описание</span><span class="sxs-lookup"><span data-stu-id="cb4b0-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb4b0-141">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="cb4b0-141">accountEnabled</span></span> |<span data-ttu-id="cb4b0-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb4b0-142">Boolean</span></span> |<span data-ttu-id="cb4b0-143">Значение true, если учетная запись включена; в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-143">True if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="cb4b0-144">displayName</span><span class="sxs-lookup"><span data-stu-id="cb4b0-144">displayName</span></span> |<span data-ttu-id="cb4b0-145">строка</span><span class="sxs-lookup"><span data-stu-id="cb4b0-145">string</span></span> |<span data-ttu-id="cb4b0-146">Имя, которое следует отобразить в адресной книге для пользователя.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-146">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="cb4b0-147">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="cb4b0-147">onPremisesImmutableId</span></span> |<span data-ttu-id="cb4b0-148">string</span><span class="sxs-lookup"><span data-stu-id="cb4b0-148">string</span></span> |<span data-ttu-id="cb4b0-149">Необходимо указывать только при создании учетной записи пользователя, если вы используете федеративный домен для свойства userPrincipalName (UPN) этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-149">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="cb4b0-150">mailNickname</span><span class="sxs-lookup"><span data-stu-id="cb4b0-150">mailNickname</span></span> |<span data-ttu-id="cb4b0-151">string</span><span class="sxs-lookup"><span data-stu-id="cb4b0-151">string</span></span> |<span data-ttu-id="cb4b0-152">Почтовый псевдоним для пользователя.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-152">The mail alias for the user.</span></span>|
|<span data-ttu-id="cb4b0-153">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="cb4b0-153">passwordProfile</span></span>|[<span data-ttu-id="cb4b0-154">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="cb4b0-154">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="cb4b0-155">Пароль для профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-155">The password profile for the user.</span></span>|
|<span data-ttu-id="cb4b0-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cb4b0-156">userPrincipalName</span></span> |<span data-ttu-id="cb4b0-157">string</span><span class="sxs-lookup"><span data-stu-id="cb4b0-157">string</span></span> |<span data-ttu-id="cb4b0-158">Имя участника-пользователя (polzovatel@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="cb4b0-158">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="cb4b0-159">Так как ресурс **user** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными в экземпляр user при его создании.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-159">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

<span data-ttu-id="cb4b0-160">Федеративные пользователи, созданные с помощью этого API, будут вынуждены подписываться каждые 12 часов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-160">Federated users created via this API will be forced to sign in every 12 hours by default.</span></span> <span data-ttu-id="cb4b0-161">Сведения о том, как это сделать, приведены в статье [исключения для времени существования маркеров](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span><span class="sxs-lookup"><span data-stu-id="cb4b0-161">For information about how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

>[!NOTE]
><span data-ttu-id="cb4b0-162">Добавление [локальной учетной записи B2C](../resources/objectidentity.md) к существующему объекту **пользователя** запрещено, если объект **пользователя** еще не содержит удостоверение локальной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-162">Adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="response"></a><span data-ttu-id="cb4b0-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb4b0-163">Response</span></span>

<span data-ttu-id="cb4b0-164">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [user](../resources/user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-164">If successful, this method returns a `201 Created` response code and a [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb4b0-165">Пример</span><span class="sxs-lookup"><span data-stu-id="cb4b0-165">Example</span></span>

### <a name="example-1-create-a-user"></a><span data-ttu-id="cb4b0-166">Пример 1: создание пользователя</span><span class="sxs-lookup"><span data-stu-id="cb4b0-166">Example 1: Create a user</span></span>

#### <a name="request"></a><span data-ttu-id="cb4b0-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb4b0-167">Request</span></span>
<span data-ttu-id="cb4b0-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-168">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cb4b0-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb4b0-169">HTTP</span></span>](#tab/http)
<!-- {  
  "blockType": "request",   
  "name": "create_user_from_users_2"    
}-->

```http
POST https://graph.microsoft.com/beta/users
Content-type: application/json

{
  "accountEnabled": true,
  "displayName": "displayName-value",
  "mailNickname": "mailNickname-value",
  "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com",
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": "password-value"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cb4b0-170">C#</span><span class="sxs-lookup"><span data-stu-id="cb4b0-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cb4b0-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb4b0-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cb4b0-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb4b0-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="cb4b0-173">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-173">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="cb4b0-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb4b0-174">Response</span></span>
<span data-ttu-id="cb4b0-175">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-175">Here is an example of the response.</span></span> 

[!NOTE]
<span data-ttu-id="cb4b0-176">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-176">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cb4b0-177">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-177">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/$entity",
    "id": "id-value",
    "businessPhones": [],
    "displayName": "displayName-value",
    "givenName": null,
    "jobTitle": null,
    "mail": null,
    "mobilePhone": null,
    "officeLocation": null,
    "preferredLanguage": null,
    "surname": null,
    "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com"
}
```

### <a name="example-2-create-a-user-with-social-and-local-account-identities"></a><span data-ttu-id="cb4b0-178">Пример 2: создание пользователя с удостоверениями социальных сетей и локальных учетных записей</span><span class="sxs-lookup"><span data-stu-id="cb4b0-178">Example 2: Create a user with social and local account identities</span></span>

<span data-ttu-id="cb4b0-179">Создайте нового пользователя с удостоверением локальной учетной записи с именем для входа, адресом электронной почты в качестве входа и с помощью социальных удостоверений.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-179">Create a new user, with a local account identity with a sign-in name, an email address as sign-in, and with a social identity.</span></span> <span data-ttu-id="cb4b0-180">Этот пример обычно используется для сценариев миграции в клиентах B2C.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-180">This example is typically used for migration scenarios in B2C tenants.</span></span>  

[!NOTE] 
<span data-ttu-id="cb4b0-181">Для удостоверений локальных учетных записей необходимо отключить срок действия паролей и принудительно изменить пароль при следующем входе в систему.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-181">For local account identities, password expirations must be disabled, and force change password at next sign-in must also be disabled.</span></span>

#### <a name="request"></a><span data-ttu-id="cb4b0-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb4b0-182">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cb4b0-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb4b0-183">HTTP</span></span>](#tab/http)
<!-- {  
  "blockType": "request",   
  "name": "create_user_from_users_identities"   
}-->

```http
POST https://graph.microsoft.com/beta/users
Content-type: application/json

{
  "displayName": "John Smith",
  "identities": [
    {
      "signInType": "userName",
      "issuer": "contoso.onmicrosoft.com",
      "issuerAssignedId": "johnsmith"
    },
    {
      "signInType": "emailAddress",
      "issuer": "contoso.onmicrosoft.com",
      "issuerAssignedId": "jsmith@yahoo.com"
    },
    {
      "signInType": "federated",
      "issuer": "facebook.com",
      "issuerAssignedId": "5eecb0cd"
    }
  ],
  "passwordProfile" : {
    "password": "password-value"
  },
  "passwordPolicies": "DisablePasswordExpiration"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cb4b0-184">C#</span><span class="sxs-lookup"><span data-stu-id="cb4b0-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-identities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cb4b0-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb4b0-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-identities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cb4b0-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb4b0-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-identities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cb4b0-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb4b0-187">Response</span></span>

<span data-ttu-id="cb4b0-188">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-188">Here is an example of the response.</span></span> 

> <span data-ttu-id="cb4b0-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cb4b0-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/$entity",
  "displayName": "John Smith",
  "id": "4c7be08b-361f-41a8-b1ef-1712f7a3dfb2",
  "identities": [
    {
      "signInType": "userName",
      "issuer": "contoso.onmicrosoft.com",
      "issuerAssignedId": "johnsmith"
    },
    {
      "signInType": "emailAddress",
      "issuer": "contoso.onmicrosoft.com",
      "issuerAssignedId": "jsmith@yahoo.com"
    },
    {
      "signInType": "federated",
      "issuer": "facebook.com",
      "issuerAssignedId": "5eecb0cd"
    }
  ],
  "passwordPolicies": "DisablePasswordExpiration"
}
```

## <a name="see-also"></a><span data-ttu-id="cb4b0-191">См. также</span><span class="sxs-lookup"><span data-stu-id="cb4b0-191">See also</span></span>

- [<span data-ttu-id="cb4b0-192">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="cb4b0-192">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="cb4b0-193">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="cb4b0-193">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="cb4b0-194">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="cb4b0-194">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
