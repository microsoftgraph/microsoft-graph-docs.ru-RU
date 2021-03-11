---
title: Создание пользователя
description: Создание пользователя.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 9e60e01bcf530533f6827af2d93a90573f39c760
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720046"
---
# <a name="create-user"></a><span data-ttu-id="c1b8f-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="c1b8f-103">Create user</span></span>

<span data-ttu-id="c1b8f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1b8f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1b8f-p101">Создание [пользователя](../resources/user.md). В теле запроса указан пользователь, которого нужно создать. Вам нужно указать как минимум обязательные свойства для пользователя. При необходимости вы можете указать другие записываемые свойства.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-p101">Create a new [user](../resources/user.md). The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>

<span data-ttu-id="c1b8f-109">Эта операция возвращает по умолчанию только подмножество свойств для каждого пользователя.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-109">This operation returns by default only a subset of the properties for each user.</span></span> <span data-ttu-id="c1b8f-110">Эти свойства по умолчанию указаны в разделе [Свойства](../resources/user.md#properties).</span><span class="sxs-lookup"><span data-stu-id="c1b8f-110">These default properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="c1b8f-111">Чтобы получить свойства, которые не возвращаются по умолчанию, выполните [операцию GET](user-get.md) и укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-111">To get properties that are not returned by default, do a [GET operation](user-get.md) and specify the properties in a `$select` OData query option.</span></span>

>[!NOTE]
><span data-ttu-id="c1b8f-112">Чтобы создать внешних пользователей, используйте [API приглашений](invitation-post.md).</span><span class="sxs-lookup"><span data-stu-id="c1b8f-112">To create external users, use the [invitation API](invitation-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c1b8f-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1b8f-113">Permissions</span></span>

<span data-ttu-id="c1b8f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1b8f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1b8f-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1b8f-116">Permission type</span></span>      | <span data-ttu-id="c1b8f-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1b8f-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1b8f-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1b8f-118">Delegated (work or school account)</span></span> | <span data-ttu-id="c1b8f-119">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c1b8f-119">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c1b8f-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1b8f-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1b8f-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-121">Not supported.</span></span>    |
|<span data-ttu-id="c1b8f-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1b8f-122">Application</span></span> | <span data-ttu-id="c1b8f-123">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1b8f-123">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1b8f-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1b8f-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="c1b8f-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1b8f-125">Request headers</span></span>
| <span data-ttu-id="c1b8f-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1b8f-126">Header</span></span>       | <span data-ttu-id="c1b8f-127">Значение</span><span class="sxs-lookup"><span data-stu-id="c1b8f-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c1b8f-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1b8f-128">Authorization</span></span>  | <span data-ttu-id="c1b8f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c1b8f-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1b8f-131">Content-Type</span></span>  | <span data-ttu-id="c1b8f-132">application/json</span><span class="sxs-lookup"><span data-stu-id="c1b8f-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c1b8f-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c1b8f-133">Request body</span></span>

<span data-ttu-id="c1b8f-134">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-134">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="c1b8f-135">В приведенной ниже таблице перечислены обязательные свойства при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-135">The following table lists the properties that are required when you create a user.</span></span> <span data-ttu-id="c1b8f-136">Если вы включаете свойство **identities** для создаваемого пользователя, не все перечисленные свойства являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-136">If you're including an **identities** property for the user you're creating, not all the properties listed are required.</span></span> <span data-ttu-id="c1b8f-137">Для [удостоверения локальной учетной записи B2C](../resources/objectidentity.md) обязательным является только **passwordProfile**, а свойству **passwordPolicy** должно быть присвоено значение `DisablePasswordExpiration`.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-137">For a [B2C local account identity](../resources/objectidentity.md), only  **passwordProfile** is required, and **passwordPolicy** must be set to `DisablePasswordExpiration`.</span></span> <span data-ttu-id="c1b8f-138">Для удостоверения социальных сетей ни одно свойство не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-138">For a social identity, none of the properties are required.</span></span>

| <span data-ttu-id="c1b8f-139">Параметр</span><span class="sxs-lookup"><span data-stu-id="c1b8f-139">Parameter</span></span> | <span data-ttu-id="c1b8f-140">Тип</span><span class="sxs-lookup"><span data-stu-id="c1b8f-140">Type</span></span> | <span data-ttu-id="c1b8f-141">Описание</span><span class="sxs-lookup"><span data-stu-id="c1b8f-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1b8f-142">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="c1b8f-142">accountEnabled</span></span> |<span data-ttu-id="c1b8f-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1b8f-143">Boolean</span></span> |<span data-ttu-id="c1b8f-144">True, если учетная запись включена; в противном случае, false.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-144">True if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="c1b8f-145">displayName</span><span class="sxs-lookup"><span data-stu-id="c1b8f-145">displayName</span></span> |<span data-ttu-id="c1b8f-146">string</span><span class="sxs-lookup"><span data-stu-id="c1b8f-146">string</span></span> |<span data-ttu-id="c1b8f-147">Имя, которое следует отобразить в адресной книге для пользователя.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-147">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="c1b8f-148">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="c1b8f-148">onPremisesImmutableId</span></span> |<span data-ttu-id="c1b8f-149">string</span><span class="sxs-lookup"><span data-stu-id="c1b8f-149">string</span></span> |<span data-ttu-id="c1b8f-150">Необходимо указывать только при создании учетной записи пользователя, если вы используете федеративный домен для свойства userPrincipalName (UPN) этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-150">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="c1b8f-151">mailNickname</span><span class="sxs-lookup"><span data-stu-id="c1b8f-151">mailNickname</span></span> |<span data-ttu-id="c1b8f-152">string</span><span class="sxs-lookup"><span data-stu-id="c1b8f-152">string</span></span> |<span data-ttu-id="c1b8f-153">Почтовый псевдоним для пользователя.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-153">The mail alias for the user.</span></span>|
|<span data-ttu-id="c1b8f-154">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="c1b8f-154">passwordProfile</span></span>|[<span data-ttu-id="c1b8f-155">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="c1b8f-155">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="c1b8f-156">Пароль для профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-156">The password profile for the user.</span></span>|
|<span data-ttu-id="c1b8f-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c1b8f-157">userPrincipalName</span></span> |<span data-ttu-id="c1b8f-158">string</span><span class="sxs-lookup"><span data-stu-id="c1b8f-158">string</span></span> |<span data-ttu-id="c1b8f-159">Имя участника-пользователя (polzovatel@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="c1b8f-159">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="c1b8f-160">Так как ресурс **user** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными в экземпляр user при его создании.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-160">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

<span data-ttu-id="c1b8f-161">Федератный пользователь, созданный с помощью этого API, будет вынужден войти каждые 12 часов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-161">Federated users created via this API will be forced to sign in every 12 hours by default.</span></span> <span data-ttu-id="c1b8f-162">Сведения о том, как это изменить, см. в руб. [Исключения для жизни маркеров.](/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions)</span><span class="sxs-lookup"><span data-stu-id="c1b8f-162">For information about how to change this, see [Exceptions for token lifetimes](/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

>[!NOTE]
><span data-ttu-id="c1b8f-163">Добавление [локальной учетной](../resources/objectidentity.md) записи  B2C к существующему  объекту пользователя запрещено, если объект пользователя уже не содержит локальный идентификатор учетной записи.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-163">Adding a [B2C local account](../resources/objectidentity.md) to an existing **user** object is not allowed, unless the **user** object already contains a local account identity.</span></span>

## <a name="response"></a><span data-ttu-id="c1b8f-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1b8f-164">Response</span></span>

<span data-ttu-id="c1b8f-165">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [user](../resources/user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-165">If successful, this method returns a `201 Created` response code and a [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1b8f-166">Пример</span><span class="sxs-lookup"><span data-stu-id="c1b8f-166">Example</span></span>

### <a name="example-1-create-a-user"></a><span data-ttu-id="c1b8f-167">Пример 1. Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="c1b8f-167">Example 1: Create a user</span></span>

#### <a name="request"></a><span data-ttu-id="c1b8f-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1b8f-168">Request</span></span>
<span data-ttu-id="c1b8f-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-169">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c1b8f-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1b8f-170">HTTP</span></span>](#tab/http)
<!-- {  
  "blockType": "request",   
  "name": "create_user_from_users_2"    
}-->

```http
POST https://graph.microsoft.com/beta/users
Content-type: application/json

{
  "accountEnabled": true,
  "displayName": "Adele Vance",
  "mailNickname": "AdeleV",
  "userPrincipalName": "AdeleV@contoso.onmicrosoft.com",
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": "xWwvJ]6NMw+bWH-d"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="c1b8f-171">C#</span><span class="sxs-lookup"><span data-stu-id="c1b8f-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1b8f-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1b8f-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1b8f-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1b8f-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c1b8f-174">Java</span><span class="sxs-lookup"><span data-stu-id="c1b8f-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-user-from-users-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="c1b8f-175">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-175">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c1b8f-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1b8f-176">Response</span></span>
<span data-ttu-id="c1b8f-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-177">Here is an example of the response.</span></span> 

>[!NOTE]
><span data-ttu-id="c1b8f-178">Объект отклика, показанный здесь, может быть сокращен для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-178">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c1b8f-179">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-179">All the properties will be returned from an actual call.</span></span>

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
    "id": "87d349ed-44d7-43e1-9a83-5f2406dee5bd",
    "businessPhones": [],
    "displayName": "Adele Vance",
    "givenName": "Adele",
    "jobTitle": "Product Marketing Manager",
    "mail": "AdeleV@contoso.onmicrosoft.com",
    "mobilePhone": "+1 425 555 0109",
    "officeLocation": "18/2111",
    "preferredLanguage": "en-US",
    "surname": "Vance",
    "userPrincipalName": "AdeleV@contoso.onmicrosoft.com"
}
```

### <a name="example-2-create-a-user-with-social-and-local-account-identities"></a><span data-ttu-id="c1b8f-180">Пример 2. Создание пользователя с удостоверениями учетной записи социальных сетей и локальной учетной записи</span><span class="sxs-lookup"><span data-stu-id="c1b8f-180">Example 2: Create a user with social and local account identities</span></span>

<span data-ttu-id="c1b8f-181">Создайте нового пользователя с удостоверением локальной учетной записи с именем для входа, адресом электронной почты для входа и удостоверением социальной сети.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-181">Create a new user, with a local account identity with a sign-in name, an email address as sign-in, and with a social identity.</span></span> <span data-ttu-id="c1b8f-182">Этот пример обычно применяется для сценариев миграции в клиентах B2C.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-182">This example is typically used for migration scenarios in B2C tenants.</span></span>  

>[!NOTE] 
><span data-ttu-id="c1b8f-183">Для удостоверений локальных учетных записей срок действия паролей должен быть отключен. Также должна быть отключена принудительная смена пароля при следующем входе.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-183">For local account identities, password expirations must be disabled, and force change password at next sign-in must also be disabled.</span></span>

#### <a name="request"></a><span data-ttu-id="c1b8f-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1b8f-184">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c1b8f-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1b8f-185">HTTP</span></span>](#tab/http)
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
    "password": "password-value",
    "forceChangePasswordNextSignIn": false
  },
  "passwordPolicies": "DisablePasswordExpiration"
}
```
# <a name="c"></a>[<span data-ttu-id="c1b8f-186">C#</span><span class="sxs-lookup"><span data-stu-id="c1b8f-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-identities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1b8f-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1b8f-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-identities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1b8f-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1b8f-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-identities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c1b8f-189">Java</span><span class="sxs-lookup"><span data-stu-id="c1b8f-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-user-from-users-identities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c1b8f-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1b8f-190">Response</span></span>

<span data-ttu-id="c1b8f-191">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-191">Here is an example of the response.</span></span> 

> <span data-ttu-id="c1b8f-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="c1b8f-194">См. также</span><span class="sxs-lookup"><span data-stu-id="c1b8f-194">See also</span></span>

- [<span data-ttu-id="c1b8f-195">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="c1b8f-195">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c1b8f-196">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="c1b8f-196">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="c1b8f-197">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="c1b8f-197">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
