---
title: Создание пользователя
description: Создание пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e1a3e1a74d4ddf66017f36fa3f373d910dcdf793
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "38657902"
---
# <a name="create-user"></a><span data-ttu-id="788a5-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="788a5-103">Create user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="788a5-p101">Создание [пользователя](../resources/user.md). В теле запроса указан пользователь, которого нужно создать. Вам нужно указать как минимум обязательные свойства для пользователя. При необходимости вы можете указать другие записываемые свойства.</span><span class="sxs-lookup"><span data-stu-id="788a5-p101">Create a new [user](../resources/user.md). The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>

>[!NOTE]
><span data-ttu-id="788a5-108">Чтобы создать внешних пользователей, используйте [API приглашений](invitation-post.md).</span><span class="sxs-lookup"><span data-stu-id="788a5-108">To create external users, use the [invitation API](invitation-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="788a5-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="788a5-109">Permissions</span></span>

<span data-ttu-id="788a5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="788a5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="788a5-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="788a5-112">Permission type</span></span>      | <span data-ttu-id="788a5-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="788a5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="788a5-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="788a5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="788a5-115">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="788a5-115">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="788a5-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="788a5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="788a5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="788a5-117">Not supported.</span></span>    |
|<span data-ttu-id="788a5-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="788a5-118">Application</span></span> | <span data-ttu-id="788a5-119">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="788a5-119">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="788a5-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="788a5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="788a5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="788a5-121">Request headers</span></span>
| <span data-ttu-id="788a5-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="788a5-122">Header</span></span>       | <span data-ttu-id="788a5-123">Значение</span><span class="sxs-lookup"><span data-stu-id="788a5-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="788a5-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="788a5-124">Authorization</span></span>  | <span data-ttu-id="788a5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="788a5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="788a5-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="788a5-127">Content-Type</span></span>  | <span data-ttu-id="788a5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="788a5-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="788a5-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="788a5-129">Request body</span></span>

<span data-ttu-id="788a5-130">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="788a5-130">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="788a5-131">В следующей таблице перечислены свойства, необходимые при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="788a5-131">The following table lists the properties that are required when you create a user.</span></span> <span data-ttu-id="788a5-132">Если вы включаете свойство **удостоверения** для создаваемого пользователя, не все перечисленные свойства являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="788a5-132">If you're including an **identities** property for the user you're creating, not all the properties listed are required.</span></span> <span data-ttu-id="788a5-133">Для [удостоверения локальной учетной записи B2C](../resources/objectidentity.md)требуется **только passwordprofile необходима** , а для \*\*\*\* `DisablePasswordExpiration`пассвордполици необходимо задать значение.</span><span class="sxs-lookup"><span data-stu-id="788a5-133">For a [B2C local account identity](../resources/objectidentity.md), only  **passwordProfile** is required, and **passwordPolicy** must be set to `DisablePasswordExpiration`.</span></span> <span data-ttu-id="788a5-134">Для социальных удостоверений никакие свойства не требуются.</span><span class="sxs-lookup"><span data-stu-id="788a5-134">For a social identity, none of the properties are required.</span></span>

| <span data-ttu-id="788a5-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="788a5-135">Parameter</span></span> | <span data-ttu-id="788a5-136">Тип</span><span class="sxs-lookup"><span data-stu-id="788a5-136">Type</span></span> | <span data-ttu-id="788a5-137">Описание</span><span class="sxs-lookup"><span data-stu-id="788a5-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="788a5-138">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="788a5-138">accountEnabled</span></span> |<span data-ttu-id="788a5-139">Логический</span><span class="sxs-lookup"><span data-stu-id="788a5-139">Boolean</span></span> |<span data-ttu-id="788a5-140">Значение true, если учетная запись включена; в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="788a5-140">True if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="788a5-141">displayName</span><span class="sxs-lookup"><span data-stu-id="788a5-141">displayName</span></span> |<span data-ttu-id="788a5-142">строка</span><span class="sxs-lookup"><span data-stu-id="788a5-142">string</span></span> |<span data-ttu-id="788a5-143">Имя, которое следует отобразить в адресной книге для пользователя.</span><span class="sxs-lookup"><span data-stu-id="788a5-143">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="788a5-144">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="788a5-144">onPremisesImmutableId</span></span> |<span data-ttu-id="788a5-145">string</span><span class="sxs-lookup"><span data-stu-id="788a5-145">string</span></span> |<span data-ttu-id="788a5-146">Необходимо указывать только при создании учетной записи пользователя, если вы используете федеративный домен для свойства userPrincipalName (UPN) этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="788a5-146">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="788a5-147">mailNickname</span><span class="sxs-lookup"><span data-stu-id="788a5-147">mailNickname</span></span> |<span data-ttu-id="788a5-148">string</span><span class="sxs-lookup"><span data-stu-id="788a5-148">string</span></span> |<span data-ttu-id="788a5-149">Почтовый псевдоним для пользователя.</span><span class="sxs-lookup"><span data-stu-id="788a5-149">The mail alias for the user.</span></span>|
|<span data-ttu-id="788a5-150">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="788a5-150">passwordProfile</span></span>|[<span data-ttu-id="788a5-151">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="788a5-151">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="788a5-152">Пароль для профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="788a5-152">The password profile for the user.</span></span>|
|<span data-ttu-id="788a5-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="788a5-153">userPrincipalName</span></span> |<span data-ttu-id="788a5-154">string</span><span class="sxs-lookup"><span data-stu-id="788a5-154">string</span></span> |<span data-ttu-id="788a5-155">Имя участника-пользователя (polzovatel@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="788a5-155">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="788a5-156">Так как ресурс **user** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными в экземпляр user при его создании.</span><span class="sxs-lookup"><span data-stu-id="788a5-156">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

<span data-ttu-id="788a5-157">Федеративные пользователи, созданные с помощью этого API, будут вынуждены подписываться каждые 12 часов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="788a5-157">Federated users created via this API will be forced to sign in every 12 hours by default.</span></span> <span data-ttu-id="788a5-158">Сведения о том, как это сделать, приведены в статье [исключения для времени существования маркеров](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span><span class="sxs-lookup"><span data-stu-id="788a5-158">For information about how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

>[!NOTE]
><span data-ttu-id="788a5-159">Добавление [локальной учетной записи B2C](../resources/objectidentity.md) к существующему объекту **пользователя** запрещено, если объект **пользователя** еще не содержит удостоверение локальной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="788a5-159">Adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="response"></a><span data-ttu-id="788a5-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="788a5-160">Response</span></span>

<span data-ttu-id="788a5-161">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [user](../resources/user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="788a5-161">If successful, this method returns a `201 Created` response code and a [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="788a5-162">Пример</span><span class="sxs-lookup"><span data-stu-id="788a5-162">Example</span></span>

### <a name="example-1-create-a-user"></a><span data-ttu-id="788a5-163">Пример 1: создание пользователя</span><span class="sxs-lookup"><span data-stu-id="788a5-163">Example 1: Create a user</span></span>

#### <a name="request"></a><span data-ttu-id="788a5-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="788a5-164">Request</span></span>
<span data-ttu-id="788a5-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="788a5-165">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="788a5-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="788a5-166">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="788a5-167">C#</span><span class="sxs-lookup"><span data-stu-id="788a5-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="788a5-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="788a5-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="788a5-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="788a5-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="788a5-170">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="788a5-170">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="788a5-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="788a5-171">Response</span></span>
<span data-ttu-id="788a5-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="788a5-172">Here is an example of the response.</span></span> 

[!NOTE]
<span data-ttu-id="788a5-173">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="788a5-173">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="788a5-174">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="788a5-174">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-a-user-with-social-and-local-account-identities"></a><span data-ttu-id="788a5-175">Пример 2: создание пользователя с удостоверениями социальных сетей и локальных учетных записей</span><span class="sxs-lookup"><span data-stu-id="788a5-175">Example 2: Create a user with social and local account identities</span></span>

<span data-ttu-id="788a5-176">Создайте нового пользователя с удостоверением локальной учетной записи с именем для входа, адресом электронной почты в качестве входа и с помощью социальных удостоверений.</span><span class="sxs-lookup"><span data-stu-id="788a5-176">Create a new user, with a local account identity with a sign-in name, an email address as sign-in, and with a social identity.</span></span> <span data-ttu-id="788a5-177">Этот пример обычно используется для сценариев миграции в клиентах B2C.</span><span class="sxs-lookup"><span data-stu-id="788a5-177">This example is typically used for migration scenarios in B2C tenants.</span></span>  

[!NOTE] 
<span data-ttu-id="788a5-178">Для удостоверений локальных учетных записей необходимо отключить срок действия паролей и принудительно изменить пароль при следующем входе в систему.</span><span class="sxs-lookup"><span data-stu-id="788a5-178">For local account identities, password expirations must be disabled, and force change password at next sign-in must also be disabled.</span></span>

#### <a name="request"></a><span data-ttu-id="788a5-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="788a5-179">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="788a5-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="788a5-180">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="788a5-181">C#</span><span class="sxs-lookup"><span data-stu-id="788a5-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-identities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="788a5-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="788a5-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-identities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="788a5-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="788a5-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-identities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="788a5-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="788a5-184">Response</span></span>

<span data-ttu-id="788a5-185">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="788a5-185">Here is an example of the response.</span></span> 

> <span data-ttu-id="788a5-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="788a5-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "signInType": "signInName",
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

## <a name="see-also"></a><span data-ttu-id="788a5-188">См. также</span><span class="sxs-lookup"><span data-stu-id="788a5-188">See also</span></span>

- [<span data-ttu-id="788a5-189">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="788a5-189">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="788a5-190">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="788a5-190">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="788a5-191">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="788a5-191">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
