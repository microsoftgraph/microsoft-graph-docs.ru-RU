---
title: Создание пользователя
description: С помощью этого API можно создать объект User.
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 42a3b4a1c0cb5cef9606ddea62c1f9d15d0ff493
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721407"
---
# <a name="create-user"></a><span data-ttu-id="ccfe0-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="ccfe0-103">Create User</span></span>

<span data-ttu-id="ccfe0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccfe0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ccfe0-p101">Создание [пользователя](../resources/user.md). В теле запроса указан пользователь, которого нужно создать. Вам нужно указать как минимум обязательные свойства для пользователя. При необходимости вы можете указать другие записываемые свойства.</span><span class="sxs-lookup"><span data-stu-id="ccfe0-p101">Create a new [user](../resources/user.md). The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>

>[!NOTE]
><span data-ttu-id="ccfe0-109">Чтобы создать внешних пользователей, используйте [API приглашений](invitation-post.md).</span><span class="sxs-lookup"><span data-stu-id="ccfe0-109">To create external users, use the [invitation API](invitation-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ccfe0-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ccfe0-110">Permissions</span></span>

<span data-ttu-id="ccfe0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccfe0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccfe0-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccfe0-113">Permission type</span></span>      | <span data-ttu-id="ccfe0-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccfe0-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccfe0-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccfe0-115">Delegated (work or school account)</span></span> | <span data-ttu-id="ccfe0-116">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ccfe0-116">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ccfe0-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccfe0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccfe0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccfe0-118">Not supported.</span></span>    |
|<span data-ttu-id="ccfe0-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ccfe0-119">Application</span></span> | <span data-ttu-id="ccfe0-120">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccfe0-120">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ccfe0-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccfe0-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="ccfe0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ccfe0-122">Request headers</span></span>

| <span data-ttu-id="ccfe0-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ccfe0-123">Header</span></span>       | <span data-ttu-id="ccfe0-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ccfe0-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ccfe0-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ccfe0-125">Authorization</span></span>  | <span data-ttu-id="ccfe0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ccfe0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ccfe0-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ccfe0-128">Content-Type</span></span>  | <span data-ttu-id="ccfe0-129">application/json</span><span class="sxs-lookup"><span data-stu-id="ccfe0-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ccfe0-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ccfe0-130">Request body</span></span>

<span data-ttu-id="ccfe0-131">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ccfe0-131">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="ccfe0-132">В приведенной ниже таблице перечислены обязательные свойства при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="ccfe0-132">The following table lists the properties that are required when you create a user.</span></span> <span data-ttu-id="ccfe0-133">Если вы включаете свойство **identities** для создаваемого пользователя, не все перечисленные свойства являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="ccfe0-133">If you're including an **identities** property for the user you're creating, not all the properties listed are required.</span></span> <span data-ttu-id="ccfe0-134">Для [удостоверения локальной учетной записи B2C](../resources/objectidentity.md) обязательным является только **passwordProfile**, а свойству **passwordPolicy** должно быть присвоено значение `DisablePasswordExpiration`.</span><span class="sxs-lookup"><span data-stu-id="ccfe0-134">For a [B2C local account identity](../resources/objectidentity.md), only  **passwordProfile** is required, and **passwordPolicy** must be set to `DisablePasswordExpiration`.</span></span> <span data-ttu-id="ccfe0-135">Для удостоверения социальных сетей ни одно свойство не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="ccfe0-135">For a social identity, none of the properties are required.</span></span>

| <span data-ttu-id="ccfe0-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="ccfe0-136">Parameter</span></span> | <span data-ttu-id="ccfe0-137">Тип</span><span class="sxs-lookup"><span data-stu-id="ccfe0-137">Type</span></span> | <span data-ttu-id="ccfe0-138">Описание</span><span class="sxs-lookup"><span data-stu-id="ccfe0-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ccfe0-139">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="ccfe0-139">accountEnabled</span></span> |<span data-ttu-id="ccfe0-140">boolean</span><span class="sxs-lookup"><span data-stu-id="ccfe0-140">boolean</span></span> |<span data-ttu-id="ccfe0-141">Если учетная запись обеспечена — true, в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="ccfe0-141">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="ccfe0-142">displayName</span><span class="sxs-lookup"><span data-stu-id="ccfe0-142">displayName</span></span> |<span data-ttu-id="ccfe0-143">string</span><span class="sxs-lookup"><span data-stu-id="ccfe0-143">string</span></span> |<span data-ttu-id="ccfe0-144">Имя, которое следует отобразить в адресной книге для пользователя.</span><span class="sxs-lookup"><span data-stu-id="ccfe0-144">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="ccfe0-145">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="ccfe0-145">onPremisesImmutableId</span></span> |<span data-ttu-id="ccfe0-146">string</span><span class="sxs-lookup"><span data-stu-id="ccfe0-146">string</span></span> |<span data-ttu-id="ccfe0-147">Необходимо указывать только при создании учетной записи пользователя, если вы используете федеративный домен для свойства userPrincipalName (UPN) этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="ccfe0-147">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="ccfe0-148">mailNickname</span><span class="sxs-lookup"><span data-stu-id="ccfe0-148">mailNickname</span></span> |<span data-ttu-id="ccfe0-149">string</span><span class="sxs-lookup"><span data-stu-id="ccfe0-149">string</span></span> |<span data-ttu-id="ccfe0-150">Почтовый псевдоним для пользователя.</span><span class="sxs-lookup"><span data-stu-id="ccfe0-150">The mail alias for the user.</span></span>|
|<span data-ttu-id="ccfe0-151">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="ccfe0-151">passwordProfile</span></span>|[<span data-ttu-id="ccfe0-152">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="ccfe0-152">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="ccfe0-153">Пароль для профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="ccfe0-153">The password profile for the user.</span></span>|
|<span data-ttu-id="ccfe0-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ccfe0-154">userPrincipalName</span></span> |<span data-ttu-id="ccfe0-155">string</span><span class="sxs-lookup"><span data-stu-id="ccfe0-155">string</span></span> |<span data-ttu-id="ccfe0-156">Имя участника-пользователя (polzovatel@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="ccfe0-156">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="ccfe0-157">Так как ресурс **user** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными в экземпляр user при его создании.</span><span class="sxs-lookup"><span data-stu-id="ccfe0-157">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

>[!NOTE]
><span data-ttu-id="ccfe0-158">Федеративные пользователи, созданные с помощью этого API, по умолчанию должны выполнять вход каждые 12 часов.</span><span class="sxs-lookup"><span data-stu-id="ccfe0-158">Federated users created using this API will be forced to sign-in every 12 hours by default.</span></span>  <span data-ttu-id="ccfe0-159">Дополнительные сведения об изменении этого параметра см. в разделе [Исключения для сроков действия маркеров](/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span><span class="sxs-lookup"><span data-stu-id="ccfe0-159">For more information on how to change this, see [Exceptions for token lifetimes](/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

## <a name="response"></a><span data-ttu-id="ccfe0-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccfe0-160">Response</span></span>

<span data-ttu-id="ccfe0-161">В случае успеха этот метод возвратит код отклика `201 Created` и объект [user](../resources/user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ccfe0-161">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccfe0-162">Пример</span><span class="sxs-lookup"><span data-stu-id="ccfe0-162">Example</span></span>

### <a name="example-1-create-a-user"></a><span data-ttu-id="ccfe0-163">Пример 1. Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="ccfe0-163">Example 1: Create a user</span></span>

#### <a name="request"></a><span data-ttu-id="ccfe0-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccfe0-164">Request</span></span>

<span data-ttu-id="ccfe0-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ccfe0-165">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ccfe0-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccfe0-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
}-->

```http
POST https://graph.microsoft.com/v1.0/users
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
# <a name="c"></a>[<span data-ttu-id="ccfe0-167">C#</span><span class="sxs-lookup"><span data-stu-id="ccfe0-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccfe0-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccfe0-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccfe0-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccfe0-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ccfe0-170">Java</span><span class="sxs-lookup"><span data-stu-id="ccfe0-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-user-from-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="ccfe0-171">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ccfe0-171">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="ccfe0-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccfe0-172">Response</span></span>

<span data-ttu-id="ccfe0-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ccfe0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
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

### <a name="example-2-create-a-user-with-social-and-local-account-identities"></a><span data-ttu-id="ccfe0-176">Пример 2. Создание пользователя с удостоверениями учетной записи социальных сетей и локальной учетной записи</span><span class="sxs-lookup"><span data-stu-id="ccfe0-176">Example 2: Create a user with social and local account identities</span></span>

<span data-ttu-id="ccfe0-177">Создайте нового пользователя с удостоверением локальной учетной записи с именем для входа, адресом электронной почты для входа и удостоверением социальной сети.</span><span class="sxs-lookup"><span data-stu-id="ccfe0-177">Create a new user, with a local account identity with a sign-in name, an email address as sign-in, and with a social identity.</span></span> <span data-ttu-id="ccfe0-178">Этот пример обычно применяется для сценариев миграции в клиентах B2C.</span><span class="sxs-lookup"><span data-stu-id="ccfe0-178">This example is typically used for migration scenarios in B2C tenants.</span></span>  

>[!NOTE] 
><span data-ttu-id="ccfe0-179">Для удостоверений локальных учетных записей срок действия паролей должен быть отключен. Также должна быть отключена принудительная смена пароля при следующем входе.</span><span class="sxs-lookup"><span data-stu-id="ccfe0-179">For local account identities, password expirations must be disabled, and force change password at next sign-in must also be disabled.</span></span>

#### <a name="request"></a><span data-ttu-id="ccfe0-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccfe0-180">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ccfe0-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccfe0-181">HTTP</span></span>](#tab/http)
<!-- {  
  "blockType": "request",   
  "name": "create_user_from_users_identities"   
}-->

```http
POST https://graph.microsoft.com/v1.0/users
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
# <a name="c"></a>[<span data-ttu-id="ccfe0-182">C#</span><span class="sxs-lookup"><span data-stu-id="ccfe0-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-identities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccfe0-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccfe0-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-identities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccfe0-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccfe0-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-identities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ccfe0-185">Java</span><span class="sxs-lookup"><span data-stu-id="ccfe0-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-user-from-users-identities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ccfe0-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccfe0-186">Response</span></span>

<span data-ttu-id="ccfe0-187">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ccfe0-187">Here is an example of the response.</span></span> 

> <span data-ttu-id="ccfe0-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ccfe0-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
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
## <a name="see-also"></a><span data-ttu-id="ccfe0-190">См. также</span><span class="sxs-lookup"><span data-stu-id="ccfe0-190">See also</span></span>

- [<span data-ttu-id="ccfe0-191">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="ccfe0-191">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="ccfe0-192">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="ccfe0-192">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
