---
title: Создание пользователя
description: С помощью этого API можно создать объект User.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0193ab061f98d1cf799a9f84133ed88a2122c2b9
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536451"
---
# <a name="create-user"></a><span data-ttu-id="8b4b2-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="8b4b2-103">Create User</span></span>

<span data-ttu-id="8b4b2-p101">Создание пользователя. В теле запроса указан пользователь, которого нужно создать. Вам нужно указать как минимум обязательные свойства для пользователя. При необходимости вы можете указать другие записываемые свойства.</span><span class="sxs-lookup"><span data-stu-id="8b4b2-p101">Use this API to create a new User. The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b4b2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b4b2-108">Permissions</span></span>

<span data-ttu-id="8b4b2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b4b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b4b2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b4b2-111">Permission type</span></span>      | <span data-ttu-id="8b4b2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b4b2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b4b2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b4b2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8b4b2-114">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8b4b2-114">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8b4b2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b4b2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b4b2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b4b2-116">Not supported.</span></span>    |
|<span data-ttu-id="8b4b2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b4b2-117">Application</span></span> | <span data-ttu-id="8b4b2-118">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b4b2-118">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b4b2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b4b2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="8b4b2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b4b2-120">Request headers</span></span>

| <span data-ttu-id="8b4b2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b4b2-121">Header</span></span>       | <span data-ttu-id="8b4b2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8b4b2-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8b4b2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b4b2-123">Authorization</span></span>  | <span data-ttu-id="8b4b2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b4b2-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8b4b2-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8b4b2-126">Content-Type</span></span>  | <span data-ttu-id="8b4b2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8b4b2-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8b4b2-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8b4b2-128">Request body</span></span>

<span data-ttu-id="8b4b2-129">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b4b2-129">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="8b4b2-130">В приведенной ниже таблице показаны обязательные свойства при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b4b2-130">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="8b4b2-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="8b4b2-131">Parameter</span></span> | <span data-ttu-id="8b4b2-132">Тип</span><span class="sxs-lookup"><span data-stu-id="8b4b2-132">Type</span></span> | <span data-ttu-id="8b4b2-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8b4b2-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b4b2-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="8b4b2-134">accountEnabled</span></span> |<span data-ttu-id="8b4b2-135">boolean</span><span class="sxs-lookup"><span data-stu-id="8b4b2-135">boolean</span></span> |<span data-ttu-id="8b4b2-136">Если учетная запись обеспечена — true, в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="8b4b2-136">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="8b4b2-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8b4b2-137">displayName</span></span> |<span data-ttu-id="8b4b2-138">string</span><span class="sxs-lookup"><span data-stu-id="8b4b2-138">string</span></span> |<span data-ttu-id="8b4b2-139">Имя, которое следует отобразить в адресной книге для пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b4b2-139">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="8b4b2-140">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="8b4b2-140">onPremisesImmutableId</span></span> |<span data-ttu-id="8b4b2-141">string</span><span class="sxs-lookup"><span data-stu-id="8b4b2-141">string</span></span> |<span data-ttu-id="8b4b2-142">Необходимо указывать только при создании учетной записи пользователя, если вы используете федеративный домен для свойства userPrincipalName (UPN) этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b4b2-142">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="8b4b2-143">mailNickname</span><span class="sxs-lookup"><span data-stu-id="8b4b2-143">mailNickname</span></span> |<span data-ttu-id="8b4b2-144">string</span><span class="sxs-lookup"><span data-stu-id="8b4b2-144">string</span></span> |<span data-ttu-id="8b4b2-145">Почтовый псевдоним для пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b4b2-145">The mail alias for the user.</span></span>|
|<span data-ttu-id="8b4b2-146">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="8b4b2-146">passwordProfile</span></span>|[<span data-ttu-id="8b4b2-147">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="8b4b2-147">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="8b4b2-148">Пароль для профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b4b2-148">The password profile for the user.</span></span>|
|<span data-ttu-id="8b4b2-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8b4b2-149">userPrincipalName</span></span> |<span data-ttu-id="8b4b2-150">string</span><span class="sxs-lookup"><span data-stu-id="8b4b2-150">string</span></span> |<span data-ttu-id="8b4b2-151">Имя участника-пользователя (polzovatel@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="8b4b2-151">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="8b4b2-152">Так как ресурс **user** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными в экземпляр user при его создании.</span><span class="sxs-lookup"><span data-stu-id="8b4b2-152">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

>[!NOTE]
><span data-ttu-id="8b4b2-153">Федеративные пользователи, созданные с помощью этого API, по умолчанию должны выполнять вход каждые 12 часов.</span><span class="sxs-lookup"><span data-stu-id="8b4b2-153">Federated users created using this API will be forced to sign-in every 12 hours by default.</span></span>  <span data-ttu-id="8b4b2-154">Дополнительные сведения об изменении этого параметра см. в разделе [Исключения для сроков действия маркеров](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span><span class="sxs-lookup"><span data-stu-id="8b4b2-154">For more information on how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

## <a name="response"></a><span data-ttu-id="8b4b2-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b4b2-155">Response</span></span>

<span data-ttu-id="8b4b2-156">В случае успеха этот метод возвратит код отклика `201 Created` и объект [user](../resources/user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8b4b2-156">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b4b2-157">Пример</span><span class="sxs-lookup"><span data-stu-id="8b4b2-157">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8b4b2-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b4b2-158">Request</span></span>

<span data-ttu-id="8b4b2-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b4b2-159">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
}-->

```http
POST https://graph.microsoft.com/v1.0/users
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

<span data-ttu-id="8b4b2-160">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b4b2-160">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="8b4b2-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b4b2-161">Response</span></span>

<span data-ttu-id="8b4b2-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b4b2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

#### <a name="sdk-sample-code"></a><span data-ttu-id="8b4b2-165">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="8b4b2-165">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8b4b2-166">C#</span><span class="sxs-lookup"><span data-stu-id="8b4b2-166">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_user_from_users-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8b4b2-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b4b2-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_user_from_users-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-post-users.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-post-users.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
