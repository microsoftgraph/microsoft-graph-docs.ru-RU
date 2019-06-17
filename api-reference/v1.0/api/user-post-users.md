---
title: Создание пользователя
description: С помощью этого API можно создать объект User.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2f023c8882600952feeacffea62b90dc167cf58a
ms.sourcegitcommit: 8aaf10f7c11d1bf481e9acac19884346dbd44cb8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/13/2019
ms.locfileid: "34914688"
---
# <a name="create-user"></a><span data-ttu-id="7b772-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="7b772-103">Create User</span></span>

<span data-ttu-id="7b772-p101">Создание пользователя. В теле запроса указан пользователь, которого нужно создать. Вам нужно указать как минимум обязательные свойства для пользователя. При необходимости вы можете указать другие записываемые свойства.</span><span class="sxs-lookup"><span data-stu-id="7b772-p101">Use this API to create a new User. The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>

>[!NOTE]
><span data-ttu-id="7b772-108">Внешние пользователи должны создаваться с помощью приглашения.</span><span class="sxs-lookup"><span data-stu-id="7b772-108">External users must be created through an invitation.</span></span> <span data-ttu-id="7b772-109">Если нужно включить создание внешних пользователей, см. ресурс [invitation](../resources/invitation.md).</span><span class="sxs-lookup"><span data-stu-id="7b772-109">If you need to enable the creation of external users, see [invitation](../resources/invitation.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7b772-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b772-110">Permissions</span></span>

<span data-ttu-id="7b772-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b772-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b772-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b772-113">Permission type</span></span>      | <span data-ttu-id="7b772-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b772-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b772-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b772-115">Delegated (work or school account)</span></span> | <span data-ttu-id="7b772-116">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7b772-116">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7b772-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b772-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b772-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b772-118">Not supported.</span></span>    |
|<span data-ttu-id="7b772-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b772-119">Application</span></span> | <span data-ttu-id="7b772-120">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b772-120">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b772-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b772-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="7b772-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b772-122">Request headers</span></span>

| <span data-ttu-id="7b772-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7b772-123">Header</span></span>       | <span data-ttu-id="7b772-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7b772-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7b772-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b772-125">Authorization</span></span>  | <span data-ttu-id="7b772-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b772-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7b772-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7b772-128">Content-Type</span></span>  | <span data-ttu-id="7b772-129">application/json</span><span class="sxs-lookup"><span data-stu-id="7b772-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7b772-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7b772-130">Request body</span></span>

<span data-ttu-id="7b772-131">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b772-131">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="7b772-132">В приведенной ниже таблице показаны обязательные свойства при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="7b772-132">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="7b772-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="7b772-133">Parameter</span></span> | <span data-ttu-id="7b772-134">Тип</span><span class="sxs-lookup"><span data-stu-id="7b772-134">Type</span></span> | <span data-ttu-id="7b772-135">Описание</span><span class="sxs-lookup"><span data-stu-id="7b772-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b772-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="7b772-136">accountEnabled</span></span> |<span data-ttu-id="7b772-137">boolean</span><span class="sxs-lookup"><span data-stu-id="7b772-137">boolean</span></span> |<span data-ttu-id="7b772-138">Если учетная запись обеспечена — true, в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="7b772-138">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="7b772-139">displayName</span><span class="sxs-lookup"><span data-stu-id="7b772-139">displayName</span></span> |<span data-ttu-id="7b772-140">string</span><span class="sxs-lookup"><span data-stu-id="7b772-140">string</span></span> |<span data-ttu-id="7b772-141">Имя, которое следует отобразить в адресной книге для пользователя.</span><span class="sxs-lookup"><span data-stu-id="7b772-141">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="7b772-142">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="7b772-142">onPremisesImmutableId</span></span> |<span data-ttu-id="7b772-143">string</span><span class="sxs-lookup"><span data-stu-id="7b772-143">string</span></span> |<span data-ttu-id="7b772-144">Необходимо указывать только при создании учетной записи пользователя, если вы используете федеративный домен для свойства userPrincipalName (UPN) этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="7b772-144">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="7b772-145">mailNickname</span><span class="sxs-lookup"><span data-stu-id="7b772-145">mailNickname</span></span> |<span data-ttu-id="7b772-146">string</span><span class="sxs-lookup"><span data-stu-id="7b772-146">string</span></span> |<span data-ttu-id="7b772-147">Почтовый псевдоним для пользователя.</span><span class="sxs-lookup"><span data-stu-id="7b772-147">The mail alias for the user.</span></span>|
|<span data-ttu-id="7b772-148">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="7b772-148">passwordProfile</span></span>|[<span data-ttu-id="7b772-149">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="7b772-149">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="7b772-150">Пароль для профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="7b772-150">The password profile for the user.</span></span>|
|<span data-ttu-id="7b772-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7b772-151">userPrincipalName</span></span> |<span data-ttu-id="7b772-152">string</span><span class="sxs-lookup"><span data-stu-id="7b772-152">string</span></span> |<span data-ttu-id="7b772-153">Имя участника-пользователя (polzovatel@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="7b772-153">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="7b772-154">Так как ресурс **user** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными в экземпляр user при его создании.</span><span class="sxs-lookup"><span data-stu-id="7b772-154">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

>[!NOTE]
><span data-ttu-id="7b772-155">Федеративные пользователи, созданные с помощью этого API, по умолчанию должны выполнять вход каждые 12 часов.</span><span class="sxs-lookup"><span data-stu-id="7b772-155">Federated users created using this API will be forced to sign-in every 12 hours by default.</span></span>  <span data-ttu-id="7b772-156">Дополнительные сведения об изменении этого параметра см. в разделе [Исключения для сроков действия маркеров](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span><span class="sxs-lookup"><span data-stu-id="7b772-156">For more information on how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

## <a name="response"></a><span data-ttu-id="7b772-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b772-157">Response</span></span>

<span data-ttu-id="7b772-158">В случае успеха этот метод возвратит код отклика `201 Created` и объект [user](../resources/user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7b772-158">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b772-159">Пример</span><span class="sxs-lookup"><span data-stu-id="7b772-159">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7b772-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b772-160">Request</span></span>

<span data-ttu-id="7b772-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b772-161">Here is an example of the request.</span></span>
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

<span data-ttu-id="7b772-162">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b772-162">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="7b772-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b772-163">Response</span></span>

<span data-ttu-id="7b772-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7b772-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

#### <a name="sdk-sample-code"></a><span data-ttu-id="7b772-167">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="7b772-167">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7b772-168">C#</span><span class="sxs-lookup"><span data-stu-id="7b772-168">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_user_from_users-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7b772-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b772-169">Javascript</span></span>](#tab/javascript)
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
